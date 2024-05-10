# Comparing `tmp/aksharamukha-2.1.2.tar.gz` & `tmp/aksharamukha-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aksharamukha-2.1.2.tar", last modified: Fri Jan  6 20:18:10 2023, max compression
+gzip compressed data, was "aksharamukha-2.2.1.tar", last modified: Fri May 10 19:14:47 2024, max compression
```

## Comparing `aksharamukha-2.1.2.tar` & `aksharamukha-2.2.1.tar`

### file list

```diff
@@ -1,162 +1,199 @@
-drwxrwxrwx   0        0        0        0 2023-01-06 20:18:10.510525 aksharamukha-2.1.2/
--rw-rw-rw-   0        0        0     4648 2023-01-06 20:18:10.511525 aksharamukha-2.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     3255 2022-05-26 09:31:49.000000 aksharamukha-2.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-01-06 20:18:10.328521 aksharamukha-2.1.2/aksharamukha/
--rw-rw-rw-   0        0        0    13272 2023-01-05 14:54:31.000000 aksharamukha-2.1.2/aksharamukha/Convert.py
--rw-rw-rw-   0        0        0   121147 2023-01-05 15:54:46.000000 aksharamukha-2.1.2/aksharamukha/ConvertFix.py
--rw-rw-rw-   0        0        0     9131 2022-05-23 16:00:54.000000 aksharamukha-2.1.2/aksharamukha/GeneralMap.py
--rw-rw-rw-   0        0        0     3226 2023-01-04 14:07:25.000000 aksharamukha-2.1.2/aksharamukha/PostOptions.py
--rw-rw-rw-   0        0        0    91660 2023-01-05 15:55:03.000000 aksharamukha-2.1.2/aksharamukha/PostProcess.py
--rw-rw-rw-   0        0        0      494 2022-05-07 22:19:20.000000 aksharamukha-2.1.2/aksharamukha/PreOptions.py
--rw-rw-rw-   0        0        0    47648 2023-01-05 16:22:47.000000 aksharamukha-2.1.2/aksharamukha/PreProcess.py
-drwxrwxrwx   0        0        0        0 2023-01-06 20:18:10.350276 aksharamukha-2.1.2/aksharamukha/ScriptMap/
-drwxrwxrwx   0        0        0        0 2023-01-06 20:18:10.385518 aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/
--rw-rw-rw-   0        0        0     3710 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/Balinese.py
--rw-rw-rw-   0        0        0     3926 2022-05-20 16:07:56.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/BatakKaro.py
--rw-rw-rw-   0        0        0     3986 2022-05-20 16:29:53.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/BatakManda.py
--rw-rw-rw-   0        0        0     3950 2022-05-20 16:30:03.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/BatakPakpak.py
--rw-rw-rw-   0        0        0     3944 2022-05-20 16:30:19.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/BatakSima.py
--rw-rw-rw-   0        0        0     3962 2022-05-20 16:30:30.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/BatakToba.py
--rw-rw-rw-   0        0        0     4081 2022-05-20 16:30:32.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/Buginese.py
--rw-rw-rw-   0        0        0     4100 2022-05-20 16:30:33.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/Buhid.py
--rw-rw-rw-   0        0        0     3727 2022-05-20 16:06:51.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/Burmese.py
--rw-rw-rw-   0        0        0     3958 2022-05-20 16:07:54.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/Cham.py
--rw-rw-rw-   0        0        0     4118 2022-05-20 16:30:34.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/Hanunoo.py
--rw-rw-rw-   0        0        0     3742 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/Javanese.py
--rw-rw-rw-   0        0        0     3742 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/Kawi.py
--rw-rw-rw-   0        0        0     3738 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/KhamtiShan.py
--rw-rw-rw-   0        0        0     3724 2022-05-20 16:07:54.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/Khmer.py
--rw-rw-rw-   0        0        0     3918 2022-05-20 16:07:54.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/KhomThai.py
--rw-rw-rw-   0        0        0     3898 2022-05-20 16:07:54.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/KhuenTham.py
--rw-rw-rw-   0        0        0     4134 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/Lao.py
--rw-rw-rw-   0        0        0     4128 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/Lao2.py
--rw-rw-rw-   0        0        0     3942 2022-05-20 16:07:54.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/LaoPali.py
--rw-rw-rw-   0        0        0     3898 2022-05-20 16:07:54.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/LaoTham.py
--rw-rw-rw-   0        0        0     3898 2022-05-20 16:07:54.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/LueTham.py
--rw-rw-rw-   0        0        0     4572 2022-05-20 16:30:35.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/Makasar.py
--rw-rw-rw-   0        0        0     4585 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/Marchen.py
--rw-rw-rw-   0        0        0     3703 2022-05-20 16:07:54.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/Mon.py
--rw-rw-rw-   0        0        0     3768 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/Pallava.py
--rw-rw-rw-   0        0        0     4104 2022-05-20 16:30:39.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/PhagsPa.py
--rw-rw-rw-   0        0        0     3916 2022-05-20 16:30:41.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/Rejang.py
--rw-rw-rw-   0        0        0     3765 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/Shan.py
--rw-rw-rw-   0        0        0     3955 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/Siddham.py
--rw-rw-rw-   0        0        0     2391 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/SiddhamRanjana.py
--rw-rw-rw-   0        0        0     4310 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/Soyombo.py
--rw-rw-rw-   0        0        0     3873 2022-05-20 16:30:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/Sundanese.py
--rw-rw-rw-   0        0        0     4166 2022-05-20 16:30:43.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/Tagalog.py
--rw-rw-rw-   0        0        0     4106 2022-05-20 16:30:44.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/Tagbanwa.py
--rw-rw-rw-   0        0        0     3757 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/TaiLaing.py
--rw-rw-rw-   0        0        0     3898 2022-05-20 16:07:54.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/TaiTham.py
--rw-rw-rw-   0        0        0     4318 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/Thaana.py
--rw-rw-rw-   0        0        0     3902 2022-05-20 16:07:54.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/Thai.py
--rw-rw-rw-   0        0        0     3825 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/Tibetan.py
--rw-rw-rw-   0        0        0     4424 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/ZanabazarSquare.py
--rw-rw-rw-   0        0        0        0 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/__init__.py
--rw-rw-rw-   0        0        0      286 2022-05-21 13:56:18.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/FallBack.py
-drwxrwxrwx   0        0        0        0 2023-01-06 20:18:10.440868 aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/
--rw-rw-rw-   0        0        0     4643 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/Ahom.py
--rw-rw-rw-   0        0        0     3758 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/Assamese.py
--rw-rw-rw-   0        0        0     3650 2022-05-14 22:40:45.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/Bengali.py
--rw-rw-rw-   0        0        0     4315 2022-05-20 16:22:30.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/Bhaiksuki.py
--rw-rw-rw-   0        0        0     3459 2022-05-20 16:28:20.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/Brahmi.py
--rw-rw-rw-   0        0        0     4422 2022-05-20 16:07:54.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/Chakma.py
--rw-rw-rw-   0        0        0     3527 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/Devanagari.py
--rw-rw-rw-   0        0        0     4224 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/Dogra.py
--rw-rw-rw-   0        0        0     4116 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/Grantha.py
--rw-rw-rw-   0        0        0     3769 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/GranthaGrantamil.py
--rw-rw-rw-   0        0        0     3655 2022-05-20 16:07:54.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/GranthaPandya.py
--rw-rw-rw-   0        0        0     3742 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/Gujarati.py
--rw-rw-rw-   0        0        0     4283 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/GunjalaGondi.py
--rw-rw-rw-   0        0        0     3874 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/Gurmukhi.py
--rw-rw-rw-   0        0        0     3926 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/Kaithi.py
--rw-rw-rw-   0        0        0     3626 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/Kannada.py
--rw-rw-rw-   0        0        0     3687 2022-05-20 16:28:15.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/Kharoshthi.py
--rw-rw-rw-   0        0        0     4360 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/Khojki.py
--rw-rw-rw-   0        0        0     4010 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/Khudawadi.py
--rw-rw-rw-   0        0        0     3975 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/Lepcha.py
--rw-rw-rw-   0        0        0     3971 2022-05-20 16:07:59.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/Limbu.py
--rw-rw-rw-   0        0        0     4392 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/Mahajani.py
--rw-rw-rw-   0        0        0     3620 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/Malayalam.py
--rw-rw-rw-   0        0        0     4325 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/MasaramGondi.py
--rw-rw-rw-   0        0        0     3939 2022-05-20 16:08:01.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/MeeteiMayek.py
--rw-rw-rw-   0        0        0     4103 2022-05-20 16:07:54.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/Modi.py
--rw-rw-rw-   0        0        0     4326 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/Multani.py
--rw-rw-rw-   0        0        0     4096 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/Nandinagari.py
--rw-rw-rw-   0        0        0     4073 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/Newa.py
--rw-rw-rw-   0        0        0     3752 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/Oriya.py
--rw-rw-rw-   0        0        0     3661 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/Ranjana.py
--rw-rw-rw-   0        0        0     3657 2022-05-20 16:08:01.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/Saurashtra.py
--rw-rw-rw-   0        0        0     4342 2022-05-20 16:30:50.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/Shahmukhi.py
--rw-rw-rw-   0        0        0     4230 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/Sharada.py
--rw-rw-rw-   0        0        0     3608 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/SiddhamDevanagari.py
--rw-rw-rw-   0        0        0     3681 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/Sinhala.py
--rw-rw-rw-   0        0        0     3791 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/SylotiNagri.py
--rw-rw-rw-   0        0        0     3523 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/SyriacMalayalam.py
--rw-rw-rw-   0        0        0     4064 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/Takri.py
--rw-rw-rw-   0        0        0     3962 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/Tamil.py
--rw-rw-rw-   0        0        0     4448 2022-05-20 16:08:04.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/TamilBrahmi.py
--rw-rw-rw-   0        0        0     3545 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/TamilExtended.py
--rw-rw-rw-   0        0        0     3771 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/TamilGrantha.py
--rw-rw-rw-   0        0        0     3660 2022-06-28 18:36:24.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/Telugu.py
--rw-rw-rw-   0        0        0     4069 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/Tirhuta.py
--rw-rw-rw-   0        0        0     4361 2022-05-20 16:30:51.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/Urdu.py
--rw-rw-rw-   0        0        0     3875 2022-05-20 16:30:52.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/Vatteluttu.py
--rw-rw-rw-   0        0        0        0 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-06 20:18:10.445380 aksharamukha-2.1.2/aksharamukha/ScriptMap/NonIndic/
--rw-rw-rw-   0        0        0     3935 2022-05-19 17:35:48.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/NonIndic/Hebrew.py
--rw-rw-rw-   0        0        0     4207 2022-05-20 16:30:17.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/NonIndic/OldPersian.py
--rw-rw-rw-   0        0        0        0 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/NonIndic/__init__.py
--rw-rw-rw-   0        0        0    24451 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/NonIndic/kana2roman.py
-drwxrwxrwx   0        0        0        0 2023-01-06 20:18:10.488527 aksharamukha-2.1.2/aksharamukha/ScriptMap/Roman/
--rw-rw-rw-   0        0        0     2890 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/Roman/Aksharaa.py
--rw-rw-rw-   0        0        0     2772 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/Roman/Ariyaka.py
--rw-rw-rw-   0        0        0     3624 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/Roman/Avestan.py
--rw-rw-rw-   0        0        0     2731 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/Roman/BarahaNorth.py
--rw-rw-rw-   0        0        0     2731 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/Roman/BarahaSouth.py
--rw-rw-rw-   0        0        0     3189 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/Roman/GreekModern.py
--rw-rw-rw-   0        0        0     3189 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/Roman/HK.py
--rw-rw-rw-   0        0        0     3743 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/Roman/HanifiRohingya.py
--rw-rw-rw-   0        0        0     3141 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/Roman/IAST.py
--rw-rw-rw-   0        0        0     3150 2022-07-13 16:30:10.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/Roman/IASTLOC.py
--rw-rw-rw-   0        0        0     3152 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/Roman/IASTPali.py
--rw-rw-rw-   0        0        0     3297 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/Roman/IPA.py
--rw-rw-rw-   0        0        0     3155 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/Roman/ISO.py
--rw-rw-rw-   0        0        0     3161 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/Roman/ISOPali.py
--rw-rw-rw-   0        0        0     1008 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/Roman/Inter.py
--rw-rw-rw-   0        0        0     3193 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/Roman/Itrans.py
--rw-rw-rw-   0        0        0     3022 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/Roman/Mongolian.py
--rw-rw-rw-   0        0        0     3709 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/Roman/Mro.py
--rw-rw-rw-   0        0        0     2766 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/Roman/RomanColloquial.py
--rw-rw-rw-   0        0        0     2725 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/Roman/RomanKana.py
--rw-rw-rw-   0        0        0     2794 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/Roman/RomanReadable.py
--rw-rw-rw-   0        0        0     3238 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/Roman/RomanSemitic.py
--rw-rw-rw-   0        0        0     3307 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/Roman/RussianCyrillic.py
--rw-rw-rw-   0        0        0     2773 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/Roman/SLP1.py
--rw-rw-rw-   0        0        0     3267 2022-05-20 16:08:03.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/Roman/Santali.py
--rw-rw-rw-   0        0        0     3891 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/Roman/SoraSompeng.py
--rw-rw-rw-   0        0        0     3159 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/Roman/Titus.py
--rw-rw-rw-   0        0        0     3313 2022-05-20 16:06:35.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/Roman/TolongSiki.py
--rw-rw-rw-   0        0        0     3448 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/Roman/Velthuis.py
--rw-rw-rw-   0        0        0     3178 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/Roman/WX-kok.py
--rw-rw-rw-   0        0        0     3202 2022-05-13 23:12:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/Roman/WX.py
--rw-rw-rw-   0        0        0     3583 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/Roman/Wancho.py
--rw-rw-rw-   0        0        0     3821 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/Roman/WarangCiti.py
--rw-rw-rw-   0        0        0        0 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/Roman/__init__.py
--rw-rw-rw-   0        0        0        0 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/ScriptMap/__init__.py
--rw-rw-rw-   0        0        0        0 2022-04-20 19:00:42.000000 aksharamukha-2.1.2/aksharamukha/__init__.py
--rw-rw-rw-   0        0        0     5127 2022-05-24 17:34:01.000000 aksharamukha-2.1.2/aksharamukha/gimeltra.py
-drwxrwxrwx   0        0        0        0 2023-01-06 20:18:10.493526 aksharamukha-2.1.2/aksharamukha/json/
--rw-rw-rw-   0        0        0    77016 2022-05-22 22:22:45.000000 aksharamukha-2.1.2/aksharamukha/json/gimeltra_data.json
--rw-rw-rw-   0        0        0    31078 2023-01-06 20:14:24.000000 aksharamukha-2.1.2/aksharamukha/transliterate.py
-drwxrwxrwx   0        0        0        0 2023-01-06 20:18:10.509546 aksharamukha-2.1.2/aksharamukha/yaml/
--rw-rw-rw-   0        0        0     8250 2022-05-19 16:05:38.000000 aksharamukha-2.1.2/aksharamukha/yaml/aksharamukha-scripts.yaml
--rw-rw-rw-   0        0        0   189327 2022-05-19 15:32:30.000000 aksharamukha-2.1.2/aksharamukha/yaml/wikitra2-data.yaml
-drwxrwxrwx   0        0        0        0 2023-01-06 20:18:10.347924 aksharamukha-2.1.2/aksharamukha.egg-info/
--rw-rw-rw-   0        0        0     4648 2023-01-06 20:18:09.000000 aksharamukha-2.1.2/aksharamukha.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6270 2023-01-06 20:18:10.000000 aksharamukha-2.1.2/aksharamukha.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-06 20:18:10.000000 aksharamukha-2.1.2/aksharamukha.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      155 2023-01-06 20:18:10.000000 aksharamukha-2.1.2/aksharamukha.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-01-06 20:18:10.000000 aksharamukha-2.1.2/aksharamukha.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-01-06 20:18:10.512545 aksharamukha-2.1.2/setup.cfg
--rw-rw-rw-   0        0        0     4561 2023-01-06 20:16:17.000000 aksharamukha-2.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 19:14:47.283116 aksharamukha-2.2.1/
+-rw-rw-rw-   0        0        0     4648 2024-05-10 19:14:47.283116 aksharamukha-2.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3255 2022-05-26 09:31:49.000000 aksharamukha-2.2.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-10 19:14:47.108475 aksharamukha-2.2.1/aksharamukha/
+-rw-rw-rw-   0        0        0    13357 2024-03-19 23:12:33.000000 aksharamukha-2.2.1/aksharamukha/Convert.py
+-rw-rw-rw-   0        0        0   131047 2024-05-10 16:16:47.000000 aksharamukha-2.2.1/aksharamukha/ConvertFix.py
+-rw-rw-rw-   0        0        0    24800 2024-05-09 22:03:51.000000 aksharamukha-2.2.1/aksharamukha/FallBack.py
+-rw-rw-rw-   0        0        0    16360 2024-05-10 18:04:10.000000 aksharamukha-2.2.1/aksharamukha/GeneralMap.py
+-rw-rw-rw-   0        0        0     3372 2024-05-09 13:36:31.000000 aksharamukha-2.2.1/aksharamukha/PostOptions.py
+-rw-rw-rw-   0        0        0   107098 2024-05-09 23:05:19.000000 aksharamukha-2.2.1/aksharamukha/PostProcess.py
+-rw-rw-rw-   0        0        0      494 2022-05-07 22:19:20.000000 aksharamukha-2.2.1/aksharamukha/PreOptions.py
+-rw-rw-rw-   0        0        0    58079 2024-05-10 16:11:23.000000 aksharamukha-2.2.1/aksharamukha/PreProcess.py
+drwxrwxrwx   0        0        0        0 2024-05-10 19:14:47.136474 aksharamukha-2.2.1/aksharamukha/ScriptMap/
+drwxrwxrwx   0        0        0        0 2024-05-10 19:14:47.181495 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/
+-rw-rw-rw-   0        0        0     3918 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Balinese.py
+-rw-rw-rw-   0        0        0     4147 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/BatakKaro.py
+-rw-rw-rw-   0        0        0     4207 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/BatakManda.py
+-rw-rw-rw-   0        0        0     4171 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/BatakPakpak.py
+-rw-rw-rw-   0        0        0     4165 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/BatakSima.py
+-rw-rw-rw-   0        0        0     4183 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/BatakToba.py
+-rw-rw-rw-   0        0        0     4301 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Buginese.py
+-rw-rw-rw-   0        0        0     4321 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Buhid.py
+-rw-rw-rw-   0        0        0     3947 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Burmese.py
+-rw-rw-rw-   0        0        0     4178 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Cham.py
+-rw-rw-rw-   0        0        0     4565 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/DivesAkuru.py
+-rw-rw-rw-   0        0        0     4338 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Hanunoo.py
+-rw-rw-rw-   0        0        0     3962 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Javanese.py
+-rw-rw-rw-   0        0        0     4446 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Kawi.py
+-rw-rw-rw-   0        0        0     3958 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/KhamtiShan.py
+-rw-rw-rw-   0        0        0     3944 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Khmer.py
+-rw-rw-rw-   0        0        0     3944 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/KhmerLoC.py
+-rw-rw-rw-   0        0        0     4138 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/KhomThai.py
+-rw-rw-rw-   0        0        0     4118 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/KhuenTham.py
+-rw-rw-rw-   0        0        0     4354 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Lao.py
+-rw-rw-rw-   0        0        0     4348 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Lao2.py
+-rw-rw-rw-   0        0        0     4162 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/LaoPali.py
+-rw-rw-rw-   0        0        0     4118 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/LaoTham.py
+-rw-rw-rw-   0        0        0     4118 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/LueTham.py
+-rw-rw-rw-   0        0        0     4792 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Makasar.py
+-rw-rw-rw-   0        0        0     4805 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Marchen.py
+-rw-rw-rw-   0        0        0     3923 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Mon.py
+-rw-rw-rw-   0        0        0     3988 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Pallava.py
+-rw-rw-rw-   0        0        0     4324 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/PhagsPa.py
+-rw-rw-rw-   0        0        0     4136 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Rejang.py
+-rw-rw-rw-   0        0        0     3967 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Shan.py
+-rw-rw-rw-   0        0        0     3967 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/ShanLoC.py
+-rw-rw-rw-   0        0        0     4175 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Siddham.py
+-rw-rw-rw-   0        0        0     2391 2022-04-20 19:00:42.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/SiddhamRanjana.py
+-rw-rw-rw-   0        0        0     4530 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Soyombo.py
+-rw-rw-rw-   0        0        0     4093 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Sundanese.py
+-rw-rw-rw-   0        0        0     4386 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Tagalog.py
+-rw-rw-rw-   0        0        0     4326 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Tagbanwa.py
+-rw-rw-rw-   0        0        0     3977 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/TaiLaing.py
+-rw-rw-rw-   0        0        0     4118 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/TaiTham.py
+-rw-rw-rw-   0        0        0     4540 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Thaana.py
+-rw-rw-rw-   0        0        0     4122 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Thai.py
+-rw-rw-rw-   0        0        0     4094 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/ThamLoC.py
+-rw-rw-rw-   0        0        0     4045 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Tibetan.py
+-rw-rw-rw-   0        0        0     3997 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/TibetanLoC.py
+-rw-rw-rw-   0        0        0     4644 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/ZanabazarSquare.py
+-rw-rw-rw-   0        0        0        0 2022-04-20 19:00:42.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 19:14:47.229598 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/
+-rw-rw-rw-   0        0        0     4809 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Ahom.py
+-rw-rw-rw-   0        0        0     3870 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Assamese.py
+-rw-rw-rw-   0        0        0     3869 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Bengali.py
+-rw-rw-rw-   0        0        0     3863 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/BengaliRaBa.py
+-rw-rw-rw-   0        0        0     4541 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Bhaiksuki.py
+-rw-rw-rw-   0        0        0     3679 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Brahmi.py
+-rw-rw-rw-   0        0        0     4641 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Chakma.py
+-rw-rw-rw-   0        0        0     3747 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Devanagari.py
+-rw-rw-rw-   0        0        0     4444 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Dogra.py
+-rw-rw-rw-   0        0        0     4336 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Grantha.py
+-rw-rw-rw-   0        0        0     3989 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/GranthaGrantamil.py
+-rw-rw-rw-   0        0        0     3875 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/GranthaPandya.py
+-rw-rw-rw-   0        0        0     3853 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Gujarati.py
+-rw-rw-rw-   0        0        0     4503 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/GunjalaGondi.py
+-rw-rw-rw-   0        0        0     3982 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Gurmukhi.py
+-rw-rw-rw-   0        0        0     3982 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/GurmukhiLoC.py
+-rw-rw-rw-   0        0        0     4138 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Kaithi.py
+-rw-rw-rw-   0        0        0     3845 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Kannada.py
+-rw-rw-rw-   0        0        0     3907 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Kharoshthi.py
+-rw-rw-rw-   0        0        0     4548 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Khojki.py
+-rw-rw-rw-   0        0        0     4230 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Khudawadi.py
+-rw-rw-rw-   0        0        0     4195 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Lepcha.py
+-rw-rw-rw-   0        0        0     4191 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Limbu.py
+-rw-rw-rw-   0        0        0     4237 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/LimbuLoC.py
+-rw-rw-rw-   0        0        0     4612 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Mahajani.py
+-rw-rw-rw-   0        0        0     3839 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Malayalam.py
+-rw-rw-rw-   0        0        0     4545 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/MasaramGondi.py
+-rw-rw-rw-   0        0        0     4159 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/MeeteiMayek.py
+-rw-rw-rw-   0        0        0     4323 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Modi.py
+-rw-rw-rw-   0        0        0     4546 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Multani.py
+-rw-rw-rw-   0        0        0     4316 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Nandinagari.py
+-rw-rw-rw-   0        0        0     4293 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Newa.py
+-rw-rw-rw-   0        0        0     3864 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Oriya.py
+-rw-rw-rw-   0        0        0     3881 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Ranjana.py
+-rw-rw-rw-   0        0        0     3877 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Saurashtra.py
+-rw-rw-rw-   0        0        0     4562 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Shahmukhi.py
+-rw-rw-rw-   0        0        0     4449 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Sharada.py
+-rw-rw-rw-   0        0        0     3828 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/SiddhamDevanagari.py
+-rw-rw-rw-   0        0        0     3786 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Sinhala.py
+-rw-rw-rw-   0        0        0     4011 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/SylotiNagri.py
+-rw-rw-rw-   0        0        0     3743 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/SyriacMalayalam.py
+-rw-rw-rw-   0        0        0     4284 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Takri.py
+-rw-rw-rw-   0        0        0     4181 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Tamil.py
+-rw-rw-rw-   0        0        0     4668 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/TamilBrahmi.py
+-rw-rw-rw-   0        0        0     3765 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/TamilExtended.py
+-rw-rw-rw-   0        0        0     3864 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/TamilGrantha.py
+-rw-rw-rw-   0        0        0     3880 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Telugu.py
+-rw-rw-rw-   0        0        0     4289 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Tirhuta.py
+-rw-rw-rw-   0        0        0     4581 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Urdu.py
+-rw-rw-rw-   0        0        0     4095 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Vatteluttu.py
+-rw-rw-rw-   0        0        0        0 2022-04-20 19:00:42.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-10 19:14:47.232596 aksharamukha-2.2.1/aksharamukha/ScriptMap/NonIndic/
+-rw-rw-rw-   0        0        0     4155 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/NonIndic/Hebrew.py
+-rw-rw-rw-   0        0        0     4427 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/NonIndic/OldPersian.py
+-rw-rw-rw-   0        0        0        0 2022-04-20 19:00:42.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/NonIndic/__init__.py
+-rw-rw-rw-   0        0        0    24451 2022-04-20 19:00:42.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/NonIndic/kana2roman.py
+drwxrwxrwx   0        0        0        0 2024-05-10 19:14:47.274114 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/
+-rw-rw-rw-   0        0        0     3109 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/Aksharaa.py
+-rw-rw-rw-   0        0        0     2991 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/Ariyaka.py
+-rw-rw-rw-   0        0        0     3359 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/AssameseRomanLoC.py
+-rw-rw-rw-   0        0        0     3843 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/Avestan.py
+-rw-rw-rw-   0        0        0     3288 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/BalineseRomanLoC.py
+-rw-rw-rw-   0        0        0     3263 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/BalineseSimpleRomanLoC.py
+-rw-rw-rw-   0        0        0     2950 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/BarahaNorth.py
+-rw-rw-rw-   0        0        0     2950 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/BarahaSouth.py
+-rw-rw-rw-   0        0        0     3364 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/BengaliRomanLoC.py
+-rw-rw-rw-   0        0        0     3369 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/BurmeseRomanLoC.py
+-rw-rw-rw-   0        0        0     3351 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/DevanagariRomanLoC.py
+-rw-rw-rw-   0        0        0     3408 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/GreekModern.py
+-rw-rw-rw-   0        0        0     3353 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/GujaratiRomanLoC.py
+-rw-rw-rw-   0        0        0     3336 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/GurmukhiLoCRomanLoC.py
+-rw-rw-rw-   0        0        0     3409 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/HK.py
+-rw-rw-rw-   0        0        0     3962 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/HanifiRohingya.py
+-rw-rw-rw-   0        0        0     3361 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/IAST.py
+-rw-rw-rw-   0        0        0     3371 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/IASTPali.py
+-rw-rw-rw-   0        0        0     3516 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/IPA.py
+-rw-rw-rw-   0        0        0     3374 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/ISO.py
+-rw-rw-rw-   0        0        0     3380 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/ISOPali.py
+-rw-rw-rw-   0        0        0     1202 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/Inter.py
+-rw-rw-rw-   0        0        0     3412 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/Itrans.py
+-rw-rw-rw-   0        0        0     3271 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/JavaneseRomanLoC.py
+-rw-rw-rw-   0        0        0     3278 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/JavaneseSimpleRomanLoC.py
+-rw-rw-rw-   0        0        0     3368 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/KannadaRomanLoC.py
+-rw-rw-rw-   0        0        0     3358 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/KhmerLoCRomanLoC.py
+-rw-rw-rw-   0        0        0     3352 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/LimbuLoCRomanLoC.py
+-rw-rw-rw-   0        0        0     3241 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/Mongolian.py
+-rw-rw-rw-   0        0        0     3928 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/Mro.py
+-rw-rw-rw-   0        0        0     3354 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/OriyaRomanLoC.py
+-rw-rw-rw-   0        0        0     2991 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/RomanColloquial.py
+-rw-rw-rw-   0        0        0     2944 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/RomanKana.py
+-rw-rw-rw-   0        0        0     3016 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/RomanReadable.py
+-rw-rw-rw-   0        0        0     3457 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/RomanSemitic.py
+-rw-rw-rw-   0        0        0     3526 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/RussianCyrillic.py
+-rw-rw-rw-   0        0        0     2992 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/SLP1.py
+-rw-rw-rw-   0        0        0     3486 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/Santali.py
+-rw-rw-rw-   0        0        0     3328 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/ShanLoCRomanLoC.py
+-rw-rw-rw-   0        0        0     3360 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/SinhalaRomanLoC.py
+-rw-rw-rw-   0        0        0     4110 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/SoraSompeng.py
+-rw-rw-rw-   0        0        0     3365 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/TeluguRomanLoC.py
+-rw-rw-rw-   0        0        0     3371 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/ThamLoCRomanLoC.py
+-rw-rw-rw-   0        0        0     3276 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/TibetanLoCRomanLoC.py
+-rw-rw-rw-   0        0        0     3378 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/Titus.py
+-rw-rw-rw-   0        0        0     3532 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/TolongSiki.py
+-rw-rw-rw-   0        0        0     3543 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/Velthuis.py
+-rw-rw-rw-   0        0        0     3273 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/WX-kok.py
+-rw-rw-rw-   0        0        0     3422 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/WX.py
+-rw-rw-rw-   0        0        0     3802 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/Wancho.py
+-rw-rw-rw-   0        0        0     4040 2024-05-10 18:21:32.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/WarangCiti.py
+-rw-rw-rw-   0        0        0        0 2022-04-20 19:00:42.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/__init__.py
+-rw-rw-rw-   0        0        0        0 2022-04-20 19:00:42.000000 aksharamukha-2.2.1/aksharamukha/ScriptMap/__init__.py
+-rw-rw-rw-   0        0        0        0 2022-04-20 19:00:42.000000 aksharamukha-2.2.1/aksharamukha/__init__.py
+-rw-rw-rw-   0        0        0     2426 2023-01-03 15:36:17.000000 aksharamukha-2.2.1/aksharamukha/demo.py
+-rw-rw-rw-   0        0        0     5103 2023-06-19 19:15:40.000000 aksharamukha-2.2.1/aksharamukha/gimeltra.py
+drwxrwxrwx   0        0        0        0 2024-05-10 19:14:47.275114 aksharamukha-2.2.1/aksharamukha/json/
+-rw-rw-rw-   0        0        0    77047 2024-01-12 16:16:19.000000 aksharamukha-2.2.1/aksharamukha/json/gimeltra_data.json
+drwxrwxrwx   0        0        0        0 2024-05-10 19:14:47.280114 aksharamukha-2.2.1/aksharamukha/test/
+-rw-rw-rw-   0        0        0        0 2023-04-02 22:00:18.000000 aksharamukha-2.2.1/aksharamukha/test/__init__.py
+-rw-rw-rw-   0        0        0     8192 2024-03-06 18:30:06.000000 aksharamukha-2.2.1/aksharamukha/test/loc_burmese_test_cases.py
+-rw-rw-rw-   0        0        0     6118 2024-05-08 23:03:10.000000 aksharamukha-2.2.1/aksharamukha/test/loc_indic_test_cases.py
+-rw-rw-rw-   0        0        0     2843 2024-03-18 16:22:08.000000 aksharamukha-2.2.1/aksharamukha/test/loc_khmer_test_cases.py
+-rw-rw-rw-   0        0        0     3605 2024-03-07 16:31:45.000000 aksharamukha-2.2.1/aksharamukha/test/loc_shan_test_cases.py
+-rw-rw-rw-   0        0        0     1674 2024-04-16 15:17:16.000000 aksharamukha-2.2.1/aksharamukha/test/loc_tham_test_cases.py
+-rw-rw-rw-   0        0        0      664 2023-04-02 23:36:09.000000 aksharamukha-2.2.1/aksharamukha/test/test_file_generator.py
+-rw-rw-rw-   0        0        0     6403 2024-05-09 23:05:02.000000 aksharamukha-2.2.1/aksharamukha/test/testsuite.py
+-rw-rw-rw-   0        0        0    35363 2024-05-10 18:36:41.000000 aksharamukha-2.2.1/aksharamukha/transliterate.py
+-rw-rw-rw-   0        0        0     4664 2024-05-10 19:07:52.000000 aksharamukha-2.2.1/aksharamukha/transliterate_file.py
+drwxrwxrwx   0        0        0        0 2024-05-10 19:14:47.283116 aksharamukha-2.2.1/aksharamukha/yaml/
+-rw-rw-rw-   0        0        0     8250 2022-05-19 16:05:38.000000 aksharamukha-2.2.1/aksharamukha/yaml/aksharamukha-scripts.yaml
+-rw-rw-rw-   0        0        0   189327 2022-05-19 15:32:30.000000 aksharamukha-2.2.1/aksharamukha/yaml/wikitra2-data.yaml
+drwxrwxrwx   0        0        0        0 2024-05-10 19:14:47.134472 aksharamukha-2.2.1/aksharamukha.egg-info/
+-rw-rw-rw-   0        0        0     4648 2024-05-10 19:14:46.000000 aksharamukha-2.2.1/aksharamukha.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7895 2024-05-10 19:14:47.000000 aksharamukha-2.2.1/aksharamukha.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 19:14:46.000000 aksharamukha-2.2.1/aksharamukha.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      155 2024-05-10 19:14:46.000000 aksharamukha-2.2.1/aksharamukha.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-10 19:14:46.000000 aksharamukha-2.2.1/aksharamukha.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-10 19:14:47.285662 aksharamukha-2.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     4561 2024-05-10 19:14:41.000000 aksharamukha-2.2.1/setup.py
```

### Comparing `aksharamukha-2.1.2/PKG-INFO` & `aksharamukha-2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aksharamukha
-Version: 2.1.2
+Version: 2.2.1
 Summary: Provides script conversion (a.k.a transliteration) between various scripts
 Home-page: https://github.com/virtualvinodh/aksharamukha-python
 Author: Vinodh Rajan
 Author-email: vinodh@virtualvindh.com
 License: GNU AGPL 3.0
 Keywords: unicode semitic arabic syriac hebrew indic indian language script brahmi brahmic asian transliteration conversion writing alphabet romanization
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `aksharamukha-2.1.2/README.md` & `aksharamukha-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.1.2/aksharamukha/Convert.py` & `aksharamukha-2.2.1/aksharamukha/Convert.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 from . import GeneralMap as GM, PreProcess as PrP, ConvertFix as CF
 from . import PostProcess as PP
 import aksharamukha.ScriptMap.EastIndic.SiddhamRanjana as SR
-import aksharamukha.ScriptMap.FallBack as FB
+import aksharamukha.FallBack as FB
 import string
 import re
 from functools import cmp_to_key
 import json
 from . import gimeltra
 
 ### Mapping : https://viss.wordpress.com/2015/05/17/how-to-transcribe-pa%E1%B8%B7i-in-lanna-and-burmese/ ###
@@ -39,21 +39,20 @@
     SourceScript = GM.CrunchSymbols(ScriptAll,Source)
     TargetScript = GM.CrunchSymbols(ScriptAll,GM.Inter)
     ScriptMapAll = sorted(zip(SourceScript,TargetScript),key=cmp_to_key(lenSort))
 
     for x,y in ScriptMapAll:
         Strng = Strng.replace(x,y)
 
+    #print(Strng)
+
     return Strng
 
 # Conversion Module
 def convertScript(Strng,Source,Target):
-    #print(Target)
-    #print(Target in GM.IndicScripts)
-
     #print("I am here")
 
     charPairs=[];
     Schwa = '\uF000'
     DepV = '\u1E7F'
 
 
@@ -95,14 +94,15 @@
 
         SourceOld = Source
 
         Strng = convertInter(Strng,Source)
         Source = GM.Inter
         Strng = PrP.RomanPreFix(Strng,Source)
 
+        #print(Strng)
         ## HK l_R l_RR
 
         Strng = Strng.replace("ṿ×_","ṿ")
         Strng = Strng.replace("ṿ×_","ṿ")
 
         ha = GM.CrunchSymbols(GM.Consonants,Source)[32]
         charPairs=[]
@@ -121,16 +121,17 @@
             ScriptMap.sort(reverse=True);
             charPairs= charPairs + ScriptMap
 
         charPairs = sorted(charPairs,key=cmp_to_key(lenSort))
 
         # Perform replacement sequentially for each character group
         for x,y in charPairs:
-            #print x,y
+            #print(x, '-->', y)
             Strng = Strng.replace(x,y)
+            #print(Strng)
 
         ## a_i => a<dev>i<dev> ; a_u = a<dev>u<dev>
         Strng=Strng.replace('_' + GM.CrunchSymbols(GM.Vowels,Target)[2],  GM.CrunchSymbols(GM.Vowels,Target)[2])
         Strng=Strng.replace('_' + GM.CrunchSymbols(GM.Vowels,Target)[4],  GM.CrunchSymbols(GM.Vowels,Target)[4])
 
         ## Joiners Vir + ZWJ
         vir = GM.CrunchList('ViramaMap', Target)[0]
@@ -218,22 +219,24 @@
 
         #Strng = Strng.replace(GM.CrunchList('OmMap', Source)[0],GM.CrunchList('OmMap', Target)[0])
         # Apply Fixes on the Output based on the Script
 
         Strng = CF.FixIndicOutput(Strng, Source, Target)
 
     elif Source in GM.IndicScripts and Target in GM.LatinScripts:
+        #print(Strng)
         Strng = PrP.RemoveJoiners(Strng)
         Strng = CF.ShiftDiacritics(Strng, Source, reverse=True)
+        #print(Strng)
         try:
             Strng = getattr(CF,"Fix"+Source)(Strng,reverse=True)
         except AttributeError:
             pass
             #print #"Fix"+Target+" doesn't exist - Reverse"
-
+        #print(Strng)
         sOm, tOm = GM.CrunchList('OmMap', Source)[0],GM.CrunchList('OmMap', Target)[0]
 
         Strng = Strng.replace(sOm, tOm)
 
         # Iterate for each character group
         for charList in GM.ScriptAll:
             # Crunch all related characters into a list
@@ -264,18 +267,19 @@
                 if x in unasp:
                     Strng = re.sub(x + '(?!(ʰ|\u0324))', y, Strng)
                 else:
                     Strng = Strng.replace(x,y)
         # for all other transformations
         else:
             # Perform replacement sequentially for each character group
+            #print(Strng)
             for x,y in charPairs:
-                #print(x + " : " + y)
                 Strng = Strng.replace(x,y)
 
+
         # Remove all intermediate characters and fix Output
         Strng = CF.FixRomanOutput(Strng,Target)
 
         Strng = CF.VedicSvarsIndicLatin(Strng)
 
         Strng = CF.PostFixRomanOutput(Strng,Source,Target)
 
@@ -302,14 +306,16 @@
     elif Source in (GM.IndicScripts + GM.LatinScripts) and Target in GM.SemiticScripts:
         tr = gimeltra.Transliterator()
 
         Strng = convertScript(Strng, Source, "RomanSemitic")
 
         # print("The string is", Strng)
 
+        #print(Strng)
+
         Strng = Strng.replace('QQ', '').replace('mQ', '') ## avoiding Q, mQ for Urdu to Semitic : Check why
 
         # remove gemination for every script except......
         ## Add all scripts with gemination sign here or vowel killer here
         ## Syriac doesn't show gemination hence not added below
         if 'Arab' not in Target and 'Hebr' not in Target and 'Latn' not in Target:
             Strng = re.sub('(.)' + '\u033D' + r'\1', r'\1', Strng)
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ConvertFix.py` & `aksharamukha-2.2.1/aksharamukha/ConvertFix.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 from . import GeneralMap as GM
 from aksharamukha.ScriptMap.Roman import Avestan, IAST
 from aksharamukha.ScriptMap.MainIndic import Ahom, Tamil,TamilGrantha, Limbu, MeeteiMayek, Urdu, Lepcha, Chakma, Kannada, Gurmukhi, Newa
-from aksharamukha.ScriptMap.EastIndic import Lao, TaiTham,Tibetan,Burmese,Khmer,Balinese,Javanese,Thai, Sundanese, PhagsPa, Cham, Thaana, Rejang, ZanabazarSquare, Makasar
+from aksharamukha.ScriptMap.EastIndic import Lao, TaiTham,Tibetan,Burmese,Khmer,Balinese,Javanese,Thai, Sundanese, PhagsPa, Cham, Thaana, Rejang, ZanabazarSquare, Makasar, Kawi
 from . import PostProcess
 import re
 
 ## Test Syllable initial conjunct
 
 ## ListC check.. if LLA is there in ListC... just now it has only Consonant Map
 ### Rewrite all ListC, ListV as sorted(List,key=len,reverse=True)
@@ -335,18 +335,25 @@
 
     if Target == "HanifiRohingya":
         Strng = FixHanifiRohingya(Strng)
 
     if Target == "Mongolian":
         Strng = FixMongolian(Strng)
 
+    if Target == "Itrans":
+        Strng = re.sub('([aAiIuUeo])(RR)(i|I)', r'\1'+'R_L' + r'\3', Strng)
+        Strng = re.sub('([aAiIuUeo])(LL)(i|I)', r'\1'+'L_L'+ r'\3', Strng)
+
     if Source == "RomanSemitic":
         pass
         #Strng = Strng.replace('a̤', '\u0324')
 
+    if Source in ['IAST','ISO'] and Target == 'Malayalam':
+        Strng = Strng.replace('ṯ', 'ṟ')
+
     return Strng
 
 def FixSemiticOutput(Strng,Source,Target):
     Strng = Strng.replace('\u02DE', '') ## dummy
     try:
         Strng = globals()["Fix"+Target.replace('-','_')](Strng, Source)
     except KeyError:
@@ -610,15 +617,17 @@
         Strng = re.sub(consonants + consonants + vowels + '(\u1880)', r'\4\1\2\3', Strng)
         Strng = re.sub(consonants + '?' + vowels + '(\u1880)', r'\3\1\2', Strng)
         Strng = Strng.replace(' \u02BC', '\u200B')
         Strng = Strng.replace('\u02BC', '\u200B')
 
     else:
         ## add variation seelct one
-        Strng = re.sub('(ᠠ)(?<!\u180B)', r'\1' + '\u180B', Strng)
+        #print(Strng)
+        Strng = re.sub('(ᠠ)(?!\u180B)', r'\1' + '\u180B', Strng)
+        #print(Strng)
 
     return Strng
 
 def FixHanifiRohingya(Strng, reverse=False):
     consList = '(' + '|'.join(GM.CrunchSymbols(GM.Consonants, 'HanifiRohingya')+['\U00010D17', '\U00010D19']) + ')'
     vowList = '(' + '|'.join(GM.CrunchSymbols(GM.Vowels, 'HanifiRohingya')) + ')'
 
@@ -905,14 +914,16 @@
         Strng = PostProcess.RetainDandasIndic(Strng, 'Tamil', True)
         Strng = PostProcess.RetainIndicNumerals(Strng, 'Tamil', True)
 
         for x in TamilDiacritic:
             for y in VedicSign:
                 Strng = Strng.replace(x + y, y + x)
     else:
+        Strng = PostProcess.RetainDandasIndic(Strng, 'Tamil')
+        Strng = PostProcess.RetainIndicNumerals(Strng, 'Tamil')
         Strng = Strng.replace(avaA,ava+ava)
         Strng = Strng.replace('ஷ²', 'ஶ')
 
         Strng = Strng.replace('𑌃', '꞉')
 
         for x in TamilDiacritic:
             for y in VedicSign:
@@ -924,14 +935,42 @@
     if not reverse:
         pass
     else:
         Strng = Strng.replace('ଵ','ୱ')
 
     return Strng
 
+def FixGurmukhiLoC(Strng,reverse=False):
+    Strng = CorrectRuLu(Strng,"Gurmukhi",reverse)
+
+    ava = Gurmukhi.SignMap[0]
+    avaA = '\u0028\u0A06\u0029'
+
+    # Tippi/Bindu conversion options are optional. Look into PostProcess
+
+    if not reverse:
+        Strng = Strng.replace(ava+ava,avaA)
+        Strng = PostProcess.InsertGeminationSign(Strng, 'Gurmukhi')
+        Strng = PostProcess.RetainIndicNumerals(Strng, 'Gurmukhi', True)
+
+        Vedicomp = '([' + ''.join(GM.VedicSvarasList) + '])'
+
+        Strng = re.sub(Vedicomp + '\u0A71' + '(.)', r'\1' + r'\2' + Gurmukhi.ViramaMap[0] + r'\2' , Strng)
+
+    else:
+        Strng = PostProcess.RetainIndicNumerals(Strng, 'Gurmukhi')
+        Strng = Strng.replace(avaA,ava+ava)
+        Strng = PostProcess.ReverseGeminationSign(Strng, 'Gurmukhi')
+        #Strng = Strng.replace('ੰਨ','ਨ੍ਨ')
+        #Strng = Strng.replace('ੰਮ','ਮ੍ਮ')
+        # Replace Tippi by Bindu
+        #Strng = PostProcess.GurmukhiYakaash(Strng, True)
+
+    return Strng
+
 # Correct Ru'', Lu'' -> R, lR
 # Tippi/Bindu
 def FixGurmukhi(Strng,reverse=False):
     Strng = CorrectRuLu(Strng,"Gurmukhi",reverse)
 
     ava = Gurmukhi.SignMap[0]
     avaA = '\u0028\u0A06\u0029'
@@ -944,14 +983,15 @@
         Strng = PostProcess.RetainIndicNumerals(Strng, 'Gurmukhi', True)
 
         Vedicomp = '([' + ''.join(GM.VedicSvarasList) + '])'
 
         Strng = re.sub(Vedicomp + '\u0A71' + '(.)', r'\1' + r'\2' + Gurmukhi.ViramaMap[0] + r'\2' , Strng)
 
     else:
+        Strng = PostProcess.RetainIndicNumerals(Strng, 'Gurmukhi')
         Strng = Strng.replace(avaA,ava+ava)
         Strng = PostProcess.ReverseGeminationSign(Strng, 'Gurmukhi')
         Strng = Strng.replace('ੰਨ','ਨ੍ਨ')
         Strng = Strng.replace('ੰਮ','ਮ੍ਮ')
         # Replace Tippi by Bindu
         Strng = Strng.replace('\u0A70','\u0A02')
         Strng = PostProcess.GurmukhiYakaash(Strng, True)
@@ -1036,35 +1076,42 @@
         Strng = re.sub('\u200B'+TamilGrantha.SouthVowelSignMap[0]+'('+ListC+')'+TamilGrantha.VowelSignMap[0],r'\1'+ListOAU[2],Strng)
         Strng = re.sub('\u200B'+TamilGrantha.SouthVowelSignMap[0]+'('+ListC+')'+Tamil.SouthConsonantMap[0],r'\1'+ListOAU[1],Strng)
         # k + VS e/E/ai <- Joiners + VS e/E/ai + k
         Strng = re.sub('\u200B'+'('+ListEAI+')'+'('+ListC+')',r'\2\1',Strng)
 
     return Strng
 
+def FixKhmerLoC(Strng,reverse=False):
+    return FixKhmer(Strng, reverse, target="KhmerLoC")
+
 # Khmer - Subjoining Consonants and Repha
-def FixKhmer(Strng,reverse=False):
-    ListC ='|'.join(GM.CrunchSymbols(GM.Consonants,'Khmer'))
+def FixKhmer(Strng,reverse=False, target="Khmer"):
+    ListC ='|'.join(GM.CrunchSymbols(GM.Consonants,target))
+    ListV ='|'.join(GM.CrunchSymbols(GM.VowelSigns,target))
+    ListA ='|'.join(GM.CrunchSymbols(GM.CombiningSigns,target))
+
     ra = Khmer.ConsonantMap[26]
     vir = Khmer.ViramaMap[0]
 
     if not reverse:
         # Replace Explicit Virama + Cons -> Subjoining Virama + Cons
         Strng = re.sub(vir+'('+ListC+')','\u17D2'+r'\1',Strng)
         # Introduce Repha : ra + sub Virama + Cons -> Cons + Repha
         Strng = re.sub('(?<!\u17D2)('+ra+')'+'\u17D2'+'('+ListC+')',r'\2'+'\u17CC',Strng)
         # i + Anusara -> i-Anusvara ligature
-        Strng = Strng.replace('\u1787\u17C6','\u17B9')
+        Strng = Strng.replace('\u17B7\u17C6','\u17B9')
+
     else:
         # Replace Subjoining Virama with Explicit Virama
         Strng = Strng.replace('\u17D2',vir)
         Strng = re.sub(vir+'(?=[\u17AB\u17AC\u17AD\u17AE])','\u17D2',Strng)
         # Remove Repha : ra + sub Virama + Cons <- Cons + Repha
         Strng = re.sub('('+ListC+')'+'\u17CC',ra+vir+r'\1',Strng)
         # i + Anusara -> i-Anusvara ligature
-        Strng = Strng.replace('\u17B9','\u1787\u17C6')
+        Strng = Strng.replace('\u17B9','\u17B7\u17C6')
 
     return Strng
 
 def FixKhamtiShan(Strng, reverse=False):
     if not reverse:
         Strng = Strng.replace('်ရ', 'ြ')
         Strng = Strng.replace('်ယ', 'ျ')
@@ -1112,22 +1159,25 @@
     return Strng
 
 def FixShan(Strng, reverse=False):
     if not reverse:
         Strng = Strng.replace('်ရ', 'ြ')
         Strng = Strng.replace('်ယ', 'ျ')
         Strng = Strng.replace('်ဝ', '\u1082')
-        Strng = Strng.replace('်ႁ', 'ှ')
+        #Strng = Strng.replace('်ႁ', 'ှ')
 
         ## Maintain the order of the medials
         Strng = re.sub('(ှ)' + '([ျြွ])', r'\2\1', Strng)
         Strng = Strng.replace("\u103C\u103B", "\u103B\u103C")
         Strng = Strng.replace("\u103D\u103B", "\u103B\u103D")
         Strng = Strng.replace("ွ\u103C", "\u103Cွ")
 
+        ## Fix Shya
+        Strng = re.sub('သျ\u02BD?ျ', 'သျ်ယ', Strng)
+
     else:
         ## Reverse the order of the medials
         Strng = re.sub('([ျြွ])' + '(ှ)', r'\2\1', Strng)
         Strng = Strng.replace("\u103B\u103C", "\u103C\u103B")
         Strng = Strng.replace("\u103B\u103D", "\u103D\u103B")
         Strng = Strng.replace("\u103Cွ", "ွ\u103C")
 
@@ -1350,14 +1400,113 @@
 
 # Balinese Repha
 def FixBalinese(Strng,reverse=False):
     Repha = '\u1B03'
 
     Strng = AddRepha(Strng,"Balinese",Repha,reverse)
 
+    if not reverse:
+        pass
+    else:
+        # reversing archaic jna
+        Strng = Strng.replace('ᭌ', 'ᬚ᭄ᬜ')
+        # Fix a-based vowels
+        vowelsA = ['ᬅᬶ', 'ᬅᬷ', 'ᬅᬸ', 'ᬅᬹ', 'ᬅᬺ', 'ᬅᬻ', 'ᬅ᭄ᬮᭂ', 'ᬅ᭄ᬮᭃ', 'ᬅᬾ', 'ᬅᬿ', 'ᬅᭀ', 'ᬅᭁ']
+        vowels = ['ᬇ', 'ᬈ', 'ᬉ', 'ᬊ', 'ᬋ', 'ᬌ', 'ᬍ', 'ᬎ', 'ᬏ', 'ᬐ', 'ᬑ', 'ᬒ']
+
+        for v, vA in zip(vowels, vowelsA):
+            Strng = Strng.replace(vA, v)
+
+    return Strng
+
+# Javanese - Reppha & Subjoining ra & ya
+def FixDivesAkuru(Strng,reverse=False):
+    target = 'DivesAkuru'
+
+    ListC ='|'.join(GM.CrunchSymbols(GM.Consonants,target)+['\U00011926'])
+    ListV ='|'.join(GM.CrunchSymbols(GM.VowelSigns,target))
+    ListA ='|'.join(GM.CrunchSymbols(GM.CombiningSigns,target))
+
+    ra = GM.CrunchSymbols(GM.Consonants,target)[26]
+    ya = GM.CrunchSymbols(GM.Consonants,target)[25]
+    vir = GM.CrunchSymbols(GM.virama,target)[0]
+    combVir = '\U0001193E'
+    aVS = '\U00011F34'
+
+    if not reverse:
+        # Replace Explicit Virama + Cons -> Subjoining Virama + Cons
+        Strng = re.sub(vir+'('+ListC+')', combVir+r'\1',Strng)
+        # Replace Explicit Virama + Cons -> Subjoining Virama + Cons
+        Strng = re.sub(combVir +ra, '\U00011942',Strng)
+        # Replace Explicit Virama + Cons -> Subjoining Virama + Cons
+        Strng = re.sub(combVir +ya, '\U00011940',Strng)
+        # Introduce Repha : ra + sub Virama + Cons -> Cons + Repha
+        Strng = re.sub('(?<!\U0001193E)'+ra+'\U0001193E'+'('+ListC+')','\U00011941'+r'\1',Strng)
+    else:
+        # reverse homonasal
+        homoNasal = '\U0001193F'
+
+        Strng = re.sub(homoNasal+'(?=[𑤌𑤍𑤎𑤏])', '𑤐\U0001193E', Strng)
+        Strng = re.sub(homoNasal+'(?=[𑤑𑤒𑤓])', '𑤕\U0001193E', Strng)
+        Strng = re.sub(homoNasal+'(?=[𑤖𑤘𑤙])', '𑤚\U0001193E', Strng)
+        Strng = re.sub(homoNasal+'(?=[𑤛𑤜𑤝𑤞])', '𑤟\U0001193E', Strng)
+        Strng = re.sub(homoNasal+'(?=[𑤠𑤡𑤢𑤣])', '𑤤\U0001193E', Strng)
+
+        # reverse the joning virama
+        Strng = Strng.replace(combVir, vir)
+        # replace alter. ya
+        Strng = Strng.replace("\U00011926", "\U00011925")
+        # Reverse : Replace Explicit Virama + Cons -> Subjoining Virama + Cons
+        Strng = re.sub(combVir, vir, Strng)
+        # Reverse : Replace Explicit Virama + Cons -> Subjoining Virama + Cons
+        Strng = re.sub('\U00011942', vir +ra, Strng)
+        # Reverse : Replace Explicit Virama + Cons -> Subjoining Virama + Cons
+        Strng = re.sub('\U00011940', vir +ya, Strng)
+        # Reverse : Introduce Repha : ra + sub Virama + Cons -> Cons + Repha
+        Strng = re.sub('\U00011941', vir +ra, Strng)
+
+
+    return Strng
+
+# Javanese - Reppha & Subjoining ra & ya
+def FixKawi(Strng,reverse=False):
+    target = 'Kawi'
+
+    ListC ='|'.join(GM.CrunchSymbols(GM.Consonants,target))
+    ListV ='|'.join(GM.CrunchSymbols(GM.VowelSigns,target))
+    ListA ='|'.join(GM.CrunchSymbols(GM.CombiningSigns,target))
+
+    ra = Kawi.ConsonantMap[26]
+    vir = Kawi.ViramaMap[0]
+    aVS = '\U00011F34'
+    aVSAlt = '\U00011F35'
+
+    if not reverse:
+        # Replace Explicit Virama + Cons -> Subjoining Virama + Cons
+        Strng = re.sub(vir+'('+ListC+')','\U00011F42'+r'\1',Strng)
+        # Introduce Repha : ra + sub Virama + Cons -> Cons + Repha
+        Strng = re.sub('(?<!\U00011F42)'+ra+'\U00011F42'+'('+ListC+')','\U00011F02'+r'\1',Strng)
+        #special AA
+        consA = ['\U00011F26', '\U00011F16', '\U00011F1C']
+        for cons in consA:
+            Strng = Strng.replace(cons + aVS, cons + aVSAlt)
+    else:
+        # Replace Subjoining Virama with Explicit Virama
+        Strng = Strng.replace('\U00011F42',vir)
+        # Replace Repha
+        Strng = Strng.replace('\U00011F02', ra + vir)
+        # reverse AltA
+        Strng = Strng.replace(aVSAlt, aVS)
+        # reverse JNA
+        Strng = Strng.replace('\U00011F33', '𑼙𑽂𑼛')
+        # decompose ind.vowels
+        Strng = Strng.replace('\U00011F04\U00011F34', '\U00011F05').replace('\U00011F06\U00011F34', '\U00011F07').replace('\U00011F08\U00011F34', '\U00011F09')
+        # reverse Alt ai, alt au
+        Strng = Strng.replace('\U00011F3E\U00011F3E', '\U00011F3F')
+
     return Strng
 
 # Javanese - Reppha & Subjoining ra & ya
 def FixJavanese(Strng,reverse=False):
     Repha = '\uA982'
     vir = Javanese.ViramaMap[0]
     ra, ya = Javanese.ConsonantMap[26], Javanese.ConsonantMap[25]
@@ -1365,16 +1514,29 @@
 
     Strng = AddRepha(Strng,"Javanese",Repha,reverse)
 
     if not reverse:
         # Introduce subjoining Ra & Ya
         Strng = Strng.replace(vir+ra,SubRa).replace(vir+ya,SubYa)
     else:
+        #Fix Archaic Jna
+        Strng = Strng.replace('ꦘ', 'ꦗ꧀ꦚ')
+        # Fix ra agang
+        Strng = Strng.replace('ꦬ', ra)
         # Replace Subjoining forms with cons+vir
         Strng = Strng.replace(SubRa,vir+ra).replace(SubYa,vir+ya)
+        # reversing archaic jna
+        Strng = Strng.replace('ᭌ', 'ᬚ᭄ᬜ')
+        # reverse a-based vowels
+        vowelsA = ['ꦄꦶ', 'ꦄꦷ', 'ꦄꦸ', 'ꦄꦹ', 'ꦄꦽ', 'ꦄ꧀ꦉꦴ', 'ꦄ꧀ꦭꦼ', 'ꦄ꧀ꦭꦼꦴ', 'ꦄꦺ', 'ꦄꦻ', 'ꦄꦺꦴ', 'ꦄꦻꦴ']
+        vowels = ['ꦆ', 'ꦇ', 'ꦈ', 'ꦈꦴ', 'ꦉ', 'ꦉꦴ', 'ꦊ', 'ꦋ', 'ꦌ', 'ꦍ', 'ꦎ', 'ꦎꦴ']
+
+        for v, vA in zip(vowels, vowelsA):
+            Strng = Strng.replace(vA, v)
+
 
     return Strng
 
 
 def FixUrdu(Strng, reverse=False):
     return FixUrduShahmukhi("Urdu", Strng, reverse)
 
@@ -1410,14 +1572,18 @@
     if not reverse:
         ## Fixing Hamza
 
         ListVS = '(' + '|'.join(GM.CrunchSymbols(GM.VowelSigns,Target)) + ')'
         ListV = '(' + '|'.join(GM.CrunchSymbols(GM.Vowels,Target)) + ')'
         ListVSA = '(' + '|'.join(GM.CrunchSymbols(GM.VowelSigns,Target)+[a]) + ')'
 
+        ListC = '(' + '|'.join(GM.CrunchSymbols(GM.Consonants,Target)) + ')'
+        # Fix NunGhunna
+        Strng = re.sub('(\u06BA\u02BD?)' + ListC, '\u0646\u0658' + r'\2', Strng)
+
         hamzaFull = "\u0621"
         hamzaChair = "\u0626"
 
         Strng = re.sub(ListVS + ListV, r'\1' + hamzaFull + r'\2', Strng)
         Strng = re.sub(ListV + ListV, r'\1' + hamzaFull + r'\2', Strng)
         Strng = re.sub('('+a+')' + ListV +'(?!' + ListVSA + ')'   , r'\1' + hamzaFull + r'\2', Strng)
 
@@ -1492,19 +1658,25 @@
         ## Fix Retroflex with combining characters
         Strng = Strng.replace('ࣇ', 'لؕ')
 
         if Target == 'Shahmukhi':
             #aspirated nasals and liquids
             Strng = re.sub('(ن|م|ی|ر|ل|و)(\u0652)(ہ)',r'\1'+'\u06BE', Strng)
 
+        # Fix word-final ha
+
+
     else:
         #print('I am being called')
         if True:
             #print(Strng)
 
+            #Fix Nun Ghuunnai
+            Strng = Strng.replace('\u0646\u0658', '\u06BA')
+
             ## replace chaschmee ha with regular ha when not surrounded preceeded by consonnants
             Strng = re.sub('(\s)\u06BE',r'\1'+'ہ', Strng)
 
             #decompose hamza with long e
             Strng = Strng.replace('ۓ', '_\u06d2')
 
             if Target == 'Shahmukhi':
@@ -1696,16 +1868,19 @@
     if not reverse:
         Strng = Strng.replace('ꢒ꣄ꢰ', 'ꢒ꣄‍ꢰ') # Ksha
     else:
         Strng = Strng.replace('ꢴ','꣄ꢲ')
 
     return Strng
 
+def FixTibetanLoC(Strng,reverse=False):
+    return FixTibetan(Strng,reverse, swapNative=False)
+
 # Tibetan Subjoining Consnants
-def FixTibetan(Strng,reverse=False):
+def FixTibetan(Strng,reverse=False, swapNative = True):
     ListC = [Tibetan.ViramaMap[0]+chr(x) for x in range(0x0F40,0x0F68)] # Consonants
     ListSubC = [chr(x+80) for x in range(0x0F40,0x0F68)] # Subjoined Consonants
 
     SubC = ["ཝྭ","ཡྱ","རྱ","རྭ", "ྺྭ"]
     SubMinC = ["ཝྺ","ཡྻ","ཪྻ","ཪྺ", "ྺྺ"]
 
     if not reverse:
@@ -1726,16 +1901,14 @@
         Strng = Strng.replace("}", "༽")
 
 
     if reverse:
         AspirateDecom= ["གྷ", "ཌྷ", "དྷ", "བྷ", "ཛྷ", "ྒྷ", "ྜྷ", "ྡྷ", "ྦྷ", "ྫྷ"]
         AspirateAtomic = ["གྷ", "ཌྷ", "དྷ", "བྷ", "ཛྷ", "ྒྷ", "ྜྷ", "ྡྷ", "ྦྷ", "ྫྷ"]
 
-        Strng = Strng.replace('ཇྷ', 'ཛྷ') ## JHA -> DZHA
-
         for x, y in zip(AspirateDecom, AspirateAtomic):
             Strng = Strng.replace(x, y)
 
         for x,y in zip(SubC,SubMinC):
             Strng = Strng.replace(y,x)
 
         for x,y in zip(ListC,ListSubC):
@@ -1750,18 +1923,21 @@
 
         Strng = Strng.replace("༺", "(")
         Strng = Strng.replace("༻", ")")
 
         Strng = Strng.replace("༼", "{")
         Strng = Strng.replace("༽", "}")
 
-        Strng = Strng.replace("འ", "ཨ")
-        Strng = Strng.replace("ཇ", "ཛ")
-
-        Strng = Strng.replace("ཞ", "ཛྷ༹")
+        if swapNative:
+            Strng = Strng.replace('ཇྷ', 'ཛྷ') ## JHA -> DZHA
+            Strng = Strng.replace("ཇ", "ཛ")
+            Strng = Strng.replace('ཅ', 'ཙ')
+            Strng = Strng.replace('ཆ', 'ཚ')
+            Strng = Strng.replace("ཞ", "ཛྷ༹")
+            Strng = Strng.replace("འ", "ཨ")
 
     return Strng
 
 # Thai, Lao follow visual ordering of Vowels signs ; <e> + k => <e>k
 # Other Indic scripts follow logical order ; k + <e> => <e>k
 # Swapping Vowel Signs for conversion
 def ReverseVowelSigns(Strng,Script,reverse=False):
@@ -1859,20 +2035,23 @@
         Strng= Strng.replace("\u0EB3","\u0EB2\u0ECD")
 
     return Strng
 
 def FixMakasar(Strng, reverse=False):
 
     ListC = "|".join(Makasar.ConsonantMap)
-    ListV = "|".join(Makasar.VowelSignMap)
+    #ListV = "|".join(Makasar.VowelSignMap)
+    #print(ListV)
+    ListV = "|".join(['\U00011EF3', '\U00011EF4', '\U00011EF5', '\U00011EF6'])
     Anka = '\U00011EF2'
+    #print(Makasar.VowelSignMap)
 
     if not reverse:
         Strng = PostProcess.InsertGeminationSign(Strng, 'Makasar')
-        Strng = Strng.replace('\u02BE', '')
+        Strng = Strng.replace('\u02BE', '').replace('\u02BD', '')
         Strng = re.sub('(' + ListC + ')' + '(' + ListV + ')?' + r'\1', r'\1' + r'\2' + Anka, Strng)
     else:
         Strng = re.sub('(' + ListC + ')' + '(' + ListV + ')?' + Anka, r'\1' + r'\2' + r'\1', Strng)
 
     return Strng
 
 def FixAvestan(Strng, reverse=False):
@@ -2161,19 +2340,23 @@
 
     return kharnum
 
 def FixSinhala(Strng,reverse=False):
     Strng = PostProcess.SinhalaDefaultConjuncts(Strng)
 
     if not reverse:
+        #sinhala numerals
+        Strng = PostProcess.RetainIndicNumerals(Strng, 'Sinhala', True)
         #Sinhala JNA
         Strng = Strng.replace("\u0DA2\u0DCA\u0DA4","\u0DA5")
         #sinhala
         Strng = Strng.replace("(අ)(අ)","(ආ)")
     else:
+        #sinhala numerals
+        Strng = PostProcess.RetainIndicNumerals(Strng, 'Sinhala')
         Strng = Strng.replace("\u0DA5","\u0DA2\u0DCA\u0DA4")
         ## Remove joiners
         Strng = Strng.replace("‍","")
         Strng = Strng.replace("(ආ)","(අ)(අ)")
 
 
     return Strng
@@ -2218,15 +2401,18 @@
 
         Strng = Strng.replace("Mk", "ngk")
         Strng = Strng.replace("Mg", "ngg")
         Strng = Strng.replace("Mc", "njc")
         Strng = Strng.replace("Mj", "njj")
         Strng = Strng.replace("Md", "nd")
         Strng = Strng.replace("Mt", "nt")
-        Strng = Strng.replace("M", 'm')
+        Strng = Strng.replace("Mb", "mb")
+        Strng = Strng.replace("Mp", "mp")
+
+        Strng = Strng.replace("M", 'm\u034F\'')
 
         Strng = Strng.replace("ngk", "nk")
         Strng = Strng.replace("ngg", "ng")
         Strng = Strng.replace("njc", "nc")
         Strng = Strng.replace("njj", "nj")
 
         Strng = Strng.replace("jnj", "jny")
@@ -2248,15 +2434,18 @@
 
         Strng = Strng.replace("Mk", "ngk")
         Strng = Strng.replace("Mg", "ngg")
         Strng = Strng.replace("Mc", "njc")
         Strng = Strng.replace("Mj", "njj")
         Strng = Strng.replace("Md", "nd")
         Strng = Strng.replace("Mt", "nt")
-        Strng = Strng.replace("M", 'm')
+        Strng = Strng.replace("Mb", "mb")
+        Strng = Strng.replace("Mp", "mp")
+
+        Strng = Strng.replace("M", 'm\u034F')
 
         Strng = Strng.replace("ngk", "nk")
         Strng = Strng.replace("ngg", "ng")
         Strng = Strng.replace("njc", "nc")
         Strng = Strng.replace("njj", "nj")
 
         Strng = Strng.replace("jnj", "jny")
@@ -2320,14 +2509,22 @@
         ## Remove a if necessary
         Strng = Strng.replace('𑣁' + '\u02BB', '')
 
         Strng = Strng.replace('\U000118C1\u00BD', '\U000118C1\U000118D9\u02BE')
 
     return Strng
 
+def FixLimbuLoC(Strng, reverse=False):
+    Strng = FixLimbu(Strng, reverse)
+    if reverse:
+        Strng = Strng.replace('ʔ', '᤹')
+        Strng = Strng.replace('꞉', '’')
+
+    return Strng
+
 #Subojined & Final
 def FixLimbu(Strng,reverse=False):
     vir = Limbu.ViramaMap[0]
 
     SCons = [vir+x for x in [Limbu.ConsonantMap[x] for x in [25,26,28]]]  # /ya/, /ra/, /va/
     SubCons = ['\u1929','\u192A','\u192B']
 
@@ -2378,55 +2575,58 @@
     return Strng
 
 
 def FixDevanagari(Strng, reverse=False):
     Sindhi = ['ॻ','ॼ','ॾ','ॿ']
     SindhiApprox = ['ˍग','ˍज','ˍड','ˍब']
     if not reverse:
+        #print(Strng)
+
         Strng = Strng.replace('ʔ', 'ॽ')
 
         for x, y in zip(Sindhi, SindhiApprox):
             Strng = Strng.replace(y, x)
 
         Strng = Strng.replace('ज़़','ॹ')
         Strng = Strng.replace('श़','ॹ')
         Strng = Strng.replace('ऱ्', 'ऱ्‌') ## Prevent RRA from forming conjuncts
 
         ## Except for YA and HA
-
         Strng = Strng.replace('ऱ्‌य', 'ऱ्य')
         Strng = Strng.replace('ऱ्‌ह', 'ऱ्ह')
 
         # Kashmiri ux, uux
 
-        Strng = Strng.replace('उʼ', 'ॶ').replace('ऊʼ', 'ॷ').replace('ुʼ', 'ॖ').replace('ूʼ','ॗ')
+        #Strng = Strng.replace('उʼ', 'ॶ').replace('ऊʼ', 'ॷ').replace('ुʼ', 'ॖ').replace('ूʼ','ॗ')
 
         # Kashmir oe oe
 
-        Strng = Strng.replace('अʼ', 'ॳ').replace('आʼ', 'ॴ')
+        #Strng = Strng.replace('अʼ', 'ॳ').replace('आʼ', 'ॴ')
 
         ListC ='|'.join(GM.CrunchSymbols(GM.Consonants,'Devanagari'))
 
         Strng = re.sub('(' + ListC + ')' + 'ʼ', r'\1' + '\u093A', Strng)
         Strng = Strng.replace('\u093Eʼ','\u093B')
 
     else:
+        # remove schwa accent
+        Strng = Strng.replace('\u0954', '')
+
         Strng = PostProcess.DevanagariPrishtamatra(Strng, reverse=True)
         Strng = Strng.replace('ॽ', 'ʔ')
         Strng = Strng.replace('ॹ', 'ज़़')
 
         for x, y in zip(Sindhi, SindhiApprox):
             Strng = Strng.replace(x, y)
 
         # Kashmiri ux, uux
-
-        Strng = Strng.replace('ॶ', 'उʼ').replace('ॷ', 'ऊʼ').replace('ॖ', 'ुʼ').replace('ॗ', 'ूʼ')
+        #Strng = Strng.replace('ॶ', 'उʼ').replace('ॷ', 'ऊʼ').replace('ॖ', 'ुʼ').replace('ॗ', 'ूʼ')
 
         # oe
-        Strng = Strng.replace('ॳ', 'अʼ').replace('ॴ', 'आʼ').replace('\u093B', '\u093Eʼ').replace('\u093A','ʼ')
+        #Strng = Strng.replace('ॳ', 'अʼ').replace('ॴ', 'आʼ').replace('\u093B', '\u093Eʼ').replace('\u093A','ʼ')
 
 
     return Strng
 
 def FixKaithi(Strng, reverse=False):
     if not reverse:
         Strng = Strng.replace(' ', '⸱')
@@ -2476,15 +2676,15 @@
             Strng = Strng.replace(y,x)
 
     ## Word Final Consonants
 
     ## Consider adding -u instead of mass replacement [for Cham too] !
 
     listNF = [Lepcha.ConsonantMap[x] for x in [1,2,3,4,5,6,7,8,9,10,11,12,13,14,16,17,18,21,22,23,29,30,31]]
-    listF = [(Lepcha.ConsonantMap+Lepcha.AyogavahaMap)[x] for x in [0,0,0,34,0,0,0,0,19,15,15,15,15,19,15,15,15,20,20,20,15,15,15]]
+    listF = [(Lepcha.ConsonantMap[:33]+Lepcha.AyogavahaMap)[x] for x in [0,0,0,34,0,0,0,0,19,15,15,15,15,19,15,15,15,20,20,20,15,15,15]]
 
     listNF += Lepcha.ConsonantMap[25:26]+Lepcha.ConsonantMap[28:29]
     listF += Lepcha.VowelMap[2:3] + Lepcha.VowelMap[4:5]
 
     if not reverse:
         # Remove Nukta if it appears with Virama
         # ka + Q + Viramam -> ka + virama
@@ -2496,38 +2696,44 @@
 
 
     else:
         pass # Irreversible
 
     conFinal = [x+vir for x in [Lepcha.ConsonantMap[c] for c in [0,15,19,20,24,26,27]]]
     conF = ['\u1C2D','\u1C33','\u1C30','\u1C31','\u1C2E','\u1C32','\u1C2F',]
+    finConsList = ''.join(conF)
 
     signAll = '|'.join(GM.CrunchSymbols(GM.Consonants+GM.Vowels+GM.VowelSignsNV, "Lepcha"))
 
     for x,y in zip(conFinal,conF):
         if not reverse:
             # Replace final consonants
             Strng = re.sub('('+signAll+')'+'('+x+')',r'\1'+y,Strng)
         else:
+            # KIp ᰀᰧᰱᰶ -> rang, final consonant
+            Strng = re.sub('([' + finConsList + '])' + '(ᰶ)', r'\2\1', Strng)
             Strng = Strng.replace(y,x)
 
     # Remove Virama - Lepcha doesn't have virama ?
 
     signVow = '|'.join(GM.CrunchSymbols(GM.VowelSignsNV,"Lepcha"))
 
     if not reverse:
         Strng = Strng.replace(vir,'') ## Removing faux Virama
         # Using Sign Kang with Vowel Signs
         # Inherent Consonant uses 1C34
         # kiM -> ki + 1C35 ; kaM -> ka + 1C34
         Strng = re.sub("("+signVow+')'+'('+Lepcha.AyogavahaMap[1]+')',r'\1'+'\u1C35',Strng)
         Strng = Strng.replace("ᰧᰶᰵ", "ᰧᰵᰶ") ## Fiximg IM issues kIM swap the Ran and M to display it better
+        # swap rang + final con - unicode ordering to get the correct rendering
+        # kIP -> ᰀᰧᰱᰶ
+        Strng = re.sub('(ᰶ)' + '([' + finConsList + '])', r'\2\1', Strng)
     else:
         Strng = Strng.replace('\u1C35',Lepcha.AyogavahaMap[1])
-        Strng = Strng.replace("ᰧᰵᰶ","ᰧᰶᰵ") ## Fiximg IM issues kIM swap the Ran and M to display it better
+        Strng = Strng.replace("\u1C34\u1C36","\u1C36\u1C34") ## Fiximg IM issues kIM swap the Ran and M to display it better
 
     return Strng
 
 # Repha & Subjoined
 def FixSundanese(Strng,reverse=False):
     vir = Sundanese.ViramaMap[0]
 
@@ -2895,26 +3101,39 @@
 
     if not reverse:
         Strng = PostProcess.RetainDandasIndic(Strng, 'Malayalam', True)
         Strng = PostProcess.RetainIndicNumerals(Strng, 'Malayalam', True)
 
         # fix n2ra
         #Strng = Strng.replace('ன்ற')
+    else:
+        Strng = PostProcess.RetainIndicNumerals(Strng, 'Malayalam')
+        Strng = PostProcess.RetainDandasIndic(Strng, 'Malayalam')
+
+        #Fix Arachaic chillus
+        chilluArch = ['\u0D54', '\u0D55', '\u0D56', '\u0D7F']
+        chilluArchhVir = ['മ്', 'യ്', 'ഴ്', 'ക്']
+
+        for ch, chvir in zip(chilluArch, chilluArchhVir):
+            Strng = Strng.replace(ch, chvir)
 
     Chillus=['\u0D7A','\u0D7B','\u0D7C','\u0D7D','\u0D7E', 'ഩ‍്']
 
     Anu = GM.CrunchSymbols(GM.CombiningSigns,'Malayalam')[1]
 
+
     return Strng
 
 def FixTelugu(Strng, reverse=False):
     if not reverse:
         Strng = PostProcess.RetainDandasIndic(Strng, 'Telugu', True)
         Strng = PostProcess.RetainIndicNumerals(Strng, 'Telugu', True)
     else:
+        Strng = PostProcess.RetainIndicNumerals(Strng, 'Telugu')
+        Strng = PostProcess.RetainDandasIndic(Strng, 'Telugu')
         Strng = Strng.replace('ఁ', 'ఀ')
 
     return Strng
 
 def FixMeeteiMayek(Strng,reverse=False):
     vir = MeeteiMayek.ViramaMap[0]
     listC = [x+vir for x in [MeeteiMayek.ConsonantMap[x] for x in [0,27,24,20,19,15,4,25]]]
@@ -3028,14 +3247,15 @@
             Strng = Strng.replace(x,y)
         else:
             Strng = Strng.replace(y,x)
 
     if not reverse:
         # Strng = Strng.replace("\u1A63\u1A74","\u1A74\u1A63") # kAM -> kMA (Like Thai ำ )
         # Check above in Pali texts
+        #Strng = Strng.replace('ᩰ', 'ᩮᩣ')
         pass
     else:
         #Strng = Strng.replace("\u1A74\u1A63","\u1A63\u1A74") # kAM <- kMA
         pass
 
     ListC ='|'.join(GM.CrunchSymbols(GM.Consonants,'TaiTham'))
     ng = TaiTham.ConsonantMap[4]+vir
@@ -3070,14 +3290,29 @@
     return Strng
 
 def FixLaoTham(Strng, reverse=False):
     Strng = FixTaiTham(Strng, reverse)
 
     return Strng
 
+def FixThamLoC(Strng, reverse=False):
+    Strng = FixTaiTham(Strng, reverse)
+
+    ListC ='|'.join(GM.CrunchSymbols(GM.Consonants,'TaiTham'))
+    if not reverse:
+        E = "ᩮ"
+        AA = 'ᩣ'
+        TallACons = '|'.join(['ᩅ', 'ᨴ', 'ᨵ', 'ᨣ', 'ᨷ']) ## va da dha ga
+        Strng = re.sub('('+TallACons+')(᩠)('+ListC +')'+'('+E+'?)'+AA,r'\1\2\3\4'+'ᩤ',Strng)
+        Strng = re.sub('('+TallACons+')(᩠)('+ListC +')'+'(᩠)('+ListC +')'+'('+E+'?)'+AA,r'\1\2\3\4\5\6'+'ᩤ',Strng)
+    else:
+        pass
+
+    return Strng
+
 def FixLueTham(Strng, reverse=False):
     Strng = FixTaiTham(Strng, reverse)
 
     ListC ='|'.join(GM.CrunchSymbols(GM.Consonants,'TaiTham'))
     if not reverse:
         E = "ᩮ"
         AA = 'ᩣ'
@@ -3133,22 +3368,23 @@
 # Replace Bengali /ra/ with Assamese /ra/
 def FixBengali(Strng, reverse=False):
     Virama = ''.join(GM.CrunchSymbols(['ViramaMap'], 'Bengali'))
     ba = 'ব'
 
     if not reverse:
         Strng = re.sub('(?<![রবম])' + Virama + ba,  Virama + '\u200C' + ba, Strng)
+        #print(Strng)
+        ## Fix স্ভ়ারা  -> স্বারা ; subjoined ba is by default pronounced as /va/ in Bengali
+        Strng = re.sub('(?<![রবমভ়])' + '(\u09CD\u09AD\u09BC)', '\u09CD\u09AC', Strng)
+        #print(Strng)
     else:
         pass
 
     Strng = PostProcess.KhandaTa(Strng, 'Bengali', reverse)
-
-    ## Fix স্ভ়ারা  -> স্বারা ; subjoined ba is by default pronounced as /va/ in Bengali
-
-    Strng = Strng.replace('\u09CD\u09AD\u09BC', '\u09CD\u09AC')
+    #print(Strng)
 
     return Strng
 
 def FixAssamese(Strng,reverse=False):
     Ra = "\u09B0"
     AssRa = "\u09F0"
 
@@ -3168,46 +3404,50 @@
     Nukta = '|'.join(GM.CrunchSymbols(GM.CombiningSigns,'Sharada')[-1])
     Virama = ''.join(GM.CrunchSymbols(['ViramaMap'], 'Sharada'))
 
     if not reverse:
         Strng = Strng.replace( Nukta + Virama, Nukta + Virama + '\u200C')
         Strng = re.sub('(' + Virama + ')' + '(' + ListC + ')' + '(' + Nukta + ')', r'\1' + '\u200C' + r'\2\3', Strng)
 
-        Strng = Strng.replace('𑆇ʼ','\U00011183\U000111CB\U000111B6').replace('𑆈ʼ','\U00011183\U000111CB\U000111B7')\
+        '''Strng = Strng.replace('𑆇ʼ','\U00011183\U000111CB\U000111B6').replace('𑆈ʼ','\U00011183\U000111CB\U000111B7')\
             .replace('𑆶ʼ','\U000111CB\U000111B6').replace('𑆷ʼ','\U000111CB\U000111B7')
 
         Strng = Strng.replace('\U00011184ʼ', '𑆃𑇋𑆳')
         Strng = re.sub('(?<!\U000111BE)\U000111B3ʼ', '\U000111CB\U000111B3', Strng)
 
         Strng = Strng.replace('𑆃ʼ', '𑆃𑇋', )
-        Strng = re.sub('(' + ListC + ')'+ 'ʼ', r'\1' + '\U000111CB', Strng)
+        Strng = re.sub('(' + ListC + ')'+ 'ʼ', r'\1' + '\U000111CB', Strng)'''
 
 
     else:
+        pass
         # u^ u^^ to vriaama
         # Fix Devanagari as well u^ u^^ to devanagri vowels
 
         # half-u and half-long-u
-        Strng = Strng.replace('\U00011183\U000111CB\U000111B6', '𑆇ʼ').replace('\U00011183\U000111CB\U000111B7', '𑆈ʼ').\
-            replace('\U000111CB\U000111B6', '𑆶ʼ').replace('\U000111CB\U000111B7', '𑆷ʼ')
+        #Strng = Strng.replace('\U00011183\U000111CB\U000111B6', '𑆇ʼ').replace('\U00011183\U000111CB\U000111B7', '𑆈ʼ').\
+        #    replace('\U000111CB\U000111B6', '𑆶ʼ').replace('\U000111CB\U000111B7', '𑆷ʼ')
 
-        Strng = Strng.replace('𑆃𑇋𑆳', '\U00011184ʼ')
-        Strng = re.sub('(?<!\U000111BE)\U000111CB\U000111B3', '\U000111B3ʼ', Strng)
+        #Strng = Strng.replace('𑆃𑇋𑆳', '\U00011184ʼ')
+        #Strng = re.sub('(?<!\U000111BE)\U000111CB\U000111B3', '\U000111B3ʼ', Strng)
 
-        Strng = Strng.replace('𑆃𑇋', '𑆃ʼ')
-        Strng = re.sub('(' + ListC + ')'+ '\U000111CB', r'\1' +  'ʼ', Strng)
+        #Strng = Strng.replace('𑆃𑇋', '𑆃ʼ')
+        #Strng = re.sub('(' + ListC + ')'+ '\U000111CB', r'\1' +  'ʼ', Strng)
 
     return Strng
 
 def FixKannada(Strng,reverse=False):
     if not reverse:
+        #print(Strng)
         Strng = PostProcess.RetainDandasIndic(Strng, 'Kannada', True)
-        Strng = PostProcess.RetainIndicNumerals(Strng, 'Kannada', True)
+        #Strng = PostProcess.RetainIndicNumerals(Strng, 'Kannada', True)
 
         Strng = re.sub('(\u0CCD)([^\u0CAB\u0C9C])(\u0CBC)', r'\1' + '\u200C' + r'\2\3', Strng)
+    else:
+        Strng = PostProcess.RetainDandasIndic(Strng, 'Kannada')
 
     return Strng
 
 def FixGrantha(Strng, reverse=False):
     if not reverse:
         Strng = Strng.replace('॑', '᳴')
         Strng = Strng.replace('᳚', '॑')
@@ -3276,15 +3516,15 @@
 
 
 def FixGujarati(Strng,reverse=False):
     if not reverse:
         Strng = PostProcess.RetainDandasIndic(Strng, 'Gujarati', True)
         Strng = Strng.replace('જ઼઼', 'ૹ').replace('શ઼', 'ૹ')
     else:
-        pass
+        Strng = PostProcess.RetainDandasIndic(Strng, 'Gujarati')
         Strng = Strng.replace('ૹ', 'જ઼઼').replace('ૹ', 'શ઼')
 
     return Strng
 
 def FixZanabazarSquare(Strng, reverse=False):
     ListC ='|'.join(GM.CrunchSymbols(GM.Consonants,'ZanabazarSquare'))
     yrlv = ZanabazarSquare.ConsonantMap[25:29]
```

### Comparing `aksharamukha-2.1.2/aksharamukha/PostOptions.py` & `aksharamukha-2.2.1/aksharamukha/PostOptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,20 @@
 
     if Target == 'Telugu':
         Options += ['NasalToAnusvara','MToAnusvara', 'TeluguRemoveNukta', 'TeluguRemoveAeAo']
 
     elif Target == 'Kannada':
         Options += ['NasalToAnusvara','MToAnusvara']
 
+    elif Target == 'Sinhala':
+        Options += ['SinhalaChandrbinduAnusvara']
+
+    elif Target == 'Khojki':
+        Options += ['KhojkiRRI']
+
     elif Target == 'Nandinagari':
         Options += ['NasalToAnusvara']
 
     elif Target == 'Hebrew':
         Options += ['HebrewVetVav', 'HebrewnonFinalShort']
 
     elif Target == 'Malayalam':
@@ -33,27 +39,27 @@
     elif Target == 'Tamil':
         Options += ['TamilNaToNNa','AnusvaraToNasal', 'TamilpredictDentaNa']
 
     elif Target == 'Bengali':
         if 'BengaliRaBa' in PostOptions:
             Options += ['YaToYYa','AnusvaraToNasal', 'BengaliConjunctVB']
         else:
-            Options += ['VaToBa','YaToYYa','AnusvaraToNasal', 'BengaliConjunctVB']
+            Options += ['AnusvaraToNasal', 'VaToBa','YaToYYa', 'BengaliConjunctVB']
 
     elif Target == 'MeeteiMayek':
         Options += ['MeeteiMayekremoveHistorical']
 
     elif Target == 'Limbu':
         Options += ['LimburemoveHistorical']
 
     elif Target == 'Assamese':
         Options += ['YaToYYa','AnusvaraToNasal']
 
     elif Target == 'Oriya':
-        Options += ['OriyaVa','YaToYYa','AnusvaraToNasal']
+        Options += ['AnusvaraToNasal', 'OriyaVa','YaToYYa']
 
     elif Target == 'Chakma':
         Options += ['YaToYYa']
 
     elif Target == 'Gurmukhi':
         Options += ['GurmukhiCandrabindu', 'GurmukhiTippiBindu','GurmukhiTippiGemination']
```

### Comparing `aksharamukha-2.1.2/aksharamukha/PostProcess.py` & `aksharamukha-2.2.1/aksharamukha/PostProcess.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,104 @@
 # -*- coding: utf-8 -*-
 
 from . import GeneralMap as GM
 from . import ScriptMap
 from aksharamukha.ScriptMap.Roman import Avestan
-from aksharamukha.ScriptMap.MainIndic import Ahom, Tamil,Malayalam,Gurmukhi,Oriya,Saurashtra,Sinhala,Urdu,Devanagari, Chakma, Limbu, Takri, TamilExtended
-from aksharamukha.ScriptMap.EastIndic import Tibetan, Thai, PhagsPa, ZanabazarSquare, Burmese, KhamtiShan
+from aksharamukha.ScriptMap.MainIndic import Ahom, Tamil,Malayalam,Gurmukhi,Oriya,Saurashtra,Sinhala,Urdu,Devanagari, Chakma, Limbu, Takri, TamilExtended, Kannada
+from aksharamukha.ScriptMap.EastIndic import Tibetan, Thai, PhagsPa, ZanabazarSquare, Burmese, KhamtiShan, Khmer, Balinese, Javanese
 from . import ConvertFix as CF
 import re
 import functools
 
-### Write Lotsssss of Comments
-### Rewrite all ListC, ListV as sorted(List,key=len,reverse=True). Then Correctrulu may be unnecessary
-
+### Rewrite all ListC, ListV as sorted(List,key=len,reverse=True).
 ### Consider Adding Options to ignore Nukta etc for Gujarati bengali by default
 
-## Todo
-## Fix Font links and names in description
+## order the functions by script ##
 
-def default(Strng):
+## This is the processing that's done immediately after calling the convert() function
+## But before the post-processing steps
+## removes extranous/artificial diacritics introduced
+def default(Strng, langage=""):
     Strng = Strng.replace("\uF001", "").replace("\u05CC", "").\
-        replace("ʻʻ", "").replace('\u05CD', '') ## remove token characters for specialized processing
+        replace("ʻʻ", "").replace('\u05CD', '').replace('\u02C2', '') ## remove token characters for specialized processing
+
+    return Strng
+
+## This is processing that's done after the post-processing steps
+## It's catch all function for all misc stuff
+def defaultPost(src, tgt, Strng, nativize, preoptions, postoptions):
+    Strng = Strng.replace('\u034F', '') ## remove token characters for specialized processing
+
+    ## Fix Dandas & Numerals
+    if 'romanNumerals' in postoptions:
+        Strng = RetainIndicNumerals(Strng,tgt,reverse=True)
+    if 'indicNumerals' in postoptions:
+        Strng = RetainIndicNumerals(Strng,tgt,reverse=False)
+    if 'romanFullStop' in postoptions:
+        Strng = RetainDandasIndic(Strng, tgt, reverse=True)
+
+    #Devanagari Dandas
+    if tgt not in GM.Transliteration:
+        Strng = Strng.replace( '│', '।',).replace('┃', '॥')
+    else:
+        Strng = Strng.replace( '│', '|',).replace('┃', '||')
+    #Pipe scripts as source
+    Strng = Strng.replace( "●", ".",)
+
+    return Strng
+
+## Ahom ##
+
+## Arabic ##
+
+## Assamese ##
+
+## Avestan ##
+
+def KhojkiRRI(Strng):
+    Strng = Strng.replace('\U00011241', '\U00011235\U00011226\U0001122D')
+    Strng = Strng.replace('\U00011240', '\U00011202')
+
+    return Strng
+
+def KhojkiQa(Strng):
+    Strng = Strng.replace('𑈈𑈶', '\U0001123F')
 
     return Strng
 
+def removePaliAhom(Strng):
+    pali = "𑝁 𑝂 𑝃 𑝄 𑝅 𑝆".split(" ")
+    nonPali ="𑜄 𑜌 𑜓 𑜔 𑜃 𑜎".split(" ")
+
+    for p, np in zip(pali, nonPali):
+        Strng = Strng.replace(p, np)
+
+    return Strng
+
+def SinhalaChandrbinduAnusvara(Strng):
+    Strng = Strng.replace('\u0D81', '\u0D82')
+
+    return Strng
+
+def LoCMarc8(Strng):
+    import unicodedata
+    Strng = unicodedata.normalize('NFD', Strng)
+    Strng = Strng.replace('\u02DA', '\u02D9')
+    return Strng
+
+def AnusvaraAsN(Strng):
+    Strng = Strng.replace('m\u034F', 'n')
+    return Strng
+
+#show Schwa
+def ShowSchwaHindi(Strng):
+    from . import PreProcess as PreP
+    Strng = PreP.RemoveSchwaHindi(Strng, True)
+    return Strng
+
 def KannadaSpacingCandrabindu(Strng):
     Strng = Strng.replace('\u0C81', '\u0C80')
 
     return Strng
 
 def KannadaNotRepha(Strng):
     ListC = "(" + "|".join(GM.CrunchSymbols(GM.Consonants, 'Kannada')) + ")"
@@ -34,15 +106,15 @@
     Strng = re.sub('ರ್(?=' + ListC + ')', 'ರ‍್', Strng)
 
     return Strng
 
 def KannadaNakaraPollu(Strng):
     ListC = "(" + "|".join(GM.CrunchSymbols(GM.Consonants, 'Kannada')) + ")"
 
-    Strng = re.sub('ನ್(?!' + ListC + ')', '\u0CDD', Strng)
+    Strng = re.sub('(?<!\u0CCD)ನ್(?!' + ListC + ')', '\u0CDD', Strng)
 
     return Strng
 
 def TeluguRemoveNukta(Strng):
     Strng = Strng.replace('\u0C3C', '')
 
     return Strng
@@ -51,43 +123,48 @@
     Strng = Strng.replace('\u0952\u200B', '')
 
     return Strng
 
 def TeluguNakaraPollu(Strng):
     ListC = "(" + "|".join(GM.CrunchSymbols(GM.Consonants, 'Telugu')) + ")"
 
-    Strng = re.sub('న్(?!' + ListC + ')', '\u0C5D', Strng)
+    Strng = re.sub('(?<!\u0C4D)న్(?!' + ListC + ')', '\u0C5D', Strng)
 
     return Strng
 
+#testcase todo
 def syriacVowelsBelow(Strng):
 
     return Strng
 
+#testcase todo
 def syriacWesternOToU(Strng):
 
     return Strng
 
+#testcase todo
 def olddogra(Strng):
 
     return Strng
 
+#testcase todo
 def ISO259Target(Strng):
     replacements = [('b', 'ḃ'), ('p', 'ṗ'), ('k', 'k̇'), ('ḵ', 'k'), ('v', 'b'), ('f', 'p'), ('꞉', '\u0307'),\
          ('š̪', 'ś'), ('š̮', 'š'), ('š', 's̀'),
         ('ā', 'å'), ('e', 'ȩ'), ('ō', 'ŵ'), ('ū', 'ẇ'), ('\u033D', '°'), ('ĕ', 'ḝ')
     ]
 
     for x, y in replacements:
         Strng = Strng.replace(x, y)
 
     Strng = Strng.replace('\u00B0\u0307', '\u0307\u00B0')
 
     return Strng
 
+#testcase todo
 def HebrewSBLTarget(Strng):
     replacements = [('v', 'ḇ'), ('f', 'p̄'), ('d', 'ḏ'), ('ḏ꞉', 'd'), \
         ('g', 'ḡ'), ('ḡ꞉', 'g'),\
             ('t', 'ṯ'), ('ṯ꞉', 't'),
          ('š̪', 'ś'), ('š̮', 'š'),
         ('ō', 'ô'), ('o', 'ō'), ('ū', 'û'), ('\u033D', 'ĕ')
     ]
@@ -100,66 +177,74 @@
     if '\u05CE' in Strng:
         Strng = Strng.replace('ḏ', 'd').replace('ṯ', 't').replace('ḡ', 'g').replace('\u05CE', '')
 
     Strng = Strng.replace('\u00B0\u0307', '\u0307\u00B0')
 
     return Strng
 
+#testcase todo
 def removetddash(Strng):
     Strng += '\u05CE'
 
     Strng = Strng.replace('d', 'd꞉').replace('t', 't꞉').replace('g', 'g꞉')
     Strng = Strng.replace('ḏ', 'd').replace('ṯ', 't').replace('ḡ', 'g').replace('\u05CE', '')
 
     return Strng
 
-
+#testcase todo
 def ISO259Source(Strng):
 
     return Strng
 
+#testcase todo
 def ISO233Source(Strng):
 
     return Strng
 
+#testcase todo
 def HebrewSBLSource(Strng):
 
     return Strng
 
+#testcase todo
 def PersianDMGSBLSource(Strng):
 
     return Strng
 
+#testcase todo
 def ISO233Target(Strng):
     replacements = [('j', 'ǧ'), ('g', 'ǧ'), ('ḧ', 'ẗ'), ('ḫ', 'ẖ'), ('a̮', 'ỳ'), ('ˀ', 'ˈ'), \
         ('aⁿ', 'á'), ('iⁿ', 'í'), ('uⁿ', 'ú'), ('ā̂', 'ʾâ'), ('\u033D', '')]
 
     for x, y in replacements:
         Strng = Strng.replace(x, y)
 
     return Strng
 
+#todo add to frontend
 def inherentAO(Strng):
     Strng = Strng.replace('a', 'ô')
 
     return Strng
 
 def BengaliOldRA(Strng):
     Strng = Strng.replace('র', 'ৰ')
 
     return Strng
 
+#testcase todo
 def PersianDMGTarget(Strng):
     replacements = [('ḏ', 'ẕ'), ('ḍ', 'ż'), ('ṯ', 's̱'), ('j', 'ǧ'), ('ˀ','ʼ'), ('ʔ', 'ʼ'), ('ȳ', 'ye'), ("ā̂", "ā"), ('\u033D', '')]
 
     for x, y in replacements:
         Strng = Strng.replace(x, y)
 
     return Strng
 
+#testcase todo
 def arabizeLatn(Strng, target='semitic'):
     cons = '(' + '|'.join(GM.SemiticConsonants) + ')'
 
     # opt 1
     Strng = re.sub(cons + '(ʾ)', r'\1' + 'ā', Strng)
     ### implement ths as a preoption for all semitic scripts
 
@@ -196,29 +281,33 @@
 
     Strng = re.sub('(ā)([iau])(ⁿ)', r'\2\3', Strng)
 
     #print('Arabized string is', Strng)
 
     return Strng
 
+#trigger - UI prompt to show "preserve source" must be enabled for this option
+#testcase todo
 def BengaliSwitchYaYYa(Strng):
     Strng = re.sub('(?<!\u09CD)য', '@#$', Strng)
     Strng = re.sub('য়', 'য', Strng)
     Strng = Strng.replace('@#$', 'য়')
 
     return Strng
 
+#testcase todo
 def AlephMaterLectionis(Strng, target='semitic'):
     cons = '(' + '|'.join(GM.SemiticConsonants) + ')'
 
     # opt 1
     Strng = re.sub(cons + '(ʾ)', r'\1' + 'ā', Strng)
 
     return Strng
 
+#testcase todo
 def urduizeLatn(Strng, target='semitic'):
     cons = '(' + '|'.join(GM.SemiticConsonants) + ')'
 
     # opt 1
     Strng = re.sub(cons + '(ʾ)', r'\1' + 'ā', Strng)
 
     if target == 'indic':
@@ -238,14 +327,15 @@
     if target != 'indic':
         Strng = LatnInitialVowels(Strng)
 
     Strng = re.sub('(ā)([iau])(ⁿ)', r'\2\3', Strng)
 
     return Strng
 
+#testcase todo
 def syricizeLatn(Strng, target='semitic'):
     cons = '(' + '|'.join(GM.SemiticConsonants) + ')'
 
     # opt 3
     if target != 'indic':
         Strng = re.sub('â', 'ʾa', Strng)
         Strng = re.sub('ā̂', 'ʾā', Strng)
@@ -253,143 +343,165 @@
         Strng = re.sub("ē̂", "ʾē", Strng)
 
     if target != 'indic':
         Strng = LatnInitialVowels(Strng)
 
     return Strng
 
+#testcase todo
 def hebraizeLatn(Strng, target='semitic'):
     #print('Hebraizing Latin')
     if target != 'indic':
         Strng = LatnInitialVowels(Strng, 'ʾ')
 
     return Strng
 
+#testcase todo
 def syriacRoman(Strng):
     Strng = Strng.replace('v', 'ḇ').replace('ġ','ḡ').replace('ḫ','ḵ').replace('f','p̄')
 
     return Strng
 
+#testcase todo
 def alephAyinLatnAlternate(Strng):
     Strng = Strng.replace('ʾ', 'ʼ').replace('ʿ', 'ʽ')
 
     return Strng
 
-
+#testcase todo
 def alephAyinLatnAlternate2(Strng):
     Strng = Strng.replace('ʾ', 'ʔ').replace('ʿ', 'ʕ')
 
     return Strng
 
+#testcase todo
 def ArabRemoveAdditions(Strng):
     Strng = Strng.replace('ڨ', 'ج').replace('ڤ', 'ف').replace('پ', 'ف')
 
     return Strng
 
+#testcase todo
 def arabicRemoveAdditionsPhonetic(Strng):
 
     Strng = Strng.replace('ڨ', 'غ').replace('ڤ', 'ف').replace('پ', 'ب')
 
     return Strng
 
+#testcase todo
 def removeSemiticLetters(Strng):
     Strng = Strng.replace('ṭ', 't').replace('ḥ', 'h').replace('ḍ', 'z').replace('ḏ', 'z').replace('ẓ', 'z')\
         .replace('w', 'v').replace('ʿ', 'ʾ').replace('ṣ', 's')
 
     return Strng
 
+#testcase todo
 def removeNikkud(Strng):
     nikkuds = ["\u05B7","\u05B8","\u05B4","\u05B4י","\u05BB", "\u05C2", "\u05C1",\
     "\u05B6","\u05B5","\u05B9","וֹ","\u05B1","\u05B2","\u05B3","\u05BC","\u05B0", "\u05C7"]
 
     for nikkud in nikkuds:
         Strng = Strng.replace(nikkud, '')
 
     return Strng
 
+#testcase todo
 def LatnInitialVowels(Strng, initLetter=''):
     initVow = 'â ā̂ î ī̂ û ū̂ ê ē̂ âŷ ô ō̂ âŵ'.split(' ')
     nonInitVow = 'a ā i ī u ū e ē aŷ o ō aŵ'.split(' ')
 
     for x, y in zip(initVow, nonInitVow):
         Strng = Strng.replace(x, initLetter+y)
 
     Strng = Strng.replace('\u0302', '')
 
     Strng = re.sub('\u033d', '', Strng)
     #Strng = 'Vinodh'
     return Strng
 
+#testcase todo
 def removeMajliyana(Strng):
     Strng = Strng.replace('\u0330', '')
 
     return Strng
 
+#testcase todo
 def removeRukkaka(Strng):
     Strng = Strng.replace('\u0741', '')
 
     return Strng
 
+#testcase todo
 def removeQussaya(Strng):
     Strng = Strng.replace('\u0742', '')
 
     return Strng
 
+#testcase todo
 def removeVowelsSyriac(Strng):
     Strng = re.sub('[\u0732\u0735\u073C\u0738\u0739\u073F]', '', Strng)
 
     Strng = re.sub('[ّܰܶܺܽܳ]', '', Strng)
 
     return Strng
 
+#testcase todo
 def removeDiacriticsArabic(Strng):
     diacrtics = ["\u0652", "\u064E", "\u0650", "\u064F"]
 
     for diacritic in diacrtics:
         Strng = Strng.replace(diacritic, '')
 
     return Strng
 
+#testcase todo
 def removeSukunEnd(Strng):
     Strng = re.sub('(\u0652)(\W|$)', r'\2', Strng)
 
     return Strng
 
+#testcase todo
 def persianPaGaFaJa(Strng):
     Strng = Strng.replace('پ', 'ف').replace('گ', 'ج')
 
     return Strng
 
+#testcase todo
 def removeDiacriticsPersian(Strng):
 
     return Strng
 
+#testcase todo
 def removeDiacriticsSyriac(Strng):
 
     return Strng
 
+#testcase todo
 def useKtivMale(Strng):
 
     return Strng
 
+#testcase todo
 def PhoneticMapping(Strng):
 
     return Strng
 
+#testcase todo
 def ArabicGimelGaGha(Strng):
     Strng = Strng.replace('ج', 'غ')
 
     return Strng
 
+#testcase todo
 def ArabicGimelPaBa(Strng):
     Strng = Strng.replace('ف', 'ب')
 
     return Strng
 
-def IASTLOCBurmeseSource(Strng):
+#testcase todo
+def BurmeseRomanLoCSource(Strng):
     # remove marking for pure virama
     Strng = Strng.replace('ʻ', '')
 
     # restore superscript Ga into normal subjoined y, r , v, h
     yrvh = Burmese.ConsonantMap[25:27] + Burmese.ConsonantMap[28:29] + Burmese.ConsonantMap[32:33]
     yrvhPat = ''.join(yrvh)
     Strng = re.sub(f'(\u103A)(\u1039)([{yrvhPat}])', r'\2\3', Strng)
@@ -419,24 +531,130 @@
     Strng = Strng.replace('’အ', 'အ')
 
     # swap tone + virama to proper order
     Strng = Strng.replace("့်", "့်")
 
     return Strng
 
+#testcase todo
 def removeSegmentSpacesBurmese(Strng):
     # segment text into syllables
     import regex
 
     Strng = regex.sub('(\p{L}\p{M}*) (\p{L})', r'\1\2', Strng)
     Strng = regex.sub('(\p{L}\p{M}*) (\p{L})', r'\1\2', Strng)
 
     return Strng
 
-def IASTLOCBurmeseTarget(Strng):
+def UseAlternateo1(Strng):
+    Strng = Strng.replace('ᩮᩣ', 'ᩰ')
+
+    return Strng
+
+
+def UseAlternateo2(Strng):
+    Strng = Strng.replace('ᩰ', 'ᩮᩣ')
+
+    return Strng
+
+#ThamLoC
+def ThamLoCRomanLoCTarget(Strng):
+    return Strng
+
+def ThamLoCRomanLoCSource(Strng):
+    #cryptogammic dot to Sakot
+    Strng = Strng.replace('\u1A7F', '᩠')
+
+    #fixing aiy
+    Strng = Strng.replace('\u1A71\u1A3F\u1A7A', '\u1A71᩠ᨿ')
+
+    return Strng
+
+# khmer
+def KhmerLoCRomanLoCTarget(Strng):
+    import unicodedata
+    Strng = unicodedata.normalize('NFC', Strng)
+
+    #move consonant modifiers
+    #Strng = re.sub('(‛ʹ)(′?)(a)(?![ṃḥ])', r'\1\2', Strng)
+    Strng = re.sub('(ʹ)(′?)(?=[aāiīuūẏȳeoăáâààáéíóúàèìòùă])', r'\2', Strng)
+    #Strng = re.sub('(ʹ)(′?)(a)(?=[aāiīuūẏȳeoă])', r'\2', Strng)
+
+    #fix Oh
+    Strng = Strng.replace('oḥ', 'oaḥ')
+    Strng = Strng.replace('  ', ' ')
+
+
+    return Strng
+
+def KhmerLoCRomanLoCSource(Strng):
+    ListC ='|'.join(GM.CrunchSymbols(GM.Consonants,'Khmer'))
+    ListV ='|'.join(GM.CrunchSymbols(GM.VowelSigns,'Khmer'))
+    ListA ='|'.join(GM.CrunchSymbols(GM.CombiningSigns,'Khmer'))
+
+    vir = Khmer.ViramaMap[0]
+
+    #move bantoc around
+    Strng = re.sub('(\u17CB)(.)', r'\2\1', Strng)
+
+    #move tonemarks around
+    Strng = re.sub('('+ListC+')'+'('+ListV+')''('+ListA+')?''([៎៏])',r'\1\4\2\3',Strng)
+
+    #subjoined a
+    #Strng = Strng.replace(vir + '‛', '\u17D2')
+
+    #mark consonant modifiers with subbase form
+    Strng = re.sub('([ងញមបយរវ])(៉)([ិឹីឺ])', r'\1''ុ'r'\3', Strng)
+    Strng = re.sub('([សហអ])(៊)([ិឹីឺ])', r'\1''ុ'r'\3', Strng)
+
+    #remove virama
+    Strng = Strng.replace(vir, '')
+
+    return Strng
+
+# shan
+def ShanLoCRomanLoCTarget(Strng):
+    Strng = re.sub('(ʻ)([\u0310\u0322])', r'\2\1', Strng)
+    Strng = re.sub('(ō)([\u0310\u0322]?)(ʻ)', r'\1\2', Strng)
+
+    return Strng
+
+def ShanLoCRomanLoCSource(Strng):
+    # restrore special yrvh
+    yrv = Burmese.ConsonantMap[25:27] + Burmese.ConsonantMap[28:29]
+    vir = '်'
+    yrvsub = ['\u103B','\u103C','\u1082']
+
+    for x,y in zip(yrv,yrvsub):
+        # Undo Replace subjoining forms: exp-virama + y/r/v/h <- subjoining y/r/v/h
+        Strng = Strng.replace(vir + x, y)
+
+    ## Fix modifier letter apostrephe to normal quotation mark
+    Strng = Strng.replace('ʼ', '’')
+    #remove purevowel marker
+    Strng = Strng.replace('’', '')
+    # remove marking for pure virama
+    Strng = Strng.replace('ʻ', '')
+
+    #ai reversal
+    Strng = Strng.replace('\u036E', 'ႂ်')
+
+    # closed vs open
+    cons = "[ၵၶၷꧠငၸꧡꩡꧢၺꩦꩧꩨꩩꧣတထၻꩪၼပၽၿꧤမယရလဝသႁꩮၹၾႀဢ]"
+    open = ['ႃ', 'ႄ', 'ေ']
+    closed = ['ၢ', 'ႅ', 'ဵ']
+
+    for o, c in zip(open, closed):
+        pass
+        Strng = re.sub('(' + cons + ')' + '(' + o + ')' + '(' + cons + ')', r'\1' + c + r'\3', Strng)
+
+    return Strng
+
+#testcase todo
+def BurmeseRomanLoCTarget(Strng):
     #print(Strng)
     # mark tone
     Strng = Strng.replace('˳', 'ʹ')
 
     # mark depaend au -> o'
     Strng = Strng.replace('auʻ','oʻ')
 
@@ -458,14 +676,15 @@
         Strng = Strng.replace(bur, lat)
 
     #Strng = Strng.replace('ṃ', 'ṁ')
 
     return Strng
 
 ### Add new consonants here when added to gimeltra_data
+#testcase todo
 def insertARomanSemitic(Strng):
     Strng = Strng.replace('\u02BD', '')
     consonantsAll = '(' + '|'.join(sorted(GM.SemiticConsonants, key = len, reverse=True)) + ')'
     #above does not ocntain semitic consonants
     vowelsAll = '(' + '|'.join(GM.SemiticVowels) + ')'
     #print(Strng)
     Strng = re.sub(consonantsAll + '(?![꞉ʰ])(?!' + vowelsAll + ')', r'\1' + 'a', Strng)
@@ -476,14 +695,15 @@
     #Strng = re.sub(consonantsAll + '(?!' + vowelsAll + ')', r'\1' + 'a', Strng)
 
     #print(Strng)
 
     return Strng
 
 # Semitic Target
+#testcase todo
 def FixSemiticRoman(Strng, Target):
     vir = '\u033D'
     Strng = re.sub('ō̂̄̂', 'ō̂', Strng)
 
     ## For Gemination
     if "Arab" in Target:
         consonantsAll = '(' + '|'.join(sorted(GM.CrunchSymbols(GM.Consonants, 'RomanSemitic'), key = len, reverse=True)) + ')'
@@ -506,32 +726,37 @@
 
     Strng = Strng.replace('\u033d\u033d', '\u033d')
 
     #print('Strng is ' + Strng)
 
     return Strng
 
+#testcase todo
 def ArabAtoAleph(Strng):
     Strng = Strng.replace('أ', 'ا')
 
 
     return Strng
 
+#testcase todo
 def estrangelasyriac(Strng):
 
     return Strng
 
+#testcase todo
 def easternsyriac(Strng):
 
     return Strng
 
+#testcase todo
 def westernsyriac(Strng):
 
     return Strng
 
+
 def kawitan(Strng):
 
     return Strng
 
 def sundapura(Strng):
 
     return Strng
@@ -540,73 +765,93 @@
     pairsReadable = [('R^i','RRi'), ('R^I','RRii'), ('',''), ('',''), ('A', 'aa'), ('I', 'ii'), ('U', 'uu'), ('Ch', 'chh'), ('kSh','x'), ('M', '.m')]
 
     for x, y in pairsReadable:
         Strng = Strng.replace(x,y)
 
     return Strng
 
+#todo change UI example : haMpi  ha~pi hA~s hAMs hU~ hUM -> hampi hAA hAs
 def NasalTilde(Strng):
+    Strng = AnusvaratoNasalASTISO(Strng)
     Strng = re.sub('(m̐|ṃ|ṁ)', '\u0303', Strng)
 
     return Strng
 
+#todo feature
+def siddhamBija(Strng):
+
+    return Strng
+
+#todo feature
 def verticalKana(Strng):
 
     return Strng
 
+#todo feature
 def verticalSiddham(Strng):
 
     return Strng
 
+#todo testcase
 def vtobJapanese(txt):
 
     return txt
 
+#todo testcase
 def SogdReshAyin(Strng):
     Strng = Strng.replace('𐼽', '𐽀')
 
     return Strng
 
+#todo testcase
 def SogoReshAyinDaleth(Strng):
     Strng = Strng.replace('𐼓','𐼘')
 
     return Strng
 
+#todo testcase
 def arabPaFa(Strng):
 
     return Strng.replace('پ','ف')
 
 
+#todo testcase
 def arabChaSa(Strng):
 
     return Strng.replace('چ', 'س')
 
+#todo testcase
 def gainGimel(Strng):
     return Strng.replace('עׄ','ג')
 
+#todo testcase
 def tavTwodot(Strng):
     return Strng.replace('ת','ת̈')
 
+#todo testcase
 def tavThreedot(Strng):
     return Strng.replace('תׄ','ת֒')
 
+#todo testcase
 def gainGimel(Strng):
     return Strng.replace('ק','ק̈')
 
+#todo testcase
 def tokushuon(txt):
    txt = txt.replace('si', 'suxi').replace('zi', 'zuxi')
    txt = txt.replace('yi','ixi')
    txt = txt.replace('fy', 'fux')
    txt = txt.replace('nye', 'nixe')
 
    txt = re.sub('(?<![sc])hu', 'hoxu', txt)
    txt = re.sub('(?<![sc])hye', 'hixe', txt)
 
    return txt
 
+#todo testcase
 def JapanesePostProcess(src, tgt, txt, nativize, postoptions):
     from aksharamukha.ScriptMap.NonIndic import kana2roman
     import pykakasi
     from . import PostOptions, Convert
 
     txt = Convert.convertScript(txt, src, "Telugu")
 
@@ -710,19 +955,21 @@
 
         txt = kana2roman.to_katakana(txt)
 
     txt = Convert.convertScript(txt, "Inter", "ISO")
 
     return txt
 
+#todo check if used
 def urduRemoveInherent(Strng):
     Strng = re.sub('\Ba', '', Strng)
 
     return Strng
 
+#todo testcase
 def HebrewVetVav(Strng):
     shortVowels = '(' + '|'.join(['\u05B7', '\u05B8', '\u05B4', '\u05BB', '\u05B5', '\u05B6', '\u05B9', '\u05B0']) + ')'
 
     Strng = re.sub(shortVowels + '(' + 'ו' + ')' + '(?!\u05BC)', r'\1' + 'ב', Strng)
 
     # Bet with Holam for Vav with beth with holam
 
@@ -746,34 +993,39 @@
 
     return Strng
 
 def HiraganaaunotDipthong(Strng):
 
     return Strng
 
+#not used
 def IASTISONasalTilde(Strng):
 
     return Strng
 
+#todo testcase
 def HeberewQoph(Strng):
     Strng = Strng.replace('כּ', 'ק').replace('ךּ', 'ק')
 
     return Strng
 
+#todo testcase
 def HebewShortO(Strng):
     Strng = re.sub('(?<!ו)\u05B9', '\u05C7', Strng)
 
     return Strng
 
+#todo testcase
 def HebrewKatevMalei(Strng):
     Strng = Strng.replace('ָ', 'א') # long aa
     Strng = Strng.replace('ַ', 'א') # short a
 
     return Strng
 
+#todo testcase
 def HebrewnonFinalShort(Strng):
     finals = ['ך', 'ם', 'ן', 'ף', 'ץ', 'ףּ', 'ךּ']
     finalCons = ['כ', 'מ', 'נ', 'פ', 'צ', 'פּ', 'כּ']
 
     otherCons = 'ב,ח,ע,צ,ש,ת'.split(',')
     consonantsAll = '(' + '|'.join(GM.CrunchSymbols(GM.Consonants, 'Hebrew') + finals  + ['׳', 'י', 'ו'] + otherCons) + ')'
 
@@ -811,19 +1063,28 @@
     return Strng
 
 def GurmukhiCandrabindu(Strng):
     Strng = Strng.replace('ਁ', 'ਂ')
 
     return Strng
 
+#misnomer
 def mDotAboveToBelow(Strng):
     Strng = Strng.replace('ṃ', 'ṁ')
 
     return Strng
 
+#misnomer
+def mDotBelowToAbove(Strng):
+    Strng = Strng.replace('ṁ', 'ṃ')
+
+    return Strng
+
+#todo : ISOPali postoptions empty todo
+
 def noLongEO(Strng):
     Strng = Strng.replace('ē', 'e').replace('ō', 'o')
 
     return Strng
 
 def TamilStyleUUCore(Strng):
     Strng = re.sub('([ഖഗഘഛഝഠഡഢഥദധഫബഭ])' + '([ുൂ])', r'\1' + '\u200D' + r'\2', Strng)
@@ -1316,14 +1577,20 @@
 
 def Dot2Dandas(Strng):
     Strng = Strng.replace('..', '॥')
     Strng = Strng.replace('.', '।')
 
     return Strng
 
+def Dot2Pipes(Strng):
+    Strng = Strng.replace('..', '||')
+    Strng = Strng.replace('.', '|')
+
+    return Strng
+
 def SaurastraHaaruColon(Strng):
     vir = Tamil.ViramaMap[0]
     ha = Tamil.ConsonantMap[-1]
 
     Strng = Strng.replace(vir + ha, ':')
 
     ListVS = '|'.join(GM.CrunchSymbols(GM.VowelSigns, 'Tamil'))
@@ -1516,25 +1783,237 @@
     return Strng
 
 def SoyomboSpaceTscheg(Strng):
     Strng = Strng.replace(' ', '\U00011A9A')
 
     return Strng
 
+def KhandaTaRomanLoC(Strng):
+    Strng = Strng.replace('ṯ', 'ৎ')
+
+    return Strng
+
+# reverse these in preprocess
+def RomanLoCVaWa(Strng):
+    Strng = Strng.replace('v', 'w')
+    return Strng
+
+def RomanLoCSasha(Strng):
+    Strng = Strng.replace('ṣ', 'sh')
+    return Strng
+
+def RomanLoCSLaDotLaUnderscore(Strng):
+    Strng = Strng.replace('ḻ', 'l̳')
+    Strng = Strng.replace('l̤', 'ḻ')
+
+    return Strng
+
+def RomanLoCLaUnderscoreDoubleDot(Strng):
+    Strng = Strng.replace('ḻ', 'l̤')
+
+    return Strng
+
+def HindiMarathiRomanLoCFix(Strng):
+    Strng = Strng.replace('ṣ', 'sh')
+    Strng = Strng.replace('ḻ', 'ḷ')
+    Strng = Strng.replace('l̳', 'l̤')
+
+    return Strng
+
+def DivesAkuruHomoOrganNasal(Strng):
+    homoNasal = '\U0001193F'
+
+    Strng = re.sub('(𑤐\U0001193E)(?=[𑤌𑤍𑤎𑤏])', homoNasal, Strng)
+    Strng = re.sub('(𑤕\U0001193E)(?=[𑤑𑤒𑤓])', homoNasal, Strng)
+    Strng = re.sub('(𑤚\U0001193E)(?=[𑤖𑤘𑤙])', homoNasal, Strng)
+    Strng = re.sub('(𑤟\U0001193E)(?=[𑤛𑤜𑤝𑤞])', homoNasal, Strng)
+    Strng = re.sub('(𑤤\U0001193E)(?=[𑤠𑤡𑤢𑤣])', homoNasal, Strng)
+
+
+    return Strng
+
+def DivesAkuruAlternateIndVowels(Strng):
+    # use alt /y/
+    Strng = Strng.replace("\U00011925", "\U00011926")
+
+    # replace ind. vow with /y/
+
+    vow = "𑤀 𑤁 𑤂 𑤃 𑤄 𑤅 𑤆 𑤆𑤵 𑤉".split(" ")
+    vowy = "𑤥 𑤥𑤰 𑤥𑤱 𑤥𑤲 𑤥𑤳 𑤥𑤴 𑤥𑤵 𑤥𑤷 𑤥𑤸".split(" ")
+
+    for v, vy in zip(vow, vowy):
+        Strng = Strng.replace(v, vy)
+
+    return Strng
+
+def UseAlternateYA(Strng):
+    Strng = Strng.replace("\U00011925", "\U00011926")
+
+    return Strng
+
+def KawiMoveRepha(Strng):
+    tgt = 'Kawi'
+    repha = '\U00011F02'
+
+    cons = '(' + '|'.join(GM.CrunchSymbols(GM.Consonants + GM.Vowels, tgt)) + ')'
+    vows = '(' + '|'.join(GM.CrunchSymbols(GM.VowelSignsNV, tgt)) + ')'
+    vir = '\U00011F42'
+
+    Strng = re.sub('(('+cons+')' + '('+ vir + cons +')*'+'(' + vows + ')?)' + repha , repha + r'\1', Strng)
+
+    return Strng
+
+def KawiAltAiAU(Strng):
+    #  Alt ai, alt au
+    Strng = Strng.replace('\U00011F3F', '\U00011F3E\U00011F3E')
+
+    return Strng
+
+def KawiDecomposedVowel(Strng):
+    Strng = Strng.replace('\U00011F05', '\U00011F04\U00011F34').replace('\U00011F07', '\U00011F06\U00011F34').replace('\U00011F09', '\U00011F08\U00011F34')
+
+    return Strng
+
+def KawiArchaicJNA(Strng):
+    Strng = Strng.replace('𑼙𑽂𑼛', '\U00011F33')
+    return Strng
+
+def JavaneseArchaicJNA(Strng):
+    Strng = Strng.replace('ꦗ꧀ꦚ', 'ꦘ')
+    return Strng
+
+def JavaneseAvowels(Strng):
+    vowelsA = ['ꦄꦶ', 'ꦄꦷ', 'ꦄꦸ', 'ꦄꦹ', 'ꦄꦽ', 'ꦄ꧀ꦉꦴ', 'ꦄ꧀ꦭꦼ', 'ꦄ꧀ꦭꦼꦴ', 'ꦄꦺ', 'ꦄꦻ', 'ꦄꦺꦴ', 'ꦄꦻꦴ']
+    vowels = ['ꦆ', 'ꦇ', 'ꦈ', 'ꦈꦴ', 'ꦉ', 'ꦉꦴ', 'ꦊ', 'ꦋ', 'ꦌ', 'ꦍ', 'ꦎ', 'ꦎꦴ']
+
+    for v, vA in zip(vowels, vowelsA):
+        Strng = Strng.replace(v, vA)
+
+    return Strng
+
+def TibetanLoCRomanLoCFix(Strng):
+    Strng = re.sub('tʹ(?!s)', 't', Strng)
+    Strng = re.sub('nʹ(?!y)', 'n', Strng)
+    Strng = re.sub('j_h', 'jh', Strng)
+
+    return Strng
+
+def JavaneseSimplified(Strng):
+    Strng = Strng.replace('jny', 'ny')
+    return Strng
+
+def BalineseSimplified(Strng):
+    return Strng
+
+def BalineseRomanLoCFix(Strng):
+    Strng = Strng.replace('ḧ', 'h').replace('ng̈', '‘')
+
+    return Strng
+
+def JavaneseRomanLoCFix(Strng):
+    Strng = Strng.replace('ḧ', 'h').replace('ng̈', '‘')
+
+    return Strng
+
+def BalineseArchaicJNA(Strng):
+    Strng = Strng.replace('ᬚ᭄ᬜ', 'ᭌ')
+    return Strng
+
+def BalineseJavaneseMoveRepha(Strng, tgt, reph):
+    repha = '(' + reph + ')'
+
+    cons = '(' + '|'.join(GM.CrunchSymbols(GM.Consonants, tgt)) + ')'
+    vows = '(' + '|'.join(GM.CrunchSymbols(GM.VowelSignsNV, tgt)) + ')'
+    vir = GM.CrunchSymbols(GM.virama, tgt)[0]
+
+    Strng = re.sub(repha+'('+cons+')'+'('+ vir + cons +')*'+'(' + vows + ')?', r'\2\4\6\1', Strng)
+
+    candAnu = '[' + ''.join(GM.CrunchSymbols(GM.CombiningSigns, tgt)[:2]) + ']'
+    Strng = re.sub(repha+'(' + candAnu + ')', r'\2\1', Strng)
+
+    return Strng
+
+def JavaneseMoveRepha(Strng):
+    return BalineseJavaneseMoveRepha(Strng, 'Javanese', 'ꦂ')
+
+def BalineseMoveRepha(Strng):
+    return BalineseJavaneseMoveRepha(Strng, 'Balinese', 'ᬃ')
+
+def BalineseAvowels(Strng):
+    vowelsA = ['ᬅᬶ', 'ᬅᬷ', 'ᬅᬸ', 'ᬅᬹ', 'ᬅᬺ', 'ᬅᬻ', 'ᬅ᭄ᬮᭂ', 'ᬅ᭄ᬮᭃ', 'ᬅᬾ', 'ᬅᬿ', 'ᬅᭀ', 'ᬅᭁ']
+    vowels = ['ᬇ', 'ᬈ', 'ᬉ', 'ᬊ', 'ᬋ', 'ᬌ', 'ᬍ', 'ᬎ', 'ᬏ', 'ᬐ', 'ᬑ', 'ᬒ']
+
+    for v, vA in zip(vowels, vowelsA):
+        Strng = Strng.replace(v, vA)
+
+    return Strng
+
+def GurmukhiRomanLoCFix(Strng):
+    Strng = re.sub('(m̆|ṃ)(k|g)', 'ṅ' + r'\2', Strng)
+    Strng = re.sub('(m̆|ṃ)(c|j)', 'ñ' + r'\2', Strng)
+    Strng = re.sub('(m̆|ṃ)(ṭ|ḍ)', 'ṇ' + r'\2', Strng)
+    Strng = re.sub('(m̆|ṃ)(t|d)', 'n' + r'\2', Strng)
+    Strng = re.sub('(m̆|ṃ)(p|b)', 'm' + r'\2', Strng)
+
+    return Strng
+
+def DevanagariRomanLoCFix(Strng):
+    Strng = Strng.replace('gḧ', 'g̳h̳').replace('ṭ̈', 't̤').replace('s̈', 's̤')\
+        .replace('ḧ', 'h̤')
+
+    return Strng
+
+def MalayalamRomanLoCFix(Strng):
+    Strng = Strng.replace('ṟṟ', 'ṯṯ')
+    Strng = Strng.replace('ŭ', 'ȧ')
+    return Strng
+
+def MalayalamNTA(Strng):
+    Strng = Strng.replace('nṟ', 'nṯ')
+    return Strng
+
+def MalayalamTTNTA(Strng):
+    Strng = Strng.replace('ṟṟ', 'ṯṯ')
+    Strng = Strng.replace('nṟ', 'nṯ')
+    return Strng
+
+def SinhalaSannakaNasalization(Strng):
+    #Strng = Strng.replace('ṁ', 'ṃ')
+
+    Strng = re.sub('(n̆)(k|g)', 'ṅ' + r'\2', Strng)
+    Strng = re.sub('(n̆)(c|j)', 'ñ' + r'\2', Strng)
+    Strng = re.sub('(n̆)(ṭ|ḍ)', 'ṇ' + r'\2', Strng)
+    Strng = re.sub('(n̆)(t|d)', 'n' + r'\2', Strng)
+    Strng = re.sub('(m̆)(p|b)', 'm' + r'\2', Strng)
+
+    return Strng
+
+def RomanLoCChandrabindu(Strng):
+    #Strng = Strng.replace('ṁ', 'ṃ')
+
+    Strng = re.sub('(m̐)(k|g)', 'n̐' + r'\2', Strng)
+    Strng = re.sub('(m̐)(c|j)', 'n̐' + r'\2', Strng)
+    Strng = re.sub('(m̐)(ṭ|ḍ)', 'n̐' + r'\2', Strng)
+    Strng = re.sub('(m̐)(t|d)', 'n̐' + r'\2', Strng)
+    Strng = re.sub('(m̐)(p|b)', 'n̐' + r'\2', Strng)
+
+    return Strng
+
 def AnusvaratoNasalASTISO(Strng):
-    Strng = Strng.replace('ṁ', 'ṃ')
+    #Strng = Strng.replace('ṁ', 'ṃ')
 
-    Strng = re.sub('(ṃ)(k|g)', 'ṅ' + r'\2', Strng)
-    Strng = re.sub('(ṃ)(c|j)', 'ñ' + r'\2', Strng)
-    Strng = re.sub('(ṃ)(ṭ|ḍ)', 'ṇ' + r'\2', Strng)
-    Strng = re.sub('(ṃ)(t|d)', 'n' + r'\2', Strng)
-    Strng = re.sub('(ṃ)(p|b)', 'm' + r'\2', Strng)
+    Strng = re.sub('(ṃ|ṁ)(k|g)', 'ṅ' + r'\2', Strng)
+    Strng = re.sub('(ṃ|ṁ)(c|j)', 'ñ' + r'\2', Strng)
+    Strng = re.sub('(ṃ|ṁ)(ṭ|ḍ)', 'ṇ' + r'\2', Strng)
+    Strng = re.sub('(ṃ|ṁ)(t|d)', 'n' + r'\2', Strng)
+    Strng = re.sub('(ṃ|ṁ)(p|b)', 'm' + r'\2', Strng)
 
     return Strng
 
+
 def removeDiacritics(Strng):
     diacritics = ['\u0331', '\u0306', '\u0323', '\u035F', '\u0324', '\u035F', '\u0307', '\u0301', '\u0303', '\u0310', '\u0306', '\u0302', '\u0304']
 
     for dia in diacritics:
         Strng = Strng.replace(dia, '')
 
     vowelDia = ['а̄', 'ӣ', 'ӯ', 'ӗ']
@@ -2016,41 +2495,63 @@
              Malayalam.SouthConsonantMap[0]+vir,
              'ഩ്'
             ]
 
     ## may be include ha ?
     CList = [
             Malayalam.ConsonantMap[10:15]+Malayalam.ConsonantMap[24:26]+Malayalam.ConsonantMap[28:29],
-            Malayalam.ConsonantMap[15:20]+Malayalam.ConsonantMap[24:27]+Malayalam.ConsonantMap[28:29],
+            Malayalam.ConsonantMap[15:20]+Malayalam.ConsonantMap[24:27]+Malayalam.ConsonantMap[28:29]+['റ'],
             Malayalam.ConsonantMap[25:27],
             Malayalam.ConsonantMap[20:21] + Malayalam.ConsonantMap[24:26] + Malayalam.ConsonantMap[27:29],
             Malayalam.SouthConsonantMap[0:1]+Malayalam.ConsonantMap[25:27],
-            Malayalam.ConsonantMap[15:20]+Malayalam.ConsonantMap[24:27]+Malayalam.ConsonantMap[28:29]
+            Malayalam.ConsonantMap[15:20]+Malayalam.ConsonantMap[24:27]+Malayalam.ConsonantMap[28:29]+['റ']
             ]
 
     if not reverse:
         for i in range(len(Chillus)):
             #print '(?<!'+'['+vir+''.join(Chillus)+']'+')'+'('+ConVir[i]+')'+'(?!['+''.join(CList[i])+'])'
             Strng = re.sub(ListC + GM.VedicSvaras + '('+ConVir[i]+')'+'(?!['+''.join(CList[i])+'])',r'\1\2' + Chillus[i],Strng)
             Strng = re.sub(ListC + GM.VedicSvaras + '('+ConVir[i]+')'+'(?=(['+''.join(CList[i])+'])' + vir + r'\4' + ')',r'\1\2' + Chillus[i],Strng)
 
-
         ## remove _ appearing due to the preserve chillu option
         Strng = re.sub('(?<!ത്)ˍ', '', Strng)
 
     else:
         if preserve:
             for x,y in zip(Chillus, ConVir):
                 Strng = Strng.replace(x, y +'ˍ') ## Fix the reversal of characters of this
         else:
             for x,y in zip(Chillus, ConVir):
                 Strng = Strng.replace(x, y) ## Fix the reversal of characters of this
 
     return Strng
 
+def historicChillu(Strng):
+    chilluArch = ['\u0D54', '\u0D55', '\u0D56', '\u0D7F']
+    chilluArchhVir = ['മ്', 'യ്', 'ഴ്', 'ക്']
+
+    ListC = '(' + '|'.join(GM.CrunchSymbols(GM.CharactersNV,'Malayalam') + ['ഽ']) + ')'
+
+    vir = Malayalam.ViramaMap[0]
+
+    for ch, chvir in zip(chilluArch, chilluArchhVir):
+        Strng = re.sub('(?<!' + vir + ')' + chvir + '(?!' + ListC + ')', ch, Strng)
+
+    return Strng
+
+def MalayalamLineVirama(Strng):
+    Strng = Strng.replace('\u0D4D', '\u0D3B')
+
+    return Strng
+
+def MalayalamCircVirama(Strng):
+    Strng = Strng.replace('\u0D4D', '\u0D3C')
+
+    return Strng
+
 def RemoveSchwa(Strng,Target):
 
     vir = GM.CrunchSymbols(GM.VowelSigns,Target)[0] + GM.CrunchSymbols(GM.VowelSigns,Target)[0]
     ListC = '|'.join(GM.CrunchSymbols(GM.Consonants,Target))
     ListV = '|'.join(GM.CrunchSymbols(GM.Vowels,Target))
     ListVS = '|'.join(GM.CrunchSymbols(GM.VowelSignsNV,Target))
     ListAll = '|'.join(GM.CrunchSymbols(GM.Vowels+GM.VowelSigns+GM.Consonants+GM.CombiningSigns,Target))
@@ -2081,25 +2582,28 @@
 
     vir = GM.CrunchSymbols(GM.VowelSigns,Target)[0]
     ConUnAsp = [GM.CrunchList('ConsonantMap', Target)[x] for x in [0,2,5,7,10,12,15,17,20,22,4,9,14,19,24,25,26,27,28,29,30,31,32]]
     ConUnAsp = ConUnAsp + GM.CrunchList('SouthConsonantMap',Target) + GM.CrunchList('NuktaConsonantMap',Target)
     ConAsp   = [GM.CrunchList('ConsonantMap', Target)[x] for x in [1,3,6,8,11,13,16,18,21,23]]
     ConOthrs = [GM.CrunchList('ConsonantMap', Target)[x] for x in [0,2,5,7,10,12,15,17,20,22,4,9,14,19,24]]
 
+    if Target == 'Gurmukhi':
+        Strng = Strng.replace('ੱਸ਼਼', 'ਸ਼਼੍ਸ਼਼')
+
     Strng = re.sub('(' + GM.Gemination[Target] + ')' + '('+'|'.join(ConUnAsp)+')', r'\2' + vir + r'\2', Strng)
 
     for i in range(len(ConAsp)):
         Strng = re.sub('(' + GM.Gemination[Target] + ')' + '(' + ConAsp [i] +')', ConUnAsp[i] + vir + r'\2', Strng)
 
     return Strng
 
 def GurmukhiTippiBindu(Strng): # Check this Function
     Bindi = Gurmukhi.AyogavahaMap[1];
     Tippi = '\u0A70'
-    ListTippi = '|'.join(GM.CrunchSymbols(GM.Consonants, 'Gurmukhi')+[Gurmukhi.VowelMap[x] for x in [0,2,3,4]]
+    ListTippi = '|'.join(GM.CrunchSymbols(GM.Consonants, 'Gurmukhi')+[Gurmukhi.VowelMap[x] for x in [0,2,4]]
         +[Gurmukhi.VowelSignMap[1]]+[Gurmukhi.VowelSignMap[3]]+[Gurmukhi.VowelSignMap[4]])
 
     Char = '|'.join(GM.CrunchSymbols(GM.Consonants, 'Gurmukhi') + GM.CrunchSymbols(GM.Vowels, 'Gurmukhi'))
 
     Strng = re.sub('(' + Gurmukhi.VowelSignMap[4] +')' + Bindi + '(?!'+ Char + ')',  r'\1' + Tippi, Strng)
 
     # Strng = '(' + Gurmukhi.VowelSignMap[4] +')' + Bindi + '(=!'+ Char + ')'
@@ -2134,24 +2638,23 @@
 def khandatabatova(Strng):
     Strng = Strng.replace('ৎব', 'ত্ব')
     Strng = Strng.replace('ৎ\u200Cব', 'ত্ব')
 
     return Strng
 
 def BengaliRaBa(Strng):
-    Strng = Strng.replace('ব', 'ৰ').replace('ভ়', 'ব').replace('ৰু', 'ৰ‌ু').replace('ৰূ', 'ৰ‌ূ')
+    Strng = Strng.replace('ৰু', 'ৰ‌ু').replace('ৰূ', 'ৰ‌ূ')
     ## Avoid bba -> rra
     ## break all ba conjuncts
     Strng = Strng.replace('\u09CD\u09F0', '\u09CD\u200C\u09F0')
 
     ## bra/bya bru fix
     Strng = re.sub('(\u09F0)(\u09CD)([\u09B0\u09AF])', r'\1' + '\u200D' + r'\2\3', Strng)
     Strng = re.sub('(\u09F0)(\u09CD)', r'\1\2' + '\u200C', Strng)
 
-
     ## rba
     Strng = Strng.replace('র্‌ৰ', 'ৰ্ৰ')
 
     return Strng
 
 def BengaliIntervocalicDDA(Strng):
     Target = 'Bengali'
@@ -2166,15 +2669,16 @@
     return Strng
 
 def KhandaTa(Strng,Target, reverse=False): #Check for Bhakt - Khanda Ta not formed
 
     ta = GM.CrunchSymbols(GM.Consonants, Target)[15]
     khandata = '\u09CE'
     vir = GM.CrunchSymbols(GM.VowelSigns,Target)[0]
-    ListC = '|'.join([GM.CrunchList('ConsonantMap', Target)[x] for x in [15,16,19,27,24,25,26,28]] + ['ৰ', 'য়'])
+    ListC = '|'.join([GM.CrunchList('ConsonantMap', Target)[x] for x in [15,16,19,27,24,25,26,28]] + ['ব', 'ৰ', 'য়'])
+    #print(ListC)
     if not reverse:
         Strng = re.sub('(?<!' + vir + ')' + '('+ta+')'+'('+vir+')'+'(?!'+ListC+')',khandata, Strng)
         Strng = Strng.replace('ৎˍ', 'ৎ')
     else:
         Strng = Strng.replace(khandata, ta + vir)
 
     return Strng
@@ -2201,35 +2705,37 @@
 
     for svara in GM.VedicSvarasList:
         Strng = Strng.replace(svara + Anu, Anu + svara)
 
     return Strng
 
 def AnusvaraToNasal(Strng,Target):
+    nukta = GM.CrunchList('NuktaMap', Target)[0]
 
     ListN = [GM.CrunchSymbols(GM.Consonants, Target)[x] for x in [4,9,14,19,24]]
     ListC = [
              '|'.join(GM.CrunchList('ConsonantMap', Target)[0:4]),
              '|'.join(GM.CrunchList('ConsonantMap', Target)[5:9]),
              '|'.join(GM.CrunchList('ConsonantMap', Target)[10:14]),
              '|'.join(GM.CrunchList('ConsonantMap', Target)[15:19]),
              '|'.join(GM.CrunchList('ConsonantMap', Target)[20:24]),
             ]
     vir = GM.CrunchSymbols(GM.VowelSigns,Target)[0]
     Anu = GM.CrunchSymbols(GM.CombiningSigns,Target)[1]
 
     for i in range(len(ListN)):
-        Strng = re.sub('('+Anu+')'+ GM.VedicSvaras + '('+ListC[i]+')',ListN[i]+vir+r'\2\3',Strng)
+        Strng = re.sub('('+Anu+')'+ GM.VedicSvaras + '('+ListC[i]+')(?!' + nukta + ')',ListN[i]+vir+r'\2\3',Strng)
 
         if Target == "Tamil":
             Strng = re.sub('(ம்)'+ GM.VedicSvaras + '(ʼ)' + '('+ListC[i]+')',ListN[i]+vir+r'\2\4',Strng)
 
     return Strng
 
 def MalayalamAnusvaraNasal(Strng):
+    ListCAll = '(' + '|'.join(GM.CrunchSymbols(GM.Characters, 'Malayalam')) + ')'
 
     ListNNasal = [Malayalam.ConsonantMap[x] for x in [4,9,14,19,24]]
     ListCNasal = [
              '|'.join(Malayalam.ConsonantMap[0:1]),
              '|'.join(Malayalam.ConsonantMap[5:8]),
              '|'.join(Malayalam.ConsonantMap[10:14]),
              '|'.join(Malayalam.ConsonantMap[15:19]),
@@ -2247,15 +2753,15 @@
 
     Chillus=['\u0D7A','\u0D7B','\u0D7C','\u0D7D','\u0D7E', 'ഩ‍്']
 
     for i in range(len(ListNNasal)):
         Strng = re.sub('('+Anu+')'+'('+ListCNasal[i]+')',ListNNasal[i]+vir+r'\2',Strng)
 
     for i in range(len(ListNAnu)):
-        Strng = re.sub('(?<![' + ".".join(Chillus) + '])' + '('+ListNAnu[i]+')'+'('+vir+')'+'('+ListCAnu[i]+')',Anu+r'\3',Strng)
+        Strng = re.sub(ListCAll + GM.VedicSvaras + '(?<!' + vir + ')'+'(?<![' + ".".join(Chillus) + '])(?<!' + vir +')' + '('+ListNAnu[i]+')'+'('+vir+')'+'('+ListCAnu[i]+')',r'\1\2'+Anu+r'\5',Strng)
 
     return Strng
 
 ## Check Namna, ramya -> Malayalam; fix
 def MToAnusvara(Strng,Target):
 
     M = GM.CrunchList('ConsonantMap', Target)[24] + GM.CrunchList('ViramaMap',Target)[0]
@@ -2398,14 +2904,39 @@
             Strng = re.sub('(?<!h)' + x, y, Strng)
     else:
         for x,y in zip(NativeNumerals, ArabicNumerals):
             Strng = Strng.replace(x, y)
 
     return Strng
 
+def RetainRomanNumerals(Strng,Target, reverse=False):
+    NativeNumerals = GM.CrunchList('NumeralMap', Target)
+    ArabicNumerals = GM.CrunchList('NumeralMap', 'ISO')
+
+    if not reverse:
+        for y,x in zip(ArabicNumerals, NativeNumerals):
+            Strng = re.sub('(?<!h)' + x, y, Strng)
+    else:
+        for y,x in zip(NativeNumerals, ArabicNumerals):
+            Strng = Strng.replace(x, y)
+
+    return Strng
+
+def indicNumerals(Strng):
+    return Strng
+
+def romanFullStop(Strng):
+    return Strng
+
+def indicDandas(Strng):
+    return Strng
+
+def romanNumerals(Strng):
+    return Strng
+
 def RetainTeluguDanda(Strng):
     return RetainDandasIndic(Strng, 'Telugu')
 
 def RetainTeluguNumerals(Strng):
     return RetainIndicNumerals(Strng, 'Telugu')
 
 def RetainTamilDanda(Strng):
@@ -2469,22 +3000,24 @@
 
     for x,y in zip(SuperScript,SubScript):
         Strng = Strng.replace(x,y)
 
     return Strng
 
 def TamilAddFirstVarga(Strng):
-
-    ## Re-order rules correct stuff
-
     CM = GM.CrunchList('ConsonantMap','Tamil')
     ConUnVoiced = '|'.join([CM[x] for x in [0,5,10,15,20]])
-    SuperScript = '|'.join(['\u00B2', '\u00B3','\u2074'])
+    SuperSubScript = '|'.join(['\u00B2', '\u00B3','\u2074', '₂', '₃', '₄'])
 
-    Strng = re.sub('('+ConUnVoiced+')'+'(?!'+SuperScript+')',r'\1'+'\u00B9',Strng)
+    Strng = re.sub('('+ConUnVoiced+')'+'(?!'+SuperSubScript+')',r'\1'+'\u00B9',Strng)
+
+    from . import ConvertFix
+    Strng = ConvertFix.ShiftDiacritics(Strng,'Tamil')
+    #remove spurios one
+    Strng = re.sub('\u00B9'+'(?='+SuperSubScript+')', '', Strng)
 
     return Strng
 
 def SaurashtraHaru(Strng):
 
     ListC = '|'.join([Saurashtra.ConsonantMap[x] for x in [19,24,26,27]])
     vir = Saurashtra.ViramaMap[0]
@@ -2620,21 +3153,20 @@
         if anusvaraChange:
             Strng = Strng.replace(Anu, ng + vir)
 
         Strng = re.sub("(?<!["+EAIO+"])"+"("+cons+")"+"(?!["+AIUVir+"])",r'\1'+shortA,Strng)
         Strng = re.sub("("+shortA+")"+"(?=("+cons+")"+"("+vir+"))",shortAconj,Strng)
 
 
-        # prahlada -> ปรหลาทะ
-        Strng = Strng.replace(shortAconj + 'ห'+vir, 'ห'+vir)
+        # prahlada -> ประหลาทะ
+        Strng = Strng.replace(shortAconj + 'ห'+vir, shortA + 'ห'+vir)
         # katra -> กะตระ
         Strng = re.sub("("+shortAconj+")"+ "(.)("+vir+")([รล])",shortA + r'\2\3\4',Strng)
 
         ## swap rl
-
         consswap = "|".join(GM.CrunchSymbols(GM.Consonants, "Thai"))
         Strng = re.sub("("+consswap+")"+"("+vir+")"+"(["+EAIO+"])"+"([รล])",r"\3\1\2\4",Strng)
 
         ## katro -> กะโตร
         Strng = re.sub(shortAconj +"(["+EAIO+"])", shortA + r'\1', Strng)
 
         Strng = Strng.replace(vir, '')
@@ -2689,14 +3221,15 @@
 def ThamTallAOthers(Strng):
     TallACons = '|'.join(['ᨧ', 'ᨻ', 'ᩁ', 'ᨽ']) ## ca ba ra bha
 
     Strng = FixTallA(Strng, TallACons)
 
     return Strng
 
+#start here
 def LaoPhonetic(Strng):
     Strng = re.sub('(\u0EBA)([ໂເໄ]?)([ຍຣລວຫ])', '\u035C'+ r'\2\3', Strng)
     Strng = re.sub('([ຍຣລວຫ])' + '\u035C' + '([ໂເໄ]?)' + r'\1', r'\1' + '\u0EBA' + r'\2\1', Strng)
 
     Strng = Strng.replace('ຫ\u0EBA', 'ຫ\u035C')
 
     Strng = re.sub('([ຍຣລວຫ])' + '\u035C' + r'\1', r'\1' + '\u0EBA' + r'\1', Strng)
@@ -2721,18 +3254,21 @@
     Target = 'Malayalam'
 
     vir = GM.CrunchSymbols(GM.VowelSigns,Target)[0]
     ConUnAsp = [GM.CrunchList('ConsonantMap', Target)[x] for x in [0,2,5,7,10,12,15,17,20,22,4,9,14,19,24,25,28,29,31]]
     ConUnAsp = ConUnAsp + ['ള']
     ConAsp   = [GM.CrunchList('ConsonantMap', Target)[x] for x in [1,3,6,8,11,13,16,18,21]]
 
-    Strng = re.sub('(' + repha + ')' + '('+'|'.join(ConUnAsp)+')', r'\1\2' + vir + r'\2', Strng)
+    # don't replace after virma
+    # arka -> arkka but arkya -> arkya
+    Strng = re.sub('(' + repha + ')' + '('+'|'.join(ConUnAsp)+')' +'(?!' + vir +')', r'\1\2' + vir + r'\2', Strng)
 
+    # ardha -> arddha but ardya -> ardya
     for i in range(len(ConAsp)):
-        Strng = re.sub('(' + repha + ')' + '(' + ConAsp [i] +')', r'\1' +  ConUnAsp[i] + vir + r'\2', Strng)
+        Strng = re.sub('(' + repha + ')' + '(' + ConAsp [i] +')' +'(?!' + vir +')', r'\1' +  ConUnAsp[i] + vir + r'\2', Strng)
 
     # Dot reph with ya
 
     # Strng = Strng.replace('ൎയ', 'ൎയ്യ')
 
     return Strng
 
@@ -2750,14 +3286,15 @@
     Strng = re.sub('(\u1A58)' + ListV, r'\2\1', Strng)
     Strng = re.sub('(\u1A58)' + ListV, r'\2\1', Strng)
 
     #Strng = Strng.replace('\u1A63\u1A58', '\u1A58\u1A63')
 
     return Strng
 
+# not used
 def FixTallA(Strng, TallACons):
     ListC ='|'.join(GM.CrunchSymbols(GM.Consonants,'TaiTham'))
     Sub =['\u1A55','\u1A56'] # Subjoined Forms of /ra/ and /la/
 
     E = "ᩮ"
     AA = 'ᩣ'
 
@@ -2908,64 +3445,70 @@
     Strng = re.sub("("+tha+"|"+dha+")"+"("+uu+")",r'\1'"𐬡",Strng)
 
     Strng = re.sub("("+ta+")"+"(?!"+"(("+ListV+")"+"|"+"("+ListC+"))"+")","\U00010B1D",Strng)
     Strng = re.sub("("+ta+")"+"(?="+"("+kb+")"+")",'\U00010B1D',Strng)
 
     return Strng
 
+# not used
 def TaiThamO(Strng):
     Strng = Strng.replace("\u1A6E\u1A63","\u1A70")
 
     return Strng
 
+# not used
 def TaiThamHighNga(Strng):
     Strng = Strng.replace('\u1A58','\u1A59')
 
     return Strng
 
+# not used
 def TaiThamMoveNnga(Strng):
-    Strng = re.sub('(.)(\u1A58|\u1A50)',r'\2\1',Strng) # Probably its u1A59
+    Strng = re.sub('(.)(\u1A58)',r'\2\1',Strng) # Probably its u1A59
 
-    return Strng
+    return "Vinodh"
 
 def UrduRemoveShortVowels(Strng):
-    ShortVowels = ['\u0652','\u064E','\u0650','\u064F']
+    ShortVowels = ['\u0652','\u064E','\u0650','\u064F', '\u0658']
 
     for vow in ShortVowels:
         Strng = Strng.replace(vow,"")
 
     return Strng
 
 def LatinPipes(Strng):
     ###
 
     return Strng
 
+# not used
 def PhagsPaRearrange(Strng,Target):
     vir = GM.CrunchList('ViramaMap', Target)[0]
     ListC = '|'.join(GM.CrunchSymbols(GM.Consonants,Target))
     ListV = '|'.join(GM.CrunchSymbols(GM.Vowels,Target))
     ListVS = '|'.join(GM.CrunchSymbols(GM.VowelSignsNV,Target))
 
     Strng = re.sub("(?<!( |"+vir+"))"+"("+ListC+")"+"(?= )",r'\2'+vir,Strng)
     #print Strng
 
     Strng = Strng.replace(" ","").replace("᠂"," ").replace("᠃"," ")
     return Strng
 
+# not used
 def DevanagariAVowels(Strng):
     oldVowels = Devanagari.VowelMap[2:12]+Devanagari.SouthVowelMap[:1]
     a = Devanagari.VowelMap[0]
     newAVowels = [a+x for x in Devanagari.VowelSignMap[1:11]+Devanagari.SouthVowelSignMap[:1]]
 
     for x,y in zip(oldVowels,newAVowels):
         Strng = Strng.replace(x,y)
 
     return Strng
 
+# not used
 def AnusvaraToNasalIPA(Strng):
 
     Strng = Strng.replace("̃k","ŋk")
     Strng = Strng.replace("̃g","ŋg")
 
     Strng = Strng.replace("̃c","ɲc")
     Strng = Strng.replace("̃j","ɲj")
@@ -2986,20 +3529,22 @@
     Strng = Strng.replace("̃ːd̪","ːn̪d̪")
 
     Strng = Strng.replace("̃ːɖ","ːɳɖ")
     Strng = Strng.replace("̃ːʈ","ːɳʈ")
 
     return Strng
 
+# not used
 def IPARemoveCross(Strng):
 
     Strng = Strng.replace('×','')
 
     return Strng
 
+# not used
 def ChakmaAVowels(Strng):
 
     return Strng
 
 def ZanabazarSquareContextual(Strng):
     yrlv = ZanabazarSquare.ConsonantMap[25:29]
     yrlv_sub = ['\U00011A3B', '\U00011A3C', '\U00011A3D', '\U00011A3E']
@@ -3019,20 +3564,20 @@
 
 def ZanabazarSquareMongolianFinal(Strng):
     Strng = Strng.replace(ZanabazarSquare.ViramaMap[0], '\U00011A33')
 
     return Strng
 
 def TamilRemoveApostrophe(Strng):
-    Strng = Strng.replace('ʼ', '')
+    Strng = Strng.replace('ʼ', '').replace('ˮ', '')
 
     return Strng
 
 def TamilRemoveNumbers(Strng):
-    numerals = ['²', '³', '⁴', '₂', '₃', '₄']
+    numerals = ['²', '³', '⁴', '₂', '₃', '₄', '¹', '₁']
 
     for num in numerals:
         Strng = Strng.replace(num, '')
 
     return Strng
 
 def NewaSpecialTa(Strng):
@@ -3041,20 +3586,37 @@
 
     return Strng
 
 def TamilDisableSHA(Strng):
     Strng = Strng.replace('ஶ', 'ஷ²')
     Strng = CF.ShiftDiacritics(Strng,'Tamil')
 
+    Strng = Strng.replace( 'ஷ்²ரீ', 'ஶ்ரீ')
+
     return Strng
 
 def swapEe(Strng):
-    Strng = Strng.replace('e', 'X@X@')
+    Strng = Strng.replace('E', 'X@X@')
     Strng = Strng.replace('e', 'E')
-    Strng = Strng.replace('X@X@')
+    Strng = Strng.replace('X@X@', 'e')
+
+    Strng = Strng.replace('O', 'X@X@')
+    Strng = Strng.replace('o', 'O')
+    Strng = Strng.replace('X@X@', 'o')
+
+    return Strng
+
+def swapEeItrans(Strng):
+    Strng = Strng.replace('^e', 'X@X@')
+    Strng = Strng.replace('e', 'E')
+    Strng = Strng.replace('X@X@', 'e')
+
+    Strng = Strng.replace('^o', 'X@X@')
+    Strng = Strng.replace('o', 'O')
+    Strng = Strng.replace('X@X@', 'o')
 
     return Strng
 
 def capitalizeSentence(Strng):
     Strng = re.sub(r"(\A\w)|"+            # start of string
              "(?<!\.\w)([\.?!]\s*)\w|"+     # after a ?/!/. and a space,
              "\w(?:\.\w)|"+
```

### Comparing `aksharamukha-2.1.2/aksharamukha/PreProcess.py` & `aksharamukha-2.2.1/aksharamukha/PreProcess.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,301 @@
 # -*- coding: utf-8 -*-
 
 from ast import Str
 from asyncio import constants
 from . import GeneralMap as GM
 import re
 import string
+import unicodedata
 from . import PostProcess
 from . import ConvertFix as CF
-from aksharamukha.ScriptMap.EastIndic import PhagsPa, Burmese
+from aksharamukha.ScriptMap.EastIndic import PhagsPa, Burmese, Khmer
 from aksharamukha.ScriptMap.MainIndic import Tamil, Malayalam, Limbu, Chakma
 ### Use escape char in all functions
 
-def IASTLOCBurmeseSource(Strng):
+def ItransLL(Strng):
+    return Strng
+
+def RomanLoCChandrabindu(Strng):
+    Strng = re.sub('n̐', 'm̐', Strng)
+
+    return Strng
+
+def BalineseRomanLoCFix(Strng):
+    Strng = Strng.replace('‘', 'ng̈')
+
+    return Strng
+
+def JavaneseRomanLoCFix(Strng):
+    Strng = Strng.replace('‘', 'ng̈')
+
+    return Strng
+
+def HindiMarathiRomanLoCFix(Strng):
+    Strng = Strng.replace('sh', 'ṣ')
+    Strng = Strng.replace('ḷ', 'ḻ')
+    Strng = Strng.replace('l̤', 'l̳')
+
+    return Strng
+
+def RomanLoCLaUnderscoreDoubleDot(Strng):
+    Strng = Strng.replace('ḻ', 'l̤')
+
+# reverse these in preprocess
+def RomanLoCVaWa(Strng):
+    Strng = Strng.replace('w', 'v')
+    return Strng
+
+def RomanLoCSasha(Strng):
+    Strng = Strng.replace('sh', 'ṣ')
+
+    return Strng
+
+def RomanLoCSLaDotLaUnderscore(Strng):
+    Strng = Strng.replace('ḻ', 'l̤')
+    Strng = Strng.replace( 'l̳', 'ḻ',)
+
+    return Strng
+
+def RomanLoCLaUnderscoreDoubleDot(Strng):
+    Strng = Strng.replace('l̤', 'ḻ')
+
+    return Strng
+
+def MalayalamRomanLoCFix(Strng):
+    Strng = Strng.replace('ṯṯ', 'ṟṟ')
+    Strng = Strng.replace('ȧ', 'ŭ')
+    return Strng
+
+def DevanagariRomanLoCFix(Strng):
+    Strng = Strng.replace('g̳h̳', 'gḧ').replace('t̤', 'ṭ̈').replace('s̤', 's̈')\
+        .replace('h̤', 'ḧ')
+
+    return Strng
+
+def IASTLDotRetroflex(Strng):
+    Strng = Strng.replace('ḷ', 'l̤')
+
+    return Strng
+
+def ArchaicJnaSimplifyRomanLOC(Strng):
+    Strng = Strng.replace('ꦘ', 'ꦚ')
+    return Strng
+
+def KhandaTaRomanLoC(Strng):
+    Strng = Strng.replace('ৎ', 'ṯ')
+
+    return Strng
+
+def TibetanLoCRomanLoCFix(Strng):
+    Strng = re.sub('t(?![ʹhs])', 'tʹ', Strng)
+    Strng = re.sub('n(?![ʹy])', 'nʹ', Strng)
+
+    return Strng
+
+def BalineseJavaneseMoveRepha(Strng, tgt, reph):
+    repha = '(' + reph + ')'
+
+    cons = '(' + '|'.join(GM.CrunchSymbols(GM.Consonants, tgt)) + ')'
+    vows = '(' + '|'.join(GM.CrunchSymbols(GM.VowelSignsNV, tgt)) + ')'
+    vir = GM.CrunchSymbols(GM.virama, tgt)[0]
+
+    candAnu = '[' + ''.join(GM.CrunchSymbols(GM.CombiningSigns, tgt)[:2]) + ']'
+    Strng = re.sub('(' + candAnu + ')' + repha, r'\2\1', Strng)
+
+    Strng = re.sub('('+cons+')'+'('+ vir + cons +')*'+'(' + vows + ')?'+ repha, r'\7\1\3\5', Strng)
+
+    return Strng
+
+def DivesAkuruAlternateIndVowels(Strng):
+    # use alt /y/
+    #Strng = Strng.replace("\U00011925", "\U00011926")
+
+    # replace ind. vow with /y/
+
+    vow = "𑤁 𑤂 𑤃 𑤄 𑤅 𑤆 𑤆𑤵 𑤉 𑤀".split(" ")
+    vowy = "𑤥𑤰 𑤥𑤱 𑤥𑤲 𑤥𑤳 𑤥𑤴 𑤥𑤵 𑤥𑤷 𑤥𑤸 𑤥".split(" ")
+
+    for v, vy in zip(vow, vowy):
+        Strng = Strng.replace(vy, v)
+
+    return Strng
+
+def KawiMoveRepha(Strng):
+    tgt = 'Kawi'
+    repha = '\U00011F02'
+
+    cons = '(' + '|'.join(GM.CrunchSymbols(GM.Consonants + GM.Vowels, tgt)) + ')'
+    vows = '(' + '|'.join(GM.CrunchSymbols(GM.VowelSignsNV, tgt)) + ')'
+    vir = '\U00011F42'
+
+    Strng = re.sub(repha + '(('+cons+')' + '('+ vir + cons +')*'+'(' + vows + ')?)', r'\1' + repha, Strng)
+
+    return Strng
+
+def JavaneseMoveRepha(Strng):
+    return BalineseJavaneseMoveRepha(Strng, 'Javanese', 'ꦂ')
+
+def BalineseMoveRepha(Strng):
+    return BalineseJavaneseMoveRepha(Strng, 'Balinese', 'ᬃ')
+
+def OriyaSubojinedVa(Strng):
+    Strng = re.sub('(??<![ମବ])(୍ବ)', '୍ୱ', Strng)
+
+    return Strng
+
+def BengaliSubojinedVa(Strng):
+    Strng = re.sub('(?<![মব])(্ব)', '্ভ়', Strng)
+
+    return Strng
+
+def BengaliTargetVa(Strng):
+    Strng = Strng.replace('ব', 'ভ়')
+
+    return Strng
+
+def OriyaTargetVa(Strng):
+    Strng = Strng.replace('ବ', 'ୱ')
+
+    return Strng
+
+def RetainDevangariDanda(Strng):
+    Strng = Strng.replace('।', '│').replace('॥', '┃')
+
+    return Strng
+
+def RetainPipeDanda(Strng):
+    Strng = Strng.replace("।", "|").replace("॥", "||")
+    Strng = Strng.replace(".", "●")
+    Strng = Strng.replace("||", "┃").replace("|", "│")
+
+    return Strng
+
+#ThamLoC
+def ThamLoCRomanLoCTarget(Strng):
+    ListC ='|'.join(GM.CrunchSymbols(GM.Consonants,'ThamLoC'))
+
+    #Fix o
+    Strng = Strng.replace('ᩮᩣ', 'ᩰ')
+
+    #eo
+    Strng = re.sub('ᩴ᩠ᨿ', '\u1A74\u1A7Fᨿ', Strng)
+
+    #aiy
+    Strng = re.sub('ᩱ᩠ᨿ', 'ᩱ\u1A7Fᨿ', Strng)
+
+    #koi
+    Strng = re.sub('᩠ᩅᩭ', '\u1A7Fᩅᩭ', Strng)
+
+    #au
+    Strng = re.sub('\u1A60\u1A45\u1A6B', '\u1A7F\u1A45\u1A6B', Strng)
+
+    #close e/au
+    Strng = re.sub('(᩠)(ᨿ|ᩅ)(?=(' + ListC + '))', '\u1A7F'+r'\2', Strng)
+
+
+    return Strng
+
+def ThamLoCRomanLoCSource(Strng):
+    ListC ='|'.join(GM.CrunchSymbols(GM.Consonants,'ThamLoCRomanLoC'))
+    ListV ='|'.join(GM.CrunchSymbols(GM.Vowels,'ThamLoCRomanLoC'))
+
+    #a
+    Strng = re.sub('(a|ǫḥ|ǫ|œ|au)(?=(' + ListC + '))', r'\1''\u02BD', Strng)
+
+    return Strng
+
+def KhmerWordSplit(Strng):
+    from khmernltk import word_tokenize
+    sents = Strng.split('\n')
+    sent_token = []
+    for sent in sents:
+        sent_token.append(' '.join(word_tokenize(sent)))
+    Strng = '\n'.join(sent_token)
+    Strng = Strng.replace('  ', ' ')
+
+    return Strng
+
+def KhmerLoCRomanLoCTarget(Strng):
+    ListC ='|'.join(GM.CrunchSymbols(GM.Consonants,'Khmer'))
+    ListV ='|'.join(GM.CrunchSymbols(GM.VowelSigns,'Khmer'))
+    ListA ='|'.join(GM.CrunchSymbols(GM.CombiningSigns,'Khmer'))
+
+    vir = Khmer.ViramaMap[0]
+
+    #Mark im
+    Strng = Strng.replace('ឹ', 'ិំ\u02BD')
+
+    #move bantoc around
+    Strng = re.sub('(.)(.(\u17D2.)*)(\u17CB)', r'\1\4\2', Strng)
+
+    #mark consonant modifiers with subbase form
+    Strng = re.sub('([ងញមបយរវ])(ុ)([ិឹីឺ])', r'\1''៉'r'\3', Strng)
+    Strng = re.sub('([សហអ])(ុ)([ិឹីឺ])', r'\1''៊'r'\3', Strng)
+
+    #move tonemarks around
+    Strng = re.sub('('+ListC+')'+'([៎៏])''('+ListV+')''('+ListA+')?',r'\1\3\4\2',Strng)
+    Strng = re.sub('('+ListC+')'+'('+ListV+')''([៎៏៊៉])''('+ListA+')?',r'\1\2\4\3',Strng)
+
+    #fix oya to oy
+    Strng = Strng.replace('ឲ្យ', 'ឱ្យ').replace('ឱ្យ', 'ឱ្យ' + vir)
+
+    #ignore the following
+    Strng = re.sub('[៙៚]', '', Strng)
+
+    return Strng
+
+def KhmerLoCRomanLoCSource(Strng):
+    listdenormalize = ['å', 'ẙ', 'à', 'á', 'é', 'í', 'ó', 'ú', 'à', 'è', 'ì', 'ò', 'ù', 'ă']
+
+    for let in listdenormalize:
+        Strng = Strng.replace(let, unicodedata.normalize('NFD', let))
+
+    Strng = re.sub('‛(?!ʹ)', '‛ʹ', Strng)
+    Strng = re.sub('oaḥ', 'oḥ', Strng)
+
+    return Strng
+
+# shan
+def ShanLoCRomanLoCTarget(Strng):
+    #preserve ႂ်
+    Strng = Strng.replace('ႂ်', '\u036E')
+
+    # Shan normalize /aa/
+    Strng = Strng.replace('ၢ', 'ႃ')
+    Strng = Strng.replace('ါ', 'ႃ')
+
+    Strng = Strng.replace('ႃႆ', 'ၢႆ').replace('ႆၢ', 'ၢႆ').replace('ႆႃ', 'ၢႆ')
+
+    # asat + virma to just virama
+    Strng = Strng.replace('\u103A\u1039', '\u1039')
+
+    ## sort subjoined consonants
+    yrv = Burmese.ConsonantMap[25:27] + Burmese.ConsonantMap[28:29]
+    yrvsub = ['\u103B','\u103C','\u1082']
+    vir = Burmese.ViramaMap[0]
+
+    for x,y in zip(yrv,yrvsub):
+        # Undo Replace subjoining forms: exp-virama + y/r/v/h <- subjoining y/r/v/h
+        Strng = Strng.replace(y, vir + vir + x)
+
+    # mark pure viramas
+    aThat = r'်'
+    Strng = re.sub('(?<!ႃ)'+aThat, aThat + 'ʻ', Strng)
+
+    # mark a as glottalstop
+    Strng = Strng.replace('ဢ','’ဢ')
+
+    return Strng
+
+def ShanLoCRomanLoCSource(Strng):
+
+    return Strng
+
+def BurmeseRomanLoCSource(Strng):
     # adhoc chars
     chars_misc = {
         "e*": "၏",
         'n*': "၌",
         'r*': '၍',
         'l*': '၎'
     }
@@ -45,14 +325,33 @@
     Strng = Strng.replace('o‘', 'oʻ')
 
     # reverse o' to au
     Strng = Strng.replace('oʻ', 'au')
 
     return Strng
 
+def paliTham(Strng):
+
+    return Strng
+
+def segmentThamSyllabes(Strng):
+    # segment text into syllables
+
+    # https://github.com/ye-kyaw-thu/myWord/blob/main/syl_segment.py
+    myConsonant = r"ᨠ-ᩌ"
+    otherChar = r"ᩍ-ᩔ!-/:-@[-`{-~\s"
+    ssSymbol = r'᩠'
+    aThat = r'᩺'
+
+    BreakPattern = re.compile(r"((?<!" + ssSymbol + r")["+ myConsonant + r"](?![" + aThat + ssSymbol + r"])" + r"|["  + otherChar + r"])", re.UNICODE)
+    #Strng = Strng.replace("့်", "့်")
+    Strng = BreakPattern.sub(' ' + r"\1", Strng)
+
+    return Strng
+
 def segmentBurmeseSyllables(Strng):
     # segment text into syllables
 
     # https://github.com/ye-kyaw-thu/myWord/blob/main/syl_segment.py
     myConsonant = r"က-အ"
     otherChar = r"ဣဤဥဦဧဩဪဿ၌၍၏၀-၉၊။!-/:-@[-`{-~\s"
     ssSymbol = r'္'
@@ -60,15 +359,30 @@
 
     BreakPattern = re.compile(r"((?<!" + ssSymbol + r")["+ myConsonant + r"](?![" + aThat + ssSymbol + r"])" + r"|["  + otherChar + r"])", re.UNICODE)
     Strng = Strng.replace("့်", "့်")
     Strng = BreakPattern.sub(' ' + r"\1", Strng)
 
     return Strng
 
-def IASTLOCBurmeseTarget(Strng):
+def segmentShanSyllables(Strng):
+    # segment text into syllables
+
+    # https://github.com/ye-kyaw-thu/myWord/blob/main/syl_segment.py
+    myConsonant = r"ၵၶၷꧠငၸꧡꩡꧢၺꩦꩧꩨꩩꧣတထၻꩪၼပၽၿꧤမယရလဝသႁꩮၹၾႀဢ"
+    otherChar = r"႞႟႐-႙၊။!-/:-@[-`{-~\s"
+    ssSymbol = r'္'
+    aThat = r'်'
+
+    BreakPattern = re.compile(r"((?<!" + ssSymbol + r")["+ myConsonant + r"](?![" + aThat + ssSymbol + r"])" + r"|["  + otherChar + r"])", re.UNICODE)
+    Strng = Strng.replace("့်", "့်")
+    Strng = BreakPattern.sub(' ' + r"\1", Strng)
+
+    return Strng
+
+def BurmeseRomanLoCTarget(Strng):
     # asat + virma to just virama
     Strng = Strng.replace('\u103A\u1039', '\u1039')
 
     # swap iu -> ui
     Strng = Strng.replace('\u102D\u102F', '\u102F\u102D')
 
     # mark Independent au -> o'
@@ -285,17 +599,15 @@
     return Strng
 
 def ShowChillus(Strng):
 
     return PostProcess.MalayalamChillu(Strng, True, True)
 
 def ShowKhandaTa(Strng):
-    print(Strng)
     Strng = Strng.replace('ৎ', 'ত্ˍ')
-    print(Strng)
 
     return Strng
 
 def eiaudipthongs(Strng):
 
     return Strng
 
@@ -390,14 +702,17 @@
         # Medials + Unvoiced -> Voiced
         Strng = re.sub('('+ConMedials+')'+'('+vir+')'+ConUnVoiced[i]+'(?!'+vir+')',r'\1\2'+ConVoicedS[i],Strng)
 
     #RRA NRA
 
     Strng = Strng.replace('റ്റ', 'ട്ട').replace('ന്റ', 'ണ്ഡ')
 
+    #anusvara with m
+    Strng = Strng.replace('ം', 'മ്')
+
     return Strng
 
 def retainLatin(Strng, reverse=False):
     latn_basic_lower = 'a b c d e f g h i j k l m n o p q r s t u v w x y z ḥ ṭ ṣ ʾ ʿ š ā ī ū ē ō'
     latn_basic_upper = latn_basic_lower.upper()
     latn_all = latn_basic_lower + latn_basic_upper
     latn_all = latn_all.split(' ')
@@ -667,26 +982,30 @@
 def LaoSajhayaOrthographywithA(Strng):
     Strng = Strng.replace('ະ', '')
     Strng = LaoSajhayaOrthography(Strng)
 
     return Strng
 
 # consider adding an optional NUkta to the post consonantal position
-def RemoveSchwaHindi(Strng):
+def RemoveSchwaHindi(Strng, showschwa=False):
     VowI = "(" + '|'.join(GM.CrunchSymbols(GM.Vowels,'Devanagari')) + ")"
     VowS = "(" + '|'.join(GM.CrunchSymbols(GM.VowelSignsNV, 'Devanagari')) + ")"
     Cons = "(" + '|'.join(GM.CrunchSymbols(GM.Consonants, 'Devanagari')) + ")"
     Char = "(" + '|'.join(GM.CrunchSymbols(GM.Characters, 'Devanagari')) + ")"
     Nas = "([ंःँ]?)"
     ISyl = "((" + VowI + "|" + "(" + Cons + VowS + "?" + "))" + Nas +')'
     Syl = "((" + Cons + VowS + ')' + Nas + ")"
     SylAny = "((" + Cons + VowS + "?" + ')' + Nas + ")"
 
-    vir = '्'
-    vir2 = '्'
+    if not showschwa:
+        vir = '्'
+        vir2 = '्'
+    else:
+        vir = '\u0954'
+        vir2 = '\u0954'
 
     Strng = re.sub(ISyl+Cons+Cons+SylAny+"(?!" + Char + ")", r'\1\8' + vir + r'\9\10', Strng) # bhAratIya --> bhArtIy
     Strng = re.sub(ISyl+Cons+Syl+SylAny+"(?!" + Char + ")", r'\1\8' + vir + r'\9\15', Strng) # bhAratIya --> bhArtIy
     Strng = re.sub(ISyl+Cons+Syl+"(?!" + Char + ")", r'\1\8' + vir + r'\9', Strng) # namakIn -> namkIn
 
     Strng = re.sub(ISyl+Cons+"(?!" + Char + ")", r'\1\8' + vir, Strng) # kama -> kam
 
@@ -724,29 +1043,36 @@
     if Target == 'Bengali':
         Strng = PostProcess.KhandaTa(Strng, Target, True)
 
     VowI = "(" + '|'.join(GM.CrunchSymbols(GM.Vowels,Target)) + ")"
     VowS = "(" + '|'.join(GM.CrunchSymbols(GM.VowelSignsNV, Target)) + ")"
     Cons = "(" + '|'.join(GM.CrunchSymbols(GM.Consonants, Target)) + ")"
     Char = "(" + '|'.join(GM.CrunchSymbols(GM.Characters, Target)) + ")"
-
     Nas = "([" + '|'.join(GM.CrunchList('AyogavahaMap',Target)) + "]?)"
 
     ISyl = "((" + VowI + "|" + "(" + Cons + VowS + "?" + ")" + Nas + '))'
     Syl = "((" + Cons + VowS + ')' + Nas + ")"
     SylAny = "((" + Cons + VowS + "?" + ')' + Nas + ")"
 
     vir = GM.CrunchList("ViramaMap", Target)[0]
     if Target != 'Bengali':
         Cons2 = '((' + Cons + vir + ')?' + Cons + ')'
     else:
         Cons2 = '(()?' + Cons + ')'
 
-    Strng = re.sub(ISyl + Cons2+"(?!" + Char + ")", r'\1\8' + vir, Strng) # kama -> kam
-    Strng = re.sub(ISyl + Cons2+"(?!" + Char + ")", r'\1\8' + vir, Strng) # kama -> kam
+    if Target == 'Khmer' or Target == 'KhmerLoC':
+        ListC ='|'.join(GM.CrunchSymbols(sorted(GM.Consonants, key=len, reverse=True),Target))
+        ra = Khmer.ConsonantMap[26]
+        Strng = re.sub('('+ListC+')'+'\u17CC',ra+'\u17D2'+r'\1',Strng)
+
+        Strng = re.sub(ISyl + '('+ListC +')' + '(((\u17D2)' + '('+ListC +'))*)([៍៎៏]?)(?=[\s\n])', r'\1\8\9' + vir + r'\13', Strng) # kama -> kam
+        Strng = re.sub(ISyl + '('+ListC +')' + '(((\u17D2)' + '('+ListC +'))*)([៍៎៏]?)$', r'\1\8\9' + vir + r'\13', Strng) # kama -> kam
+    else:
+        Strng = re.sub(ISyl + Cons2+"(?!" + Char + ")", r'\1\8' + vir, Strng) # kama -> kam
+        Strng = re.sub(ISyl + Cons2+"(?!" + Char + ")", r'\1\8' + vir, Strng) # kama -> kam
 
     #Strng = re.sub(VowI + Nas + Cons2+"(?!" + Char + ")", r'\1\2\3' + vir, Strng)
 
     return Strng
 
 def SchwaFinalGurmukhi(Strng):
 
@@ -762,14 +1088,26 @@
 
 def SchwaFinalBengali(Strng):
 
     Strng = RemoveFinal(Strng, 'Bengali')
 
     return Strng
 
+def SchwaFinalKhmerLoC(Strng):
+
+    Strng = RemoveFinal(Strng, 'KhmerLoC')
+
+    return Strng
+
+def SchwaFinalKhmer(Strng):
+
+    Strng = RemoveFinal(Strng, 'Khmer')
+
+    return Strng
+
 def SchwaFinalWarangCiti(Strng):
     Target = "WarangCiti"
 
     VowI = "(" + '|'.join(GM.CrunchSymbols(GM.Vowels,Target)) + ")"
     VowS = "(" + '|'.join(GM.CrunchSymbols(GM.VowelSignsNV, Target)) + ")"
     Cons = "(" + '|'.join(GM.CrunchSymbols(GM.Consonants, Target)) + ")"
     Char = "(" + '|'.join(GM.CrunchSymbols(GM.Characters, Target)) + ")"
@@ -907,23 +1245,23 @@
 
 def joinVowelConsIAST(Strng):
     return joinVowelCons(Strng, 'IAST')
 
 def joinVowelConsISO(Strng):
     return joinVowelCons(Strng, 'ISO')
 
-def PreProcess(Strng,Source,Target):
+def PreProcess(Strng,Source,Target,postoptions,preoptions):
     if Source in GM.RomanDiacritic or Source == 'Latn':
         Strng = Strng.lower()
 
-
-    pipeScripts = ["HK", "IASTPali", "IAST", "ISO"]
-
-    if Source in pipeScripts:
-        Strng = Strng.replace("|", ".").replace("||", "..")
+    if Source in GM.pipeScripts:
+        if '|' in Strng:
+            Strng = Strng.replace(".", "●")
+            Strng = Strng.replace("।", "|").replace("॥", "||")
+            Strng = Strng.replace("|", ".").replace("||", "..")
 
     if 'Arab' in Source:
         Strng = re.sub('([وي])(?=[\u064E\u0650\u064F\u0651\u064B\u064C\u064D])', '\u02DE' + r'\1', Strng)
         #Strng = re.sub('((\u064E|\u0650|\u0652|\u064F))(\u0651)', r'\2', Strng)
 
     if Source in ["Syrj", "Syrn"]:
         Strng = Strng.replace('\u0323', '\u0742')
@@ -945,61 +1283,55 @@
 
         Strng = re.sub(punc + sOm + punc, r'\1' + tOm + r'\2', Strng)
         Strng = re.sub('^' + sOm + punc, tOm + r'\1', Strng)
         Strng = re.sub(punc + sOm + '$', r'\1' + tOm, Strng)
         Strng = re.sub('^' + sOm + '$', tOm, Strng)
 
 
+        # kaRRi -> katri etc. not kaVoc.R
+        Strng = re.sub('([aAiuUeoEO])([R]){2}([iI])', r'\1'+r'\2'+'_'+r'\2'+r'\3', Strng)
+        Strng = re.sub('([aAiuUeoEO])([L]){2}([iI])', r'\1'+r'\2'+'_'+r'\2'+r'\3', Strng)
+
         AltForm = ['O', 'aa','ii','uu','RRi','RRI','LLi','LLI','N^','JN','chh','shh','x','GY','.n','.m','.h', 'AUM', 'E', 'J', 'c.o', 'c.e']
         NormForm = ['^o', 'A','I','U','R^i','R^I','L^i','L^I','~N','~n','Ch','Sh','kSh','j~n','M','M','','oM', '^e', 'z', 'A.c', 'e.c']
 
         for x,y in zip(AltForm,NormForm):
             Strng = Strng.replace(x,y)
 
         AltForms = [('ee', 'I'), ('dny', 'j~n'), ('oo', 'U'), ('kS', 'kSh'), ('w', 'v'), ('|', '.'), ('kShh', 'kSh')]
 
         for x,y in AltForms:
             Strng = Strng.replace(x,y)
 
         Strng = Strng.replace('OM', 'oM')
 
+
     if Source == 'BarahaNorth' or Source == 'BarahaSouth':
-        Strng = Strng.replace('A', 'aa')
-        Strng = Strng.replace('I', 'ee')
-        Strng = Strng.replace('U', 'oo')
-
-        Strng = Strng.replace('ou', 'au')
-        Strng = Strng.replace('K', 'kh')
-        Strng = Strng.replace('G','gh')
-        Strng = Strng.replace('ch', 'c')
-        Strng = Strng.replace('Ch', 'C')
-        Strng = Strng.replace('J','jh')
-        Strng = Strng.replace('w', 'v')
-        Strng = Strng.replace('sh', 'S')
-        Strng = Strng.replace('~h', '_h')
-        Strng = Strng.replace('^', '()')
-        Strng = Strng.replace('^^', '{}')
-
-        Strng = Strng.replace('tx', 'rx')
-        Strng = Strng.replace('zh', 'Lx')
-
-        Strng = Strng.replace('q', '\_')
-        Strng = Strng.replace('#', "\\'")
-        Strng = Strng.replace('$', '\\"')
+        # alternate representations
 
+        alt_baraha = [('A', 'aa'), ('I', 'ee'), ('U', 'oo'), ('~loo', '~lU'), ('Roo', 'RU'), ('ou', 'au'), ('K', 'kh'), ('G','gh'), ('ch', 'c'), ('Ch', 'C'), ('J','jh'), ('P', 'ph'), ('B', 'bh'), ('w', 'v'), ('sh', 'S'), ('~h', '_h'), ('Y', 'yx'), ('^^', '{}'), ('^', '()'), ('tx', 'rx'), ('zh', 'Lx'), ('~e', '~a'), ('q', '\_'), ('#', "\\'"), ('$', '\\"')]
 
-    if Source == 'IAST':
+        for alt, norm in alt_baraha:
+            Strng = Strng.replace(alt, norm)
+
+        if Target == 'Tamil':
+            Strng = Strng.replace('n', 'nx').replace('~nx', 'n')
+            print(Strng)
+
+    if 'IAST' in Source:
         Strng = Strng.replace("aï", "a_i")
         Strng = Strng.replace("aü", "a_u")
         Strng = Strng.replace('\u0303', 'ṃ')
 
-    if Source == "ISO":
+    if "ISO" in Source:
         Strng = Strng.replace('a:i', 'a_i')
         Strng = Strng.replace('a:u', 'a_u')
         Strng = Strng.replace('\u0303', 'ṁ')
+        ## People use the wrong convention sometimes
+        Strng = Strng.replace('ṃ', 'ṁ')
 
     if Source == "Titus":
         Strng = Strng
 
     if Source == "ISO" or Source == "IAST" or Source == "Titus" or "RussianCyrillic":
         Strng = CF.VedicSvarasNonDiacritic(Strng)
 
@@ -1028,14 +1360,24 @@
 
     ## Normalize Input Strings
 
     Strng = normalize(Strng,Source)
 
     ## Remove unsupported letters and replace with supported ones
 
+    #Fix Udata + Avagraha combination
+    # नमो॑ऽयम् --> namo̍​'yam
+    if Source in GM.IndicScripts and Target in GM.Transliteration:
+        udatta = '\u0951'
+        avagrahaSrc = GM.CrunchList('SignMap', Source)[0]
+        avagrahaTgt = GM.CrunchList('SignMap', Target)[0]
+
+        if avagrahaTgt == "'":
+            Strng = Strng.replace(udatta + avagrahaSrc, udatta + '\u200B' + avagrahaSrc)
+
     return Strng
 
 def ISO259Target(Strng):
     Strng = Strng.replace('א', 'ʾ').replace('׳', '’')
 
     return Strng
 
@@ -1098,15 +1440,14 @@
         ('š̮', 'š'), ('š', 's̀'), ('š̪', 'ś'),
         ('ā', 'å'), ('e', 'ȩ'), ('ō', 'ŵ'), ('ū', 'ẇ'), ('\u033D', '°'), ('ĕ', 'ḝ')
     ]
 
     for x, y in replacements:
         Strng = Strng.replace(y, x)
 
-    import unicodedata
     Strng = unicodedata.normalize('NFD', Strng)
     Strng = Strng.replace('\u0307', '꞉')
     Strng = unicodedata.normalize('NFC', Strng)
 
     return Strng
 
 def UnSupThaana(Strng):
@@ -1136,17 +1477,24 @@
     nuktaDecom = ["\u0915\u093C","\u0916\u093C","\u0917\u093C","\u091C\u093C","\u0921\u093C","\u0922\u093C","\u092B\u093C","\u092F\u093C","\u0A32\u0A3C","\u0A38\u0A3C","\u0A16\u0A3C","\u0A17\u0A3C","\u0A1C\u0A3C","\u0A2B\u0A3C","\u09A1\u09BC","\u09A2\u09BC","\u09AF\u09BC","\u0B21\u0B3C","\u0B22\u0B3C"]
     nuktaPrecom = ["\u0958","\u0959","\u095A","\u095B","\u095C","\u095D","\u095E","\u095F","\u0A33","\u0A36","\u0A59","\u0A5A","\u0A5B","\u0A5E","\u09DC","\u09DD","\u09DF","\u0B5C","\u0B5D"]
 
     if Source not in ["Grantha","TamilGrantha"]:
         for x,y in zip(nuktaDecom,nuktaPrecom):
             Strng = Strng.replace(x,y)
 
-    if Source in ['IAST', 'ISO', 'ISOPali', 'Titus']:
+    if Source in ['IAST', 'ISO', 'ISOPali', 'Titus', 'IASTPali']:
         Strng = Strng.replace("ü", "uʼ").replace("ǖ", "ūʼ").replace( 'ö', 'aʼ',).replace('ȫ', 'āʼ')
 
+    if Source in ['IAST', 'ISO', 'ISOPali', 'IASTPali', 'Titus'] or 'RomanLoC' in Source:
+        Strng = unicodedata.normalize('NFC', Strng)
+        Strng = Strng.replace("ẗ", "ẗ").replace("ÿ", "ÿ").replace("ḧ", "ḧ")
+
+        if 'RomanLoC' in Source:
+            Strng = Strng.replace('\u02D9', '\u02DA')
+
     if Source == 'Arab-Ur' or Source == 'Arab-Pa':
         Strng = Strng.replace('ك', 'ک')
         Strng = Strng.replace('ي', 'ی')
 
     if Source == "Hebr":
         vowels = ['ְ','ֱ','ֲ','ֳ','ִ','ֵ','ֶ','ַ','ָ','ֹ','ֺ','ֻ','ׇ']
         vowelsR = '(' + '|'.join(vowels + ['וֹ', 'וּ']) + ')'
@@ -1208,19 +1556,14 @@
 
     oldVow = ["ྲྀ","ཷ","ླྀ","ཹ","ཱི","ཱུ","ཀྵ","ྐྵ"]
     newVow= ["ྲྀ","ྲཱྀ","ླྀ","ླཱྀ","ཱི","ཱུ","ཀྵ","ྐྵ"]
 
     for x,y in zip(oldVow,newVow):
         Strng = Strng.replace(x,y)
 
-    ## Tibetan ca, ja
-
-    Strng = Strng.replace('ཅ', 'ཙ')
-    Strng = Strng.replace('ཆ', 'ཚ')
-
     # Decomposed to Precomposed Roman Characters
 
     latinDecom= ["ā","ī","ū","ē","ō","ṃ","ṁ","ḥ","ś","ṣ","ṇ","ṛ","ṝ","ḷ","ḹ","ḻ","ṉ","ṟ"]
     latinPrecom = ["ā","ī","ū","ē","ō","ṃ","ṁ","ḥ","ś","ṣ","ṇ","ṛ","ṝ","ḷ","ḹ","ḻ","ṉ","ṟ"]
 
     for x,y in zip(latinDecom,latinPrecom):
         Strng = Strng.replace(x,y)
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/Balinese.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Balinese.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,20 +21,20 @@
 
 SouthVowelMap = [
                 '\u1B0F\u02BD',
                 '\u1B11\u02BD',
                 ]
 
 ModernVowelMap = [
-                 '\u1B33\u1B42\u02BD',
+                 '\u1B05\u1B42',
                  '\u1B06\u02BD',
                  ]
 
 SinhalaVowelMap = [
-                  '\u1B33\u1B43\u02BD'
+                  '\u1B05\u1B43'
                   ]
 
 VowelSignMap =  [
                 '\u1B35',
                 '\u1B36',
                 '\u1B37',
                 '\u1B38',
@@ -169,7 +169,13 @@
              '\u1B54',
              '\u1B55',
              '\u1B56',
              '\u1B57',
              '\u1B58',
              '\u1B59',
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/BatakKaro.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/BatakPakpak.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 VowelMap =  [
             '\u1BC0',
             '\u1BC0\u02BD',
             '\u1BE4',
             '\u1BE4\u02BD',
             '\u1BE5',
             '\u1BE5\u02BD',
-            '\u1BD2\u1BEC\u02BD',
-            '\u1BD2\u1BEC\u02BD',
-            'ᯞᯬ\u02BD',
-            'ᯞᯬ\u02BD',
+            'ᯒᯮ\u02BD',
+            'ᯒᯮ\u02BD',
+            'ᯞᯮ\u02BD',
+            'ᯞᯮ\u02BD',
             '\u1BE4\u02BD',
             '\u1BC0\u1BE4\u02BD',
             '\u1BE5\u02BD',
             '\u1BC0\u1BE5\u02BD',
             ]
 
 SouthVowelMap = [
@@ -30,62 +30,62 @@
                  ]
 
 SinhalaVowelMap = [
                   '\u1BE4\u02BD'
                   ]
 
 VowelSignMap =  [
-                '\u02BD',
-                '\u1BEB',
-                '\u1BEB\u02BD',
-                '\u1BEC',
-                '\u1BEC\u02BD',
-                '\u1BD2\u1BEC\u02BD',
-                '\u1BD2\u1BEC\u02BD',
-                'ᯞᯬ\u02BD',
-                'ᯞᯬ\u02BD',
-                '\u1BE9\u02BD',
+                '\u02BD\u02BD',
+                '\u1BEA',
+                '\u1BEA\u02BD',
+                '\u1BEE',
+                '\u1BEE\u02BD',
+                'ᯒᯮ\u02BD',
+                'ᯒᯮ\u02BD',
+                'ᯞᯮ\u02BD',
+                'ᯞᯮ\u02BD',
+                '\u1BE8\u02BD',
                 '\u1BE4\u02BD',
-                '\u1BED\u02BD',
+                '\u1BEC\u02BD',
                 '\u1BE5\u02BD',
                 ]
 
 SouthVowelSignMap = [
-                     '\u1BE9',
-                     '\u1BED',
+                     '\u1BE8',
+                     '\u1BEC',
                     ]
 
 ModernVowelSignMap =[
                      '\u1BE7',
-                     '\u02BD',
+                     '\u02BD\u02BD',
                     ]
 
 SinhalaVowelSignMap = [
                       '\u1BE9\u02BD'
                       ]
 
 AyogavahaMap = [
                '\u1BF0\u02BD',
                '\u1BF0',
                '\u1BF1'
                ]
 
 ViramaMap =  [
-             '\u1BF3'
+             '\u1BF2'
              ]
 
 ConsonantMap =  [
                 '\u1BC2',
                 '\u1BC2\u02BD',
                 '\u1BCE',
                 '\u1BCE\u02BD',
                 '\u1BDD',
 
-                '\u1BE1',
-                '\u1BE1\u02BD',
+                '\u1BD8\u02BD',
+                '\u1BD8\u02BD',
                 '\u1BD0',
                 '\u1BD0\u02BD',
                 '\u1BC9\u02BD',
 
                 '\u1BD7\u02BD',
                 '\u1BD7\u02BD',
                 '\u1BD1\u02BD',
@@ -96,22 +96,22 @@
                 '\u1BD7\u02BD',
                 '\u1BD1',
                 '\u1BD1\u02BD',
                 '\u1BC9',
 
                 '\u1BC7',
                 '\u1BC7\u02BD',
-                '\u1BC6',
-                '\u1BC6\u02BD',
+                '\u1BC5',
+                '\u1BC5\u02BD',
                 '\u1BD4',
 
                 '\u1BDB',
                 '\u1BD2',
                 '\u1BDE',
-                '\u1BCB',
+                '\u1BCD',
 
                 '\u1BD8\u02BD',
                 '\u1BD8\u02BD',
                 '\u1BD8',
                 '\u1BC0\u02BD'
                 ]
 
@@ -132,25 +132,25 @@
                      '\u1BC7\u02BD',
                      '\u1BDB\u02BD'
                      ]
 
 SinhalaConsonantMap =[
                      '\u1BF0\u1BCE\u02BD',
                      '\u1BF0\u1BD0\u02BD',
-                     '\u1BE2\u02BD',
-                     '\u1BE2',
-                     '\u1BE3',
+                     '\u1BF0\u1BD1\u02BD',
+                     '\u1BF0\u1BD1\u02BD',
+                     '\u1BF0\u1BC5\u02BD',
                       ]
 
 NuktaMap = [
            '\u02BD\u02BD\u02BD\u02BD'
            ]
 
 OmMap = [
-        'ᯥᯔ᯳\u02BD'
+        'ᯥᯔ᯲\u02BD'
         ]
 
 SignMap =[
          "'",
          '\u002E',
          '\u002E'
          ]
@@ -164,8 +164,14 @@
              '\u0033',
              '\u0034',
              '\u0035',
              '\u0036',
              '\u0037',
              '\u0038',
              '\u0039',
-             ]
+             ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/BatakManda.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/BatakToba.py`

 * *Files 14% similar despite different names*

```diff
@@ -62,73 +62,73 @@
 SinhalaVowelSignMap = [
                       '\u1BE9\u02BD'
                       ]
 
 AyogavahaMap = [
                '\u1BF0\u02BD',
                '\u1BF0',
-               '\u1BC4\u1BF2\u02BD'
+               '\u1BC2\u1BF2\u02BD'
                ]
 
 ViramaMap =  [
              '\u1BF2'
              ]
 
 ConsonantMap =  [
-                '\u1BC4\u1BE6',
-                '\u1BC4\u1BE6\u02BD',
+                '\u1BC2',
+                '\u1BC2\u02BD',
                 '\u1BCE',
                 '\u1BCE\u02BD',
                 '\u1BDD',
 
-                '\u1BDA\u1BE6',
-                '\u1BDA\u1BE6\u02BD',
+                '\u1BD8\u02BD',
+                '\u1BD8\u02BD',
                 '\u1BD0',
                 '\u1BD0\u02BD',
                 '\u1BE0',
 
-                '\u1BD6\u02BD',
-                '\u1BD6\u02BD',
+                '\u1BD7\u02BD',
+                '\u1BD7\u02BD',
                 '\u1BD1\u02BD',
                 '\u1BD1\u02BD',
-                '\u1BCA\u02BD',
+                '\u1BC9\u02BD',
 
-                '\u1BD6',
-                '\u1BD6\u02BD',
+                '\u1BD7',
+                '\u1BD7\u02BD',
                 '\u1BD1',
                 '\u1BD1\u02BD',
-                '\u1BCA',
+                '\u1BC9',
 
                 '\u1BC7',
                 '\u1BC7\u02BD',
                 '\u1BC5',
                 '\u1BC5\u02BD',
                 '\u1BD4',
 
                 '\u1BDB',
                 '\u1BD2',
                 '\u1BDE',
                 '\u1BCD',
 
-                '\u1BDA\u02BD',
-                '\u1BDA\u02BD',
-                '\u1BDA',
-                '\u1BC4'
+                '\u1BD8\u02BD',
+                '\u1BD8\u02BD',
+                '\u1BD8',
+                '\u1BC2\u02BD'
                 ]
 
 SouthConsonantMap = [
                     '\u1BDE\u02BD',
                     '\u1BDE\u02BD',
                     '\u1BD2\u02BD',
-                    '\u1BCA\u02BD'
+                    '\u1BC9\u02BD'
                     ]
 
 NuktaConsonantMap =  [
-                     '\u1BC4\u1BE6\u02BD',
-                     '\u1BC4\u1BE6\u02BD',
+                     '\u1BC2\u02BD',
+                     '\u1BC2\u02BD',
                      '\u1BCE\u02BD',
                      '\u1BD0\u02BD',
                      '\u1BD1\u02BD',
                      '\u1BD1\u02BD',
                      '\u1BC7\u02BD',
                      '\u1BDB\u02BD'
                      ]
@@ -164,8 +164,14 @@
              '\u0033',
              '\u0034',
              '\u0035',
              '\u0036',
              '\u0037',
              '\u0038',
              '\u0039',
-             ]
+             ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/BatakPakpak.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Buginese.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,162 +1,161 @@
 # -*- coding: utf-8 -*-
 
 # Script Mapping for Devanagari
 
 VowelMap =  [
-            '\u1BC0',
-            '\u1BC0\u02BD',
-            '\u1BE4',
-            '\u1BE4\u02BD',
-            '\u1BE5',
-            '\u1BE5\u02BD',
-            'ᯒᯮ\u02BD',
-            'ᯒᯮ\u02BD',
-            'ᯞᯮ\u02BD',
-            'ᯞᯮ\u02BD',
-            '\u1BE4\u02BD',
-            '\u1BC0\u1BE4\u02BD',
-            '\u1BE5\u02BD',
-            '\u1BC0\u1BE5\u02BD',
+            '\u1A15',
+            '\u1A15\u02BD',
+            '\u1A15\u1A17',
+            '\u1A15\u1A17\u02BD',
+            '\u1A15\u1A18',
+            '\u1A15\u1A18\u02BD',
+            '\u1A11\u1A18\u02BD',
+            '\u1A11\u1A18\u02BD',
+            '\u1A12\u1A18\u02BD',
+            '\u1A12\u1A18\u02BD',
+            '\u1A15\u1A19\u02BD',
+            '\u1A15\u1A15\u1A17\u02BD',
+            '\u1A15\u1A1A\u02BD',
+            '\u1A15\u1A15\u1A18\u02BD',
             ]
 
 SouthVowelMap = [
-                '\u1BE4\u02BD',
-                '\u1BE5\u02BD',
+                '\u1A15\u1A19',
+                '\u1A15\u1A1A',
                 ]
 
 ModernVowelMap = [
-                 '\u1BE4\u02BD',
-                 '\u1BC0\u02BD',
+                 '\u1A15\u1A1B',
+                 '\u1A15\u02BD',
                  ]
 
 SinhalaVowelMap = [
-                  '\u1BE4\u02BD'
+                  '\u1A15\u1A1B\u02BD'
                   ]
 
 VowelSignMap =  [
                 '\u02BD\u02BD',
-                '\u1BEA',
-                '\u1BEA\u02BD',
-                '\u1BEE',
-                '\u1BEE\u02BD',
-                'ᯒᯮ\u02BD',
-                'ᯒᯮ\u02BD',
-                'ᯞᯮ\u02BD',
-                'ᯞᯮ\u02BD',
-                '\u1BE8\u02BD',
-                '\u1BE4\u02BD',
-                '\u1BEC\u02BD',
-                '\u1BE5\u02BD',
+                '\u1A17',
+                '\u1A17\u02BD',
+                '\u1A18',
+                '\u1A18\u02BD',
+                '\u1A11\u1A18\u02BD',
+                '\u1A11\u1A18\u02BD',
+                '\u1A12\u1A18\u02BD',
+                '\u1A12\u1A18\u02BD',
+                '\u1A19\u02BD',
+                '\u1A15\u1A17\u02BD',
+                '\u1A1A\u02BD',
+                '\u1A15\u1A18\u02BD',
                 ]
 
 SouthVowelSignMap = [
-                     '\u1BE8',
-                     '\u1BEC',
+                     '\u1A19',
+                     '\u1A1A',
                     ]
 
 ModernVowelSignMap =[
-                     '\u1BE7',
-                     '\u02BD\u02BD',
+                     '\u1A1B',
+                     '\u02BD\u02BD\u02BD',
                     ]
 
 SinhalaVowelSignMap = [
-                      '\u1BE9\u02BD'
+                      '\u1A1B\u02BD'
                       ]
 
 AyogavahaMap = [
-               '\u1BF0\u02BD',
-               '\u1BF0',
-               '\u1BF1'
+               '\u1A06\u02BD',
+               '\u1A06\u02BD',
+               '\u1A16\u02BD'
                ]
 
 ViramaMap =  [
-             '\u1BF2'
+             '\u02BE'
              ]
 
 ConsonantMap =  [
-                '\u1BC2',
-                '\u1BC2\u02BD',
-                '\u1BCE',
-                '\u1BCE\u02BD',
-                '\u1BDD',
-
-                '\u1BD8\u02BD',
-                '\u1BD8\u02BD',
-                '\u1BD0',
-                '\u1BD0\u02BD',
-                '\u1BC9\u02BD',
-
-                '\u1BD7\u02BD',
-                '\u1BD7\u02BD',
-                '\u1BD1\u02BD',
-                '\u1BD1\u02BD',
-                '\u1BC9\u02BD',
-
-                '\u1BD7',
-                '\u1BD7\u02BD',
-                '\u1BD1',
-                '\u1BD1\u02BD',
-                '\u1BC9',
-
-                '\u1BC7',
-                '\u1BC7\u02BD',
-                '\u1BC5',
-                '\u1BC5\u02BD',
-                '\u1BD4',
-
-                '\u1BDB',
-                '\u1BD2',
-                '\u1BDE',
-                '\u1BCD',
-
-                '\u1BD8\u02BD',
-                '\u1BD8\u02BD',
-                '\u1BD8',
-                '\u1BC0\u02BD'
+                '\u1A00',
+                '\u1A00\u02BD',
+                '\u1A01',
+                '\u1A01\u02BD',
+                '\u1A02',
+
+                '\u1A0C',
+                '\u1A0C\u02BD',
+                '\u1A0D',
+                '\u1A0D\u02BD',
+                '\u1A0E',
+
+                '\u1A08\u02BD',
+                '\u1A08\u02BD',
+                '\u1A09\u02BD',
+                '\u1A09\u02BD',
+                '\u1A0A\u02BD',
+
+                '\u1A08',
+                '\u1A08\u02BD',
+                '\u1A09',
+                '\u1A09\u02BD',
+                '\u1A0A',
+
+                '\u1A04',
+                '\u1A04\u02BD',
+                '\u1A05',
+                '\u1A05\u02BD',
+                '\u1A06',
+
+                '\u1A10',
+                '\u1A11',
+                '\u1A12',
+                '\u1A13',
+
+                '\u1A14\u02BD',
+                '\u1A14\u02BD',
+                '\u1A14',
+                '\u1A16'
                 ]
 
 SouthConsonantMap = [
-                    '\u1BDE\u02BD',
-                    '\u1BDE\u02BD',
-                    '\u1BD2\u02BD',
-                    '\u1BC9\u02BD'
+                    '\u1A12\u02BD',
+                    '\u1A12\u02BD',
+                    '\u1A11\u02BD',
+                    '\u1A0A\u02BD'
                     ]
 
 NuktaConsonantMap =  [
-                     '\u1BC2\u02BD',
-                     '\u1BC2\u02BD',
-                     '\u1BCE\u02BD',
-                     '\u1BD0\u02BD',
-                     '\u1BD1\u02BD',
-                     '\u1BD1\u02BD',
-                     '\u1BC7\u02BD',
-                     '\u1BDB\u02BD'
+                     '\u1A00\u02BD',
+                     '\u1A00\u02BD',
+                     '\u1A01\u02BD',
+                     '\u1A0D\u02BD',
+                     '\u1A09\u02BD',
+                     '\u1A09\u02BD',
+                     '\u1A04\u02BD',
+                     '\u1A10\u02BD'
                      ]
-
 SinhalaConsonantMap =[
-                     '\u1BF0\u1BCE\u02BD',
-                     '\u1BF0\u1BD0\u02BD',
-                     '\u1BF0\u1BD1\u02BD',
-                     '\u1BF0\u1BD1\u02BD',
-                     '\u1BF0\u1BC5\u02BD',
+                     '\u1A02\u1A01\u02BD',
+                     '\u1A0E\u1A0D\u02BD',
+                     '\u1A0A\u1A09\u02BD',
+                     '\u1A0A\u1A09\u02BD',
+                     '\u1A06\u1A05\u02BD',
                       ]
 
 NuktaMap = [
            '\u02BD\u02BD\u02BD\u02BD'
            ]
 
 OmMap = [
-        'ᯥᯔ᯲\u02BD'
+        '\u1A15\u1A1A\u1A06\u02BD'
         ]
 
 SignMap =[
-         "'",
-         '\u002E',
-         '\u002E'
+         "\u02BD\u02BD",
+         '᨞',
+         '᨞᨞'
          ]
 
 Aytham =[AyogavahaMap[2]+'\u02BC']
 
 NumeralMap = [
              '\u0030',
              '\u0031',
@@ -164,8 +163,14 @@
              '\u0033',
              '\u0034',
              '\u0035',
              '\u0036',
              '\u0037',
              '\u0038',
              '\u0039',
-             ]
+             ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/BatakSima.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/BatakSima.py`

 * *Files 6% similar despite different names*

```diff
@@ -164,8 +164,14 @@
              '\u0033',
              '\u0034',
              '\u0035',
              '\u0036',
              '\u0037',
              '\u0038',
              '\u0039',
-             ]
+             ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/BatakToba.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/BatakKaro.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 VowelMap =  [
             '\u1BC0',
             '\u1BC0\u02BD',
             '\u1BE4',
             '\u1BE4\u02BD',
             '\u1BE5',
             '\u1BE5\u02BD',
-            'ᯒᯮ\u02BD',
-            'ᯒᯮ\u02BD',
-            'ᯞᯮ\u02BD',
-            'ᯞᯮ\u02BD',
+            '\u1BD2\u1BEC\u02BD',
+            '\u1BD2\u1BEC\u02BD',
+            'ᯞᯬ\u02BD',
+            'ᯞᯬ\u02BD',
             '\u1BE4\u02BD',
             '\u1BC0\u1BE4\u02BD',
             '\u1BE5\u02BD',
             '\u1BC0\u1BE5\u02BD',
             ]
 
 SouthVowelMap = [
@@ -30,65 +30,65 @@
                  ]
 
 SinhalaVowelMap = [
                   '\u1BE4\u02BD'
                   ]
 
 VowelSignMap =  [
-                '\u02BD\u02BD',
-                '\u1BEA',
-                '\u1BEA\u02BD',
-                '\u1BEE',
-                '\u1BEE\u02BD',
-                'ᯒᯮ\u02BD',
-                'ᯒᯮ\u02BD',
-                'ᯞᯮ\u02BD',
-                'ᯞᯮ\u02BD',
+                '\u02BD',
+                '\u1BEB',
+                '\u1BEB\u02BD',
+                '\u1BEC',
+                '\u1BEC\u02BD',
+                '\u1BD2\u1BEC\u02BD',
+                '\u1BD2\u1BEC\u02BD',
+                'ᯞᯬ\u02BD',
+                'ᯞᯬ\u02BD',
                 '\u1BE9\u02BD',
                 '\u1BE4\u02BD',
-                '\u1BEC\u02BD',
+                '\u1BED\u02BD',
                 '\u1BE5\u02BD',
                 ]
 
 SouthVowelSignMap = [
                      '\u1BE9',
-                     '\u1BEC',
+                     '\u1BED',
                     ]
 
 ModernVowelSignMap =[
-                     '\u1BE9\u02BD',
-                     '\u02BD\u02BD',
+                     '\u1BE7',
+                     '\u02BD',
                     ]
 
 SinhalaVowelSignMap = [
                       '\u1BE9\u02BD'
                       ]
 
 AyogavahaMap = [
                '\u1BF0\u02BD',
                '\u1BF0',
-               '\u1BC2\u1BF2\u02BD'
+               '\u1BF1'
                ]
 
 ViramaMap =  [
-             '\u1BF2'
+             '\u1BF3'
              ]
 
 ConsonantMap =  [
                 '\u1BC2',
                 '\u1BC2\u02BD',
                 '\u1BCE',
                 '\u1BCE\u02BD',
                 '\u1BDD',
 
-                '\u1BD8\u02BD',
-                '\u1BD8\u02BD',
+                '\u1BE1',
+                '\u1BE1\u02BD',
                 '\u1BD0',
                 '\u1BD0\u02BD',
-                '\u1BE0',
+                '\u1BC9\u02BD',
 
                 '\u1BD7\u02BD',
                 '\u1BD7\u02BD',
                 '\u1BD1\u02BD',
                 '\u1BD1\u02BD',
                 '\u1BC9\u02BD',
 
@@ -96,27 +96,27 @@
                 '\u1BD7\u02BD',
                 '\u1BD1',
                 '\u1BD1\u02BD',
                 '\u1BC9',
 
                 '\u1BC7',
                 '\u1BC7\u02BD',
-                '\u1BC5',
-                '\u1BC5\u02BD',
+                '\u1BC6',
+                '\u1BC6\u02BD',
                 '\u1BD4',
 
                 '\u1BDB',
                 '\u1BD2',
                 '\u1BDE',
-                '\u1BCD',
+                '\u1BCB',
 
                 '\u1BD8\u02BD',
                 '\u1BD8\u02BD',
                 '\u1BD8',
-                '\u1BC2\u02BD'
+                '\u1BC0\u02BD'
                 ]
 
 SouthConsonantMap = [
                     '\u1BDE\u02BD',
                     '\u1BDE\u02BD',
                     '\u1BD2\u02BD',
                     '\u1BC9\u02BD'
@@ -132,25 +132,25 @@
                      '\u1BC7\u02BD',
                      '\u1BDB\u02BD'
                      ]
 
 SinhalaConsonantMap =[
                      '\u1BF0\u1BCE\u02BD',
                      '\u1BF0\u1BD0\u02BD',
-                     '\u1BF0\u1BD1\u02BD',
-                     '\u1BF0\u1BD1\u02BD',
-                     '\u1BF0\u1BC5\u02BD',
+                     '\u1BE2\u02BD',
+                     '\u1BE2',
+                     '\u1BE3',
                       ]
 
 NuktaMap = [
            '\u02BD\u02BD\u02BD\u02BD'
            ]
 
 OmMap = [
-        'ᯥᯔ᯲\u02BD'
+        'ᯥᯔ᯳\u02BD'
         ]
 
 SignMap =[
          "'",
          '\u002E',
          '\u002E'
          ]
@@ -164,8 +164,14 @@
              '\u0033',
              '\u0034',
              '\u0035',
              '\u0036',
              '\u0037',
              '\u0038',
              '\u0039',
-             ]
+             ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/Buginese.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Shan.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,170 +1,178 @@
 # -*- coding: utf-8 -*-
 
 # Script Mapping for Devanagari
 
 VowelMap =  [
-            '\u1A15',
-            '\u1A15\u02BD',
-            '\u1A15\u1A17',
-            '\u1A15\u1A17\u02BD',
-            '\u1A15\u1A18',
-            '\u1A15\u1A18\u02BD',
-            '\u1A11\u1A18\u02BD',
-            '\u1A11\u1A18\u02BD',
-            '\u1A12\u1A18\u02BD',
-            '\u1A12\u1A18\u02BD',
-            '\u1A15\u1A19\u02BD',
-            '\u1A15\u1A15\u1A17\u02BD',
-            '\u1A15\u1A1A\u02BD',
-            '\u1A15\u1A15\u1A18\u02BD',
+            '\u1022',
+                '\u1022ႃ',
+                '\u1022\u102D',
+                '\u1022\u102E',
+                '\u1022\u102F',
+                '\u1022\u1030',
+                'ရိ\u02BD',
+                'ရီ\u02BD',
+                'လိ\u02BD',
+                'လီ\u02BD',
+                '\u1022\u1031',
+                '\u1022ႆ',
+                '\u1022\u1031ႃ',
+                '\u1022ဝ်\u02BD',
             ]
 
 SouthVowelMap = [
-                '\u1A15\u1A19',
-                '\u1A15\u1A1A',
+                '\u1022\u1031\u02BD',
+                'ွ',
                 ]
 
 ModernVowelMap = [
-                 '\u1A15\u1A1B',
-                 '\u1A15\u02BD',
+                 '\u1022ႄ',
+                 '\u1022ႃ\u02BD',
                  ]
 
 SinhalaVowelMap = [
-                  '\u1A15\u1A1B\u02BD'
+                  '\u1022ႄ\u02BD'
                   ]
 
 VowelSignMap =  [
-                '\u02BD\u02BD',
-                '\u1A17',
-                '\u1A17\u02BD',
-                '\u1A18',
-                '\u1A18\u02BD',
-                '\u1A11\u1A18\u02BD',
-                '\u1A11\u1A18\u02BD',
-                '\u1A12\u1A18\u02BD',
-                '\u1A12\u1A18\u02BD',
-                '\u1A19\u02BD',
-                '\u1A15\u1A17\u02BD',
-                '\u1A1A\u02BD',
-                '\u1A15\u1A18\u02BD',
+                'ႃ',
+                '\u102D',
+                '\u102E',
+                '\u102F',
+                '\u1030',
+                '\u103Aရိ\u02BD',
+                '\u103Aရီ\u02BD',
+                '\u103Aလိ\u02BD',
+                '\u103Aလီ\u02BD',
+                '\u1031',
+                'ႆ',
+                '\u1031ႃ',
+                'ဝ်\u02BD',
                 ]
 
 SouthVowelSignMap = [
-                     '\u1A19',
-                     '\u1A1A',
+                    '\u1031\u02BD',
+                    '\u1031ႃ\u02BD',
                     ]
 
 ModernVowelSignMap =[
-                     '\u1A1B',
-                     '\u02BD\u02BD\u02BD',
+                    'ႄ',
+                    'ႃ\u02BD'
                     ]
 
 SinhalaVowelSignMap = [
-                      '\u1A1B\u02BD'
+                    'ႄ\u02BD',
                       ]
 
 AyogavahaMap = [
-               '\u1A06\u02BD',
-               '\u1A06\u02BD',
-               '\u1A16\u02BD'
+               '\u1036\u02BD',
+               '\u1036',
+               '\u1038'
                ]
 
 ViramaMap =  [
-             '\u02BE'
+             '\u103A'
              ]
 
 ConsonantMap =  [
-                '\u1A00',
-                '\u1A00\u02BD',
-                '\u1A01',
-                '\u1A01\u02BD',
-                '\u1A02',
-
-                '\u1A0C',
-                '\u1A0C\u02BD',
-                '\u1A0D',
-                '\u1A0D\u02BD',
-                '\u1A0E',
-
-                '\u1A08\u02BD',
-                '\u1A08\u02BD',
-                '\u1A09\u02BD',
-                '\u1A09\u02BD',
-                '\u1A0A\u02BD',
-
-                '\u1A08',
-                '\u1A08\u02BD',
-                '\u1A09',
-                '\u1A09\u02BD',
-                '\u1A0A',
-
-                '\u1A04',
-                '\u1A04\u02BD',
-                '\u1A05',
-                '\u1A05\u02BD',
-                '\u1A06',
-
-                '\u1A10',
-                '\u1A11',
-                '\u1A12',
-                '\u1A13',
-
-                '\u1A14\u02BD',
-                '\u1A14\u02BD',
-                '\u1A14',
-                '\u1A16'
+                'ၵ',
+                'ၶ',
+                'ၷ',
+                'ꧠ',
+                '\u1004',
+
+                'ၸ',
+                'ꧡ',
+                'ꩡ',
+                'ꧢ',
+                'ၺ',
+
+                'ꩦ',
+                'ꩧ',
+                'ꩨ',
+                'ꩩ',
+                'ꧣ',
+
+                '\u1010',
+                '\u1011',
+                'ၻ',
+                'ꩪ',
+                'ၼ',
+
+                '\u1015',
+                'ၽ',
+                'ၿ',
+                'ꧤ',
+                '\u1019',
+
+                '\u101A',
+                '\u101B',
+                '\u101C',
+                '\u101D',
+
+                'သ\u103A\u101A',
+                'သျ\u02BD',
+                '\u101E',
+                'ႁ'
                 ]
 
 SouthConsonantMap = [
-                    '\u1A12\u02BD',
-                    '\u1A12\u02BD',
-                    '\u1A11\u02BD',
-                    '\u1A0A\u02BD'
+                    'ꩮ',
+                    'ꩮ\u02BD',
+                    '\u101B\u02BD',
+                    'ၼ\u02BD'
                     ]
 
 NuktaConsonantMap =  [
-                     '\u1A00\u02BD',
-                     '\u1A00\u02BD',
-                     '\u1A01\u02BD',
-                     '\u1A0D\u02BD',
-                     '\u1A09\u02BD',
-                     '\u1A09\u02BD',
-                     '\u1A04\u02BD',
-                     '\u1A10\u02BD'
+                'ၵ\u02BD',
+                'ၶ\u02BD',
+                'ၷ\u02BD',
+                     'ၹ',
+                'ꩨ\u02BD',
+                'ꩩ\u02BD',
+                     'ၾ',
+                     '\u101A\u02BD'
                      ]
+
 SinhalaConsonantMap =[
-                     '\u1A02\u1A01\u02BD',
-                     '\u1A0E\u1A0D\u02BD',
-                     '\u1A0A\u1A09\u02BD',
-                     '\u1A0A\u1A09\u02BD',
-                     '\u1A06\u1A05\u02BD',
+                     '\u1036ၷ\u02BD',
+                     '\u1036ꩡ\u02BD',
+                     '\u1036ꩨ\u02BD',
+                     '\u1036ၻ\u02BD',
+                     '\u1036ၿ\u02BD',
                       ]
 
 NuktaMap = [
-           '\u02BD\u02BD\u02BD\u02BD'
+           '\u02BD\u02BD'
            ]
 
 OmMap = [
-        '\u1A15\u1A1A\u1A06\u02BD'
+        '\u1022\u1031ႃ\u1036'
         ]
 
 SignMap =[
-         "\u02BD\u02BD",
-         '᨞',
-         '᨞᨞'
+         '\u0027',
+         '\u104A',
+         '\u104B'
          ]
 
-Aytham =[AyogavahaMap[2]+'\u02BC']
+Aytham =[AyogavahaMap[2]+'\u02BD']
+
 
 NumeralMap = [
-             '\u0030',
-             '\u0031',
-             '\u0032',
-             '\u0033',
-             '\u0034',
-             '\u0035',
-             '\u0036',
-             '\u0037',
-             '\u0038',
-             '\u0039',
+             '\u1090',
+             '\u1091',
+             '\u1092',
+             '\u1093',
+             '\u1094',
+             '\u1095',
+             '\u1096',
+             '\u1097',
+             '\u1098',
+             '\u1099',
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/Buhid.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Buhid.py`

 * *Files 14% similar despite different names*

```diff
@@ -165,7 +165,14 @@
              '\u0034',
              '\u0035',
              '\u0036',
              '\u0037',
              '\u0038',
              '\u0039',
              ]
+
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/Burmese.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/ThamLoC.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,171 +1,179 @@
 # -*- coding: utf-8 -*-
 
 # Script Mapping for Devanagari
 
+### AM - re-arrangement Tai Tham ??!!
+
 VowelMap =  [
-            '\u1021',
-            '\u1021\u102C',
-            '\u1023',
-            '\u1024',
-            '\u1025',
-            '\u1026',
-            '\u1052',
-            '\u1053',
-            '\u1054',
-            '\u1055',
-            '\u1027',
-            '\u1021\u1032',
-            '\u1029',
-            '\u102A',
+            '\u1A4B',
+            '\u1A4B\u1A63',
+            '\u1A4D',
+            '\u1A4E',
+            '\u1A4F',
+            '\u1A50',
+            '\u1A42',
+            '\u1A42\u1A63',
+            '\u1A44',
+            '\u1A44\u1A63',
+            '\u1A51',
+            '\u1A4B\u1A71',
+            '\u1A52',
+            '\u1A4B\u1A7F\u1A45\u1A6B', #http://reg.ksu.ac.th/bai_laan/THN.pdf ; Enquire about the arc above sign
             ]
 
 SouthVowelMap = [
-                '\u1027\u02BD',
-                '\u1029\u02BD',
+                '\u1A51\u02BD',
+                '\u1A52\u02BD',
                 ]
 
 ModernVowelMap = [
-                 '\u1027\u02BD',
-                 '\u1021\u102C\u02BD',
+                 '\u1A4Bᩯ',
+                 '\u1A4B\u1A63\u02BD',
                  ]
 
 SinhalaVowelMap = [
-                  '\u1027\u02BD'
+                  '\u1A51\u02BD'
                   ]
 
 VowelSignMap =  [
-                '\u102C',
-                '\u102D',
-                '\u102E',
-                '\u102F',
-                '\u1030',
-                '\u1056',
-                '\u1057',
-                '\u1058',
-                '\u1059',
-                '\u1031',
-                '\u1032',
-                '\u1031\u102C',
-                '\u1031\u102C\u103A',
+                '\u1A63',
+                '\u1A65',
+                '\u1A66',
+                '\u1A69',
+                '\u1A6A',
+                '\u1A7A\u1A42',
+                '\u1A7A\u1A42\u1A63',
+                '\u1A7A\u1A44',
+                '\u1A7A\u1A44\u1A63',
+                '\u1A6E',
+                '\u1A71',
+                'ᩰ',
+                '\u1A7F\u1A45\u1A6B',
                 ]
 
 SouthVowelSignMap = [
-                    '\u1031\u02BD',
-                    '\u1031\u102C\u02BD',
+                    '\u1A6E\u02BD',
+                    'ᩰ\u02BD',
                     ]
 
 ModernVowelSignMap =[
-                    '\u1031\u02BD',
-                    '\u102C\u02BD']
+                    'ᩯ',
+                    '\u1A63\u02BD']
 
 SinhalaVowelSignMap = [
-                      '\u1031\u02BD'
+                      '\u1A6E\u02BD'
                       ]
 
 AyogavahaMap = [
-               '\u1036\u02BD',
-               '\u1036',
-               '\u1038'
+               '\u1A74\u02BD',
+               '\u1A74',
+               '\u1A61'
                ]
 
 ViramaMap =  [
-             '\u103A'
+             '\u1A7A'
              ]
 
 ConsonantMap =  [
-                '\u1000',
-                '\u1001',
-                '\u1002',
-                '\u1003',
-                '\u1004',
-
-                '\u1005',
-                '\u1006',
-                '\u1007',
-                '\u1008',
-                '\u1009',
-
-                '\u100B',
-                '\u100C',
-                '\u100D',
-                '\u100E',
-                '\u100F',
-
-                '\u1010',
-                '\u1011',
-                '\u1012',
-                '\u1013',
-                '\u1014',
-
-                '\u1015',
-                '\u1016',
-                '\u1017',
-                '\u1018',
-                '\u1019',
-
-                '\u101A',
-                '\u101B',
-                '\u101C',
-                '\u101D',
-
-                '\u1050',
-                '\u1051',
-                '\u101E',
-                '\u101F'
+                '\u1A20',
+                '\u1A21',
+                '\u1A23',
+                '\u1A25',
+                '\u1A26',
+
+                '\u1A27',
+                '\u1A28',
+                '\u1A29',
+                '\u1A2B',
+                '\u1A2C',
+
+                '\u1A2D',
+                '\u1A2E',
+                '\u1A2F',
+                '\u1A30',
+                '\u1A31',
+
+                '\u1A32',
+                '\u1A33',
+                '\u1A34',
+                '\u1A35',
+                '\u1A36',
+
+                '\u1A38',
+                '\u1A39',
+                '\u1A3B',
+                '\u1A3D',
+                '\u1A3E',
+
+                '\u1A3F',
+                '\u1A41',
+                '\u1A43',
+                '\u1A45',
+
+                '\u1A46',
+                '\u1A47',
+                '\u1A48',
+                '\u1A49'
                 ]
 
 SouthConsonantMap = [
-                    '\u1020',
-                    '\u1020\u02BD',
-                    '\u101B\u02BD',
-                    '\u1014\u02BD'
+                    '\u1A4A',
+                    '\u1A4A\u02BD',
+                    '\u1A41\u02BD',
+                    '\u1A36\u02BD'
                     ]
 
 NuktaConsonantMap =  [
-                     '\u1000\u02BD',
-                     '\u1001\u02BD',
-                     '\u1002\u02BD',
-                     '\u1007\u02BD',
-                     '\u100D\u02BD',
-                     '\u100E\u02BD',
-                     '\u1016\u02BD',
-                     '\u101A\u02BD'
+                     '\u1A20\u02BD',
+                     '\u1A21\u02BD',
+                     '\u1A23\u02BD',
+                     '\u1A29\u02BD',
+                     '\u1A2F\u02BD',
+                     '\u1A30\u02BD',
+                     '\u1A39\u02BD',
+                     '\u1A3F\u02BD'
                      ]
 
 SinhalaConsonantMap =[
-                     '\u1036\u1002\u02BD',
-                     '\u1036\u1007\u02BD',
-                     '\u1036\u100D\u02BD',
-                     '\u1036\u1012\u02BD',
-                     '\u1036\u1017\u02BD',
+                     '\u1A74\u1A23\u02BD',
+                     '\u1A74\u1A29\u02BD',
+                     '\u1A74\u1A2F\u02BD',
+                     '\u1A74\u1A34\u02BD',
+                     '\u1A74\u1A3D\u02BD',
                       ]
 
 NuktaMap = [
            '\u02BD\u02BD\u02BD\u02BD'
            ]
 
 OmMap = [
-        'ဥုံ'
+        '\u1A52\u1A74'
         ]
 
 SignMap =[
-         '\u0027',
-         '\u104A',
-         '\u104B'
+         "'",
+         '\u1AA8',
+         '\u1AA9'
          ]
 
 Aytham =[AyogavahaMap[2]+'\u02BD']
 
 
 NumeralMap = [
-             '\u1040',
-             '\u1041',
-             '\u1042',
-             '\u1043',
-             '\u1044',
-             '\u1045',
-             '\u1046',
-             '\u1047',
-             '\u1048',
-             '\u1049',
+             '\u1A90',
+             '\u1A91',
+             '\u1A92',
+             '\u1A93',
+             '\u1A94',
+             '\u1A95',
+             '\u1A96',
+             '\u1A97',
+             '\u1A98',
+             '\u1A99',
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/Cham.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Cham.py`

 * *Files 18% similar despite different names*

```diff
@@ -167,7 +167,13 @@
              '\uAA54',
              '\uAA55',
              '\uAA56',
              '\uAA57',
              '\uAA58',
              '\uAA59',
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/Hanunoo.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Hanunoo.py`

 * *Files 20% similar despite different names*

```diff
@@ -165,7 +165,13 @@
              '\u0034',
              '\u0035',
              '\u0036',
              '\u0037',
              '\u0038',
              '\u0039',
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/Javanese.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Javanese.py`

 * *Files 6% similar despite different names*

```diff
@@ -124,15 +124,15 @@
 NuktaConsonantMap =  [
                      '\uA98F\uA9B3',
                      '\uA991\uA9B3',
                      '\uA992\uA9B3',
                      '\uA997\uA9B3',
                      '\uA99D\uA9B3',
                      '\uA99E\uA9B3',
-                     '\uA9A6\uA9B3',
+                     '\uA9A5\uA9B3',
                      '\uA9AA\uA9B3'
                      ]
 
 SinhalaConsonantMap =[
                      '\uA980\uA992\u02BD',
                      '\uA980\uA997\u02BD',
                      '\uA980\uA99D\u02BD',
@@ -165,7 +165,13 @@
              '\uA9D4',
              '\uA9D5',
              '\uA9D6',
              '\uA9D7',
              '\uA9D8',
              '\uA9D9',
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/Kawi.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Pallava.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,69 +5,69 @@
 VowelMap =  [
             '\uA984',
             '\uA984\uA9B4',
             '\uA986',
             '\uA987',
             '\uA988',
             '\uA988\uA9B4',
-            '\uA989',
-            '\uA989\uA9B4',
-            '\uA98A',
-            '\uA98B',
+            'ꦫꦶ\u02BD',
+            'ꦫꦷ\u02BD',
+            'ꦭꦶ\u02BD',
+            'ꦭꦷ\u02BD',
             '\uA98C',
             '\uA98D',
             '\uA98E',
             '\uA98E\uA9B4',
             ]
 
 SouthVowelMap = [
                 '\uA98C\u02BD',
                 '\uA98E\u02BD',
                 ]
 
 ModernVowelMap = [
-                 '\uA984\uA9BC',
+                '\uA98C\u02BD',
                  '\uA984\uA9B4\u02BD',
                  ]
 
 SinhalaVowelMap = [
-                  '\uA984\uA9BC\u02BD'
+                '\uA98C\u02BD',
                   ]
 
 VowelSignMap =  [
                 '\uA9B4',
                 '\uA9B6',
                 '\uA9B7',
                 '\uA9B8',
                 '\uA9B9',
-                '\uA9BD',
-                '\uA9C0\uA989\uA9B4',
-                '\uA9C0\uA98A',
-                '\uA9C0\uA98B',
+            '\uA9C0ꦫꦶ\u02BD',
+            '\uA9C0ꦫꦷ\u02BD',
+            '\uA9C0ꦭꦶ\u02BD',
+            '\uA9C0ꦭꦷ\u02BD',
                 '\uA9BA',
                 '\uA9BB',
                 '\uA9BA\uA9B4',
                 '\uA9BB\uA9B4',
                 ]
 
 SouthVowelSignMap = [
                     '\uA9BA\u02BD',
                     '\uA9BA\uA9B4\u02BD',
                     ]
 
 ModernVowelSignMap =[
-                    '\uA9BC',
+                    '\uA9BA\u02BD',
                     '\uA9B4\u02BD']
 
 SinhalaVowelSignMap = [
-                      '\uA9BC\u02BD'
+                    '\uA9BA\u02BD',
                       ]
 
 AyogavahaMap = [
-               '\uA980',
+               '\uA981\u02BD',
                '\uA981',
                '\uA983'
                ]
 
 ViramaMap =  [
              '\uA9C0'
              ]
@@ -111,61 +111,67 @@
                 '\uA9AF',
                 '\uA9B0',
                 '\uA9B1',
                 '\uA9B2'
                 ]
 
 SouthConsonantMap = [
-                    '\uA9AD\uA9B3',
-                    '\uA9B0\uA9B3',
-                    '\uA9AB\uA9B3',
-                    '\uA9A4\uA9B3'
+                    '\uA9AD\u02BD',
+                    '\uA9B0\u02BD',
+                    '\uA9AB\u02BD',
+                    '\uA9A4\u02BD'
                     ]
 
 NuktaConsonantMap =  [
-                     '\uA98F\uA9B3',
-                     '\uA991\uA9B3',
-                     '\uA992\uA9B3',
-                     '\uA997\uA9B3',
-                     '\uA99D\uA9B3',
-                     '\uA99E\uA9B3',
-                     '\uA9A6\uA9B3',
-                     '\uA9AA\uA9B3'
+                     '\uA98F\u02BD',
+                     '\uA991\u02BD',
+                     '\uA992\u02BD',
+                     '\uA997\u02BD',
+                     '\uA99D\u02BD',
+                     '\uA99E\u02BD',
+                     '\uA9A6\u02BD',
+                     '\uA9AA\u02BD'
                      ]
 
 SinhalaConsonantMap =[
-                     '\uA980\uA992\u02BD',
-                     '\uA980\uA997\u02BD',
-                     '\uA980\uA99D\u02BD',
-                     '\uA980\uA9A2\u02BD',
-                     '\uA980\uA9A7\u02BD',
+                     '\uA981\uA992\u02BD',
+                     '\uA981\uA997\u02BD',
+                     '\uA981\uA99D\u02BD',
+                     '\uA981\uA9A2\u02BD',
+                     '\uA981\uA9A7\u02BD',
                       ]
 
 NuktaMap = [
-           '\uA9B3'
+           '\u02BD\u02BD'
            ]
 
 OmMap = [
-        '\uA98E\uA980'
+        '\uA98E\uA981'
         ]
 
 SignMap =[
          '\u0027',
-         '\uA9C8',
-         '\uA9C9'
+         '|',
+         '||'
          ]
 
 Aytham =[AyogavahaMap[2]+'\u02BD']
 
 
 NumeralMap = [
-             '\uA9D0',
-             '\uA9D1',
-             '\uA9D2',
-             '\uA9D3',
-             '\uA9D4',
-             '\uA9D5',
-             '\uA9D6',
-             '\uA9D7',
-             '\uA9D8',
-             '\uA9D9',
+             '\u0030',
+             '\u0031',
+             '\u0032',
+             '\u0033',
+             '\u0034',
+             '\u0035',
+             '\u0036',
+             '\u0037',
+             '\u0038',
+             '\u0039',
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/KhamtiShan.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/TaiLaing.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,61 +1,61 @@
 # -*- coding: utf-8 -*-
 
 # Script Mapping for Devanagari
 
 VowelMap =  [
-            '\u1022',
-                '\u1022ႃ',
-                '\u1022\u102D',
-                '\u1022\u102E',
-                '\u1022\u102F',
-                '\u1022\u1030',
-                'ရိ\u02BD',
-                'ရီ\u02BD',
+            '\u1021',
+                '\u1021ႃ',
+                '\u1021\u102D',
+                '\u1021\u102E',
+                '\u1021\u102F',
+                '\u1021\u1030',
+                'ꩺိ\u02BD',
+                'ꩺီ\u02BD',
                 'လိ\u02BD',
                 'လီ\u02BD',
-                '\u1022\u1031',
-                '\u1022ႆ',
-                '\u1022\u1031ႃ',
-                '\u1022ဝ်\u02BD',
+                '\u1021\u1031',
+                '\u1021ႆ',
+                '\u1021\u1031ႃ',
+                '\u1021ဝ်\u02BD',
             ]
 
 SouthVowelMap = [
-                '\u1022\u1031\u02BD',
-                '\u1022\u1030ဝ်\u02BD',
+                '\u1021\u1031\u02BD',
+                '\u1021\u1031ႃ\u02BD',
                 ]
 
 ModernVowelMap = [
-                 '\u1022ႄ',
-                 '\u1022ႃ\u02BD',
+                  '\u1021\u1031\u02BD',
+                 '\u1021ႃ\u02BD',
                  ]
 
 SinhalaVowelMap = [
-                  '\u1022ႄ\u02BD'
+                  '\u1021\u1031\u02BD'
                   ]
 
 VowelSignMap =  [
                 'ႃ',
                 '\u102D',
                 '\u102E',
                 '\u102F',
                 '\u1030',
-                '်ရိ\u02BD',
-                '်ရီ\u02BD',
+                '်ꩺိ\u02BD',
+                '်ꩺီ\u02BD',
                 '်လိ\u02BD',
                 '်လီ\u02BD',
                 '\u1031',
                 'ႆ',
                 '\u1031ႃ',
                 'ဝ်\u02BD',
                 ]
 
 SouthVowelSignMap = [
                     '\u1031\u02BD',
-                    '\u1030ဝ်\u02BD',
+                    '\u1031ႃ\u02BD',
                     ]
 
 ModernVowelSignMap =[
                     'ႄ',
                     'ႃ\u02BD'
                     ]
 
@@ -72,101 +72,107 @@
 ViramaMap =  [
              '\u103A'
              ]
 
 ConsonantMap =  [
                 'က',
                 'ၵ',
-                'ꩠ',
-                'ၷ',
+                'ꧩ',
+                'ꧪ',
                 '\u1004',
 
-                'ꩡ',
-                'ꩢ',
-                'ꩣ',
-                'ꩤ',
-                'ꩥ',
+                'ၸ',
+                'ꩬ',
+                'ꧫ',
+                'ꧬ',
+                'ꧧ',
 
                 'ꩦ',
                 'ꩧ',
-                'ꩨ',
-                'ꩩ',
-                'ꧣ',
+                'ꧭ',
+                'ꧮ',
+                'ꧯ',
 
                 '\u1010',
                 '\u1011',
-                'ၻ',
-                'ꩪ',
+                'ꧻ',
+                'ꧼ',
                 'ꩫ',
 
-                '\u1015',
-                'ၸ',
-                'ၿ',
-                'ၹ',
+                'ပ',
+                'ꧤ',
+                'ꧽ',
+                'ꧾ',
                 '\u1019',
 
                 '\u101A',
-                'ရ',
+                'ꩺ',
                 '\u101C',
                 '\u101D',
 
-                'ꩬ\u02BD',
-                'ꩬ\u02BD',
-                'ꩬ',
-                'ꩭ'
+                'ꧬ\u02BD',
+                'ꧬ\u02BD',
+                'ꧬ',
+                'ၯ'
                 ]
 
 SouthConsonantMap = [
-                    'ꩮ',
-                    'ꩮ\u02BD',
-                    '\u101B\u02BD',
-                    'ၼ\u02BD'
+                    'ꧺ',
+                    'ꧺ\u02BD',
+                    'ꩺ\u02BD',
+                    'ꩫ\u02BD'
                     ]
 
 NuktaConsonantMap =  [
                 'က\u02BD',
-                'ꩱ',
-                'ꩠ\u02BD',
-                     'ꩲ',
-                'ꩨ\u02BD',
-                'ꩩ\u02BD',
-                     'ꩯ',
+                'ၵ\u02BD',
+                'ꧩ\u02BD',
+                     'ꧫ\u02BD',
+                'ꧭ\u02BD',
+                'ꧮ\u02BD',
+                     'ꧨ',
                      '\u101A\u02BD'
                      ]
 
 SinhalaConsonantMap =[
-                     '\u1036ၷ\u02BD',
-                     '\u1036ꩡ\u02BD',
-                     '\u1036ꩨ\u02BD',
-                     '\u1036ၻ\u02BD',
-                     '\u1036ၿ\u02BD',
+                     '\u1036ၵ\u02BD',
+                     '\u1036ꧫ\u02BD',
+                     '\u1036ꧭ\u02BD',
+                     '\u1036ꧻ\u02BD',
+                     '\u1036ꧽ\u02BD',
                       ]
 
 NuktaMap = [
-           '\u02BD\u02BD'
+           '\u02BD\u02BD\u02BD'
            ]
 
 OmMap = [
-        '\u1022\u1031ႃ\u1036'
+        '\u1021\u1031ႃ\u1036'
         ]
 
 SignMap =[
          '\u0027',
          '\u104A',
          '\u104B'
          ]
 
 Aytham =[AyogavahaMap[2]+'\u02BD']
 
 
 NumeralMap = [
-             '\u1090',
-             '\u1091',
-             '\u1092',
-             '\u1093',
-             '\u1094',
-             '\u1095',
-             '\u1096',
-             '\u1097',
-             '\u1098',
-             '\u1099',
+             '\uA9F0',
+             '\uA9F1',
+             '\uA9F2',
+             '\uA9F3',
+             '\uA9F4',
+             '\uA9F5',
+             '\uA9F6',
+             '\uA9F7',
+             '\uA9F8',
+             '\uA9F9',
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/Khmer.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/KhmerLoC.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 # -*- coding: utf-8 -*-
 
 # Script Mapping for Devanagari
 
 VowelMap =  [
-            '\u17A2',
-            '\u17A2\u17B6',
+            '\u17A2\u02BD',
+            '\u17A2\u17B6\u02BD',
             '\u17A5',
             '\u17A6',
             '\u17A7',
             '\u17A9',
             '\u17AB',
             '\u17AC',
             '\u17AD',
             '\u17AE',
-            '\u17AF',
+            'អេ\u02BD',
             '\u17B0',
             '\u17B1',
             '\u17B3',
             ]
 
 SouthVowelMap = [
                 '\u17AF\u02BD',
                 '\u17B1\u02BD',
                 ]
 
 ModernVowelMap = [
-                 '\u17AF\u02BD',
+                 'ឯ',
                  '\u17A2\u17B6\u02BD',
                  ]
 
 SinhalaVowelMap = [
                   '\u17AF\u02BD'
                   ]
 
@@ -51,15 +51,15 @@
 
 SouthVowelSignMap = [
                     '\u17C1\u02BD',
                     '\u17C4\u02BD',
                     ]
 
 ModernVowelSignMap =[
-                    '\u17C1\u02BD',
+                    'ែ',
                     '\u17B6\u02BD']
 
 SinhalaVowelSignMap = [
                       '\u17C1\u02BD'
                       ]
 
 AyogavahaMap = [
@@ -165,7 +165,13 @@
              '\u17E4',
              '\u17E5',
              '\u17E6',
              '\u17E7',
              '\u17E8',
              '\u17E9',
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/KhomThai.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/KhomThai.py`

 * *Files 19% similar despite different names*

```diff
@@ -168,7 +168,13 @@
              '\u0E54',
              '\u0E55',
              '\u0E56',
              '\u0E57',
              '\u0E58',
              '\u0E59',
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/KhuenTham.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Khmer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,173 +1,177 @@
 # -*- coding: utf-8 -*-
 
 # Script Mapping for Devanagari
 
-### AM - re-arrangement Tai Tham ??!!
-
 VowelMap =  [
-            '\u1A4B',
-            '\u1A4B\u1A63',
-            '\u1A4D',
-            '\u1A4E',
-            '\u1A4F',
-            '\u1A50',
-            '\u1A42',
-            '\u1A42\u1A63',
-            '\u1A44',
-            '\u1A44\u1A63',
-            '\u1A51',
-            '\u1A4B\u1A71',
-            '\u1A52',
-            '\u1A4F\u1A6B\u1A63', #http://reg.ksu.ac.th/bai_laan/THN.pdf ; Enquire about the arc above sign
+            '\u17A2',
+            '\u17A2\u17B6',
+            '\u17A5',
+            '\u17A6',
+            '\u17A7',
+            '\u17A9',
+            '\u17AB',
+            '\u17AC',
+            '\u17AD',
+            '\u17AE',
+            '\u17AF',
+            '\u17B0',
+            '\u17B1',
+            '\u17B3',
             ]
 
 SouthVowelMap = [
-                '\u1A51\u02BD',
-                '\u1A52\u02BD',
+                '\u17AF\u02BD',
+                '\u17B1\u02BD',
                 ]
 
 ModernVowelMap = [
-                 '\u1A51\u02BD',
-                 '\u1A4B\u1A63\u02BD',
+                 '\u17AF\u02BD',
+                 '\u17A2\u17B6\u02BD',
                  ]
 
 SinhalaVowelMap = [
-                  '\u1A51\u02BD'
+                  '\u17AF\u02BD'
                   ]
 
 VowelSignMap =  [
-                '\u1A63',
-                '\u1A65',
-                '\u1A66',
-                '\u1A69',
-                '\u1A6A',
-                '\u1A7A\u1A42',
-                '\u1A7A\u1A42\u1A63',
-                '\u1A7A\u1A44',
-                '\u1A7A\u1A44\u1A63',
-                '\u1A6E',
-                '\u1A71',
-                '\u1A6E\u1A63',
-                '\u1A6E\u1A6B\u1A63',
+                '\u17B6',
+                '\u17B7',
+                '\u17B8',
+                '\u17BB',
+                '\u17BC',
+                '\u17D2\u17AB',
+                '\u17D2\u17AC',
+                '\u17D2\u17AD',
+                '\u17D2\u17AE',
+                '\u17C1',
+                '\u17C3',
+                '\u17C4',
+                '\u17C5',
                 ]
 
 SouthVowelSignMap = [
-                    '\u1A6E\u02BD',
-                    '\u1A6E\u1A63\u02BD',
+                    '\u17C1\u02BD',
+                    '\u17C4\u02BD',
                     ]
 
 ModernVowelSignMap =[
-                    '\u1A6E\u02BD',
-                    '\u1A63\u02BD']
+                    '\u17C1\u02BD',
+                    '\u17B6\u02BD']
 
 SinhalaVowelSignMap = [
-                      '\u1A6E\u02BD'
+                      '\u17C1\u02BD'
                       ]
 
 AyogavahaMap = [
-               '\u1A74\u02BD',
-               '\u1A74',
-               '\u1A61'
+               '\u17C6\u02BD',
+               '\u17C6',
+               '\u17C7'
                ]
 
 ViramaMap =  [
-             '\u1A7A'
+             '\u17D1'
              ]
 
 ConsonantMap =  [
-                '\u1A20',
-                '\u1A21',
-                '\u1A23',
-                '\u1A25',
-                '\u1A26',
-
-                '\u1A27',
-                '\u1A28',
-                '\u1A29',
-                '\u1A2B',
-                '\u1A2C',
-
-                '\u1A2D',
-                '\u1A2E',
-                '\u1A2F',
-                '\u1A30',
-                '\u1A31',
-
-                '\u1A32',
-                '\u1A33',
-                '\u1A34',
-                '\u1A35',
-                '\u1A36',
-
-                '\u1A38',
-                '\u1A39',
-                '\u1A3B',
-                '\u1A3D',
-                '\u1A3E',
-
-                '\u1A3F',
-                '\u1A41',
-                '\u1A43',
-                '\u1A45',
-
-                '\u1A46',
-                '\u1A47',
-                '\u1A48',
-                '\u1A49'
+                '\u1780',
+                '\u1781',
+                '\u1782',
+                '\u1783',
+                '\u1784',
+
+                '\u1785',
+                '\u1786',
+                '\u1787',
+                '\u1788',
+                '\u1789',
+
+                '\u178A',
+                '\u178B',
+                '\u178C',
+                '\u178D',
+                '\u178E',
+
+                '\u178F',
+                '\u1790',
+                '\u1791',
+                '\u1792',
+                '\u1793',
+
+                '\u1794',
+                '\u1795',
+                '\u1796',
+                '\u1797',
+                '\u1798',
+
+                '\u1799',
+                '\u179A',
+                '\u179B',
+                '\u179C',
+
+                '\u179D',
+                '\u179E',
+                '\u179F',
+                '\u17A0'
                 ]
 
 SouthConsonantMap = [
-                    '\u1A4A',
-                    '\u1A4A\u02BD',
-                    '\u1A41\u02BD',
-                    '\u1A36\u02BD'
+                    '\u17A1',
+                    '\u17A1\u02BD',
+                    '\u179A\u02BD',
+                    '\u1793\u02BD'
                     ]
 
 NuktaConsonantMap =  [
-                     '\u1A20\u02BD',
-                     '\u1A21\u02BD',
-                     '\u1A23\u02BD',
-                     '\u1A29\u02BD',
-                     '\u1A2F\u02BD',
-                     '\u1A30\u02BD',
-                     '\u1A39\u02BD',
-                     '\u1A3F\u02BD'
+                     '\u1780\u02BD',
+                     '\u1781\u02BD',
+                     '\u1782\u02BD',
+                     '\u1787\u02BD',
+                     '\u178C\u02BD',
+                     '\u178D\u02BD',
+                     '\u1795\u02BD',
+                     '\u1799\u02BD'
                      ]
 
 SinhalaConsonantMap =[
-                     '\u1A74\u1A23\u02BD',
-                     '\u1A74\u1A29\u02BD',
-                     '\u1A74\u1A2F\u02BD',
-                     '\u1A74\u1A34\u02BD',
-                     '\u1A74\u1A3D\u02BD',
+                     '\u17C6\u1782\u02BD',
+                     '\u17C6\u1787\u02BD',
+                     '\u17C6\u178C\u02BD',
+                     '\u17C6\u1791\u02BD',
+                     '\u17C6\u1796\u02BD',
                       ]
 
 NuktaMap = [
            '\u02BD\u02BD\u02BD\u02BD'
            ]
 
 OmMap = [
-        '\u1A52\u1A74'
+        '\u17B1\u17C6'
         ]
 
 SignMap =[
-         "'",
-         '\u1AA8',
-         '\u1AA9'
+         '\u17DC',
+         '\u17D4',
+         '\u17D5'
          ]
 
 Aytham =[AyogavahaMap[2]+'\u02BD']
 
 
 NumeralMap = [
-             '\u1A90',
-             '\u1A91',
-             '\u1A92',
-             '\u1A93',
-             '\u1A94',
-             '\u1A95',
-             '\u1A96',
-             '\u1A97',
-             '\u1A98',
-             '\u1A99',
+             '\u17E0',
+             '\u17E1',
+             '\u17E2',
+             '\u17E3',
+             '\u17E4',
+             '\u17E5',
+             '\u17E6',
+             '\u17E7',
+             '\u17E8',
+             '\u17E9',
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/Lao.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Lao.py`

 * *Files 12% similar despite different names*

```diff
@@ -169,7 +169,13 @@
              '\u0ED4',
              '\u0ED5',
              '\u0ED6',
              '\u0ED7',
              '\u0ED8',
              '\u0ED9'
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/Lao2.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/LaoPali.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,44 +1,40 @@
 # -*- coding: utf-8 -*-
 
 # Script Mapping for Devanagari
 
-#http://www.laomanuscripts.net/downloads/DLLM_pali_laoromanisation.pdf
-
-#Lao aG to aM, check for buddhaM vs buddhaG...
-
 VowelMap =  [
             '\u0EAD',
             '\u0EAD\u0EB2',
             '\u0EAD\u0EB4',
             '\u0EAD\u0EB5',
             '\u0EAD\u0EB8',
             '\u0EAD\u0EB9',
             '\u0EA3\u0EB8\u02BD',
             '\u0EA3\u0EB9\u02BD',
             '\u0EA5\u0EB8\u02BD',
             '\u0EA5\u0EB9\u02BD',
-            '\u0EC0\u0EAD',
-            '\u0EC4\u0EAD',
-            '\u0EC2\u0EAD',
-            '\u0EC0\u0EAD\u0EBB\u0EB2',
+            '\u0EAD\u0EC0',
+            '\u0EAD\u0EC4',
+            '\u0EAD\u0EC2',
+            '\u0EAD\u0EC0\u0EBB\u0EB2',
             ]
 
 SouthVowelMap = [
-                '\u0EC0\u0EAD\u0EB0',
-                '\u0EC2\u0EAD\u0EB0',
+                '\u0EAD\u0EC0\u0EB0',
+                '\u0EAD\u0EC2\u0EB0',
                 ]
 
 ModernVowelMap = [
-                 '\u0EC1\u0EAD\u0EB0',
-                 '\u0EC0\u0EAD\u0EB2\u0EB0',
+                 '\u0EAD\u0EC1\u0EB0',
+                 '\u0EAD\u0EC0\u0EB2\u0EB0',
                  ]
 
 SinhalaVowelMap = [
-                  '\u0EC1\u0EAD'
+                  '\u0EAD\u0EC1'
                   ]
 
 VowelSignMap =  [
                  '\u0EB2',
                  '\u0EB4',
                  '\u0EB5',
                  '\u0EB8',
@@ -66,95 +62,95 @@
 SinhalaVowelSignMap = [
                        '\u0EC1'
                       ]
 
 AyogavahaMap = [
                '\u0ECD\u02BD',
                '\u0ECD',
-               '\u0EAB\u0EBA\u02BD'
+               '\u0EAB\u0ECC'
                ]
 
 ViramaMap =  [
              '\u0EBA'
              ]
 
 ConsonantMap =  [
                 '\u0E81',
                 '\u0E82',
                 '\u0E84',
-                '\u0E84\u02BD',
+                '\u0E86',
                 '\u0E87',
 
                 '\u0E88',
-                '\u0EAA',
+                '\u0E89',
                 '\u0E8A',
-                '\u0E8A\u02BD',
-                '\u0E8D',
+                '\u0E8C',
+                '\u0E8E',
 
-                '\u0E95\u02BD',
-                '\u0E96\u02BD',
-                '\u0E97\u02BD',
-                '\u0E97\u02BD',
-                '\u0E99\u02BD',
+                '\u0E8F',
+                '\u0E90',
+                '\u0E91',
+                '\u0E92',
+                '\u0E93',
 
                 '\u0E95',
                 '\u0E96',
                 '\u0E97',
-                '\u0E97\u02BD',
+                '\u0E98',
                 '\u0E99',
 
                 '\u0E9B',
                 '\u0E9C',
                 '\u0E9E',
-                '\u0E9E\u02BD',
+                '\u0EA0',
                 '\u0EA1',
 
                 '\u0E8D',
                 '\u0EA3',
                 '\u0EA5',
                 '\u0EA7',
 
-                '\u0EAA\u02BD',
-                '\u0EAA\u02BD',
+                '\u0EA8',
+                '\u0EA9',
                 '\u0EAA',
                 '\u0EAB'
                 ]
 
 SouthConsonantMap = [
-                    '\u0EA5\u02BD',
-                    '\u0EA5\u02BD',
+                    '\u0EAC',
+                    '\u0EAC\u02BD',
                     'ຮ',
                     '\u0E99\u02BD'
                     ]
 
 NuktaConsonantMap =  [
                     '\u0E81\u02BD',
                     '\u0E82\u02BD',
                     '\u0E84\u02BD',
                     '\u0E8A\u02BD',
-                    '\u0E94\u02BD',
-                    '\u0E97\u02BD',
+                    '\u0E90\u02BD',
+                    '\u0E91\u02BD',
                     'ຝ',
-                    '\u0EA2\u02BD',
+                    '\u0EA2',
                      ]
 
 SinhalaConsonantMap =[
                      '\u0ECD\u0E84\u02BD',
                      '\u0ECD\u0E8A\u02BD',
-                     '\u0ECD\u0E97\u02BD',
+                     '\u0ECD\u0E90\u02BD',
                      '\u0ECD\u0E97\u02BD',
                      '\u0ECD\u0E9E\u02BD',
                       ]
 
 NuktaMap = [
-           '\uEB0A'
+           '\u02BD\u02BD\u02BD\u02BD'
            ]
 
 OmMap = [
-        '\u0EC2\u0EAD\u0E87\u0EBA'
+        '\u0EC2\u0EAD\u0ECD\u02BD'
         ]
 
 SignMap =[
          "'",
          '\u0EAF',
          '\u0EAF\u0EAF'
          ]
@@ -169,7 +165,13 @@
              '\u0ED4',
              '\u0ED5',
              '\u0ED6',
              '\u0ED7',
              '\u0ED8',
              '\u0ED9'
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/LaoPali.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Ranjana.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,171 +1,177 @@
 # -*- coding: utf-8 -*-
 
 # Script Mapping for Devanagari
 
 VowelMap =  [
-            '\u0EAD',
-            '\u0EAD\u0EB2',
-            '\u0EAD\u0EB4',
-            '\u0EAD\u0EB5',
-            '\u0EAD\u0EB8',
-            '\u0EAD\u0EB9',
-            '\u0EA3\u0EB8\u02BD',
-            '\u0EA3\u0EB9\u02BD',
-            '\u0EA5\u0EB8\u02BD',
-            '\u0EA5\u0EB9\u02BD',
-            '\u0EAD\u0EC0',
-            '\u0EAD\u0EC4',
-            '\u0EAD\u0EC2',
-            '\u0EAD\u0EC0\u0EBB\u0EB2',
+            '\u0905',
+            '\u0906',
+            '\u0907',
+            '\u0908',
+            '\u0909',
+            '\u090A',
+            '\u090B',
+            '\u0960',
+            '\u090C',
+            '\u0961',
+            '\u090F',
+            '\u0910',
+            '\u0913',
+            '\u0914',
             ]
 
 SouthVowelMap = [
-                '\u0EAD\u0EC0\u0EB0',
-                '\u0EAD\u0EC2\u0EB0',
+                '\u090F\u02BD',
+                '\u0913\u02BD',
                 ]
 
 ModernVowelMap = [
-                 '\u0EAD\u0EC1\u0EB0',
-                 '\u0EAD\u0EC0\u0EB2\u0EB0',
+                '\u090F\u02BD',
+                '\u0906\u02BD',
                  ]
 
 SinhalaVowelMap = [
-                  '\u0EAD\u0EC1'
+                '\u090F\u02BD',
                   ]
 
 VowelSignMap =  [
-                 '\u0EB2',
-                 '\u0EB4',
-                 '\u0EB5',
-                 '\u0EB8',
-                 '\u0EB9',
-                 '\u0EBA\u0EA3\u0EB8\u02BD',
-                 '\u0EBA\u0EA3\u0EB9\u02BD',
-                 '\u0EBA\u0EA5\u0EB8\u02BD',
-                 '\u0EBA\u0EA5\u0EB9\u02BD',
-                 '\u0EC0',
-                 '\u0EC4',
-                 '\u0EC2',
-                 '\u0EC0\u0EBB\u0EB2',
+                '\u093E',
+                '\u093F',
+                '\u0940',
+                '\u0941',
+                '\u0942',
+                '\u0943',
+                '\u0944',
+                '\u0962',
+                '\u0963',
+                '\u0947',
+                '\u0948',
+                '\u094B',
+                '\u094C',
                 ]
 
 SouthVowelSignMap = [
-                     '\u0EC0\u0EB0',
-                     '\u0EC2\u0EB0',
+                    '\u0947\u02BD',
+                    '\u094B\u02BD',
                     ]
 
 ModernVowelSignMap =[
-                     '\u0EC1\u0EB0',
-                     '\u0EC0\u0EB2\u0EB0',
+                    '\u0947\u02BD',
+                    '\u093E\u02BD',
                     ]
 
 SinhalaVowelSignMap = [
-                       '\u0EC1'
+                    '\u0947\u02BD',
                       ]
 
 AyogavahaMap = [
-               '\u0ECD\u02BD',
-               '\u0ECD',
-               '\u0EAB\u0ECC'
+               '\u0901',
+               '\u0902',
+               '\u0903'
                ]
 
 ViramaMap =  [
-             '\u0EBA'
+             '\u094D'
              ]
 
 ConsonantMap =  [
-                '\u0E81',
-                '\u0E82',
-                '\u0E84',
-                '\u0E86',
-                '\u0E87',
-
-                '\u0E88',
-                '\u0E89',
-                '\u0E8A',
-                '\u0E8C',
-                '\u0E8E',
-
-                '\u0E8F',
-                '\u0E90',
-                '\u0E91',
-                '\u0E92',
-                '\u0E93',
-
-                '\u0E95',
-                '\u0E96',
-                '\u0E97',
-                '\u0E98',
-                '\u0E99',
-
-                '\u0E9B',
-                '\u0E9C',
-                '\u0E9E',
-                '\u0EA0',
-                '\u0EA1',
-
-                '\u0E8D',
-                '\u0EA3',
-                '\u0EA5',
-                '\u0EA7',
-
-                '\u0EA8',
-                '\u0EA9',
-                '\u0EAA',
-                '\u0EAB'
+                '\u0915',
+                '\u0916',
+                '\u0917',
+                '\u0918',
+                '\u0919',
+
+                '\u091A',
+                '\u091B',
+                '\u091C',
+                '\u091D',
+                '\u091E',
+
+                '\u091F',
+                '\u0920',
+                '\u0921',
+                '\u0922',
+                '\u0923',
+
+                '\u0924',
+                '\u0925',
+                '\u0926',
+                '\u0927',
+                '\u0928',
+
+                '\u092A',
+                '\u092B',
+                '\u092C',
+                '\u092D',
+                '\u092E',
+
+                '\u092F',
+                '\u0930',
+                '\u0932',
+                '\u0935',
+
+                '\u0936',
+                '\u0937',
+                '\u0938',
+                '\u0939'
                 ]
 
 SouthConsonantMap = [
-                    '\u0EAC',
-                    '\u0EAC\u02BD',
-                    'ຮ',
-                    '\u0E99\u02BD'
+                    'ल\u02BD',
+                    'ल\u02BD',
+                    '\u0930\u02BD',
+                    '\u0928\u02BD'
                     ]
 
 NuktaConsonantMap =  [
-                    '\u0E81\u02BD',
-                    '\u0E82\u02BD',
-                    '\u0E84\u02BD',
-                    '\u0E8A\u02BD',
-                    '\u0E90\u02BD',
-                    '\u0E91\u02BD',
-                    'ຝ',
-                    '\u0EA2',
+                    '\u0915\u02BD',
+                    '\u0916\u02BD',
+                    '\u0917\u02BD',
+                     '\u091C\u02BD',
+                '\u0921\u02BD',
+                '\u0922\u02BD',
+                     '\u092B\u02BD',
+                     '\u092F\u02BD'
                      ]
 
 SinhalaConsonantMap =[
-                     '\u0ECD\u0E84\u02BD',
-                     '\u0ECD\u0E8A\u02BD',
-                     '\u0ECD\u0E90\u02BD',
-                     '\u0ECD\u0E97\u02BD',
-                     '\u0ECD\u0E9E\u02BD',
+                     '\u0901\u02BD\u0917',
+                     '\u0901\u02BD\u091C',
+                     '\u0901\u02BD\u0921',
+                     '\u0901\u02BD\u0926',
+                     '\u0901\u02BD\u092C',
                       ]
 
 NuktaMap = [
-           '\u02BD\u02BD\u02BD\u02BD'
+           '\u093C'
            ]
 
 OmMap = [
-        '\u0EC2\u0EAD\u0ECD\u02BD'
+        '\u0950'
         ]
 
 SignMap =[
-         "'",
-         '\u0EAF',
-         '\u0EAF\u0EAF'
+         '\u093D',
+         '\u0964',
+         '\u0965'
          ]
 
 Aytham =[AyogavahaMap[2]+'\u02BD']
 
 NumeralMap = [
-             '\u0ED0',
-             '\u0ED1',
-             '\u0ED2',
-             '\u0ED3',
-             '\u0ED4',
-             '\u0ED5',
-             '\u0ED6',
-             '\u0ED7',
-             '\u0ED8',
-             '\u0ED9'
+             '\u0966',
+             '\u0967',
+             '\u0968',
+             '\u0969',
+             '\u096A',
+             '\u096B',
+             '\u096C',
+             '\u096D',
+             '\u096E',
+             '\u096F'
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/LaoTham.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Gurmukhi.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,173 +1,177 @@
 # -*- coding: utf-8 -*-
 
 # Script Mapping for Devanagari
 
-### AM - re-arrangement Tai Tham ??!!
-
 VowelMap =  [
-            '\u1A4B',
-            '\u1A4B\u1A63',
-            '\u1A4D',
-            '\u1A4E',
-            '\u1A4F',
-            '\u1A50',
-            '\u1A42',
-            '\u1A42\u1A63',
-            '\u1A44',
-            '\u1A44\u1A63',
-            '\u1A51',
-            '\u1A4B\u1A71',
-            '\u1A52',
-            '\u1A4F\u1A6B\u1A63', #http://reg.ksu.ac.th/bai_laan/THN.pdf ; Enquire about the arc above sign
+            '\u0A05',
+            '\u0A06',
+            '\u0A07',
+            '\u0A08',
+            '\u0A09',
+            '\u0A0A',
+            '\u0A30\u0A41\u02BC',
+            '\u0A30\u0A42\u02BC',
+            '\u0A32\u0A41\u02BC',
+            '\u0A32\u0A42\u02BC',
+            '\u0A0F',
+            '\u0A10',
+            '\u0A13',
+            '\u0A14',
             ]
 
 SouthVowelMap = [
-                '\u1A51\u02BD',
-                '\u1A52\u02BD',
+                '\u0A0F\u02D8',
+                '\u0A13\u02D8',
                 ]
 
 ModernVowelMap = [
-                 '\u1A51\u02BD',
-                 '\u1A4B\u1A63\u02BD',
+                 '\u0A0F\u02BC',
+                 '\u0A06\u02BC',
                  ]
 
 SinhalaVowelMap = [
-                  '\u1A51\u02BD'
+                  '\u0A0F\u02C7'
                   ]
 
 VowelSignMap =  [
-                '\u1A63',
-                '\u1A65',
-                '\u1A66',
-                '\u1A69',
-                '\u1A6A',
-                '\u1A7A\u1A42',
-                '\u1A7A\u1A42\u1A63',
-                '\u1A7A\u1A44',
-                '\u1A7A\u1A44\u1A63',
-                '\u1A6E',
-                '\u1A71',
-                '\u1A6E\u1A63',
-                '\u1A6E\u1A6B\u1A63',
+                '\u0A3E',
+                '\u0A3F',
+                '\u0A40',
+                '\u0A41',
+                '\u0A42',
+                '\u0A4D\u0A30\u0A41\u02BC',
+                '\u0A4D\u0A30\u0A42\u02BC',
+                '\u0A4D\u0A32\u0A41\u02BC',
+                '\u0A4D\u0A32\u0A42\u02BC',
+                '\u0A47',
+                '\u0A48',
+                '\u0A4B',
+                '\u0A4C',
                 ]
 
 SouthVowelSignMap = [
-                    '\u1A6E\u02BD',
-                    '\u1A6E\u1A63\u02BD',
+                    '\u0A47\u02D8',
+                    '\u0A4B\u02D8',
                     ]
 
 ModernVowelSignMap =[
-                    '\u1A6E\u02BD',
-                    '\u1A63\u02BD']
+                    '\u0A47\u02BC',
+                    '\u0A3E\u02BC']
 
 SinhalaVowelSignMap = [
-                      '\u1A6E\u02BD'
+                      '\u0A47\u02C7'
                       ]
 
 AyogavahaMap = [
-               '\u1A74\u02BD',
-               '\u1A74',
-               '\u1A61'
+               '\u0A01',
+               '\u0A02',
+               '\u0A03'
                ]
 
 ViramaMap =  [
-             '\u1A7A'
+             '\u0A4D'
              ]
 
 ConsonantMap =  [
-                '\u1A20',
-                '\u1A21',
-                '\u1A23',
-                '\u1A25',
-                '\u1A26',
-
-                '\u1A27',
-                '\u1A28',
-                '\u1A29',
-                '\u1A2B',
-                '\u1A2C',
-
-                '\u1A2D',
-                '\u1A2E',
-                '\u1A2F',
-                '\u1A30',
-                '\u1A31',
-
-                '\u1A32',
-                '\u1A33',
-                '\u1A34',
-                '\u1A35',
-                '\u1A36',
-
-                '\u1A38',
-                '\u1A39',
-                '\u1A3B',
-                '\u1A3D',
-                '\u1A3E',
-
-                '\u1A3F',
-                '\u1A41',
-                '\u1A43',
-                '\u1A45',
-
-                '\u1A46',
-                '\u1A47',
-                '\u1A48',
-                '\u1A49'
+                '\u0A15',
+                '\u0A16',
+                '\u0A17',
+                '\u0A18',
+                '\u0A19',
+
+                '\u0A1A',
+                '\u0A1B',
+                '\u0A1C',
+                '\u0A1D',
+                '\u0A1E',
+
+                '\u0A1F',
+                '\u0A20',
+                '\u0A21',
+                '\u0A22',
+                '\u0A23',
+
+                '\u0A24',
+                '\u0A25',
+                '\u0A26',
+                '\u0A27',
+                '\u0A28',
+
+                '\u0A2A',
+                '\u0A2B',
+                '\u0A2C',
+                '\u0A2D',
+                '\u0A2E',
+
+                '\u0A2F',
+                '\u0A30',
+                '\u0A32',
+                '\u0A35',
+
+                '\u0A36',
+                '\u0A36\u0A3C',
+                '\u0A38',
+                '\u0A39'
                 ]
 
 SouthConsonantMap = [
-                    '\u1A4A',
-                    '\u1A4A\u02BD',
-                    '\u1A41\u02BD',
-                    '\u1A36\u02BD'
+                    '\u0A33',
+                    '\u0A33\u0A3C',
+                    '\u0A30\u0A3C',
+                    '\u0A28\u0A3C'
                     ]
 
 NuktaConsonantMap =  [
-                     '\u1A20\u02BD',
-                     '\u1A21\u02BD',
-                     '\u1A23\u02BD',
-                     '\u1A29\u02BD',
-                     '\u1A2F\u02BD',
-                     '\u1A30\u02BD',
-                     '\u1A39\u02BD',
-                     '\u1A3F\u02BD'
+                     '\u0A15\u0A3C',
+                     '\u0A59',
+                     '\u0A5A',
+                     '\u0A5B',
+                     '\u0A5C',
+                     'ੜ੍ਹ',
+                     '\u0A5E',
+                     '\u0A2F\u0A3C'
                      ]
 
 SinhalaConsonantMap =[
-                     '\u1A74\u1A23\u02BD',
-                     '\u1A74\u1A29\u02BD',
-                     '\u1A74\u1A2F\u02BD',
-                     '\u1A74\u1A34\u02BD',
-                     '\u1A74\u1A3D\u02BD',
+                     '\u0A01\u02C6\u0A17',
+                     '\u0A01\u02C6\u0A1C',
+                     '\u0A01\u02C6\u0A21',
+                     '\u0A01\u02C6\u0A26',
+                     '\u0A01\u02C6\u0A2C',
                       ]
 
 NuktaMap = [
-           '\u02BD\u02BD\u02BD\u02BD'
+           '\u0A3C'
            ]
 
 OmMap = [
-        '\u1A52\u1A74'
+        '\u0A74'
         ]
 
 SignMap =[
-         "'",
-         '\u1AA8',
-         '\u1AA9'
+         '\u0028\u0A05\u0029',
+         '\u0964',
+         '\u0965'
          ]
 
-Aytham =[AyogavahaMap[2]+'\u02BD']
+Aytham =[AyogavahaMap[2]+'\u02BC']
 
 
 NumeralMap = [
-             '\u1A90',
-             '\u1A91',
-             '\u1A92',
-             '\u1A93',
-             '\u1A94',
-             '\u1A95',
-             '\u1A96',
-             '\u1A97',
-             '\u1A98',
-             '\u1A99',
+             '\u0A66',
+             '\u0A67',
+             '\u0A68',
+             '\u0A69',
+             '\u0A6A',
+             '\u0A6B',
+             '\u0A6C',
+             '\u0A6D',
+             '\u0A6E',
+             '\u0A6F'
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/LueTham.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Assamese.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,173 +1,176 @@
 # -*- coding: utf-8 -*-
 
 # Script Mapping for Devanagari
 
-### AM - re-arrangement Tai Tham ??!!
-
 VowelMap =  [
-            '\u1A4B',
-            '\u1A4B\u1A63',
-            '\u1A4D',
-            '\u1A4E',
-            '\u1A4F',
-            '\u1A50',
-            '\u1A42',
-            '\u1A42\u1A63',
-            '\u1A44',
-            '\u1A44\u1A63',
-            '\u1A51',
-            '\u1A4B\u1A71',
-            '\u1A52',
-            '\u1A4F\u1A6B\u1A63', #http://reg.ksu.ac.th/bai_laan/THN.pdf ; Enquire about the arc above sign
+            '\u0985',
+            '\u0986',
+            '\u0987',
+            '\u0988',
+            '\u0989',
+            '\u098A',
+            '\u098B',
+            '\u09E0',
+            '\u098C',
+            '\u09E1',
+            '\u098F',
+            '\u0990',
+            '\u0993',
+            '\u0994',
             ]
 
 SouthVowelMap = [
-                '\u1A51\u02BD',
-                '\u1A52\u02BD',
+                '\u098F\u02D8',
+                '\u0993\u02D8',
                 ]
 
 ModernVowelMap = [
-                 '\u1A51\u02BD',
-                 '\u1A4B\u1A63\u02BD',
+                 '\u098F\u02BC',
+                 '\u0986\u02BC',
                  ]
 
 SinhalaVowelMap = [
-                  '\u1A51\u02BD'
+                  '\u098F\u02C7'
                   ]
 
 VowelSignMap =  [
-                '\u1A63',
-                '\u1A65',
-                '\u1A66',
-                '\u1A69',
-                '\u1A6A',
-                '\u1A7A\u1A42',
-                '\u1A7A\u1A42\u1A63',
-                '\u1A7A\u1A44',
-                '\u1A7A\u1A44\u1A63',
-                '\u1A6E',
-                '\u1A71',
-                '\u1A6E\u1A63',
-                '\u1A6E\u1A6B\u1A63',
+                '\u09BE',
+                '\u09BF',
+                '\u09C0',
+                '\u09C1',
+                '\u09C2',
+                '\u09C3',
+                '\u09C4',
+                '\u09E2',
+                '\u09E3',
+                '\u09C7',
+                '\u09C8',
+                '\u09CB',
+                '\u09CC',
                 ]
 
 SouthVowelSignMap = [
-                    '\u1A6E\u02BD',
-                    '\u1A6E\u1A63\u02BD',
+                    '\u09C7\u02D8',
+                    '\u09CB\u02D8',
                     ]
 
 ModernVowelSignMap =[
-                    '\u1A6E\u02BD',
-                    '\u1A63\u02BD']
+                    '\u09C7\u02BC',
+                    '\u09BE\u02BC']
 
 SinhalaVowelSignMap = [
-                      '\u1A6E\u02BD'
+                      '\u09C7\u02C7'
                       ]
 
 AyogavahaMap = [
-               '\u1A74\u02BD',
-               '\u1A74',
-               '\u1A61'
+               '\u0981',
+               '\u0982',
+               '\u0983'
                ]
 
 ViramaMap =  [
-             '\u1A7A'
+             '\u09CD'
              ]
 
 ConsonantMap =  [
-                '\u1A20',
-                '\u1A21',
-                '\u1A23',
-                '\u1A25',
-                '\u1A26',
-
-                '\u1A27',
-                '\u1A28',
-                '\u1A29',
-                '\u1A2B',
-                '\u1A2C',
-
-                '\u1A2D',
-                '\u1A2E',
-                '\u1A2F',
-                '\u1A30',
-                '\u1A31',
-
-                '\u1A32',
-                '\u1A33',
-                '\u1A34',
-                '\u1A35',
-                '\u1A36',
-
-                '\u1A38',
-                '\u1A39',
-                '\u1A3B',
-                '\u1A3D',
-                '\u1A3E',
-
-                '\u1A3F',
-                '\u1A41',
-                '\u1A43',
-                '\u1A45',
-
-                '\u1A46',
-                '\u1A47',
-                '\u1A48',
-                '\u1A49'
+                '\u0995',
+                '\u0996',
+                '\u0997',
+                '\u0998',
+                '\u0999',
+
+                '\u099A',
+                '\u099B',
+                '\u099C',
+                '\u099D',
+                '\u099E',
+
+                '\u099F',
+                '\u09A0',
+                '\u09A1',
+                '\u09A2',
+                '\u09A3',
+
+                '\u09A4',
+                '\u09A5',
+                '\u09A6',
+                '\u09A7',
+                '\u09A8',
+
+                '\u09AA',
+                '\u09AB',
+                '\u09AC',
+                '\u09AD',
+                '\u09AE',
+
+                '\u09AF',
+                '\u09B0',
+                '\u09B2',
+                '\u09F1',
+
+                '\u09B6',
+                '\u09B7',
+                '\u09B8',
+                '\u09B9'
                 ]
 
 SouthConsonantMap = [
-                    '\u1A4A',
-                    '\u1A4A\u02BD',
-                    '\u1A41\u02BD',
-                    '\u1A36\u02BD'
+                    '\u09B2\u09BC',
+                    '\u09B7\u09BC',
+                    '\u09B0\u09BC',
+                    '\u09A8\u09BC'
                     ]
 
 NuktaConsonantMap =  [
-                     '\u1A20\u02BD',
-                     '\u1A21\u02BD',
-                     '\u1A23\u02BD',
-                     '\u1A29\u02BD',
-                     '\u1A2F\u02BD',
-                     '\u1A30\u02BD',
-                     '\u1A39\u02BD',
-                     '\u1A3F\u02BD'
+                     '\u0995\u09BC',
+                     '\u0996\u09BC',
+                     '\u0997\u09BC',
+                     '\u099C\u09BC',
+                     '\u09DC',
+                     '\u09DD',
+                     '\u09AB\u09BC',
+                     '\u09DF'
                      ]
 
 SinhalaConsonantMap =[
-                     '\u1A74\u1A23\u02BD',
-                     '\u1A74\u1A29\u02BD',
-                     '\u1A74\u1A2F\u02BD',
-                     '\u1A74\u1A34\u02BD',
-                     '\u1A74\u1A3D\u02BD',
+                     '\u0981\u02C6\u0997',
+                     '\u0981\u02C6\u099C',
+                     '\u0981\u02C6\u09A1',
+                     '\u0981\u02C6\u09A6',
+                     '\u0981\u02C6\u09AC',
                       ]
 
 NuktaMap = [
-           '\u02BD\u02BD\u02BD\u02BD'
+           '\u09BC'
            ]
 
 OmMap = [
-        '\u1A52\u1A74'
+        '\u0993\u0981'
         ]
 
 SignMap =[
-         "'",
-         '\u1AA8',
-         '\u1AA9'
+         '\u09BD',
+         '\u0964',
+         '\u0965'
          ]
 
-Aytham =[AyogavahaMap[2]+'\u02BD']
-
+Aytham =[AyogavahaMap[2]+'\u02BC']
 
 NumeralMap = [
-             '\u1A90',
-             '\u1A91',
-             '\u1A92',
-             '\u1A93',
-             '\u1A94',
-             '\u1A95',
-             '\u1A96',
-             '\u1A97',
-             '\u1A98',
-             '\u1A99',
+             '\u09E6',
+             '\u09E7',
+             '\u09E8',
+             '\u09E9',
+             '\u09EA',
+             '\u09EB',
+             '\u09EC',
+             '\u09ED',
+             '\u09EE',
+             '\u09EF'
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/Makasar.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Makasar.py`

 * *Files 20% similar despite different names*

```diff
@@ -164,7 +164,13 @@
              '\u06F4',
              '\u06F5',
              '\u06F6',
              '\u06F7',
              '\u06F8',
              '\u06F9',
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/Marchen.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Marchen.py`

 * *Files 9% similar despite different names*

```diff
@@ -165,7 +165,13 @@
              '\u0F24',
              '\u0F25',
              '\u0F26',
              '\u0F27',
              '\u0F28',
              '\u0F29'
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/Mon.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Burmese.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,45 +2,45 @@
 
 # Script Mapping for Devanagari
 
 VowelMap =  [
             '\u1021',
             '\u1021\u102C',
             '\u1023',
-            'ဣဳ',
+            '\u1024',
             '\u1025',
-            'ဥူ',
+            '\u1026',
             '\u1052',
             '\u1053',
             '\u1054',
             '\u1055',
-            'ဨ',
+            '\u1027',
             '\u1021\u1032',
             '\u1029',
             '\u102A',
             ]
 
 SouthVowelMap = [
-                'ဨ\u02BD',
+                '\u1027\u02BD',
                 '\u1029\u02BD',
                 ]
 
 ModernVowelMap = [
-                 'ဨ\u02BD',
+                 '\u1027\u02BD',
                  '\u1021\u102C\u02BD',
                  ]
 
 SinhalaVowelMap = [
-                  'ဨ\u02BD'
+                  '\u1027\u02BD'
                   ]
 
 VowelSignMap =  [
                 '\u102C',
                 '\u102D',
-                'ဳ',
+                '\u102E',
                 '\u102F',
                 '\u1030',
                 '\u1056',
                 '\u1057',
                 '\u1058',
                 '\u1059',
                 '\u1031',
@@ -73,21 +73,21 @@
              ]
 
 ConsonantMap =  [
                 '\u1000',
                 '\u1001',
                 '\u1002',
                 '\u1003',
-                'ၚ',
+                '\u1004',
 
                 '\u1005',
                 '\u1006',
                 '\u1007',
-                'ၛ',
-                'ည',
+                '\u1008',
+                '\u1009',
 
                 '\u100B',
                 '\u100C',
                 '\u100D',
                 '\u100E',
                 '\u100F',
 
@@ -165,7 +165,13 @@
              '\u1044',
              '\u1045',
              '\u1046',
              '\u1047',
              '\u1048',
              '\u1049',
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/Pallava.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Rejang.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,171 +1,176 @@
 # -*- coding: utf-8 -*-
 
 # Script Mapping for Devanagari
 
 VowelMap =  [
-            '\uA984',
-            '\uA984\uA9B4',
-            '\uA986',
-            '\uA987',
-            '\uA988',
-            '\uA988\uA9B4',
-            'ꦫꦶ\u02BD',
-            'ꦫꦷ\u02BD',
-            'ꦭꦶ\u02BD',
-            'ꦭꦷ\u02BD',
-            '\uA98C',
-            '\uA98D',
-            '\uA98E',
-            '\uA98E\uA9B4',
+            '\uA946',
+            '\uA946\u02BD',
+            '\uA946\uA947',
+            '\uA946\uA947\u02BD',
+            '\uA946\uA948',
+            '\uA946\uA948\u02BD',
+            '\uA93D\uA948\u02BD',
+            '\uA93D\uA948\u02BD',
+            '\uA93E\uA948\u02BD',
+            '\uA93E\uA948\u02BD',
+            '\uA946\uA949\u02BD',
+            '\uA946\uA94A',
+            '\uA946\uA94B\u02BD',
+            '\uA946\uA94C',
             ]
 
 SouthVowelMap = [
-                '\uA98C\u02BD',
-                '\uA98E\u02BD',
+                '\uA946\uA949',
+                '\uA946\uA94B',
                 ]
 
 ModernVowelMap = [
-                '\uA98C\u02BD',
-                 '\uA984\uA9B4\u02BD',
+                '\uA946\uA94E',
+                '\uA946\uA94D',
                  ]
 
 SinhalaVowelMap = [
-                '\uA98C\u02BD',
+                '\uA946\uA94E\u02BD'
                   ]
 
 VowelSignMap =  [
-                '\uA9B4',
-                '\uA9B6',
-                '\uA9B7',
-                '\uA9B8',
-                '\uA9B9',
-            '\uA9C0ꦫꦶ\u02BD',
-            '\uA9C0ꦫꦷ\u02BD',
-            '\uA9C0ꦭꦶ\u02BD',
-            '\uA9C0ꦭꦷ\u02BD',
-                '\uA9BA',
-                '\uA9BB',
-                '\uA9BA\uA9B4',
-                '\uA9BB\uA9B4',
+                '\u02BD\u02BD',
+                '\uA947',
+                '\uA947\u02BD',
+                '\uA948',
+                '\uA948\u02BD',
+                '\uA953\uA93D\uA948\u02BD',
+                '\uA953\uA93D\uA948\u02BD',
+                '\uA953\uA93E\uA948\u02BD',
+                '\uA953\uA93E\uA948\u02BD',
+                '\uA949\u02BD',
+                '\uA94A',
+                '\uA94B\u02BD',
+                '\uA94C',
                 ]
 
 SouthVowelSignMap = [
-                    '\uA9BA\u02BD',
-                    '\uA9BA\uA9B4\u02BD',
+                     '\uA949',
+                     '\uA94B',
                     ]
 
 ModernVowelSignMap =[
-                    '\uA9BA\u02BD',
-                    '\uA9B4\u02BD']
+                     '\uA94E',
+                     '\uA94D',
+                    ]
 
 SinhalaVowelSignMap = [
-                    '\uA9BA\u02BD',
+                      '\uA94E\u02BD'
                       ]
 
 AyogavahaMap = [
-               '\uA981\u02BD',
-               '\uA981',
-               '\uA983'
+               '\uA94F\u02BD',
+               '\uA94F',
+               '\uA952'
                ]
 
 ViramaMap =  [
-             '\uA9C0'
+             '\uA953'
              ]
 
 ConsonantMap =  [
-                '\uA98F',
-                '\uA991',
-                '\uA992',
-                '\uA993',
-                '\uA994',
-
-                '\uA995',
-                '\uA996',
-                '\uA997',
-                '\uA999',
-                '\uA99A',
-
-                '\uA99B',
-                '\uA99C',
-                '\uA99D',
-                '\uA99E',
-                '\uA99F',
-
-                '\uA9A0',
-                '\uA9A1',
-                '\uA9A2',
-                '\uA9A3',
-                '\uA9A4',
-
-                '\uA9A5',
-                '\uA9A6',
-                '\uA9A7',
-                '\uA9A8',
-                '\uA9A9',
-
-                '\uA9AA',
-                '\uA9AB',
-                '\uA9AD',
-                '\uA9AE',
-
-                '\uA9AF',
-                '\uA9B0',
-                '\uA9B1',
-                '\uA9B2'
+                '\uA930',
+                '\uA930\u02BD',
+                '\uA931',
+                '\uA931\u02BD',
+                '\uA932',
+
+                '\uA939',
+                '\uA939\u02BD',
+                '\uA93A',
+                '\uA93A\u02BD',
+                '\uA93B',
+
+                '\uA933\u02BD',
+                '\uA933\u02BD',
+                '\uA934\u02BD',
+                '\uA934\u02BD',
+                '\uA935\u02BD',
+
+                '\uA933',
+                '\uA933\u02BD',
+                '\uA934',
+                '\uA934\u02BD',
+                '\uA935',
+
+                '\uA936',
+                '\uA936\u02BD',
+                '\uA937',
+                '\uA937\u02BD',
+                '\uA938',
+
+                '\uA93F',
+                '\uA93D',
+                '\uA93E',
+                '\uA940',
+
+                '\uA93C\u02BD',
+                '\uA93C\u02BD',
+                '\uA93C',
+                '\uA941'
                 ]
 
 SouthConsonantMap = [
-                    '\uA9AD\u02BD',
-                    '\uA9B0\u02BD',
-                    '\uA9AB\u02BD',
-                    '\uA9A4\u02BD'
+                    '\uA93E\u02BD',
+                    '\uA93E\u02BD',
+                    '\uA93D\u02BD',
+                    '\uA935\u02BD'
                     ]
 
 NuktaConsonantMap =  [
-                     '\uA98F\u02BD',
-                     '\uA991\u02BD',
-                     '\uA992\u02BD',
-                     '\uA997\u02BD',
-                     '\uA99D\u02BD',
-                     '\uA99E\u02BD',
-                     '\uA9A6\u02BD',
-                     '\uA9AA\u02BD'
+                     '\uA930\u02BD',
+                     '\uA930\u02BD',
+                     '\uA931\u02BD',
+                     '\uA93A\u02BD',
+                     '\uA934\u02BD',
+                     '\uA934\u02BD',
+                     '\uA936\u02BD',
+                     '\uA93F\u02BD'
                      ]
-
 SinhalaConsonantMap =[
-                     '\uA981\uA992\u02BD',
-                     '\uA981\uA997\u02BD',
-                     '\uA981\uA99D\u02BD',
-                     '\uA981\uA9A2\u02BD',
-                     '\uA981\uA9A7\u02BD',
+                     '\uA943',
+                     '\uA945',
+                     '\uA944\u02BD',
+                     '\uA944',
+                     '\uA942',
                       ]
 
 NuktaMap = [
-           '\u02BD\u02BD'
+           '\u02BD\u02BD\u02BD'
            ]
 
 OmMap = [
-        '\uA98E\uA981'
+        '\uA946\uA94B\uA94F\u02BD'
         ]
 
 SignMap =[
-         '\u0027',
-         '|',
-         '||'
+         "'",
+         '\u002E',
+         '\u002E\u002E'
          ]
 
 Aytham =[AyogavahaMap[2]+'\u02BD']
 
-
 NumeralMap = [
-             '\u0030',
-             '\u0031',
-             '\u0032',
-             '\u0033',
-             '\u0034',
-             '\u0035',
-             '\u0036',
-             '\u0037',
-             '\u0038',
-             '\u0039',
+             '0',
+             '1',
+             '2',
+             '3',
+             '4',
+             '5',
+             '6',
+             '7',
+             '8',
+             '9'
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/PhagsPa.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/PhagsPa.py`

 * *Files 17% similar despite different names*

```diff
@@ -164,7 +164,13 @@
              '\u0034',
              '\u0035',
              '\u0036',
              '\u0037',
              '\u0038',
              '\u0039',
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/Rejang.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/TamilExtended.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,170 +1,176 @@
 # -*- coding: utf-8 -*-
 
 # Script Mapping for Devanagari
 
 VowelMap =  [
-            '\uA946',
-            '\uA946\u02BD',
-            '\uA946\uA947',
-            '\uA946\uA947\u02BD',
-            '\uA946\uA948',
-            '\uA946\uA948\u02BD',
-            '\uA93D\uA948\u02BD',
-            '\uA93D\uA948\u02BD',
-            '\uA93E\uA948\u02BD',
-            '\uA93E\uA948\u02BD',
-            '\uA946\uA949\u02BD',
-            '\uA946\uA94A',
-            '\uA946\uA94B\u02BD',
-            '\uA946\uA94C',
+            '\u0D05',
+            '\u0D06',
+            '\u0D07',
+            '\u0D08',
+            '\u0D09',
+            '\u0D0A',
+            '\u0D0B',
+            '\u0D60',
+            '\u0D0C',
+            '\u0D61',
+            '\u0D0F',
+            '\u0D10',
+            '\u0D13',
+            '\u0D14',
             ]
 
 SouthVowelMap = [
-                '\uA946\uA949',
-                '\uA946\uA94B',
+                '\u0D0E',
+                '\u0D12',
                 ]
 
 ModernVowelMap = [
-                '\uA946\uA94E',
-                '\uA946\uA94D',
+                 '\u0D0E\u02BC',
+                 '\u0D06\u02BC',
                  ]
 
 SinhalaVowelMap = [
-                '\uA946\uA94E\u02BD'
+                  '\u0D0F\u02C7'
                   ]
 
 VowelSignMap =  [
-                '\u02BD\u02BD',
-                '\uA947',
-                '\uA947\u02BD',
-                '\uA948',
-                '\uA948\u02BD',
-                '\uA953\uA93D\uA948\u02BD',
-                '\uA953\uA93D\uA948\u02BD',
-                '\uA953\uA93E\uA948\u02BD',
-                '\uA953\uA93E\uA948\u02BD',
-                '\uA949\u02BD',
-                '\uA94A',
-                '\uA94B\u02BD',
-                '\uA94C',
+                '\u0D3E',
+                '\u0D3F',
+                '\u0D40',
+                '\u0D41',
+                '\u0D42',
+                '\u0D43',
+                '\u0D44',
+                '\u0D62',
+                '\u0D63',
+                '\u0D47',
+                '\u0D48',
+                '\u0D4B',
+                '\u0D57',
                 ]
 
 SouthVowelSignMap = [
-                     '\uA949',
-                     '\uA94B',
+                    '\u0D46',
+                    '\u0D4A',
                     ]
 
 ModernVowelSignMap =[
-                     '\uA94E',
-                     '\uA94D',
-                    ]
+                    '\u0D46\u02BC',
+                    '\u0D3E\u02BC']
 
 SinhalaVowelSignMap = [
-                      '\uA94E\u02BD'
+                      '\u0D47\u02C7'
                       ]
 
 AyogavahaMap = [
-               '\uA94F\u02BD',
-               '\uA94F',
-               '\uA952'
+               '\u0D01',
+               '\u0D02',
+               '\u0D03'
                ]
 
 ViramaMap =  [
-             '\uA953'
+             '\u0D4D\u200C'
              ]
 
 ConsonantMap =  [
-                '\uA930',
-                '\uA930\u02BD',
-                '\uA931',
-                '\uA931\u02BD',
-                '\uA932',
-
-                '\uA939',
-                '\uA939\u02BD',
-                '\uA93A',
-                '\uA93A\u02BD',
-                '\uA93B',
-
-                '\uA933\u02BD',
-                '\uA933\u02BD',
-                '\uA934\u02BD',
-                '\uA934\u02BD',
-                '\uA935\u02BD',
-
-                '\uA933',
-                '\uA933\u02BD',
-                '\uA934',
-                '\uA934\u02BD',
-                '\uA935',
-
-                '\uA936',
-                '\uA936\u02BD',
-                '\uA937',
-                '\uA937\u02BD',
-                '\uA938',
-
-                '\uA93F',
-                '\uA93D',
-                '\uA93E',
-                '\uA940',
-
-                '\uA93C\u02BD',
-                '\uA93C\u02BD',
-                '\uA93C',
-                '\uA941'
+                '\u0D15',
+                '\u0D16',
+                '\u0D17',
+                '\u0D18',
+                '\u0D19',
+
+                '\u0D1A',
+                '\u0D1B',
+                '\u0D1C',
+                '\u0D1D',
+                '\u0D1E',
+
+                '\u0D1F',
+                '\u0D20',
+                '\u0D21',
+                '\u0D22',
+                '\u0D23',
+
+                '\u0D24',
+                '\u0D25',
+                '\u0D26',
+                '\u0D27',
+                '\u0D28',
+
+                '\u0D2A',
+                '\u0D2B',
+                '\u0D2C',
+                '\u0D2D',
+                '\u0D2E',
+
+                '\u0D2F',
+                '\u0D30',
+                '\u0D32',
+                '\u0D35',
+
+                '\u0D36',
+                '\u0D37',
+                '\u0D38',
+                '\u0D39'
                 ]
 
 SouthConsonantMap = [
-                    '\uA93E\u02BD',
-                    '\uA93E\u02BD',
-                    '\uA93D\u02BD',
-                    '\uA935\u02BD'
+                    '\u0D33',
+                    '\u0D34',
+                    '\u0D31',
+                    '\u0D29'
                     ]
 
 NuktaConsonantMap =  [
-                     '\uA930\u02BD',
-                     '\uA930\u02BD',
-                     '\uA931\u02BD',
-                     '\uA93A\u02BD',
-                     '\uA934\u02BD',
-                     '\uA934\u02BD',
-                     '\uA936\u02BD',
-                     '\uA93F\u02BD'
+                     '\u0D15\u00B7',
+                     '\u0D16\u00B7',
+                     '\u0D17\u00B7',
+                     '\u0D1C\u00B7',
+                     '\u0D21\u00B7',
+                     '\u0D22\u00B7',
+                     '\u0D2B\u00B7',
+                     '\u0D2F\u00B7'
                      ]
+
 SinhalaConsonantMap =[
-                     '\uA943',
-                     '\uA945',
-                     '\uA944\u02BD',
-                     '\uA944',
-                     '\uA942',
+                     '\u0D02\u02C6\u0D17',
+                     '\u0D02\u02C6\u0D1C',
+                     '\u0D02\u02C6\u0D21',
+                     '\u0D02\u02C6\u0D26',
+                     '\u0D02\u02C6\u0D2C',
                       ]
 
 NuktaMap = [
-           '\u02BD\u02BD\u02BD'
+           '\u00B7'
            ]
 
 OmMap = [
-        '\uA946\uA94B\uA94F\u02BD'
+        '\u0BD0'
         ]
 
 SignMap =[
-         "'",
-         '\u002E',
-         '\u002E\u002E'
+         '\u0D3D',
+         '.',
+         '..'
          ]
 
-Aytham =[AyogavahaMap[2]+'\u02BD']
+Aytham =['\u0B83']
 
 NumeralMap = [
              '0',
              '1',
              '2',
              '3',
              '4',
              '5',
              '6',
              '7',
              '8',
              '9'
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/Shan.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/ShanLoC.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
                 'ရိ\u02BD',
                 'ရီ\u02BD',
                 'လိ\u02BD',
                 'လီ\u02BD',
                 '\u1022\u1031',
                 '\u1022ႆ',
                 '\u1022\u1031ႃ',
-                '\u1022ဝ်\u02BD',
+                '\u1022ွ',
             ]
 
 SouthVowelMap = [
                 '\u1022\u1031\u02BD',
                 '\u1022\u1031ႃ\u02BD',
                 ]
 
@@ -42,15 +42,15 @@
                 '\u103Aရိ\u02BD',
                 '\u103Aရီ\u02BD',
                 '\u103Aလိ\u02BD',
                 '\u103Aလီ\u02BD',
                 '\u1031',
                 'ႆ',
                 '\u1031ႃ',
-                'ဝ်\u02BD',
+                'ွ',
                 ]
 
 SouthVowelSignMap = [
                     '\u1031\u02BD',
                     '\u1031ႃ\u02BD',
                     ]
 
@@ -166,7 +166,13 @@
              '\u1094',
              '\u1095',
              '\u1096',
              '\u1097',
              '\u1098',
              '\u1099',
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/Siddham.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Tirhuta.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,171 +1,177 @@
 # -*- coding: utf-8 -*-
 
 # Script Mapping for Devanagari
 
 VowelMap =  [
-            '\U00011580',
-            '\U00011581',
-            '\U00011582',
-            '\U00011583',
-            '\U00011584',
-            '\U00011585',
-            '\U00011586',
-            '\U00011587',
-            '\U00011588',
-            '\U00011589',
-            '\U0001158A',
-            '\U0001158B',
-            '\U0001158C',
-            '\U0001158D'
+            '\U00011481',
+            '\U00011482',
+            '\U00011483',
+            '\U00011484',
+            '\U00011485',
+            '\U00011486',
+            '\U00011487',
+            '\U00011488',
+            '\U00011489',
+            '\U0001148A',
+            '\U0001148B',
+            '\U0001148C',
+            '\U0001148D',
+            '\U0001148E',
             ]
 
 SouthVowelMap = [
-                '\U0001158A\u02BD',
-                '\U0001158C\u02BD',
+                '\U00011481\U000114BA',
+                '\U00011481\U000114BD',
                 ]
 
 ModernVowelMap = [
-                 '\U0001158A\u02BD',
-                 '\U00011581\u02BD',
+                 '\U0001148B\u02BD',
+                 '\U00011482\u02BD',
                  ]
 
 SinhalaVowelMap = [
-                  '\U0001158A\u02BD'
+                  '\U0001148B\u02BD'
                   ]
 
 VowelSignMap =  [
-                '\U000115AF',
-                '\U000115B0',
-                '\U000115B1',
-                '\U000115B2',
-                '\U000115B3',
-                '\U000115B4',
-                '\U000115B5',
-                '𑖿𑖩𑖰\u02BD',
-                '𑖿𑖩𑖱\u02BD',
-                '\U000115B8',
-                '\U000115B9',
-                '\U000115BA',
-                '\U000115BB',
+                '\U000114B0',
+                '\U000114B1',
+                '\U000114B2',
+                '\U000114B3',
+                '\U000114B4',
+                '\U000114B5',
+                '\U000114B6',
+                '\U000114B7',
+                '\U000114B8',
+                '\U000114B9',
+                '\U000114BB',
+                '\U000114BC',
+                '\U000114BE',
                 ]
 
 SouthVowelSignMap = [
-                    '\U000115B8\u02BD',
-                    '\U000115BA\u02BD',
+                    '\U000114BA',
+                    '\U000114BD',
                     ]
 
 ModernVowelSignMap =[
-                    '\U000115B8\u02BD',
-                    '\U000115AF\u02BD'
+                    '\U000114B9\u02BD',
+                    '\U000114B0\u02BD'
                     ]
 
 SinhalaVowelSignMap = [
-                    '\U000115B8\u02BD',
+                      '\U000114B9\u02BD'
                       ]
 
 AyogavahaMap = [
-               '\U000115BC',
-               '\U000115BD',
-               '\U000115BE'
+               '\U000114BF',
+               '\U000114C0',
+               '\U000114C1'
                ]
 
 ViramaMap =  [
-             '\U000115BF'
+             '\U000114C2'
              ]
 
 ConsonantMap =  [
-                '\U0001158E',
-                '\U0001158F',
-                '\U00011590',
-                '\U00011591',
-                '\U00011592',
-
-                '\U00011593',
-                '\U00011594',
-                '\U00011595',
-                '\U00011596',
-                '\U00011597',
-
-                '\U00011598',
-                '\U00011599',
-                '\U0001159A',
-                '\U0001159B',
-                '\U0001159C',
-
-                '\U0001159D',
-                '\U0001159E',
-                '\U0001159F',
-                '\U000115A0',
-                '\U000115A1',
-
-                '\U000115A2',
-                '\U000115A3',
-                '\U000115A4',
-                '\U000115A5',
-                '\U000115A6',
-
-                '\U000115A7',
-                '\U000115A8',
-                '\U000115A9',
-                '\U000115AA',
-
-                '\U000115AB',
-                '\U000115AC',
-                '\U000115AD',
-                '\U000115AE'
+                '\U0001148F',
+                '\U00011490',
+                '\U00011491',
+                '\U00011492',
+                '\U00011493',
+
+                '\U00011494',
+                '\U00011495',
+                '\U00011496',
+                '\U00011497',
+                '\U00011498',
+
+                '\U00011499',
+                '\U0001149A',
+                '\U0001149B',
+                '\U0001149C',
+                '\U0001149D',
+
+                '\U0001149E',
+                '\U0001149F',
+                '\U000114A0',
+                '\U000114A1',
+                '\U000114A2',
+
+                '\U000114A3',
+                '\U000114A4',
+                '\U000114A5',
+                '\U000114A6',
+                '\U000114A7',
+
+                '\U000114A8',
+                '\U000114A9',
+                '\U000114AA',
+                '\U000114AB',
+
+                '\U000114AC',
+                '\U000114AD',
+                '\U000114AE',
+                '\U000114AF'
                 ]
 
 SouthConsonantMap = [
-                    '𑖩𑗀',
-                    '𑖬𑗀',
-                    '𑖨𑗀',
-                    '𑖡𑗀'
+                    '𑒝𑓃',
+                    '𑒭𑓃',
+                    '𑒩\u02BD',
+                    '𑒪𑓃'
                     ]
 
 NuktaConsonantMap =  [
-                     '𑖎𑗀',
-                     '𑖏𑗀',
-                     '𑖐𑗀',
-                     '𑖕𑗀',
-                     '𑖚𑗀',
-                     '𑖛𑗀',
-                     '𑖣𑗀',
-                     '𑖧𑗀'
+                     '\U0001148F\U000114C3',
+                     '\U00011490\U000114C3',
+                     '\U00011491\U000114C3',
+                     '\U00011496\U000114C3',
+                     '\U0001149B\U000114C3',
+                     '\U0001149C\U000114C3',
+                     '\U000114A4\U000114C3',
+                     '\U000114A8\U000114C3'
                      ]
 
 SinhalaConsonantMap =[
-                     '\U000115BC\u02BD\U00011590',
-                     '\U000115BC\u02BD\U00011595',
-                     '\U000115BC\u02BD\U0001159A',
-                     '\U000115BC\u02BD\U0001159F',
-                     '\U000115BC\u02BD\U000115A4',
+                     '\U000114BF𑒑\u02BD',
+                     '\U000114BF𑒖\u02BD',
+                     '\U000114BF𑒛\u02BD',
+                     '\U000114BF𑒠\u02BD',
+                     '\U000114BF𑒥\u02BD',
                       ]
 
 NuktaMap = [
-           '\U000115C0'
+           '\U000114C3'
            ]
 
 OmMap = [
-        '𑖌𑖼'
+        '𑓇'
         ]
 
 SignMap =[
-         '\u02BD\u02BD',
-         '\U000115C2',
-         '\U000115C3'
+         '𑓄',
+         '।',
+         '॥'
          ]
 
 Aytham =[AyogavahaMap[2]+'\u02BD']
 
 NumeralMap = [
-             '0',
-             '1',
-             '2',
-             '3',
-             '4',
-             '5',
-             '6',
-             '7',
-             '8',
-             '9'
+             '\U000114D0',
+             '\U000114D1',
+             '\U000114D2',
+             '\U000114D3',
+             '\U000114D4',
+             '\U000114D5',
+             '\U000114D6',
+             '\U000114D7',
+             '\U000114D8',
+             '\U000114D9'
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/SiddhamRanjana.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/SiddhamRanjana.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/Soyombo.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Soyombo.py`

 * *Files 8% similar despite different names*

```diff
@@ -165,7 +165,13 @@
              '4',
              '5',
              '6',
              '7',
              '8',
              '9'
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/Sundanese.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Sundanese.py`

 * *Files 21% similar despite different names*

```diff
@@ -164,7 +164,13 @@
              '\u1BB4',
              '\u1BB5',
              '\u1BB6',
              '\u1BB7',
              '\u1BB8',
              '\u1BB9'
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/Tagalog.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Tagbanwa.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,156 +1,156 @@
 # -*- coding: utf-8 -*-
 
 # Script Mapping for Devanagari
 
 VowelMap =  [
-            '\u1700',
-            '\u1700\u02BD',
-            '\u1701',
-            '\u1701\u02BD',
-            '\u1702',
-            '\u1702\u02BD',
-            '\u170E\u1713\u02BD',
-            '\u170E\u1713\u02BD',
-            '\u170E\u1713\u02BD',
-            '\u170E\u1713\u02BD',
-            '\u1701\u02BD',
-            '\u1700\u1701\u02BD',
-            '\u1702\u02BD',
-            '\u1700\u1702\u02BD',
+            '\u1760',
+            '\u1760\u02BD',
+            '\u1761',
+            '\u1761\u02BD',
+            '\u1762',
+            '\u1762\u02BD',
+            '\u176E\u1773\u02BD',
+            '\u176E\u1773\u02BD',
+            '\u176E\u1773\u02BD',
+            '\u176E\u1773\u02BD',
+            '\u1761\u02BD',
+            '\u1760\u1761\u02BD',
+            '\u1762\u02BD',
+            '\u1760\u1762\u02BD',
             ]
 
 SouthVowelMap = [
-                '\u1701\u02BD',
-                '\u1702\u02BD',
+                '\u1761\u02BD',
+                '\u1762\u02BD',
                 ]
 
 ModernVowelMap = [
-                 '\u1701\u02BD',
-                 '\u1700\u02BD',
+                 '\u1761\u02BD',
+                 '\u1760\u02BD',
                  ]
 
 SinhalaVowelMap = [
-                  '\u1701\u02BD'
+                  '\u1761\u02BD'
                   ]
 
 VowelSignMap =  [
                 '\u02BD\u02BD',
-                '\u1712',
-                '\u1712\u02BD',
-                '\u1713',
-                '\u1713\u02BD',
-                '\u1714\u170E\u1713\u02BD',
-                '\u1714\u170E\u1713\u02BD',
-                '\u1714\u170E\u1713\u02BD',
-                '\u1714\u170E\u1713\u02BD',
-                '\u1712\u02BD',
-                '\u1701\u02BD',
-                '\u1713\u02BD',
-                '\u1702\u02BD',
+                '\u1772',
+                '\u1772\u02BD',
+                '\u1773',
+                '\u1773\u02BD',
+                '\u176E\u1773\u02BD',
+                '\u176E\u1773\u02BD',
+                '\u176E\u1773\u02BD',
+                '\u176E\u1773\u02BD',
+                '\u1772\u02BD',
+                '\u1761\u02BD',
+                '\u1773\u02BD',
+                '\u1762\u02BD',
                 ]
 
 SouthVowelSignMap = [
-                     '\u1712\u02BD',
-                     '\u1713\u02BD',
+                     '\u1772\u02BD',
+                     '\u1773\u02BD',
                     ]
 
 ModernVowelSignMap =[
-                     '\u1712\u02BD',
+                     '\u1772\u02BD',
                      '\u02BD\u02BD',
                     ]
 
 SinhalaVowelSignMap = [
-                      '\u1712\u02BD'
+                      '\u1772\u02BD'
                       ]
 
 AyogavahaMap = [
-               '\u170B\u1714\u02BD',
-               '\u170B\u1714\u02BD',
-               '\u1711\u1714\u02BD'
+               '\u176B\u02BD',
+               '\u176B\u02BD',
+               '\u1763\u02BD'
                ]
 
 ViramaMap =  [
-             '\u1714'
+             '\u02BD\u02BD'
              ]
 
 ConsonantMap =  [
-                '\u1703',
-                '\u1703\u02BD',
-                '\u1704',
-                '\u1704\u02BD',
-                '\u1705',
-
-                '\u1710\u02BD', # sa instead of cha
-                '\u1710\u02BD',
-                '\u1707\u02BD',       # da instead of ja
-                '\u1707\u02BD',
-                '\u1708\u02BD',
-
-                '\u1706\u02BD',
-                '\u1706\u02BD',
-                '\u1707\u02BD',
-                '\u1707\u02BD',
-                '\u1708\u02BD',
-
-                '\u1706',
-                '\u1706\u02BD',
-                '\u1707',
-                '\u1707\u02BD',
-                '\u1708',
-
-                '\u1709',
-                '\u1709\u02BD',
-                '\u170A',
-                '\u170A\u02BD',
-                '\u170B',
-
-                '\u170C',
-                '\u170D',
-                '\u170E',
-                '\u170F',
-
-                '\u1710\u02BD',
-                '\u1710\u02BD',
-                '\u1710',
-                '\u1711'
+                '\u1763',
+                '\u1763\u02BD',
+                '\u1764',
+                '\u1764\u02BD',
+                '\u1765',
+
+                '\u1770\u02BD', # sa instead of cha
+                '\u1770\u02BD',
+                '\u1767\u02BD',       # da instead of ja
+                '\u1767\u02BD',
+                '\u1768\u02BD',
+
+                '\u1766\u02BD',
+                '\u1766\u02BD',
+                '\u1767\u02BD',
+                '\u1767\u02BD',
+                '\u1768\u02BD',
+
+                '\u1766',
+                '\u1766\u02BD',
+                '\u1767',
+                '\u1767\u02BD',
+                '\u1768',
+
+                '\u1769',
+                '\u1769\u02BD',
+                '\u176A',
+                '\u176A\u02BD',
+                '\u176B',
+
+                '\u176C',
+                '\u176E\u02BD',
+                '\u176E',
+                '\u176F',
+
+                '\u1770\u02BD',
+                '\u1770\u02BD',
+                '\u1770',
+                '\u1763\u02BD'
                 ]
 
 SouthConsonantMap = [
-                    '\u170E\u02BD',
-                    '\u170E\u02BD',
-                    '\u170D\u02BD',
-                    '\u1708\u02BD'
+                    '\u176E\u02BD',
+                    '\u176E\u02BD',
+                    '\u176E\u02BD',
+                    '\u1768\u02BD'
                     ]
 
 NuktaConsonantMap =  [
-                     '\u1703\u02BD',
-                     '\u1703\u02BD',
-                     '\u1704\u02BD',
-                     '\u1707\u02BD',
-                     '\u1707\u02BD',
-                     '\u1707\u02BD',
-                     '\u1709\u02BD',
-                     '\u170C\u02BD'
+                     '\u1763\u02BD',
+                     '\u1763\u02BD',
+                     '\u1764\u02BD',
+                     '\u1767\u02BD',
+                     '\u1767\u02BD',
+                     '\u1767\u02BD',
+                     '\u1769\u02BD',
+                     '\u176C\u02BD'
                      ]
 
 SinhalaConsonantMap =[
-                     '\u1705\u1714\u1704\u02BD',
-                     '\u1708\u1707\u1704\u02BD',
-                     '\u1708\u1707\u1704\u02BD',
-                     '\u1708\u1707\u1704\u02BD',
-                     '\u170B\u170A\u1704\u02BD',
+                     '\u1765\u1764\u02BD',
+                     '\u1768\u1767\u02BD',
+                     '\u1768\u1767\u02BD',
+                     '\u1768\u1767\u02BD',
+                     '\u176B\u176A\u02BD',
                       ]
 
 NuktaMap = [
            '\u02BD\u02BD\u02BD\u02BD'
            ]
 
 OmMap = [
-        '\u1702\u170B\u1714\u02BD'
+        '\u1762\u176B\u02BD'
         ]
 
 SignMap =[
          "\u02BD\u02BD",
          '\u1735',
          '\u1736'
          ]
@@ -165,7 +165,13 @@
              '\u0034',
              '\u0035',
              '\u0036',
              '\u0037',
              '\u0038',
              '\u0039',
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/Tagbanwa.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/SiddhamDevanagari.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,171 +1,177 @@
 # -*- coding: utf-8 -*-
 
 # Script Mapping for Devanagari
 
 VowelMap =  [
-            '\u1760',
-            '\u1760\u02BD',
-            '\u1761',
-            '\u1761\u02BD',
-            '\u1762',
-            '\u1762\u02BD',
-            '\u176E\u1773\u02BD',
-            '\u176E\u1773\u02BD',
-            '\u176E\u1773\u02BD',
-            '\u176E\u1773\u02BD',
-            '\u1761\u02BD',
-            '\u1760\u1761\u02BD',
-            '\u1762\u02BD',
-            '\u1760\u1762\u02BD',
+            '\u0905',
+            '\u0906',
+            '\u0907',
+            '\u0908',
+            '\u0909',
+            '\u090A',
+            '\u090B',
+            '\u0960',
+            '\u090C',
+            '\u0961',
+            '\u090F',
+            '\u0910',
+            '\u0913',
+            '\u0914',
             ]
 
 SouthVowelMap = [
-                '\u1761\u02BD',
-                '\u1762\u02BD',
+                '\u090F\u02BD',
+                '\u0913\u02BD',
                 ]
 
 ModernVowelMap = [
-                 '\u1761\u02BD',
-                 '\u1760\u02BD',
+                '\u090F\u02BD',
+                '\u0906\u02BD',
                  ]
 
 SinhalaVowelMap = [
-                  '\u1761\u02BD'
+                '\u090F\u02BD',
                   ]
 
 VowelSignMap =  [
-                '\u02BD\u02BD',
-                '\u1772',
-                '\u1772\u02BD',
-                '\u1773',
-                '\u1773\u02BD',
-                '\u176E\u1773\u02BD',
-                '\u176E\u1773\u02BD',
-                '\u176E\u1773\u02BD',
-                '\u176E\u1773\u02BD',
-                '\u1772\u02BD',
-                '\u1761\u02BD',
-                '\u1773\u02BD',
-                '\u1762\u02BD',
+                '\u093E',
+                '\u093F',
+                '\u0940',
+                '\u0941',
+                '\u0942',
+                '\u0943',
+                '\u0944',
+                '\u0962',
+                '\u0963',
+                '\u0947',
+                '\u0948',
+                '\u094B',
+                '\u094C',
                 ]
 
 SouthVowelSignMap = [
-                     '\u1772\u02BD',
-                     '\u1773\u02BD',
+                    '\u0947\u02BD',
+                    '\u094B\u02BD',
                     ]
 
 ModernVowelSignMap =[
-                     '\u1772\u02BD',
-                     '\u02BD\u02BD',
+                    '\u0947\u02BD',
+                    '\u093E\u02BD',
                     ]
 
 SinhalaVowelSignMap = [
-                      '\u1772\u02BD'
+                    '\u0947\u02BD',
                       ]
 
 AyogavahaMap = [
-               '\u176B\u02BD',
-               '\u176B\u02BD',
-               '\u1763\u02BD'
+               '\u0901',
+               '\u0902',
+               '\u0903'
                ]
 
 ViramaMap =  [
-             '\u02BD\u02BD'
+             '\u094D'
              ]
 
 ConsonantMap =  [
-                '\u1763',
-                '\u1763\u02BD',
-                '\u1764',
-                '\u1764\u02BD',
-                '\u1765',
-
-                '\u1770\u02BD', # sa instead of cha
-                '\u1770\u02BD',
-                '\u1767\u02BD',       # da instead of ja
-                '\u1767\u02BD',
-                '\u1768\u02BD',
-
-                '\u1766\u02BD',
-                '\u1766\u02BD',
-                '\u1767\u02BD',
-                '\u1767\u02BD',
-                '\u1768\u02BD',
-
-                '\u1766',
-                '\u1766\u02BD',
-                '\u1767',
-                '\u1767\u02BD',
-                '\u1768',
-
-                '\u1769',
-                '\u1769\u02BD',
-                '\u176A',
-                '\u176A\u02BD',
-                '\u176B',
-
-                '\u176C',
-                '\u176E\u02BD',
-                '\u176E',
-                '\u176F',
-
-                '\u1770\u02BD',
-                '\u1770\u02BD',
-                '\u1770',
-                '\u1763\u02BD'
+                '\u0915',
+                '\u0916',
+                '\u0917',
+                '\u0918',
+                '\u0919',
+
+                '\u091A',
+                '\u091B',
+                '\u091C',
+                '\u091D',
+                '\u091E',
+
+                '\u091F',
+                '\u0920',
+                '\u0921',
+                '\u0922',
+                '\u0923',
+
+                '\u0924',
+                '\u0925',
+                '\u0926',
+                '\u0927',
+                '\u0928',
+
+                '\u092A',
+                '\u092B',
+                '\u092C',
+                '\u092D',
+                '\u092E',
+
+                '\u092F',
+                '\u0930',
+                '\u0932',
+                '\u0935',
+
+                '\u0936',
+                '\u0937',
+                '\u0938',
+                '\u0939'
                 ]
 
 SouthConsonantMap = [
-                    '\u176E\u02BD',
-                    '\u176E\u02BD',
-                    '\u176E\u02BD',
-                    '\u1768\u02BD'
+                    'ल़',
+                    'ष़',
+                    '\u0931',
+                    '\u0929'
                     ]
 
 NuktaConsonantMap =  [
-                     '\u1763\u02BD',
-                     '\u1763\u02BD',
-                     '\u1764\u02BD',
-                     '\u1767\u02BD',
-                     '\u1767\u02BD',
-                     '\u1767\u02BD',
-                     '\u1769\u02BD',
-                     '\u176C\u02BD'
+                     '\u0958',
+                     '\u0959',
+                     '\u095A',
+                     '\u095B',
+                     '\u095C',
+                     '\u095D',
+                     '\u095E',
+                     '\u095F'
                      ]
 
 SinhalaConsonantMap =[
-                     '\u1765\u1764\u02BD',
-                     '\u1768\u1767\u02BD',
-                     '\u1768\u1767\u02BD',
-                     '\u1768\u1767\u02BD',
-                     '\u176B\u176A\u02BD',
+                     '\u0901\u02BD\u0917',
+                     '\u0901\u02BD\u091C',
+                     '\u0901\u02BD\u0921',
+                     '\u0901\u02BD\u0926',
+                     '\u0901\u02BD\u092C',
                       ]
 
 NuktaMap = [
-           '\u02BD\u02BD\u02BD\u02BD'
+           '\u093C'
            ]
 
 OmMap = [
-        '\u1762\u176B\u02BD'
+        '\u0950'
         ]
 
 SignMap =[
-         "\u02BD\u02BD",
-         '\u1735',
-         '\u1736'
+         '\u093D',
+         '\u0964',
+         '\u0965'
          ]
 
 Aytham =[AyogavahaMap[2]+'\u02BD']
 
 NumeralMap = [
-             '\u0030',
-             '\u0031',
-             '\u0032',
-             '\u0033',
-             '\u0034',
-             '\u0035',
-             '\u0036',
-             '\u0037',
-             '\u0038',
-             '\u0039',
+             '\u0966',
+             '\u0967',
+             '\u0968',
+             '\u0969',
+             '\u096A',
+             '\u096B',
+             '\u096C',
+             '\u096D',
+             '\u096E',
+             '\u096F'
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/TaiLaing.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Mon.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,172 +1,177 @@
 # -*- coding: utf-8 -*-
 
 # Script Mapping for Devanagari
 
 VowelMap =  [
             '\u1021',
-                '\u1021ႃ',
-                '\u1021\u102D',
-                '\u1021\u102E',
-                '\u1021\u102F',
-                '\u1021\u1030',
-                'ꩺိ\u02BD',
-                'ꩺီ\u02BD',
-                'လိ\u02BD',
-                'လီ\u02BD',
-                '\u1021\u1031',
-                '\u1021ႆ',
-                '\u1021\u1031ႃ',
-                '\u1021ဝ်\u02BD',
+            '\u1021\u102C',
+            '\u1023',
+            'ဣဳ',
+            '\u1025',
+            'ဥူ',
+            '\u1052',
+            '\u1053',
+            '\u1054',
+            '\u1055',
+            'ဨ',
+            '\u1021\u1032',
+            '\u1029',
+            '\u102A',
             ]
 
 SouthVowelMap = [
-                '\u1021\u1031\u02BD',
-                '\u1021\u1031ႃ\u02BD',
+                'ဨ\u02BD',
+                '\u1029\u02BD',
                 ]
 
 ModernVowelMap = [
-                  '\u1021\u1031\u02BD',
-                 '\u1021ႃ\u02BD',
+                 'ဨ\u02BD',
+                 '\u1021\u102C\u02BD',
                  ]
 
 SinhalaVowelMap = [
-                  '\u1021\u1031\u02BD'
+                  'ဨ\u02BD'
                   ]
 
 VowelSignMap =  [
-                'ႃ',
+                '\u102C',
                 '\u102D',
-                '\u102E',
+                'ဳ',
                 '\u102F',
                 '\u1030',
-                '်ꩺိ\u02BD',
-                '်ꩺီ\u02BD',
-                '်လိ\u02BD',
-                '်လီ\u02BD',
+                '\u1056',
+                '\u1057',
+                '\u1058',
+                '\u1059',
                 '\u1031',
-                'ႆ',
-                '\u1031ႃ',
-                'ဝ်\u02BD',
+                '\u1032',
+                '\u1031\u102C',
+                '\u1031\u102C\u103A',
                 ]
 
 SouthVowelSignMap = [
                     '\u1031\u02BD',
-                    '\u1031ႃ\u02BD',
+                    '\u1031\u102C\u02BD',
                     ]
 
 ModernVowelSignMap =[
-                    'ႄ',
-                    'ႃ\u02BD'
-                    ]
+                    '\u1031\u02BD',
+                    '\u102C\u02BD']
 
 SinhalaVowelSignMap = [
-                    'ႄ\u02BD',
+                      '\u1031\u02BD'
                       ]
 
 AyogavahaMap = [
                '\u1036\u02BD',
                '\u1036',
                '\u1038'
                ]
 
 ViramaMap =  [
              '\u103A'
              ]
 
 ConsonantMap =  [
-                'က',
-                'ၵ',
-                'ꧩ',
-                'ꧪ',
-                '\u1004',
-
-                'ၸ',
-                'ꩬ',
-                'ꧫ',
-                'ꧬ',
-                'ꧧ',
-
-                'ꩦ',
-                'ꩧ',
-                'ꧭ',
-                'ꧮ',
-                'ꧯ',
+                '\u1000',
+                '\u1001',
+                '\u1002',
+                '\u1003',
+                'ၚ',
+
+                '\u1005',
+                '\u1006',
+                '\u1007',
+                'ၛ',
+                'ည',
+
+                '\u100B',
+                '\u100C',
+                '\u100D',
+                '\u100E',
+                '\u100F',
 
                 '\u1010',
                 '\u1011',
-                'ꧻ',
-                'ꧼ',
-                'ꩫ',
-
-                'ပ',
-                'ꧤ',
-                'ꧽ',
-                'ꧾ',
+                '\u1012',
+                '\u1013',
+                '\u1014',
+
+                '\u1015',
+                '\u1016',
+                '\u1017',
+                '\u1018',
                 '\u1019',
 
                 '\u101A',
-                'ꩺ',
+                '\u101B',
                 '\u101C',
                 '\u101D',
 
-                'ꧬ\u02BD',
-                'ꧬ\u02BD',
-                'ꧬ',
-                'ၯ'
+                '\u1050',
+                '\u1051',
+                '\u101E',
+                '\u101F'
                 ]
 
 SouthConsonantMap = [
-                    'ꧺ',
-                    'ꧺ\u02BD',
-                    'ꩺ\u02BD',
-                    'ꩫ\u02BD'
+                    '\u1020',
+                    '\u1020\u02BD',
+                    '\u101B\u02BD',
+                    '\u1014\u02BD'
                     ]
 
 NuktaConsonantMap =  [
-                'က\u02BD',
-                'ၵ\u02BD',
-                'ꧩ\u02BD',
-                     'ꧫ\u02BD',
-                'ꧭ\u02BD',
-                'ꧮ\u02BD',
-                     'ꧨ',
+                     '\u1000\u02BD',
+                     '\u1001\u02BD',
+                     '\u1002\u02BD',
+                     '\u1007\u02BD',
+                     '\u100D\u02BD',
+                     '\u100E\u02BD',
+                     '\u1016\u02BD',
                      '\u101A\u02BD'
                      ]
 
 SinhalaConsonantMap =[
-                     '\u1036ၵ\u02BD',
-                     '\u1036ꧫ\u02BD',
-                     '\u1036ꧭ\u02BD',
-                     '\u1036ꧻ\u02BD',
-                     '\u1036ꧽ\u02BD',
+                     '\u1036\u1002\u02BD',
+                     '\u1036\u1007\u02BD',
+                     '\u1036\u100D\u02BD',
+                     '\u1036\u1012\u02BD',
+                     '\u1036\u1017\u02BD',
                       ]
 
 NuktaMap = [
-           '\u02BD\u02BD\u02BD'
+           '\u02BD\u02BD\u02BD\u02BD'
            ]
 
 OmMap = [
-        '\u1021\u1031ႃ\u1036'
+        'ဥုံ'
         ]
 
 SignMap =[
          '\u0027',
          '\u104A',
          '\u104B'
          ]
 
 Aytham =[AyogavahaMap[2]+'\u02BD']
 
 
 NumeralMap = [
-             '\uA9F0',
-             '\uA9F1',
-             '\uA9F2',
-             '\uA9F3',
-             '\uA9F4',
-             '\uA9F5',
-             '\uA9F6',
-             '\uA9F7',
-             '\uA9F8',
-             '\uA9F9',
+             '\u1040',
+             '\u1041',
+             '\u1042',
+             '\u1043',
+             '\u1044',
+             '\u1045',
+             '\u1046',
+             '\u1047',
+             '\u1048',
+             '\u1049',
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/TaiTham.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Bengali.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,173 +1,176 @@
 # -*- coding: utf-8 -*-
 
 # Script Mapping for Devanagari
 
-### AM - re-arrangement Tai Tham ??!!
-
 VowelMap =  [
-            '\u1A4B',
-            '\u1A4B\u1A63',
-            '\u1A4D',
-            '\u1A4E',
-            '\u1A4F',
-            '\u1A50',
-            '\u1A42',
-            '\u1A42\u1A63',
-            '\u1A44',
-            '\u1A44\u1A63',
-            '\u1A51',
-            '\u1A4B\u1A71',
-            '\u1A52',
-            '\u1A4F\u1A6B\u1A63', #http://reg.ksu.ac.th/bai_laan/THN.pdf ; Enquire about the arc above sign
+            '\u0985',
+            '\u0986',
+            '\u0987',
+            '\u0988',
+            '\u0989',
+            '\u098A',
+            '\u098B',
+            '\u09E0',
+            '\u098C',
+            '\u09E1',
+            '\u098F',
+            '\u0990',
+            '\u0993',
+            '\u0994',
             ]
 
 SouthVowelMap = [
-                '\u1A51\u02BD',
-                '\u1A52\u02BD',
+                '\u098F\u02D8',
+                '\u0993\u02D8',
                 ]
 
 ModernVowelMap = [
-                 '\u1A51\u02BD',
-                 '\u1A4B\u1A63\u02BD',
+                 '\u098F\u02BC',
+                 '\u0986\u02BC',
                  ]
 
 SinhalaVowelMap = [
-                  '\u1A51\u02BD'
+                  '\u098F\u02C7'
                   ]
 
 VowelSignMap =  [
-                '\u1A63',
-                '\u1A65',
-                '\u1A66',
-                '\u1A69',
-                '\u1A6A',
-                '\u1A7A\u1A42',
-                '\u1A7A\u1A42\u1A63',
-                '\u1A7A\u1A44',
-                '\u1A7A\u1A44\u1A63',
-                '\u1A6E',
-                '\u1A71',
-                '\u1A6E\u1A63',
-                '\u1A6E\u1A6B\u1A63',
+                '\u09BE',
+                '\u09BF',
+                '\u09C0',
+                '\u09C1',
+                '\u09C2',
+                '\u09C3',
+                '\u09C4',
+                '\u09E2',
+                '\u09E3',
+                '\u09C7',
+                '\u09C8',
+                '\u09CB',
+                '\u09CC',
                 ]
 
 SouthVowelSignMap = [
-                    '\u1A6E\u02BD',
-                    '\u1A6E\u1A63\u02BD',
+                    '\u09C7\u02D8',
+                    '\u09CB\u02D8',
                     ]
 
 ModernVowelSignMap =[
-                    '\u1A6E\u02BD',
-                    '\u1A63\u02BD']
+                    '\u09C7\u02BC',
+                    '\u09BE\u02BC']
 
 SinhalaVowelSignMap = [
-                      '\u1A6E\u02BD'
+                      '\u09C7\u02C7'
                       ]
 
 AyogavahaMap = [
-               '\u1A74\u02BD',
-               '\u1A74',
-               '\u1A61'
+               '\u0981',
+               '\u0982',
+               '\u0983'
                ]
 
 ViramaMap =  [
-             '\u1A7A'
+             '\u09CD'
              ]
 
 ConsonantMap =  [
-                '\u1A20',
-                '\u1A21',
-                '\u1A23',
-                '\u1A25',
-                '\u1A26',
-
-                '\u1A27',
-                '\u1A28',
-                '\u1A29',
-                '\u1A2B',
-                '\u1A2C',
-
-                '\u1A2D',
-                '\u1A2E',
-                '\u1A2F',
-                '\u1A30',
-                '\u1A31',
-
-                '\u1A32',
-                '\u1A33',
-                '\u1A34',
-                '\u1A35',
-                '\u1A36',
-
-                '\u1A38',
-                '\u1A39',
-                '\u1A3B',
-                '\u1A3D',
-                '\u1A3E',
-
-                '\u1A3F',
-                '\u1A41',
-                '\u1A43',
-                '\u1A45',
-
-                '\u1A46',
-                '\u1A47',
-                '\u1A48',
-                '\u1A49'
+                '\u0995',
+                '\u0996',
+                '\u0997',
+                '\u0998',
+                '\u0999',
+
+                '\u099A',
+                '\u099B',
+                '\u099C',
+                '\u099D',
+                '\u099E',
+
+                '\u099F',
+                '\u09A0',
+                '\u09A1',
+                '\u09A2',
+                '\u09A3',
+
+                '\u09A4',
+                '\u09A5',
+                '\u09A6',
+                '\u09A7',
+                '\u09A8',
+
+                '\u09AA',
+                '\u09AB',
+                '\u09AC',
+                '\u09AD',
+                '\u09AE',
+
+                '\u09AF',
+                '\u09B0',
+                '\u09B2',
+                'ভ়',
+
+                '\u09B6',
+                '\u09B7',
+                '\u09B8',
+                '\u09B9'
                 ]
 
 SouthConsonantMap = [
-                    '\u1A4A',
-                    '\u1A4A\u02BD',
-                    '\u1A41\u02BD',
-                    '\u1A36\u02BD'
+                    '\u09B2\u09BC',
+                    '\u09B7\u09BC',
+                    '\u09B0\u09BC',
+                    '\u09A8\u09BC'
                     ]
 
 NuktaConsonantMap =  [
-                     '\u1A20\u02BD',
-                     '\u1A21\u02BD',
-                     '\u1A23\u02BD',
-                     '\u1A29\u02BD',
-                     '\u1A2F\u02BD',
-                     '\u1A30\u02BD',
-                     '\u1A39\u02BD',
-                     '\u1A3F\u02BD'
+                     '\u0995\u09BC',
+                     '\u0996\u09BC',
+                     '\u0997\u09BC',
+                     '\u099C\u09BC',
+                     '\u09DC',
+                     '\u09DD',
+                     '\u09AB\u09BC',
+                     '\u09DF'
                      ]
 
 SinhalaConsonantMap =[
-                     '\u1A74\u1A23\u02BD',
-                     '\u1A74\u1A29\u02BD',
-                     '\u1A74\u1A2F\u02BD',
-                     '\u1A74\u1A34\u02BD',
-                     '\u1A74\u1A3D\u02BD',
+                     '\u0981\u02C6\u0997',
+                     '\u0981\u02C6\u099C',
+                     '\u0981\u02C6\u09A1',
+                     '\u0981\u02C6\u09A6',
+                     '\u0981\u02C6\u09AC',
                       ]
 
 NuktaMap = [
-           '\u02BD\u02BD\u02BD\u02BD'
+           '\u09BC'
            ]
 
 OmMap = [
-        '\u1A52\u1A74'
+        '\u0993\u0981'
         ]
 
 SignMap =[
-         "'",
-         '\u1AA8',
-         '\u1AA9'
+         '\u09BD',
+         '\u0964',
+         '\u0965'
          ]
 
-Aytham =[AyogavahaMap[2]+'\u02BD']
-
+Aytham =[AyogavahaMap[2]+'\u02BC']
 
 NumeralMap = [
-             '\u1A90',
-             '\u1A91',
-             '\u1A92',
-             '\u1A93',
-             '\u1A94',
-             '\u1A95',
-             '\u1A96',
-             '\u1A97',
-             '\u1A98',
-             '\u1A99',
+             '\u09E6',
+             '\u09E7',
+             '\u09E8',
+             '\u09E9',
+             '\u09EA',
+             '\u09EB',
+             '\u09EC',
+             '\u09ED',
+             '\u09EE',
+             '\u09EF'
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/Thaana.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Thaana.py`

 * *Files 11% similar despite different names*

```diff
@@ -164,8 +164,15 @@
              '\u0033',
              '\u0034',
              '\u0035',
              '\u0036',
              '\u0037',
              '\u0038',
              '\u0039',
-             ]
+             ]
+
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/Thai.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Thai.py`

 * *Files 16% similar despite different names*

```diff
@@ -168,7 +168,13 @@
              '\u0E54',
              '\u0E55',
              '\u0E56',
              '\u0E57',
              '\u0E58',
              '\u0E59',
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/Tibetan.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Tibetan.py`

 * *Files 18% similar despite different names*

```diff
@@ -164,7 +164,13 @@
              '\u0F24',
              '\u0F25',
              '\u0F26',
              '\u0F27',
              '\u0F28',
              '\u0F29'
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/EastIndic/ZanabazarSquare.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/ZanabazarSquare.py`

 * *Files 9% similar despite different names*

```diff
@@ -165,7 +165,13 @@
              '4',
              '5',
              '6',
              '7',
              '8',
              '9'
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/Ahom.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Ahom.py`

 * *Files 15% similar despite different names*

```diff
@@ -76,25 +76,25 @@
 ConsonantMap =  [
                 '\U00011700',
                 '\U00011701',
                 '\U00011715',
                 '\U00011717',
                 '\U00011702',
 
-                '\U0001170B\u02BD',
+                '\U00011740',
                 '\U0001170B',
                 '\U0001170A',
                 '\U00011719',
                 '\U00011710',
 
-                '\U00011704\u02BD',
-                '\U0001170C\u02BD',
-                '\U00011713\u02BD',
-                '\U00011714\u02BD',
-                '\U00011703\u02BD',
+                '\U00011741',
+                '\U00011742',
+                '\U00011743',
+                '\U00011744',
+                '\U00011745',
 
                 '\U00011704',
                 '\U0001170C',
                 '\U00011713',
                 '\U00011714',
                 '\U00011703',
 
@@ -103,25 +103,25 @@
                 '\U00011708',
                 '\U00011718',
                 '\U00011709',
 
                 '\U0001170A\u02BD',
                 '\U0001170D',
                 '\U0001170E',
-                '\U00011708\u02BD',
+                '𑜚',
 
                 '\U0001170F\u02BD',
                 '\U0001170F\u02BD',
                 '\U0001170F',
                 '\U00011711'
                 ]
 
 SouthConsonantMap = [
-                    '\U0001170E\u02BD',
-                    '\U0001170E\u02BD',
+                    '\U00011746',
+                    '\U00011746\u02BD',
                     '\U0001170D\u02BD',
                     '\U00011703\u02BD'
                     ]
 
 NuktaConsonantMap =  [
                      '\U00011700\u02BD',
                      '\U00011701\u02BD',
@@ -165,7 +165,13 @@
              '\U00011734',
              '\U00011735',
              '\U00011736',
              '\U00011737',
              '\U00011738',
              '\U00011739',
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/Assamese.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/WX.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,170 +1,156 @@
 # -*- coding: utf-8 -*-
 
-# Script Mapping for Devanagari
+# Script Mapping for ISO
 
 VowelMap =  [
-            '\u0985',
-            '\u0986',
-            '\u0987',
-            '\u0988',
-            '\u0989',
-            '\u098A',
-            '\u098B',
-            '\u09E0',
-            '\u098C',
-            '\u09E1',
-            '\u098F',
-            '\u0990',
-            '\u0993',
-            '\u0994',
+            '\u0061',
+            '\u0041',
+            '\u0069',
+            '\u0049',
+            '\u0075',
+            '\u0055',
+            '\u0071',
+            '\u0071\u0056',
+            '\u004C',
+            '\u004C\u0056',
+            '\u0065',
+            '\u0045',
+            '\u006F',
+            '\u004F'
             ]
 
 SouthVowelMap = [
-                '\u098F\u02D8',
-                '\u0993\u02D8',
+                '\u0065\u0056',
+                '\u006F\u0056',
                 ]
 
 ModernVowelMap = [
-                 '\u098F\u02BC',
-                 '\u0986\u02BC',
+                 '\u0061\u0045\u0056',
+                 '\u0061\u004F\u0056',
                  ]
 
 SinhalaVowelMap = [
-                  '\u098F\u02C7'
+                  '\u0041\u0045\u0056'
                   ]
-    
-VowelSignMap =  [
-                '\u09BE',
-                '\u09BF',
-                '\u09C0',
-                '\u09C1',
-                '\u09C2',
-                '\u09C3',
-                '\u09C4',
-                '\u09E2',
-                '\u09E3',
-                '\u09C7',
-                '\u09C8',
-                '\u09CB',
-                '\u09CC',
-                ]
 
-SouthVowelSignMap = [
-                    '\u09C7\u02D8',
-                    '\u09CB\u02D8',
-                    ]
+VowelSignMap =  VowelMap[1:]
 
-ModernVowelSignMap =[
-                    '\u09C7\u02BC',
-                    '\u09BE\u02BC']
+SouthVowelSignMap = SouthVowelMap[:]
 
-SinhalaVowelSignMap = [
-                      '\u09C7\u02C7'
-                      ]
+ModernVowelSignMap = ModernVowelMap[:]
+
+SinhalaVowelSignMap = SinhalaVowelMap[:]
 
 AyogavahaMap = [
-               '\u0981',
-               '\u0982',
-               '\u0983'
+               '\u007A',
+               '\u004D',
+               '\u0048'
                ]
-    
+
 ViramaMap =  [
-             '\u09CD'
+             '\u00D7'
              ]
 
 ConsonantMap =  [
-                '\u0995',
-                '\u0996',
-                '\u0997',
-                '\u0998',
-                '\u0999',
-                
-                '\u099A',
-                '\u099B',
-                '\u099C',
-                '\u099D',
-                '\u099E',
-                
-                '\u099F',
-                '\u09A0',
-                '\u09A1',
-                '\u09A2',
-                '\u09A3',
-                
-                '\u09A4',
-                '\u09A5',
-                '\u09A6',
-                '\u09A7',
-                '\u09A8',
-                
-                '\u09AA',
-                '\u09AB',
-                '\u09AC',
-                '\u09AD',
-                '\u09AE',
-                
-                '\u09AF',
-                '\u09B0',
-                '\u09B2',
-                '\u09F1',
-                
-                '\u09B6',
-                '\u09B7',
-                '\u09B8',
-                '\u09B9'
+                '\u006B',
+                '\u004B',
+                '\u0067',
+                '\u0047',
+                '\u0066',
+
+                '\u0063',
+                '\u0043',
+                '\u006A',
+                '\u004A',
+                '\u0046',
+
+                '\u0074',
+                '\u0054',
+                '\u0064',
+                '\u0044',
+                '\u004E',
+
+                '\u0077',
+                '\u0057',
+                '\u0078',
+                '\u0058',
+                '\u006E',
+
+                '\u0070',
+                '\u0050',
+                '\u0062',
+                '\u0042',
+                '\u006D',
+
+                '\u0079',
+                '\u0072',
+                '\u006C',
+                '\u0076',
+
+                '\u0053',
+                '\u0052',
+                '\u0073',
+                '\u0068',
                 ]
 
 SouthConsonantMap = [
-                    '\u09B2\u09BC',
-                    '\u09B7\u09BC',
-                    '\u09B0\u09BC',
-                    '\u09A8\u09BC'
+                    '\u006C\u0059',
+                    '\u006C\u0059\u0059',
+                    '\u0072\u0059',
+                    '\u006E\u0059'
                     ]
 
 NuktaConsonantMap =  [
-                     '\u0995\u09BC',
-                     '\u0996\u09BC',
-                     '\u0997\u09BC',
-                     '\u099C\u09BC',
-                     '\u09DC',
-                     '\u09DD',
-                     '\u09AB\u09BC',
-                     '\u09DF'
+                     '\u006B\u0059',
+                     '\u004B\u0059',
+                     '\u0047\u0059',
+                     '\u007A\u0059',
+                     '\u0064\u0059',
+                     '\u0044\u0059',
+                     '\u0050\u0059',
+                     '\u0079\u0059'
                      ]
 
 SinhalaConsonantMap =[
-                     '\u0981\u02C6\u0997',
-                     '\u0981\u02C6\u099C',
-                     '\u0981\u02C6\u09A1',
-                     '\u0981\u02C6\u09A6',
-                     '\u0981\u02C6\u09AC',
+                     '\u006E\u0059\u0059\u0067',
+                     '\u006E\u0059\u0059\u006A',
+                     '\u006E\u0059\u0059\u0064',
+                     '\u006E\u0059\u0059\u0078',
+                     '\u006D\u0059\u0059\u0062',
                       ]
 
 NuktaMap = [
-           '\u09BC'
+           '\u0051'
            ]
-    
+
 OmMap = [
-        '\u0993\u0981'
+        '\u006F\u004D'
         ]
 
 SignMap =[
-         '\u09BD',
-         '\u0964',
-         '\u0965'
+         'Z',
+         '\u002E',
+         '\u002E\u002E'
          ]
 
-Aytham =[AyogavahaMap[2]+'\u02BC']
+Aytham =['\u006B\u0059\u0059']
 
 NumeralMap = [
-             '\u09E6',
-             '\u09E7',
-             '\u09E8',
-             '\u09E9',
-             '\u09EA',
-             '\u09EB',
-             '\u09EC',
-             '\u09ED',
-             '\u09EE',
-             '\u09EF'
+             '\u0030',
+             '\u0031',
+             '\u0032',
+             '\u0033',
+             '\u0034',
+             '\u0035',
+             '\u0036',
+             '\u0037',
+             '\u0038',
+             '\u0039',
              ]
+
+from ... import GeneralMap as GM
+
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/Bengali.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/Itrans.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,170 +1,155 @@
 # -*- coding: utf-8 -*-
 
-# Script Mapping for Devanagari
+# Script Mapping for ISO
 
 VowelMap =  [
-            '\u0985',
-            '\u0986',
-            '\u0987',
-            '\u0988',
-            '\u0989',
-            '\u098A',
-            '\u098B',
-            '\u09E0',
-            '\u098C',
-            '\u09E1',
-            '\u098F',
-            '\u0990',
-            '\u0993',
-            '\u0994',
+            '\u0061',
+            '\u0041',
+            '\u0069',
+            '\u0049',
+            '\u0075',
+            '\u0055',
+            '\u0052\u005E\u0069',
+            '\u0052\u005E\u0049',
+            '\u004C\u005E\u0069',
+            '\u004C\u005E\u0049',
+            '\u0065',
+            '\u0061\u0069',
+            '\u006F',
+            '\u0061\u0075'
             ]
 
 SouthVowelMap = [
-                '\u098F\u02D8',
-                '\u0993\u02D8',
+                '^e',
+                '^o',
                 ]
 
 ModernVowelMap = [
-                 '\u098F\u02BC',
-                 '\u0986\u02BC',
+                 'e.c',
+                 'A.c',
                  ]
 
 SinhalaVowelMap = [
-                  '\u098F\u02C7'
+                  '\u0061\u002E\u0043'
                   ]
 
-VowelSignMap =  [
-                '\u09BE',
-                '\u09BF',
-                '\u09C0',
-                '\u09C1',
-                '\u09C2',
-                '\u09C3',
-                '\u09C4',
-                '\u09E2',
-                '\u09E3',
-                '\u09C7',
-                '\u09C8',
-                '\u09CB',
-                '\u09CC',
-                ]
+VowelSignMap =  VowelMap[1:]
 
-SouthVowelSignMap = [
-                    '\u09C7\u02D8',
-                    '\u09CB\u02D8',
-                    ]
+SouthVowelSignMap = SouthVowelMap[:]
 
-ModernVowelSignMap =[
-                    '\u09C7\u02BC',
-                    '\u09BE\u02BC']
+ModernVowelSignMap = ModernVowelMap[:]
 
-SinhalaVowelSignMap = [
-                      '\u09C7\u02C7'
-                      ]
+SinhalaVowelSignMap = SinhalaVowelMap[:]
 
 AyogavahaMap = [
-               '\u0981',
-               '\u0982',
-               '\u0983'
+               '\u002E\u004E',
+               '\u004D',
+               '\u0048'
                ]
 
 ViramaMap =  [
-             '\u09CD'
+             '\u00D7'
              ]
 
 ConsonantMap =  [
-                '\u0995',
-                '\u0996',
-                '\u0997',
-                '\u0998',
-                '\u0999',
-
-                '\u099A',
-                '\u099B',
-                '\u099C',
-                '\u099D',
-                '\u099E',
-
-                '\u099F',
-                '\u09A0',
-                '\u09A1',
-                '\u09A2',
-                '\u09A3',
-
-                '\u09A4',
-                '\u09A5',
-                '\u09A6',
-                '\u09A7',
-                '\u09A8',
-
-                '\u09AA',
-                '\u09AB',
-                '\u09AC',
-                '\u09AD',
-                '\u09AE',
-
-                '\u09AF',
-                '\u09B0',
-                '\u09B2',
-                'ভ়',
-
-                '\u09B6',
-                '\u09B7',
-                '\u09B8',
-                '\u09B9'
+                '\u006B',
+                '\u006B\u0068',
+                '\u0067',
+                '\u0067\u0068',
+                '\u007E\u004E',
+
+                '\u0063\u0068',
+                '\u0043\u0068',
+                '\u006A',
+                '\u006A\u0068',
+                '\u007E\u006E',
+
+                '\u0054',
+                '\u0054\u0068',
+                '\u0044',
+                '\u0044\u0068',
+                '\u004E',
+
+                '\u0074',
+                '\u0074\u0068',
+                '\u0064',
+                '\u0064\u0068',
+                '\u006E',
+
+                '\u0070',
+                '\u0070\u0068',
+                '\u0062',
+                '\u0062\u0068',
+                '\u006D',
+
+                '\u0079',
+                '\u0072',
+                '\u006C',
+                '\u0076',
+
+                '\u0073\u0068',
+                '\u0053\u0068',
+                '\u0073',
+                '\u0068',
                 ]
 
 SouthConsonantMap = [
-                    '\u09B2\u09BC',
-                    '\u09B7\u09BC',
-                    '\u09B0\u09BC',
-                    '\u09A8\u09BC'
+                    'L',
+                    'zh',
+                    'R',
+                    '\u005E\u006E'
                     ]
 
 NuktaConsonantMap =  [
-                     '\u0995\u09BC',
-                     '\u0996\u09BC',
-                     '\u0997\u09BC',
-                     '\u099C\u09BC',
-                     '\u09DC',
-                     '\u09DD',
-                     '\u09AB\u09BC',
-                     '\u09DF'
+                     '\u0071',
+                     '\u004B',
+                     '\u0047',
+                     '\u007A',
+                     '\u002E\u0044',
+                     '\u002E\u0044\u0068',
+                     '\u0066',
+                     '\u0059'
                      ]
 
 SinhalaConsonantMap =[
-                     '\u0981\u02C6\u0997',
-                     '\u0981\u02C6\u099C',
-                     '\u0981\u02C6\u09A1',
-                     '\u0981\u02C6\u09A6',
-                     '\u0981\u02C6\u09AC',
+                     '\u006E\u002A\u0067',
+                     '\u006E\u002A\u006A',
+                     '\u006E\u002A\u0044',
+                     '\u006E\u002A\u0064',
+                     '\u006D\u002A\u0062',
                       ]
 
 NuktaMap = [
-           '\u09BC'
+           '\u0051'
            ]
 
 OmMap = [
-        '\u0993\u0981'
+        'oM'
         ]
 
 SignMap =[
-         '\u09BD',
-         '\u0964',
-         '\u0965'
+         '\u002E\u0061',
+         '\u002E',
+         '\u002E\u002E'
          ]
 
-Aytham =[AyogavahaMap[2]+'\u02BC']
+Aytham =['\u004B\u005E']
 
 NumeralMap = [
-             '\u09E6',
-             '\u09E7',
-             '\u09E8',
-             '\u09E9',
-             '\u09EA',
-             '\u09EB',
-             '\u09EC',
-             '\u09ED',
-             '\u09EE',
-             '\u09EF'
+             '\u0030',
+             '\u0031',
+             '\u0032',
+             '\u0033',
+             '\u0034',
+             '\u0035',
+             '\u0036',
+             '\u0037',
+             '\u0038',
+             '\u0039',
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/Bhaiksuki.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Bhaiksuki.py`

 * *Files 15% similar despite different names*

```diff
@@ -165,7 +165,13 @@
              '\U00011C54',
              '\U00011C55',
              '\U00011C56',
              '\U00011C57',
              '\U00011C58',
              '\U00011C59'
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/Chakma.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Chakma.py`

 * *Files 11% similar despite different names*

```diff
@@ -166,7 +166,13 @@
              '\U0001113A',
              '\U0001113B',
              '\U0001113C',
              '\U0001113D',
              '\U0001113E',
              '\U0001113F'
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/Devanagari.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Devanagari.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,7 +164,14 @@
              '\u096A',
              '\u096B',
              '\u096C',
              '\u096D',
              '\u096E',
              '\u096F'
              ]
+
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/Dogra.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Grantha.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,170 +1,176 @@
 # -*- coding: utf-8 -*-
 
 # Script Mapping for Devanagari
 
 VowelMap =  [
-            '\U00011800',
-            '\U00011801',
-            '\U00011802',
-            '\U00011803',
-            '\U00011804',
-            '\U00011805',
-            '\U00011824\U0001182D\u02BD',
-            '\U00011824\U0001182E\u02BD',
-            '\U00011825\U0001182D\u02BD',
-            '\U00011825\U0001182E\u02BD',
-            '\U00011806',
-            '\U00011807',
-            '\U00011808',
-            '\U00011809',
+            '\U00011305',
+            '\U00011306',
+            '\U00011307',
+            '\U00011308',
+            '\U00011309',
+            '\U0001130A',
+            '\U0001130B',
+            '\U00011360',
+            '\U0001130C',
+            '\U00011361',
+            '\U0001130F',
+            '\U00011310',
+            '\U00011313',
+            '\U00011314',
             ]
 
 SouthVowelMap = [
-                '\U00011806\u02BD',
-                '\U00011808\u02BD',
+                '\U0001130F\U00011300',
+                '\U00011313\U00011300',
                 ]
 
 ModernVowelMap = [
-                 '\U00011806\u02BD',
-                 '\U00011801\u02BD',
+                 '\U0001130F\u02BD',
+                 '\U00011306\u02BD',
                  ]
 
 SinhalaVowelMap = [
-                  '\U00011806\u02BD'
+                  '\U0001130F\u02BD'
                   ]
 
 VowelSignMap =  [
-                '\U0001182C',
-                '\U0001182D',
-                '\U0001182E',
-                '\U0001182F',
-                '\U00011830',
-                '\U00011831',
-                '\U00011832',
-                '\U00011839\U00011825\U0001182D\u02BD',
-                '\U00011839\U00011825\U0001182E\u02BD',
-                '\U00011833',
-                '\U00011834',
-                '\U00011835',
-                '\U00011836',
+                '\U0001133E',
+                '\U0001133F',
+                '\U00011340',
+                '\U00011341',
+                '\U00011342',
+                '\U00011343',
+                '\U00011344',
+                '\U00011362',
+                '\U00011363',
+                '\U00011347',
+                '\U00011348',
+                '\U0001134B',
+                '\U00011357',
                 ]
 
 SouthVowelSignMap = [
-                    '\U00011833\u02BD',
-                    '\U00011835\u02BD',
+                    '\U00011347\U00011300',
+                    '\U0001134B\U00011300',
                     ]
 
 ModernVowelSignMap =[
-                    '\U00011833\u02BD',
-                    '\U0001182C\u02BD']
+                    '\U00011347\u02BD',
+                    '\U0001133E\u02BD']
 
 SinhalaVowelSignMap = [
-                      '\U00011833\u02BD'
+                      '\U00011347\u02BD'
                       ]
 
 AyogavahaMap = [
-               '\U00011837\u02BD',
-               '\U00011837',
-               '\U00011838'
+               '\U00011301',
+               '\U00011302',
+               '\U00011303',
                ]
 
 ViramaMap =  [
-             '\U00011839'
+               '\U0001134D',
              ]
 
 ConsonantMap =  [
-                '\U0001180A',
-                '\U0001180B',
-                '\U0001180C',
-                '\U0001180D',
-                '\U0001180E',
-
-                '\U0001180F',
-                '\U00011810',
-                '\U00011811',
-                '\U00011812',
-                '\U00011813',
-
-                '\U00011814',
-                '\U00011815',
-                '\U00011816',
-                '\U00011817',
-                '\U00011818',
-
-                '\U00011819',
-                '\U0001181A',
-                '\U0001181B',
-                '\U0001181C',
-                '\U0001181D',
-
-                '\U0001181E',
-                '\U0001181F',
-                '\U00011820',
-                '\U00011821',
-                '\U00011822',
-
-                '\U00011823',
-                '\U00011824',
-                '\U00011825',
-                '\U00011826',
-
-                '\U00011827',
-                '\U00011828',
-                '\U00011829',
-                '\U0001182A'
+                '\U00011315',
+                '\U00011316',
+                '\U00011317',
+                '\U00011318',
+                '\U00011319',
+
+                '\U0001131A',
+                '\U0001131B',
+                '\U0001131C',
+                '\U0001131D',
+                '\U0001131E',
+
+                '\U0001131F',
+                '\U00011320',
+                '\U00011321',
+                '\U00011322',
+                '\U00011323',
+
+                '\U00011324',
+                '\U00011325',
+                '\U00011326',
+                '\U00011327',
+                '\U00011328',
+
+                '\U0001132A',
+                '\U0001132B',
+                '\U0001132C',
+                '\U0001132D',
+                '\U0001132E',
+
+                '\U0001132F',
+                '\U00011330',
+                '\U00011332',
+                '\U00011335',
+
+                '\U00011336',
+                '\U00011337',
+                '\U00011338',
+                '\U00011339'
                 ]
 
 SouthConsonantMap = [
-                    '\U00011825\U0001183A',
-                    '\U00011828\U0001183A',
-                    '\U00011824\U0001183A',
-                    '\U0001181D\U0001183A'
+                    '\U00011333',
+                    '\U00011333\U0001133C',
+                    '\U00011330\U0001133C',
+                    '\U00011328\U0001133C'
                     ]
 
 NuktaConsonantMap =  [
-                     '\U0001180A\U0001183A',
-                     '\U0001180B\U0001183A',
-                     '\U0001180C\U0001183A',
-                     '\U00011811\U0001183A',
-                     '\U0001182B',
-                     '\U00011817\U0001183A',
-                     '\U0001181F\U0001183A',
-                     '\U00011823\U0001183A'
+                     '\U00011315\U0001133C',
+                     '\U00011316\U0001133C',
+                     '\U00011317\U0001133C',
+                     '\U0001131C\U0001133C',
+                     '\U00011321\U0001133C',
+                     '\U00011322\U0001133C',
+                     '\U0001132B\U0001133C',
+                     '\U0001132F\U0001133C'
                      ]
 
 SinhalaConsonantMap =[
-                     '\U00011837\U0001180C\u02BD',
-                     '\U00011837\U00011811\u02BD',
-                     '\U00011837\U00011816\u02BD',
-                     '\U00011837\U0001181B\u02BD',
-                     '\U00011837\U00011820\u02BD',
+                     '\U00011301\u02BD\U00011317',
+                     '\U00011301\u02BD\U0001131C',
+                     '\U00011301\u02BD\U00011321',
+                     '\U00011301\u02BD\U00011326',
+                     '\U00011301\u02BD\U0001132C',
                       ]
 
 NuktaMap = [
-           '\U0001183A'
+           '\U0001133C'
            ]
 
 OmMap = [
-        '\U00011808\U00011837'
+        '\U00011350'
         ]
 
 SignMap =[
-         '\u093D',
+         '\U0001133D',
          '\u0964',
          '\u0965'
          ]
 
 Aytham =[AyogavahaMap[2]+'\u02BD']
 
 NumeralMap = [
-             '\u0966',
-             '\u0967',
-             '\u0968',
-             '\u0969',
-             '\u096A',
-             '\u096B',
-             '\u096C',
-             '\u096D',
-             '\u096E',
-             '\u096F'
+             '\u0BE6',
+             '\u0BE7',
+             '\u0BE8',
+             '\u0BE9',
+             '\u0BEA',
+             '\u0BEB',
+             '\u0BEC',
+             '\u0BED',
+             '\u0BEE',
+             '\u0BEF'
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/Grantha.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Kawi.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,170 +1,177 @@
 # -*- coding: utf-8 -*-
 
 # Script Mapping for Devanagari
 
 VowelMap =  [
-            '\U00011305',
-            '\U00011306',
-            '\U00011307',
-            '\U00011308',
-            '\U00011309',
-            '\U0001130A',
-            '\U0001130B',
-            '\U00011360',
-            '\U0001130C',
-            '\U00011361',
-            '\U0001130F',
-            '\U00011310',
-            '\U00011313',
-            '\U00011314',
+            '\U00011F04',
+            '\U00011F05',
+            '\U00011F06',
+            '\U00011F07',
+            '\U00011F08',
+            '\U00011F09',
+            '\U00011F0A',
+            '\U00011F0B',
+            '\U00011F0C',
+            '\U00011F0D',
+            '\U00011F0E',
+            '\U00011F0F',
+            '\U00011F10',
+            '\U00011F10\U00011F34',
             ]
 
 SouthVowelMap = [
-                '\U0001130F\U00011300',
-                '\U00011313\U00011300',
+                '\U00011F0E\u02BD',
+                '\U00011F10\u02BD',
                 ]
 
 ModernVowelMap = [
-                 '\U0001130F\u02BD',
-                 '\U00011306\u02BD',
+                 '\U00011F04\U00011F40',
+                 '\U00011F05\u02BD',
                  ]
 
 SinhalaVowelMap = [
-                  '\U0001130F\u02BD'
+                  '\U00011F04\U00011F40\U00011F34'
                   ]
 
 VowelSignMap =  [
-                '\U0001133E',
-                '\U0001133F',
-                '\U00011340',
-                '\U00011341',
-                '\U00011342',
-                '\U00011343',
-                '\U00011344',
-                '\U00011362',
-                '\U00011363',
-                '\U00011347',
-                '\U00011348',
-                '\U0001134B',
-                '\U00011357',
+                '\U00011F34',
+                '\U00011F36',
+                '\U00011F37',
+                '\U00011F38',
+                '\U00011F39',
+                '\U00011F3A',
+                '\U00011F42\U00011F0B',
+                '\U00011F42\U00011F0C',
+                '\U00011F42\U00011F0D',
+                '\U00011F3E',
+                '\U00011F3F',
+                '\U00011F3E\U00011F34',
+                '\U00011F3F\U00011F34',
                 ]
 
 SouthVowelSignMap = [
-                    '\U00011347\U00011300',
-                    '\U0001134B\U00011300',
+                    '\U00011F3E\u02BD',
+                    '\U00011F3E\U00011F34\u02BD',
                     ]
 
 ModernVowelSignMap =[
-                    '\U00011347\u02BD',
-                    '\U0001133E\u02BD']
+                    '\U00011F40',
+                    '\U00011F34\u02BD']
 
 SinhalaVowelSignMap = [
-                      '\U00011347\u02BD'
+                      '\U00011F40\U00011F34'
                       ]
 
 AyogavahaMap = [
-               '\U00011301',
-               '\U00011302',
-               '\U00011303',
+               '\U00011F00',
+               '\U00011F01',
+               '\U00011F03'
                ]
 
 ViramaMap =  [
-               '\U0001134D',
+             '\U00011F41'
              ]
 
 ConsonantMap =  [
-                '\U00011315',
-                '\U00011316',
-                '\U00011317',
-                '\U00011318',
-                '\U00011319',
-
-                '\U0001131A',
-                '\U0001131B',
-                '\U0001131C',
-                '\U0001131D',
-                '\U0001131E',
-
-                '\U0001131F',
-                '\U00011320',
-                '\U00011321',
-                '\U00011322',
-                '\U00011323',
-
-                '\U00011324',
-                '\U00011325',
-                '\U00011326',
-                '\U00011327',
-                '\U00011328',
-
-                '\U0001132A',
-                '\U0001132B',
-                '\U0001132C',
-                '\U0001132D',
-                '\U0001132E',
-
-                '\U0001132F',
-                '\U00011330',
-                '\U00011332',
-                '\U00011335',
-
-                '\U00011336',
-                '\U00011337',
-                '\U00011338',
-                '\U00011339'
+                '\U00011F12',
+                '\U00011F13',
+                '\U00011F14',
+                '\U00011F15',
+                '\U00011F16',
+
+                '\U00011F17',
+                '\U00011F18',
+                '\U00011F19',
+                '\U00011F1A',
+                '\U00011F1B',
+
+                '\U00011F1C',
+                '\U00011F1D',
+                '\U00011F1E',
+                '\U00011F1F',
+                '\U00011F20',
+
+                '\U00011F21',
+                '\U00011F22',
+                '\U00011F23',
+                '\U00011F24',
+                '\U00011F25',
+
+                '\U00011F26',
+                '\U00011F27',
+                '\U00011F28',
+                '\U00011F29',
+                '\U00011F2A',
+
+                '\U00011F2B',
+                '\U00011F2C',
+                '\U00011F2D',
+                '\U00011F2E',
+
+                '\U00011F2F',
+                '\U00011F30',
+                '\U00011F31',
+                '\U00011F32'
                 ]
 
 SouthConsonantMap = [
-                    '\U00011333',
-                    '\U00011333\U0001133C',
-                    '\U00011330\U0001133C',
-                    '\U00011328\U0001133C'
+                    '\U00011F2D\u02BD',
+                    '\U00011F2D\u02BD',
+                    '\U00011F2C\u02BD',
+                    '\U00011F25\u02BD'
                     ]
 
 NuktaConsonantMap =  [
-                     '\U00011315\U0001133C',
-                     '\U00011316\U0001133C',
-                     '\U00011317\U0001133C',
-                     '\U0001131C\U0001133C',
-                     '\U00011321\U0001133C',
-                     '\U00011322\U0001133C',
-                     '\U0001132B\U0001133C',
-                     '\U0001132F\U0001133C'
+                     '\U00011F12\u02BD',
+                     '\U00011F13\u02BD',
+                     '\U00011F14\u02BD',
+                     '\U00011F19\u02BD',
+                     '\U00011F1E\u02BD',
+                     '\U00011F1E\u02BD',
+                     '\U00011F27\u02BD',
+                     '\U00011F2B\u02BD'
                      ]
 
 SinhalaConsonantMap =[
-                     '\U00011301\u02BD\U00011317',
-                     '\U00011301\u02BD\U0001131C',
-                     '\U00011301\u02BD\U00011321',
-                     '\U00011301\u02BD\U00011326',
-                     '\U00011301\u02BD\U0001132C',
+                     '\U00011F00\U00011F14\u02BD',
+                     '\U00011F00\U00011F19\u02BD',
+                     '\U00011F00\U00011F1E\u02BD',
+                     '\U00011F00\U00011F23\u02BD',
+                     '\U00011F00\U00011F28\u02BD',
                       ]
 
 NuktaMap = [
-           '\U0001133C'
+           '\u02BD\u02BD\u02BD\u02BD'
            ]
 
 OmMap = [
-        '\U00011350'
+        '\U00011F10\U00011F00'
         ]
 
 SignMap =[
-         '\U0001133D',
-         '\u0964',
-         '\u0965'
+         '\u02BD\u02BD\u02BD',
+         '\U00011F43',
+         '\U00011F44'
          ]
 
 Aytham =[AyogavahaMap[2]+'\u02BD']
 
+
 NumeralMap = [
-             '\u0BE6',
-             '\u0BE7',
-             '\u0BE8',
-             '\u0BE9',
-             '\u0BEA',
-             '\u0BEB',
-             '\u0BEC',
-             '\u0BED',
-             '\u0BEE',
-             '\u0BEF'
+             '\U00011F50',
+             '\U00011F51',
+             '\U00011F52',
+             '\U00011F53',
+             '\U00011F54',
+             '\U00011F55',
+             '\U00011F56',
+             '\U00011F57',
+             '\U00011F58',
+             '\U00011F59',
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/GranthaGrantamil.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/GranthaGrantamil.py`

 * *Files 20% similar despite different names*

```diff
@@ -164,7 +164,13 @@
              u'\u09EA',
              u'\u09EB',
              u'\u09EC',
              u'\u09ED',
              u'\u09EE',
              u'\u09EF'
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/GranthaPandya.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/GranthaPandya.py`

 * *Files 9% similar despite different names*

```diff
@@ -165,7 +165,13 @@
              '4',
              '5',
              '6',
              '7',
              '8',
              '9'
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/Gujarati.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Gujarati.py`

 * *Files 19% similar despite different names*

```diff
@@ -28,15 +28,15 @@
                  '\u0A8D',
                  '\u0A91',
                  ]
 
 SinhalaVowelMap = [
                   '\u0A8D\u02C7'
                   ]
-    
+
 VowelSignMap =  [
                 '\u0ABE',
                 '\u0ABF',
                 '\u0AC0',
                 '\u0AC1',
                 '\u0AC2',
                 '\u0AC3',
@@ -63,55 +63,55 @@
                       ]
 
 AyogavahaMap = [
                '\u0A81',
                '\u0A82',
                '\u0A83'
                ]
-    
+
 ViramaMap =  [
              '\u0ACD'
              ]
 
 ConsonantMap =  [
                 '\u0A95',
                 '\u0A96',
                 '\u0A97',
                 '\u0A98',
                 '\u0A99',
-                
+
                 '\u0A9A',
                 '\u0A9B',
                 '\u0A9C',
                 '\u0A9D',
                 '\u0A9E',
-                
+
                 '\u0A9F',
                 '\u0AA0',
                 '\u0AA1',
                 '\u0AA2',
                 '\u0AA3',
-                
+
                 '\u0AA4',
                 '\u0AA5',
                 '\u0AA6',
                 '\u0AA7',
                 '\u0AA8',
-                
+
                 '\u0AAA',
                 '\u0AAB',
                 '\u0AAC',
                 '\u0AAD',
                 '\u0AAE',
-                
+
                 '\u0AAF',
                 '\u0AB0',
                 '\u0AB2',
                 '\u0AB5',
-                
+
                 '\u0AB6',
                 '\u0AB7',
                 '\u0AB8',
                 '\u0AB9'
                 ]
 
 SouthConsonantMap = [
@@ -135,20 +135,20 @@
 
 SinhalaConsonantMap =[
                      '\u0A81\u02C6\u0A97',
                      '\u0A81\u02C6\u0A9C',
                      '\u0A81\u02C6\u0AA1',
                      '\u0A81\u02C6\u0AA6',
                      '\u0A81\u02C6\u0AAC',
-                      ] 
+                      ]
 
 NuktaMap = [
            '\u0ABC'
            ]
-    
+
 OmMap = [
         '\u0AD0'
         ]
 
 SignMap =[
          '\u0ABD',
          '\u0964',
@@ -165,7 +165,13 @@
              '\u0AEA',
              '\u0AEB',
              '\u0AEC',
              '\u0AED',
              '\u0AEE',
              '\u0AEF'
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/GunjalaGondi.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/GunjalaGondi.py`

 * *Files 14% similar despite different names*

```diff
@@ -164,7 +164,13 @@
              '\U00011DA4',
              '\U00011DA5',
              '\U00011DA6',
              '\U00011DA7',
              '\U00011DA8',
              '\U00011DA9',
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/Gurmukhi.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Oriya.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,171 +1,176 @@
 # -*- coding: utf-8 -*-
 
 # Script Mapping for Devanagari
 
 VowelMap =  [
-            '\u0A05',
-            '\u0A06',
-            '\u0A07',
-            '\u0A08',
-            '\u0A09',
-            '\u0A0A',
-            '\u0A30\u0A41\u02BC',
-            '\u0A30\u0A42\u02BC',
-            '\u0A32\u0A41\u02BC',
-            '\u0A32\u0A42\u02BC',
-            '\u0A0F',
-            '\u0A10',
-            '\u0A13',
-            '\u0A14',
+            '\u0B05',
+            '\u0B06',
+            '\u0B07',
+            '\u0B08',
+            '\u0B09',
+            '\u0B0A',
+            '\u0B0B',
+            '\u0B60',
+            '\u0B0C',
+            '\u0B61',
+            '\u0B0F',
+            '\u0B10',
+            '\u0B13',
+            '\u0B14',
             ]
 
 SouthVowelMap = [
-                '\u0A0F\u02D8',
-                '\u0A13\u02D8',
+                '\u0B0F\u02D8',
+                '\u0B13\u02D8',
                 ]
 
 ModernVowelMap = [
-                 '\u0A0F\u02BC',
-                 '\u0A06\u02BC',
+                 '\u0B0F\u02BC',
+                 '\u0B06\u02BC',
                  ]
 
 SinhalaVowelMap = [
-                  '\u0A0F\u02C7'
+                  '\u0B0F\u02C7'
                   ]
-    
+
 VowelSignMap =  [
-                '\u0A3E',
-                '\u0A3F',
-                '\u0A40',
-                '\u0A41',
-                '\u0A42',
-                '\u0A4D\u0A30\u0A41\u02BC',
-                '\u0A4D\u0A30\u0A42\u02BC',
-                '\u0A4D\u0A32\u0A41\u02BC',
-                '\u0A4D\u0A32\u0A42\u02BC',
-                '\u0A47',
-                '\u0A48',
-                '\u0A4B',
-                '\u0A4C',
+                '\u0B3E',
+                '\u0B3F',
+                '\u0B40',
+                '\u0B41',
+                '\u0B42',
+                '\u0B43',
+                '\u0B44',
+                '\u0B62',
+                '\u0B63',
+                '\u0B47',
+                '\u0B48',
+                '\u0B4B',
+                '\u0B4C',
                 ]
 
 SouthVowelSignMap = [
-                    '\u0A47\u02D8',
-                    '\u0A4B\u02D8',
+                    '\u0B47\u02D8',
+                    '\u0B4B\u02D8',
                     ]
 
 ModernVowelSignMap =[
-                    '\u0A47\u02BC',
-                    '\u0A3E\u02BC']
+                    '\u0B47\u02BC',
+                    '\u0B3E\u02BC']
 
 SinhalaVowelSignMap = [
-                      '\u0A47\u02C7'
+                      '\u0B47\u02C7'
                       ]
 
 AyogavahaMap = [
-               '\u0A01',
-               '\u0A02',
-               '\u0A03'
+               '\u0B01',
+               '\u0B02',
+               '\u0B03'
                ]
-    
+
 ViramaMap =  [
-             '\u0A4D'
+             '\u0B4D'
              ]
 
 ConsonantMap =  [
-                '\u0A15',
-                '\u0A16',
-                '\u0A17',
-                '\u0A18',
-                '\u0A19',
-                
-                '\u0A1A',
-                '\u0A1B',
-                '\u0A1C',
-                '\u0A1D',
-                '\u0A1E',
-                
-                '\u0A1F',
-                '\u0A20',
-                '\u0A21',
-                '\u0A22',
-                '\u0A23',
-                
-                '\u0A24',
-                '\u0A25',
-                '\u0A26',
-                '\u0A27',
-                '\u0A28',
-                
-                '\u0A2A',
-                '\u0A2B',
-                '\u0A2C',
-                '\u0A2D',
-                '\u0A2E',
-                
-                '\u0A2F',
-                '\u0A30',
-                '\u0A32',
-                '\u0A35',
-                
-                '\u0A36',
-                '\u0A36\u0A3C',
-                '\u0A38',
-                '\u0A39'
+                '\u0B15',
+                '\u0B16',
+                '\u0B17',
+                '\u0B18',
+                '\u0B19',
+
+                '\u0B1A',
+                '\u0B1B',
+                '\u0B1C',
+                '\u0B1D',
+                '\u0B1E',
+
+                '\u0B1F',
+                '\u0B20',
+                '\u0B21',
+                '\u0B22',
+                '\u0B23',
+
+                '\u0B24',
+                '\u0B25',
+                '\u0B26',
+                '\u0B27',
+                '\u0B28',
+
+                '\u0B2A',
+                '\u0B2B',
+                '\u0B2C',
+                '\u0B2D',
+                '\u0B2E',
+
+                '\u0B2F',
+                '\u0B30',
+                '\u0B32',
+                '\u0B71',
+
+                '\u0B36',
+                '\u0B37',
+                '\u0B38',
+                '\u0B39'
                 ]
 
 SouthConsonantMap = [
-                    '\u0A33',
-                    '\u0A33\u0A3C',
-                    '\u0A30\u0A3C',
-                    '\u0A28\u0A3C'
+                    '\u0B33',
+                    '\u0B33\u0B3C',
+                    '\u0B30\u0B3C',
+                    '\u0B28\u0B3C'
                     ]
 
 NuktaConsonantMap =  [
-                     '\u0A15\u0A3C',
-                     '\u0A59',
-                     '\u0A5A',
-                     '\u0A5B',
-                     '\u0A5C',
-                     '\u0A22\u0A3C',
-                     '\u0A5E',
-                     '\u0A2F\u0A3C'
+                     '\u0B15\u0B3C',
+                     '\u0B16\u0B3C',
+                     '\u0B17\u0B3C',
+                     '\u0B1C\u0B3C',
+                     '\u0B5C',
+                     '\u0B5D',
+                     '\u0B2B\u0B3C',
+                     '\u0B5F'
                      ]
 
 SinhalaConsonantMap =[
-                     '\u0A01\u02C6\u0A17',
-                     '\u0A01\u02C6\u0A1C',
-                     '\u0A01\u02C6\u0A21',
-                     '\u0A01\u02C6\u0A26',
-                     '\u0A01\u02C6\u0A2C',
-                      ] 
+                     '\u0B01\u02C6\u0B17',
+                     '\u0B01\u02C6\u0B1C',
+                     '\u0B01\u02C6\u0B21',
+                     '\u0B01\u02C6\u0B26',
+                     '\u0B01\u02C6\u0B2C',
+                      ]
 
 NuktaMap = [
-           '\u0A3C'
+           '\u0B3C'
            ]
-    
+
 OmMap = [
-        '\u0A74'
+        '\u0B13\u0B01'
         ]
 
 SignMap =[
-         '\u0028\u0A05\u0029',
+         '\u0B3D',
          '\u0964',
          '\u0965'
          ]
 
 Aytham =[AyogavahaMap[2]+'\u02BC']
 
-
 NumeralMap = [
-             '\u0A66',
-             '\u0A67',
-             '\u0A68',
-             '\u0A69',
-             '\u0A6A',
-             '\u0A6B',
-             '\u0A6C',
-             '\u0A6D',
-             '\u0A6E',
-             '\u0A6F'
+             '\u0B66',
+             '\u0B67',
+             '\u0B68',
+             '\u0B69',
+             '\u0B6A',
+             '\u0B6B',
+             '\u0B6C',
+             '\u0B6D',
+             '\u0B6E',
+             '\u0B6F'
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/Kaithi.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Kaithi.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 VowelSignMap =  [
                 '\U000110B0',
                 '\U000110B1',
                 '\U000110B2',
                 '\U000110B3',
                 '\U000110B4',
-                '𑂹𑂩𑂱\u02BD',
+                '\U000110C2',
                 '𑂹𑂩𑂲\u02BD',
                 '𑂹𑂪𑂱\u02BD',
                 '𑂹𑂪𑂲\u02BD',
                 '\U000110B5',
                 '\U000110B6',
                 '\U000110B7',
                 '\U000110B8',
@@ -164,7 +164,13 @@
              '\u096A',
              '\u096B',
              '\u096C',
              '\u096D',
              '\u096E',
              '\u096F'
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/Kannada.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Kannada.py`

 * *Files 14% similar despite different names*

```diff
@@ -164,7 +164,13 @@
              '\u0CEA',
              '\u0CEB',
              '\u0CEC',
              '\u0CED',
              '\u0CEE',
              '\u0CEF'
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/Kharoshthi.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/RomanSemitic.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,171 +1,171 @@
 # -*- coding: utf-8 -*-
 
-# Script Mapping for Devanagari
+# Script Mapping for ISO
 
 VowelMap =  [
-            '𐨀',
-            '𐨀𐨌',
-            '𐨀𐨁',
-            '𐨀𐨁𐨌',
-            '𐨀𐨂',
-            '𐨀𐨂𐨌',
-            '𐨀𐨃',
-            '𐨀𐨃𐨌',
-            '𐨫𐨂\u02BD',
-            '𐨫𐨂𐨌\u02BD',
-            '𐨀𐨅',
-            '𐨀𐨅𐨌',
-            '𐨀𐨆',
-            '𐨀𐨆𐨌',
+            'â',
+            'ā̂', # A
+            'î', #i
+            'ī̂', #I
+            'û', # u
+            'ū̂', # U
+            'ru\u02BD',
+            'rū\u02BD',
+            'lu\u02BD',
+            'lū\u02BD',
+            'ē̂', #e
+            'âŷ', #ai
+            'ō̂', #o
+            'âŵ' #au
             ]
 
 SouthVowelMap = [
-                '𐨀𐨅\u02BD',
-                '𐨀𐨆\u02BD',
+                'ê',
+                'ô'
                 ]
 
 ModernVowelMap = [
-                 '𐨀𐨅\u02BD',
-                 '𐨀𐨌\u02BD',
+                 'ē̂\u02BD',
+                 'ā̂\u02BD'
                  ]
 
 SinhalaVowelMap = [
-                  '𐨀𐨅\u02BD'
+                  'ê\u02BD'
                   ]
 
 VowelSignMap =  [
-                '𐨌',
-                '𐨁',
-                '𐨁𐨌',
-                '𐨂',
-                '𐨂𐨌',
-                '𐨃',
-                '𐨃𐨌',
-                '𐨿𐨫𐨂\u02BD',
-                '𐨿𐨫𐨂𐨌\u02BD',
-                '𐨅',
-                '𐨅𐨌',
-                '𐨆',
-                '𐨆𐨌',
-                ]
+            'ā', # A
+            'i', #i
+            'ī', #I
+            'u', # u
+            'ū', # U
+            '\u033Dru\u02BD',
+            '\u033Drū\u02BD',
+            '\u033Dru\u02BD',
+            '\u033Drū\u02BD',
+            'ē', #e
+            'aŷ', #ai
+            'ō', #o
+            'aŵ' #au
+]
 
-SouthVowelSignMap = [
-                    '𐨅\u02BD',
-                    '𐨆\u02BD',
-                    ]
+SouthVowelSignMap = ['e','o']
 
-ModernVowelSignMap =[
-                    '𐨅\u02BD',
-                    '𐨌\u02BD']
+ModernVowelSignMap = ['e\u02BD','ā\u02BD']
 
 SinhalaVowelSignMap = [
-                      '𐨅\u02BD'
-                      ]
+                  'ē\u02BD'
+                  ]
 
 AyogavahaMap = [
-               '𐨎\u02BD',
-               '𐨎',
-               '𐨏'
+               'ₘ',
+               'ₘ', ## Check nasalization
+               'h\u033D\u02BD'
                ]
 
 ViramaMap =  [
-             '𐨿'
+             '\u033D'
              ]
 
 ConsonantMap =  [
-                '𐨐',
-                '𐨑',
-                '𐨒',
-                '𐨓',
-                '𐨣\u02BD',
-
-                '𐨕',
-                '𐨖',
-                '𐨗',
-                '𐨗\u02BD',
-                '𐨙',
-
-                '𐨚',
-                '𐨛',
-                '𐨜',
-                '𐨝',
-                '𐨞',
-
-                '𐨟',
-                '𐨠',
-                '𐨡',
-                '𐨢',
-                '𐨣',
-
-                '𐨤',
-                '𐨥',
-                '𐨦',
-                '𐨧',
-                '𐨨',
-
-                '𐨩',
-                '𐨪',
-                '𐨫',
-                '𐨬',
-
-                '𐨭',
-                '𐨮',
-                '𐨯',
-                '𐨱'
+                'k',
+                'kʰ',
+                'g',
+                'gʰ',
+                'n\u02BD',
+
+                'č',
+                'čʰ',
+                'j',
+                'jʰ',
+                'ɲ',
+
+                'ʈ',
+                'ʈʰ',
+                'ɖ',
+                'ɖʰ',
+                'ɳ',
+
+                't',
+                'tʰ',
+                'd',
+                'dʰ',
+                'n',
+
+                'p',
+                'pʰ',
+                'b',
+                'bʰ',
+                'm',
+
+                'y',
+                'r',
+                'l',
+                'v',
+
+                'š',
+                'ʂ',
+                's',
+                'h',
                 ]
 
 SouthConsonantMap = [
-                    '𐨫\u02BD',
-                    '𐨫\u02BD',
-                    '𐨪\u02BD',
-                    '𐨣\u02BD'
+                    'ɭ',
+                    'ɭ\u02BD',
+                    'r\u02BD',
+                    'n\u02BD'
                     ]
 
 NuktaConsonantMap =  [
-                    '𐨲',
-                    '𐨑\u02BD',
-                    '𐨒\u02BD',
-                    '𐨰',
-                    '𐨜\u02BD',
-                    '𐨝\u02BD',
-                    '𐨥\u02BD',
-                    '𐨩\u02BD'
+                     'q',
+                     'ḫ',
+                     'ġ',
+                     'z',
+                     'ɽ',
+                     'ɽʰ',
+                     'f',
+                     'y\u02BD'
                      ]
 
 SinhalaConsonantMap =[
-                     '𐨎𐨒\u02BD',
-                     '𐨎𐨗\u02BD',
-                     '𐨎𐨜\u02BD',
-                     '𐨎𐨡\u02BD',
-                     '𐨎𐨦\u02BD',
+                     'n\u033Dg\u02BD',
+                     'n\u033Dj\u02BD',
+                     'n\u033Dd\u02BD',
+                     'n\u033Dd\u02BD',
+                     'm\u033Db\u02BD',
                       ]
 
 NuktaMap = [
-           '\u02BD\u02BD\u02BD\u02BD'
+           'Q'
            ]
 
 OmMap = [
-        '𐨀𐨅𐨎'
+        'ō̂m\u033D\u02BD'
         ]
 
 SignMap =[
-         '\u02BD\u02BD',
-         '𐩖',
-         '𐩗'
+         '\u02BD\u02BD\u02BD\u02BD',
+         '.',
+         '..'
          ]
 
-Aytham =[AyogavahaMap[2]+'\u02BD']
+Aytham =['h\u033D\u02BD']
 
-## Update Numbers to Kharoshthi
 NumeralMap = [
              '\u0030',
              '\u0031',
              '\u0032',
              '\u0033',
              '\u0034',
              '\u0035',
              '\u0036',
              '\u0037',
              '\u0038',
              '\u0039',
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/Khojki.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Khojki.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
 
 # Script Mapping for Devanagari
 
 VowelMap =  [
             '\U00011200',
             '\U00011201',
+            '\U00011240',
             '\U00011202',
-            '\U00011202\u02BD',
             '\U00011203',
             '\U00011203\u02BD',
             '\U00011226\U0001122D\u02BD',
             '\U00011226\U0001122E\u02BD',
             '\U00011227\U0001122D\u02BD',
             '\U00011227\U0001122E\u02BD',
             '\U00011204',
@@ -35,15 +35,15 @@
 
 VowelSignMap =  [
                 '\U0001122C',
                 '\U0001122D',
                 '\U0001122E',
                 '\U0001122F',
                 '\U0001122F\u02BD',
-                '\U00011235\U00011226\U0001122D\u02BD',
+                '\U00011241',
                 '\U00011235\U00011226\U0001122E\u02BD',
                 '\U00011235\U00011227\U0001122D\u02BD',
                 '\U00011235\U00011227\U0001122E\u02BD',
                 '\U00011230',
                 '\U00011231',
                 '\U00011232',
                 '\U00011233',
@@ -165,7 +165,13 @@
              '\u0AEA',
              '\u0AEB',
              '\u0AEC',
              '\u0AED',
              '\u0AEE',
              '\u0AEF'
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/Khudawadi.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/Wancho.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,171 +1,155 @@
 # -*- coding: utf-8 -*-
 
-# Script Mapping for Devanagari
+# Script Mapping for ISO
 
 VowelMap =  [
-            '\U000112B0',
-            '\U000112B1',
-            '\U000112B2',
-            '\U000112B3',
-            '\U000112B4',
-            '\U000112B5',
-            '𑋙𑋡\u02BD',
-            '𑋙𑋢\u02BD',
-            '𑋚𑋡\u02BD',
-            '𑋚𑋢\u02BD',
-            '\U000112B6',
-            '\U000112B7',
-            '\U000112B8',
-            '\U000112B9',
+            '\U0001E2C1',
+            '\U0001E2C0',
+            '\U0001E2DC',
+            '\U0001E2DC\u02BD',
+            '\U0001E2DE',
+            '\U0001E2DE\u02BD',
+            '\U0001E2D7\U0001E2DE\u02BD',
+            '\U0001E2D7\U0001E2DE\u02BD',
+            '\U0001E2C8\U0001E2DE\u02BD',
+            '\U0001E2C8\U0001E2DE\u02BD',
+            '\U0001E2DB',
+            '\U0001E2C0\U0001E2DC',
+            '\U0001E2D5',
+            '\U0001E2D6'
             ]
 
 SouthVowelMap = [
-                '\U000112B6\u02BD',
-                '\U000112B8\u02BD',
+                '\U0001E2DB\u02BD',
+                '\U0001E2D5\u02BD',
                 ]
 
 ModernVowelMap = [
-                 '\U000112B6\u02BD',
-                 '\U000112B1\u02BD',
+                 '\U0001E2DB\u02BD',
+                 '\U0001E2C0\u02BD',
                  ]
 
 SinhalaVowelMap = [
-                  '\U000112B6\u02BD'
+                  '\U0001E2DB\u02BD'
                   ]
 
-VowelSignMap =  [
-                '\U000112E0',
-                '\U000112E1',
-                '\U000112E2',
-                '\U000112E3',
-                '\U000112E4',
-                '𑋪𑋙𑋡\u02BD',
-                '𑋪𑋙𑋢\u02BD',
-                '𑋪𑋚𑋡\u02BD',
-                '𑋪𑋚𑋢\u02BD',
-                '\U000112E5',
-                '\U000112E6',
-                '\U000112E7',
-                '\U000112E8',
-                ]
+VowelSignMap =  VowelMap[1:]
 
-SouthVowelSignMap = [
-                    '\U000112E5\u02BD',
-                    '\U000112E7\u02BD',
-                    ]
+SouthVowelSignMap = SouthVowelMap[:]
 
-ModernVowelSignMap =[
-                    '\U000112E5\u02BD',
-                    '\U000112E0\u02BD'
-                    ]
+ModernVowelSignMap = ModernVowelMap[:]
 
-SinhalaVowelSignMap = [
-                      '\U000112E5\u02BD'
-                      ]
+SinhalaVowelSignMap = SinhalaVowelMap[:]
 
 AyogavahaMap = [
-               '\U000112DF\u02BD',
-               '\U000112DF',
-               '𑋞𑋪\u02BD'
+               '\u02BF',
+               '\u02BE',
+               '\U0001E2EB'
                ]
 
 ViramaMap =  [
-             '\U000112EA'
+             '\u00D7'
              ]
 
 ConsonantMap =  [
-                '\U000112BA',
-                '\U000112BB',
-                '\U000112BC',
-                '\U000112BE',
-                '\U000112BF',
-
-                '\U000112C0',
-                '\U000112C1',
-                '\U000112C2',
-                '\U000112C4',
-                '\U000112C5',
-
-                '\U000112C6',
-                '\U000112C7',
-                '\U000112C8',
-                '\U000112CB',
-                '\U000112CC',
-
-                '\U000112CD',
-                '\U000112CE',
-                '\U000112CF',
-                '\U000112D0',
-                '\U000112D1',
-
-                '\U000112D2',
-                '\U000112D3',
-                '\U000112D4',
-                '\U000112D6',
-                '\U000112D7',
-
-                '\U000112D8',
-                '\U000112D9',
-                '\U000112DA',
-                '\U000112DB',
-
-                '\U000112DC',
-                '\U000112DC𑋩',
-                '\U000112DD',
-                '\U000112DE'
+                '\U0001E2D4',
+                '\U0001E2D9',
+                '\U0001E2C5',
+                '\U0001E2C5\u02BD',
+                '\U0001E2DD',
+
+                '\U0001E2C3',
+                '\U0001E2C3\u02BD',
+                '\U0001E2D0',
+                '\U0001E2D0\u02BD',
+                '\U0001E2E9',
+
+                '\U0001E2CB\u02BD',
+                '\U0001E2CC\u02BD',
+                '\U0001E2C4\u02BD',
+                '\U0001E2C4\u02BD',
+                '\U0001E2C9\u02BD',
+
+                '\U0001E2CB',
+                '\U0001E2CC',
+                '\U0001E2C4',
+                '\U0001E2C4\u02BD',
+                '\U0001E2C9',
+
+                '\U0001E2CA',
+                '\U0001E2C7',
+                '\U0001E2C2',
+                '\U0001E2C2\u02BD',
+                '\U0001E2D8',
+
+                '\U0001E2C6',
+                '\U0001E2D7',
+                '\U0001E2C8',
+                '\U0001E2D3',
+
+                '\U0001E2CF',
+                '\U0001E2CF\u02BD',
+                '\U0001E2CE',
+                '\U0001E2DA',
                 ]
 
 SouthConsonantMap = [
-                    '𑋚𑋩',
-                    '𑋚𑋩\u02BD',
-                    '𑋙𑋩',
-                    '𑋑𑋩'
+                    '\U0001E2DF',
+                    '\U0001E2DF\u02BD',
+                    '\U0001E2D7\u02BD',
+                    '\U0001E2C9\u02BD'
                     ]
 
 NuktaConsonantMap =  [
-                     '𑊺𑋩',
-                     '𑊻𑋩',
-                     '𑊾𑋩',
-                     '𑋂𑋩',
-                     '𑋊',
-                     '𑋋𑋩',
-                     '𑋓𑋩',
-                     '𑋘𑋩'
+                '\U0001E2D4\u02BD',
+                '\U0001E2D9\u02BD',
+                '\U0001E2C5\u02BD',
+                     '\U0001E2D1',
+                '\U0001E2C4\u02BD',
+                '\U0001E2C4\u02BD',
+                     '\U0001E2CD',
+                     '\U0001E2C6\u02BD'
                      ]
 
 SinhalaConsonantMap =[
-                     '𑋟𑊼\u02BD',
-                     '𑋟𑋂\u02BD',
-                     '𑋟𑋈\u02BD',
-                     '𑋟𑋏\u02BD',
-                     '𑋟𑋔\u02BD',
+                     '\U0001E2DD\U0001E2C5\u02BD',
+                     '\U0001E2E9\U0001E2D0\u02BD',
+                     '\U0001E2C9\U0001E2C4\u02BD',
+                     '\U0001E2C9\U0001E2C4\u02BD',
+                     '\U0001E2D8\U0001E2C2\u02BD',
                       ]
 
 NuktaMap = [
-           '𑋩'
+           '\u00D8'
            ]
 
 OmMap = [
-        '𑊸𑋟'
+        '\U0001E2E6\u02BD'
         ]
 
 SignMap =[
-         '\u093D',
-         '।',
-         '॥'
+         '\u02BD\u02BD',
+         '.',
+         '..'
          ]
 
-Aytham =[AyogavahaMap[2]+'\u02BD']
+Aytham =['\U0001E2D4\u02BD']
 
 NumeralMap = [
-             '\U000112F0',
-             '\U000112F1',
-             '\U000112F2',
-             '\U000112F3',
-             '\U000112F4',
-             '\U000112F5',
-             '\U000112F6',
-             '\U000112F7',
-             '\U000112F8',
-             '\U000112F9',
+             '\U0001E2F0',
+             '\U0001E2F1',
+             '\U0001E2F2',
+             '\U0001E2F3',
+             '\U0001E2F4',
+             '\U0001E2F5',
+             '\U0001E2F6',
+             '\U0001E2F7',
+             '\U0001E2F8',
+             '\U0001E2F9',
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/Lepcha.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Lepcha.py`

 * *Files 12% similar despite different names*

```diff
@@ -165,7 +165,13 @@
              '\u1C44',
              '\u1C45',
              '\u1C46',
              '\u1C47',
              '\u1C48',
              '\u1C49'
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/Limbu.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Limbu.py`

 * *Files 14% similar despite different names*

```diff
@@ -165,7 +165,13 @@
              '\u194A',
              '\u194B',
              '\u194C',
              '\u194D',
              '\u194E',
              '\u194F'
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/Mahajani.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Mahajani.py`

 * *Files 7% similar despite different names*

```diff
@@ -165,7 +165,13 @@
              '\u096A',
              '\u096B',
              '\u096C',
              '\u096D',
              '\u096E',
              '\u096F'
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/Malayalam.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/WX-kok.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,170 +1,155 @@
 # -*- coding: utf-8 -*-
 
-# Script Mapping for Devanagari
+# Script Mapping for ISO
 
 VowelMap =  [
-            '\u0D05',
-            '\u0D06',
-            '\u0D07',
-            '\u0D08',
-            '\u0D09',
-            '\u0D0A',
-            '\u0D0B',
-            '\u0D60',
-            '\u0D0C',
-            '\u0D61',
-            '\u0D0F',
-            '\u0D10',
-            '\u0D13',
-            '\u0D14',
+            'a',
+            'A',
+            'i',
+            'I',
+            'u',
+            'U',
+            'q',
+            '\u0071\u0056Y',
+            '\u004CY',
+            '\u004C\u0056Y',
+            'E',
+            'Y',
+            'O',
+            'Q'
             ]
 
 SouthVowelMap = [
-                '\u0D0E',
-                '\u0D12',
+                'e',
+                'o',
                 ]
 
 ModernVowelMap = [
-                 '\u0D0E\u02BC',
-                 '\u0D06\u02BC',
+                 'Z',
+                 'V',
                  ]
 
 SinhalaVowelMap = [
-                  '\u0D0F\u02C7'
+                  '\u0041\u0045\u0056Y'
                   ]
 
-VowelSignMap =  [
-                '\u0D3E',
-                '\u0D3F',
-                '\u0D40',
-                '\u0D41',
-                '\u0D42',
-                '\u0D43',
-                '\u0D44',
-                '\u0D62',
-                '\u0D63',
-                '\u0D47',
-                '\u0D48',
-                '\u0D4B',
-                '\u0D57',
-                ]
+VowelSignMap =  VowelMap[1:]
 
-SouthVowelSignMap = [
-                    '\u0D46',
-                    '\u0D4A',
-                    ]
+SouthVowelSignMap = SouthVowelMap[:]
 
-ModernVowelSignMap =[
-                    '\u0D46\u02BC',
-                    '\u0D3E\u02BC']
+ModernVowelSignMap = ModernVowelMap[:]
 
-SinhalaVowelSignMap = [
-                      '\u0D47\u02C7'
-                      ]
+SinhalaVowelSignMap = SinhalaVowelMap[:]
 
 AyogavahaMap = [
-               '\u0D01',
-               '\u0D02',
-               '\u0D03'
+               '~',
+               'M',
+               'H'
                ]
 
 ViramaMap =  [
-             '\u0D4D'
+             '\u00D7'
              ]
 
 ConsonantMap =  [
-                '\u0D15',
-                '\u0D16',
-                '\u0D17',
-                '\u0D18',
-                '\u0D19',
-
-                '\u0D1A',
-                '\u0D1B',
-                '\u0D1C',
-                '\u0D1D',
-                '\u0D1E',
-
-                '\u0D1F',
-                '\u0D20',
-                '\u0D21',
-                '\u0D22',
-                '\u0D23',
-
-                '\u0D24',
-                '\u0D25',
-                '\u0D26',
-                '\u0D27',
-                '\u0D28',
-
-                '\u0D2A',
-                '\u0D2B',
-                '\u0D2C',
-                '\u0D2D',
-                '\u0D2E',
-
-                '\u0D2F',
-                '\u0D30',
-                '\u0D32',
-                '\u0D35',
-
-                '\u0D36',
-                '\u0D37',
-                '\u0D38',
-                '\u0D39'
+                '\u006B',
+                '\u004B',
+                '\u0067',
+                '\u0047',
+                'f',
+
+                '\u0063',
+                '\u0043',
+                '\u006A',
+                '\u004A',
+                'F',
+
+                '\u0074',
+                '\u0054',
+                '\u0064',
+                '\u0044',
+                '\u004E',
+
+                '\u0077',
+                '\u0057',
+                '\u0078',
+                '\u0058',
+                '\u006E',
+
+                '\u0070',
+                '\u0050',
+                '\u0062',
+                '\u0042',
+                '\u006D',
+
+                '\u0079',
+                '\u0072',
+                '\u006C',
+                '\u0076',
+
+                'z',
+                'S',
+                's',
+                'h',
                 ]
 
 SouthConsonantMap = [
-                    '\u0D33',
-                    '\u0D34',
-                    '\u0D31',
-                    '\u0D29'
+                    'L',
+                    '\u006C\u0059\u0059Y',
+                    'R',
+                    '\u006E\u0059Y'
                     ]
 
 NuktaConsonantMap =  [
-                     '\u0D15\u00B7',
-                     '\u0D16\u00B7',
-                     '\u0D17\u00B7',
-                     '\u0D1C\u00B7',
-                     '\u0D21\u00B7',
-                     '\u0D22\u00B7',
-                     '\u0D2B\u00B7',
-                     '\u0D2F\u00B7'
+                     '\u006B\u0059Y',
+                     '\u004B\u0059Y',
+                     '\u0047\u0059Y',
+                     '\u007A\u0059Y',
+                     '\u0064\u0059Y',
+                     '\u0044\u0059Y',
+                     '\u0050\u0059Y',
+                     '\u0079\u0059Y'
                      ]
 
 SinhalaConsonantMap =[
-                     '\u0D02\u02C6\u0D17',
-                     '\u0D02\u02C6\u0D1C',
-                     '\u0D02\u02C6\u0D21',
-                     '\u0D02\u02C6\u0D26',
-                     '\u0D02\u02C6\u0D2C',
+                     '\u006E\u0059\u0059\u0067Y',
+                     '\u006E\u0059\u0059\u006AY',
+                     '\u006E\u0059\u0059\u0064Y',
+                     '\u006E\u0059\u0059\u0078Y',
+                     '\u006D\u0059\u0059\u0062Y',
                       ]
 
 NuktaMap = [
-           '\u00B7'
+           '\u0051Y'
            ]
 
 OmMap = [
-        '\u0D13\u0D02'
+        '\u006F\u004DY'
         ]
 
 SignMap =[
-         '\u0D3D',
-         '\u0964',
-         '\u0965'
+         '\u0027Y',
+         '\u002EY',
+         '\u002E\u002EY'
          ]
 
-Aytham =[AyogavahaMap[2]+'\u02BC']
+Aytham =['\u006B\u0059\u0059Y']
 
 NumeralMap = [
-             '\u0D66',
-             '\u0D67',
-             '\u0D68',
-             '\u0D69',
-             '\u0D6A',
-             '\u0D6B',
-             '\u0D6C',
-             '\u0D6D',
-             '\u0D6E',
-             '\u0D6F'
+             '\u0030',
+             '\u0031',
+             '\u0032',
+             '\u0033',
+             '\u0034',
+             '\u0035',
+             '\u0036',
+             '\u0037',
+             '\u0038',
+             '\u0039',
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/MasaramGondi.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/MasaramGondi.py`

 * *Files 22% similar despite different names*

```diff
@@ -164,7 +164,13 @@
              '\U00011D54',
              '\U00011D55',
              '\U00011D56',
              '\U00011D57',
              '\U00011D58',
              '\U00011D59',
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/MeeteiMayek.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Vatteluttu.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,171 +1,176 @@
 # -*- coding: utf-8 -*-
 
 # Script Mapping for Devanagari
 
 VowelMap =  [
-            '\uABD1',
-            '\uABD1\uABE5',
-            '\uABCF',
-            '\uABD1\uAAEB',
-            '\uABCE',
-            '\uABD1\uAAEC',
-            '\uABD4\uABE8\u02BD',
-            '\uABD4\uAAEC\u02BD',
-            '\uABC2\uABE8\u02BD',
-            '\uABC2\uAAEC\u02BD',
-            '\uABD1\uABE6',
-            '\uABD1\uABE9',
-            '\uABD1\uABE3',
-            '\uABD1\uABE7',
+            '\u0B85',
+            '\u0B86',
+            '\u0B87',
+            '\u0B88',
+            '\u0B89',
+            '\u0B8A',
+            '\u0BB0\u0BC1\u02BD',
+            '\u0BB0\u0BC2\u02BD',
+            '\u0BB2\u0BC1\u02BD',
+            '\u0BB2\u0BC2\u02BD',
+            '\u0B8F',
+            '\u0B90',
+            '\u0B93',
+            '\u0B94',
             ]
 
 SouthVowelMap = [
-                '\uABD1\uABE6\u02BD',
-                '\uABD1\uABE3\u02BD',
+                '\u0B8E',
+                '\u0B92',
                 ]
 
 ModernVowelMap = [
-                 '\uABD1\uABE6\u02BD',
-                 '\uABD1\uABE5\u02BD',
+                 '\u0B8E\u02BD',
+                 '\u0B86\u02BD',
                  ]
 
 SinhalaVowelMap = [
-                  '\uABD1\uABE6\u02BD'
+                  '\u0B8F\u02BD'
                   ]
 
 VowelSignMap =  [
-                 '\uABE5',
-                 '\uABE4',
-                 '\uAAEB',
-                 '\uABE8',
-                 '\uAAEC',
-                 '\uABED\uABD4\uABE8\u02BD',
-                 '\uABED\uABD4\uAAEC\u02BD',
-                 '\uABED\uABC2\uABE8\u02BD',
-                 '\uABED\uABC2\uAAEC\u02BD',
-                 '\uABE6',
-                 '\uABE9',
-                 '\uABE3',
-                 '\uABE7',
-                 ]
+                '\u0BBE',
+                '\u0BBF',
+                '\u0BC0',
+                '\u0BC1',
+                '\u0BC2',
+                '\u0BCD\u0BB0\u0BC1\u02BD',
+                '\u0BCD\u0BB0\u0BC2\u02BD',
+                '\u0BCD\u0BB2\u0BC1\u02BD',
+                '\u0BCD\u0BB2\u0BC2\u02BD',
+                '\u0BC7',
+                '\u0BC8',
+                '\u0BCB',
+                '\u0BCC',
+                ]
 
 SouthVowelSignMap = [
-                     '\uABE6\u02BD',
-                     '\uABE3\u02BD',
-                     ]
+                    '\u0BC6',
+                    '\u0BCA',
+                    ]
 
 ModernVowelSignMap =[
-                     '\uABE6\u02BD',
-                     '\uABE5\u02BD',
-                     ]
+                    '\u0BC6\u02BD',
+                    '\u0BBE\u02BD']
 
 SinhalaVowelSignMap = [
-                       '\uABE6\u02BD'
+                      '\u0BC7\u02BD'
                       ]
 
 AyogavahaMap = [
-               '\uABEA\u02BD',
-               '\uABEA',
-               '\uAAF5'
+               '\u0BAE\u0BCD\u02BD',
+               '\u0BAE\u0BCD\u02BD',
+               '꞉' # Modifying letter colon for Visarga
                ]
 
 ViramaMap =  [
-             '\uABED'
+             '\u0BCD'
              ]
 
 ConsonantMap =  [
-                '\uABC0',
-                '\uABC8',
-                '\uABD2',
-                '\uABD8',
-                '\uABC9',
-
-                '\uABC6',
-                '\uAAE2',
-                '\uABD6',
-                '\uABD3',
-                '\uAAE3',
-
-                '\uAAE4',
-                '\uAAE5',
-                '\uAAE6',
-                '\uAAE7',
-                '\uAAE8',
-
-                '\uABC7',
-                '\uABCA',
-                '\uABD7',
-                '\uABD9',
-                '\uABC5',
-
-                '\uABC4',
-                '\uABD0',
-                '\uABD5',
-                '\uABDA',
-                '\uABC3',
-
-                '\uABCC',
-                '\uABD4',
-                '\uABC2',
-                '\uABCB',
-
-                '\uAAE9',
-                '\uAAEA',
-                '\uABC1',
-                '\uABCD'
+                '\u0B95',
+                '\u0B95\u02BD',
+                '\u0B95\u02BD',
+                '\u0B95\u02BD',
+                '\u0B99',
+
+                '\u0B9A',
+                '\u0B9A\u02BD',
+                '\u0B9A\u02BD',
+                '\u0B9A\u02BD',
+                '\u0B9E',
+
+                '\u0B9F',
+                '\u0B9F\u02BD',
+                '\u0B9F\u02BD',
+                '\u0B9F\u02BD',
+                '\u0BA3',
+
+                '\u0BA4',
+                '\u0BA4\u02BD',
+                '\u0BA4\u02BD',
+                '\u0BA4\u02BD',
+                '\u0BA8',
+
+                '\u0BAA',
+                '\u0BAA\u02BD',
+                '\u0BAA\u02BD',
+                '\u0BAA\u02BD',
+                '\u0BAE',
+
+                '\u0BAF',
+                '\u0BB0',
+                '\u0BB2',
+                '\u0BB5',
+
+                '\u0B9A\u02BD',
+                '\u0B9A\u02BD',
+                '\u0B9A\u02BD',
+                '\u0B95\u02BD'
                 ]
 
 SouthConsonantMap = [
-                    '\uABC2\u02BD',
-                    '\uABC2\u02BD',
-                    '\uABD4\u02BD',
-                    '\uABC5\u02BD'
+                    '\u0BB3',
+                    '\u0BB4',
+                    '\u0BB1',
+                    '\u0BA9'
                     ]
 
 NuktaConsonantMap =  [
-                     '\uABC0\u02BD',
-                     '\uABC8\u02BD',
-                     '\uABD2\u02BD',
-                     '\uABD6\u02BD',
-                     '\uABD7\u02BD',
-                     '\uABD9\u02BD',
-                     '\uABD0\u02BD',
-                     '\uABCC\u02BD'
+                     '\u02BD\u0B95',
+                     '\u02BD\u0B95',
+                     '\u02BD\u0B95',
+                     '\u02BD\u0B9A',
+                     '\u02BD\u0B9F',
+                     '\u02BD\u0B9F',
+                     '\u02BD\u0BAA',
+                     '\u02BD\u0BAF'
                      ]
 
 SinhalaConsonantMap =[
-                     '\uABEA\uABD2\u02BD',
-                     '\uABEA\uABD6\u02BD',
-                     '\uABEA\uABD7\u02BD',
-                     '\uABEA\uABD7\u02BD',
-                     '\uABEA\uABD5\u02BD',
+                     '\u0B99\u0BCD\u02BD\u0B95',
+                     '\u0B9E\u0BCD\u02BD\u0B9A',
+                     '\u0BA3\u0BCD\u02BD\u0B9F',
+                     '\u0BA8\u0BCD\u02BD\u0BA4',
+                     '\u0BAE\u0BCD\u02BD\u0BAA',
                       ]
 
 NuktaMap = [
-           '\u02BD\u02BD\u02BD\u02BD'
+           '\u02BD\u02BD'
            ]
 
 OmMap = [
-        '\uABD1\uABE3\uABEA'
+        'ஓம்'
         ]
 
 SignMap =[
-         '\u0027',
-         '\uABEB',
-         '\uABEB\uABEB'
+         '\u02BD\u02BD',
+         '.',
+         '..'
          ]
 
-Aytham =[AyogavahaMap[2]+'\u02BC']
+Aytham =['\u0B83']
 
 NumeralMap = [
-             '\uABF0',
-             '\uABF1',
-             '\uABF2',
-             '\uABF3',
-             '\uABF4',
-             '\uABF5',
-             '\uABF6',
-             '\uABF7',
-             '\uABF8',
-             '\uABF9'
-             ]
+             '0',
+             '1',
+             '2',
+             '3',
+             '4',
+             '5',
+             '6',
+             '7',
+             '8',
+             '9'
+            ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/Modi.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Multani.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,171 +1,177 @@
 # -*- coding: utf-8 -*-
 
 # Script Mapping for Devanagari
 
 VowelMap =  [
-            '\U00011600',
-            '\U00011601',
-            '\U00011602',
-            '\U00011603',
-            '\U00011604',
-            '\U00011605',
-            '\U00011606',
-            '\U00011607',
-            '\U00011608',
-            '\U00011609',
-            '\U0001160A',
-            '\U0001160B',
-            '\U0001160C',
-            '\U0001160D',
+            '\U00011280',
+            '\U00011280\u02BD',
+            '\U00011281',
+            '\U00011281\u02BD',
+            '\U00011282',
+            '\U00011282\u02BD',
+            '\U000112A2\U00011282\u02BD',
+            '\U000112A2\U00011282\u02BD',
+            '\U000112A3\U00011282\u02BD',
+            '\U000112A3\U00011282\u02BD',
+            '\U00011283',
+            '\U00011283\u02BD',
+            '\U00011282\u02BD',
+            '\U00011282\u02BD',
             ]
 
 SouthVowelMap = [
-                '\U0001160A\u02BD',
-                '\U0001160C\u02BD',
+                '\U00011283\u02BD',
+                '\U00011282\u02BD',
                 ]
 
 ModernVowelMap = [
-                 '\U00011600\U00011640',
-                 '\U00011601\u02BD',
+                 '\U00011283\u02BD',
+                 '\U00011280\u02BD',
                  ]
 
 SinhalaVowelMap = [
-                  '\U0001160A\u02BD'
+                  '\U00011283\u02BD'
                   ]
 
 VowelSignMap =  [
-                '\U00011630',
-                '\U00011631',
-                '\U00011632',
-                '\U00011633',
-                '\U00011634',
-                '\U00011635',
-                '\U00011636',
-                '\U00011637',
-                '\U00011638',
-                '\U00011639',
-                '\U0001163A',
-                '\U0001163B',
-                '\U0001163C',
+                '\U00011280\u02BF',
+                '\U00011281\u02BF',
+                '\U00011281\u02BF',
+                '\U00011282\u02BF',
+                '\U00011282\u02BF',
+                '\U000112A2\U00011282\u02BF',
+                '\U000112A2\U00011282\u02BF',
+                '\U000112A3\U00011282\u02BF',
+                '\U000112A3\U00011282\u02BF',
+                '\U00011283\u02BF',
+                '\U00011283\u02BF',
+                '\U00011282\u02BF',
+                '\U00011282\u02BF',
                 ]
 
 SouthVowelSignMap = [
-                    '\U00011639\u02BD',
-                    '\U0001163B\u02BD',
+                '\U00011283\u02BF',
+                '\U00011282\u02BF',
                     ]
 
 ModernVowelSignMap =[
-                    '\U00011640',
-                    '\U00011630\u02BD'
+                 '\U00011283\u02BF',
+                 '\U00011280\u02BF',
                     ]
 
 SinhalaVowelSignMap = [
-                      '\U00011639\u02BD'
+                  '\U00011283\u02BF'
                       ]
 
 AyogavahaMap = [
-               '\U0001163D\u02BD',
-               '\U0001163D',
-               '\U0001163E'
+               '\U0001129A\u02BD',
+               '\U0001129A\u02BD',
+               '\U000112A6\u02BD'
                ]
 
 ViramaMap =  [
-             '\U0001163F'
+             '\u02BE'
              ]
 
 ConsonantMap =  [
-                '\U0001160E',
-                '\U0001160F',
-                '\U00011610',
-                '\U00011611',
-                '\U00011612',
-
-                '\U00011613',
-                '\U00011614',
-                '\U00011615',
-                '\U00011616',
-                '\U00011617',
-
-                '\U00011618',
-                '\U00011619',
-                '\U0001161A',
-                '\U0001161B',
-                '\U0001161C',
-
-                '\U0001161D',
-                '\U0001161E',
-                '\U0001161F',
-                '\U00011620',
-                '\U00011621',
-
-                '\U00011622',
-                '\U00011623',
-                '\U00011624',
-                '\U00011625',
-                '\U00011626',
-
-                '\U00011627',
-                '\U00011628',
-                '\U00011629',
-                '\U0001162A',
-
-                '\U0001162B',
-                '\U0001162C',
-                '\U0001162D',
-                '\U0001162E'
+                '\U00011284',
+                '\U00011285',
+                '\U00011286',
+                '\U00011288',
+                '\U0001129A\u02BD',
+
+                '\U0001128A',
+                '\U0001128B',
+                '\U0001128C',
+                '\U0001128C\u02BD',
+                '\U0001128F',
+
+                '\U00011290',
+                '\U00011291',
+                '\U00011292',
+                '\U00011294',
+                '\U00011295',
+
+                '\U00011296',
+                '\U00011297',
+                '\U00011298',
+                '\U00011299',
+                '\U0001129A',
+
+                '\U0001129B',
+                '\U0001129C',
+                '\U0001129D',
+                '\U0001129F',
+                '\U000112A0',
+
+                '\U000112A1',
+                '\U000112A2',
+                '\U000112A3',
+                '\U000112A4',
+
+                '\U000112A5\u02BD',
+                '\U000112A5\u02BD',
+                '\U000112A5',
+                '\U000112A6'
                 ]
 
 SouthConsonantMap = [
-                    '\U0001162F',
-                    '\U0001162F\u02BD',
-                    '\U0001162C\u02BD',
-                    '\U00011621\u02BD'
+                    '\U000112A3\u02BD',
+                    '\U000112A3\u02BD',
+                    '\U000112A2\u02BD',
+                    '\U0001129A\u02BD'
                     ]
 
 NuktaConsonantMap =  [
-                     '\U0001160E\u02BD',
-                     '\U0001160F\u02BD',
-                     '\U00011610\u02BD',
-                     '\U00011615\u02BD',
-                     '\U0001161A\u02BD',
-                     '\U0001161B\u02BD',
-                     '\U00011623\u02BD',
-                     '\U00011627\u02BD'
+                     '\U00011284\u02BD',
+                     '\U00011285\u02BD',
+                     '\U00011286\u02BD',
+                     '\U0001128C\u02BD',
+                     '\U000112A7',
+                     '\U000112A8',
+                     '\U0001129C\u02BD',
+                     '\U000112A1\u02BD'
                      ]
 
 SinhalaConsonantMap =[
-                     '\U0001163D𑘐\u02BD',
-                     '\U0001163D𑘕\u02BD',
-                     '\U0001163D𑘚\u02BD',
-                     '\U0001163D𑘟\u02BD',
-                     '\U0001163D𑘤\u02BD',
+                     '\U0001129A\U00011286\u02BD',
+                     '\U0001129A\U0001128C\u02BD',
+                     '\U0001129A\U00011292\u02BD',
+                     '\U0001129A\U00011298\u02BD',
+                     '\U000112A0\U0001129D\u02BD',
                       ]
 
 NuktaMap = [
-           '\u02BD\u02BD\u02BD\u02BD'
+           '\u02BD\u02BD\u02BD'
            ]
 
 OmMap = [
-        '𑘌𑘽'
+        '\U00011282\U000112A0\u02BD'
         ]
 
 SignMap =[
-         '\u093D',
-         '\U00011641',
-         '\U00011642'
+         '\u02BD\u02BD',
+         '।',
+         '॥'
          ]
 
 Aytham =[AyogavahaMap[2]+'\u02BD']
 
 NumeralMap = [
-             '\U00011650',
-             '\U00011651',
-             '\U00011652',
-             '\U00011653',
-             '\U00011654',
-             '\U00011655',
-             '\U00011656',
-             '\U00011657',
-             '\U00011658',
-             '\U00011659'
+             '\u0A66',
+             '\u0A67',
+             '\u0A68',
+             '\u0A69',
+             '\u0A6A',
+             '\u0A6B',
+             '\u0A6C',
+             '\u0A6D',
+             '\u0A6E',
+             '\u0A6F'
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/Multani.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/Lao2.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,171 +1,181 @@
 # -*- coding: utf-8 -*-
 
 # Script Mapping for Devanagari
 
+#http://www.laomanuscripts.net/downloads/DLLM_pali_laoromanisation.pdf
+
+#Lao aG to aM, check for buddhaM vs buddhaG...
+
 VowelMap =  [
-            '\U00011280',
-            '\U00011280\u02BD',
-            '\U00011281',
-            '\U00011281\u02BD',
-            '\U00011282',
-            '\U00011282\u02BD',
-            '\U000112A2\U00011282\u02BD',
-            '\U000112A2\U00011282\u02BD',
-            '\U000112A3\U00011282\u02BD',
-            '\U000112A3\U00011282\u02BD',
-            '\U00011283',
-            '\U00011283\u02BD',
-            '\U00011282\u02BD',
-            '\U00011282\u02BD',
+            '\u0EAD',
+            '\u0EAD\u0EB2',
+            '\u0EAD\u0EB4',
+            '\u0EAD\u0EB5',
+            '\u0EAD\u0EB8',
+            '\u0EAD\u0EB9',
+            '\u0EA3\u0EB8\u02BD',
+            '\u0EA3\u0EB9\u02BD',
+            '\u0EA5\u0EB8\u02BD',
+            '\u0EA5\u0EB9\u02BD',
+            '\u0EC0\u0EAD',
+            '\u0EC4\u0EAD',
+            '\u0EC2\u0EAD',
+            '\u0EC0\u0EAD\u0EBB\u0EB2',
             ]
 
 SouthVowelMap = [
-                '\U00011283\u02BD',
-                '\U00011282\u02BD',
+                '\u0EC0\u0EAD\u0EB0',
+                '\u0EC2\u0EAD\u0EB0',
                 ]
 
 ModernVowelMap = [
-                 '\U00011283\u02BD',
-                 '\U00011280\u02BD',
+                 '\u0EC1\u0EAD\u0EB0',
+                 '\u0EC0\u0EAD\u0EB2\u0EB0',
                  ]
 
 SinhalaVowelMap = [
-                  '\U00011283\u02BD'
+                  '\u0EC1\u0EAD'
                   ]
 
 VowelSignMap =  [
-                '\U00011280\u02BF',
-                '\U00011281\u02BF',
-                '\U00011281\u02BF',
-                '\U00011282\u02BF',
-                '\U00011282\u02BF',
-                '\U000112A2\U00011282\u02BF',
-                '\U000112A2\U00011282\u02BF',
-                '\U000112A3\U00011282\u02BF',
-                '\U000112A3\U00011282\u02BF',
-                '\U00011283\u02BF',
-                '\U00011283\u02BF',
-                '\U00011282\u02BF',
-                '\U00011282\u02BF',
+                 '\u0EB2',
+                 '\u0EB4',
+                 '\u0EB5',
+                 '\u0EB8',
+                 '\u0EB9',
+                 '\u0EBA\u0EA3\u0EB8\u02BD',
+                 '\u0EBA\u0EA3\u0EB9\u02BD',
+                 '\u0EBA\u0EA5\u0EB8\u02BD',
+                 '\u0EBA\u0EA5\u0EB9\u02BD',
+                 '\u0EC0',
+                 '\u0EC4',
+                 '\u0EC2',
+                 '\u0EC0\u0EBB\u0EB2',
                 ]
 
 SouthVowelSignMap = [
-                '\U00011283\u02BF',
-                '\U00011282\u02BF',
+                     '\u0EC0\u0EB0',
+                     '\u0EC2\u0EB0',
                     ]
 
 ModernVowelSignMap =[
-                 '\U00011283\u02BF',
-                 '\U00011280\u02BF',
+                     '\u0EC1\u0EB0',
+                     '\u0EC0\u0EB2\u0EB0',
                     ]
 
 SinhalaVowelSignMap = [
-                  '\U00011283\u02BF'
+                       '\u0EC1'
                       ]
 
 AyogavahaMap = [
-               '\U0001129A\u02BD',
-               '\U0001129A\u02BD',
-               '\U000112A6\u02BD'
+               '\u0ECD\u02BD',
+               '\u0ECD',
+               '\u0EAB\u0EBA\u02BD'
                ]
 
 ViramaMap =  [
-             '\u02BE'
+             '\u0EBA'
              ]
 
 ConsonantMap =  [
-                '\U00011284',
-                '\U00011285',
-                '\U00011286',
-                '\U00011288',
-                '\U0001129A\u02BD',
-
-                '\U0001128A',
-                '\U0001128B',
-                '\U0001128C',
-                '\U0001128C\u02BD',
-                '\U0001128F',
-
-                '\U00011290',
-                '\U00011291',
-                '\U00011292',
-                '\U00011294',
-                '\U00011295',
-
-                '\U00011296',
-                '\U00011297',
-                '\U00011298',
-                '\U00011299',
-                '\U0001129A',
-
-                '\U0001129B',
-                '\U0001129C',
-                '\U0001129D',
-                '\U0001129F',
-                '\U000112A0',
-
-                '\U000112A1',
-                '\U000112A2',
-                '\U000112A3',
-                '\U000112A4',
-
-                '\U000112A5\u02BD',
-                '\U000112A5\u02BD',
-                '\U000112A5',
-                '\U000112A6'
+                '\u0E81',
+                '\u0E82',
+                '\u0E84',
+                '\u0E84\u02BD',
+                '\u0E87',
+
+                '\u0E88',
+                '\u0EAA',
+                '\u0E8A',
+                '\u0E8A\u02BD',
+                '\u0E8D',
+
+                '\u0E95\u02BD',
+                '\u0E96\u02BD',
+                '\u0E97\u02BD',
+                '\u0E97\u02BD',
+                '\u0E99\u02BD',
+
+                '\u0E95',
+                '\u0E96',
+                '\u0E97',
+                '\u0E97\u02BD',
+                '\u0E99',
+
+                '\u0E9B',
+                '\u0E9C',
+                '\u0E9E',
+                '\u0E9E\u02BD',
+                '\u0EA1',
+
+                '\u0E8D',
+                '\u0EA3',
+                '\u0EA5',
+                '\u0EA7',
+
+                '\u0EAA\u02BD',
+                '\u0EAA\u02BD',
+                '\u0EAA',
+                '\u0EAB'
                 ]
 
 SouthConsonantMap = [
-                    '\U000112A3\u02BD',
-                    '\U000112A3\u02BD',
-                    '\U000112A2\u02BD',
-                    '\U0001129A\u02BD'
+                    '\u0EA5\u02BD',
+                    '\u0EA5\u02BD',
+                    'ຮ',
+                    '\u0E99\u02BD'
                     ]
 
 NuktaConsonantMap =  [
-                     '\U00011284\u02BD',
-                     '\U00011285\u02BD',
-                     '\U00011286\u02BD',
-                     '\U0001128C\u02BD',
-                     '\U000112A7',
-                     '\U000112A8',
-                     '\U0001129C\u02BD',
-                     '\U000112A1\u02BD'
+                    '\u0E81\u02BD',
+                    '\u0E82\u02BD',
+                    '\u0E84\u02BD',
+                    '\u0E8A\u02BD',
+                    '\u0E94\u02BD',
+                    '\u0E97\u02BD',
+                    'ຝ',
+                    '\u0EA2\u02BD',
                      ]
 
 SinhalaConsonantMap =[
-                     '\U0001129A\U00011286\u02BD',
-                     '\U0001129A\U0001128C\u02BD',
-                     '\U0001129A\U00011292\u02BD',
-                     '\U0001129A\U00011298\u02BD',
-                     '\U000112A0\U0001129D\u02BD',
+                     '\u0ECD\u0E84\u02BD',
+                     '\u0ECD\u0E8A\u02BD',
+                     '\u0ECD\u0E97\u02BD',
+                     '\u0ECD\u0E97\u02BD',
+                     '\u0ECD\u0E9E\u02BD',
                       ]
 
 NuktaMap = [
-           '\u02BD\u02BD\u02BD'
+           '\uEB0A'
            ]
 
 OmMap = [
-        '\U00011282\U000112A0\u02BD'
+        '\u0EC2\u0EAD\u0E87\u0EBA'
         ]
 
 SignMap =[
-         '\u02BD\u02BD',
-         '।',
-         '॥'
+         "'",
+         '\u0EAF',
+         '\u0EAF\u0EAF'
          ]
 
 Aytham =[AyogavahaMap[2]+'\u02BD']
 
 NumeralMap = [
-             '\u0A66',
-             '\u0A67',
-             '\u0A68',
-             '\u0A69',
-             '\u0A6A',
-             '\u0A6B',
-             '\u0A6C',
-             '\u0A6D',
-             '\u0A6E',
-             '\u0A6F'
+             '\u0ED0',
+             '\u0ED1',
+             '\u0ED2',
+             '\u0ED3',
+             '\u0ED4',
+             '\u0ED5',
+             '\u0ED6',
+             '\u0ED7',
+             '\u0ED8',
+             '\u0ED9'
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/Nandinagari.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/DivesAkuru.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,170 +1,177 @@
 # -*- coding: utf-8 -*-
 
 # Script Mapping for Devanagari
 
 VowelMap =  [
-            '\U000119A0',
-            '\U000119A1',
-            '\U000119A2',
-            '\U000119A3',
-            '\U000119A4',
-            '\U000119A5',
-            '\U000119A6',
-            '\U000119A7',
-            '𑧉𑧔\u02BD', #lu
-            '𑧉𑧕\u02BD', #luu
-            '\U000119AA',
-            '\U000119AB',
-            '\U000119AC',
-            '\U000119AD',
+            '\U00011900',
+            '\U00011901',
+            '\U00011902',
+            '\U00011903',
+            '\U00011904',
+            '\U00011905',
+            '\U00011927\U00011933',
+            '\U00011927\U00011934',
+            '\U00011928\U00011933',
+            '\U00011928\U00011934',
+            '\U00011906',
+            '\U00011906\U00011935',
+            '\U00011909',
+            '\U00011900\U00011904\u02BD',
             ]
 
 SouthVowelMap = [
-                '\U000119AA\u02BD',
-                '\U000119AC\u02BD',
+                '\U00011906\u02BD',
+                '\U00011909\u02BD',
                 ]
 
 ModernVowelMap = [
-                 '\U000119AA\u02BD',
-                 '\U000119A1\u02BD',
+                 '\U00011906\u02BD',
+                 '\U00011901\u02BD',
                  ]
 
 SinhalaVowelMap = [
-                '\U000119AA\u02BD',
+                  '\U00011906\u02BD',
                   ]
 
 VowelSignMap =  [
-                '\U000119D1',
-                '\U000119D2',
-                '\U000119D3',
-                '\U000119D4',
-                '\U000119D5',
-                '\U000119D6',
-                '\U000119D7',
-            '\U000119E0𑧉𑧔\u02BD', #lu
-            '\U000119E0𑧉𑧕\u02BD', #luu
-                '\U000119DA',
-                '\U000119DB',
-                '\U000119DC',
-                '\U000119DD',
+                '\U00011930',
+                '\U00011931',
+                '\U00011932',
+                '\U00011933',
+                '\U00011934',
+                '\U00011942\U00011933\u02BD',
+                '\U00011942\U00011934\u02BD',
+                '\U0001193E\U00011928\U00011933\u02BD',
+                '\U0001193E\U00011928\U00011934\u02BD',
+                '\U00011935',
+                '\U00011937',
+                '\U00011938',
+                '\U00011904\u02BD',
                 ]
 
 SouthVowelSignMap = [
-                '\U000119DA\u02BD',
-                '\U000119DC\u02BD',
+                    '\U00011935\u02BD',
+                    '\U00011938\u02BD',
                     ]
 
 ModernVowelSignMap =[
-                    '\U000119D1\u02BD',
-                    '\U000119DA\u02BD']
+                    '\U00011935\u02BD',
+                    '\U00011930\u02BD']
 
 SinhalaVowelSignMap = [
-                '\U000119DA\u02BD',
+                      '\U00011935\u02BD'
                       ]
 
 AyogavahaMap = [
-               '\U000119DE\u02BD',
-               '\U000119DE',
-               '\U000119DF'
+               '\U0001193C',
+               '\U0001193B',
+               '\U0001192D\U0001193D\u02BD'
                ]
 
 ViramaMap =  [
-             '\U000119E0'
+             '\U0001193D'
              ]
 
 ConsonantMap =  [
-                '\U000119AE',
-                '\U000119AF',
-                '\U000119B0',
-                '\U000119B1',
-                '\U000119B2',
-
-                '\U000119B3',
-                '\U000119B4',
-                '\U000119B5',
-                '\U000119B6',
-                '\U000119B7',
-
-                '\U000119B8',
-                '\U000119B9',
-                '\U000119BA',
-                '\U000119BB',
-                '\U000119BC',
-
-                '\U000119BD',
-                '\U000119BE',
-                '\U000119BF',
-                '\U000119C0',
-                '\U000119C1',
-
-                '\U000119C2',
-                '\U000119C3',
-                '\U000119C4',
-                '\U000119C5',
-                '\U000119C6',
-
-                '\U000119C7',
-                '\U000119C8',
-                '\U000119C9',
-                '\U000119CA',
-
-                '\U000119CB',
-                '\U000119CC',
-                '\U000119CD',
-                '\U000119CE'
+                '\U0001190C',
+                '\U0001190D',
+                '\U0001190E',
+                '\U0001190F',
+                '\U00011910',
+
+                '\U00011911',
+                '\U00011912',
+                '\U00011913',
+                '\U00011913\u02BD',
+                '\U00011915',
+
+                '\U00011916',
+                '\U00011916\u02BD',
+                '\U00011918',
+                '\U00011919',
+                '\U0001191A',
+
+                '\U0001191B',
+                '\U0001191C',
+                '\U0001191D',
+                '\U0001191E',
+                '\U0001191F',
+
+                '\U00011920',
+                '\U00011921',
+                '\U00011922',
+                '\U00011923',
+                '\U00011924',
+
+                '\U00011925',
+                '\U00011927',
+                '\U00011928',
+                '\U00011929',
+
+                '\U0001192A',
+                '\U0001192B',
+                '\U0001192C',
+                '\U0001192D'
                 ]
 
 SouthConsonantMap = [
-                    '\U000119CF\u02BD',
-                    '\U000119CF',
-                    '\U000119D0',
-                    '\U000119C1\u02BD'
+                    '\U0001192E',
+                    '\U0001192E\U00011943',
+                    '\U00011927\U00011943',
+                    '\U0001191F\U00011943'
                     ]
 
 NuktaConsonantMap =  [
-                     '\U000119AE\u02BD',
-                     '\U000119AF\u02BD',
-                     '\U000119B0\u02BD',
-                     '\U000119B5\u02BD',
-                     '\U000119BA\u02BD',
-                     '\U000119BB\u02BD',
-                     '\U000119C3\u02BD',
-                     '\U000119C7\u02BD'
+                     '\U0001190C\U00011943',
+                     '\U0001190D\U00011943',
+                     '\U0001190E\U00011943',
+                     '\U0001192F',
+                     '\U00011918\U00011943',
+                     '\U00011919\U00011943',
+                     '\U00011921\U00011943',
+                     '\U00011925\U00011943'
                      ]
 
 SinhalaConsonantMap =[
-                     '\U000119DE\u02BD\U000119B0',
-                     '\U000119DE\u02BD\U000119B5',
-                     '\U000119DE\u02BD\U000119BA',
-                     '\U000119DE\u02BD\U000119BF',
-                     '\U000119DE\u02BD\U000119C4',
+                     '\U0001193F\U0001190E\u02BD',
+                     '\U0001193F\U00011913\u02BD',
+                     '\U0001193F\U00011918\u02BD',
+                     '\U0001193F\U0001191D\u02BD',
+                     '\U0001193F\U00011922\u02BD',
                       ]
 
 NuktaMap = [
-           '\u02BD\u02BD'
+           '\U00011943'
            ]
 
 OmMap = [
-        '\U000119AC\U000119DE'
+        '\U00011909\U0001193C'
         ]
 
 SignMap =[
-         '\U000119E1',
-         '\u0964',
-         '\u0965'
+         '\u02BD\u02BD\u02BD',
+         '\U00011946\u02BD',
+         '\U00011946'
          ]
 
 Aytham =[AyogavahaMap[2]+'\u02BD']
 
+
 NumeralMap = [
-             '\u0CE6',
-             '\u0CE7',
-             '\u0CE8',
-             '\u0CE9',
-             '\u0CEA',
-             '\u0CEB',
-             '\u0CEC',
-             '\u0CED',
-             '\u0CEE',
-             '\u0CEF'
+             '\U00011950',
+             '\U00011951',
+             '\U00011952',
+             '\U00011953',
+             '\U00011954',
+             '\U00011955',
+             '\U00011956',
+             '\U00011957',
+             '\U00011958',
+             '\U00011959',
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/Newa.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Newa.py`

 * *Files 14% similar despite different names*

```diff
@@ -164,7 +164,13 @@
              '\U00011454',
              '\U00011455',
              '\U00011456',
              '\U00011457',
              '\U00011458',
              '\U00011459'
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/Oriya.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/TamilGrantha.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,170 +1,176 @@
 # -*- coding: utf-8 -*-
 
 # Script Mapping for Devanagari
 
 VowelMap =  [
-            '\u0B05',
-            '\u0B06',
-            '\u0B07',
-            '\u0B08',
-            '\u0B09',
-            '\u0B0A',
-            '\u0B0B',
-            '\u0B60',
-            '\u0B0C',
-            '\u0B61',
-            '\u0B0F',
-            '\u0B10',
-            '\u0B13',
-            '\u0B14',
+            '\u0B85',
+            '\u0B86',
+            '\u0B87',
+            '\u0B88',
+            '\u0B89',
+            '\u0B8A',
+            '\u098B',
+            '\u09E0',
+            '\u098C',
+            '\u09E1',
+            '\u0B8F',
+            '\u0B90',
+            '\u0B93',
+            '\u0B94',
             ]
 
 SouthVowelMap = [
-                '\u0B0F\u02D8',
-                '\u0B13\u02D8',
+                '\u0B8E',
+                '\u0B92',
                 ]
 
 ModernVowelMap = [
-                 '\u0B0F\u02BC',
-                 '\u0B06\u02BC',
+                 '\u0B8E\u02BC',
+                 '\u0B86\u02BC',
                  ]
 
 SinhalaVowelMap = [
-                  '\u0B0F\u02C7'
+                  '\u0B8F\u02C7'
                   ]
-    
+
 VowelSignMap =  [
-                '\u0B3E',
-                '\u0B3F',
-                '\u0B40',
-                '\u0B41',
-                '\u0B42',
-                '\u0B43',
-                '\u0B44',
-                '\u0B62',
-                '\u0B63',
-                '\u0B47',
-                '\u0B48',
-                '\u0B4B',
-                '\u0B4C',
+                '\u0BBE',
+                '\u0BBF',
+                '\u0BC0',
+                '\u0BC1',
+                '\u0BC2',
+                '\u09C3',
+                '\u09C4',
+                '\u09E2',
+                '\u09E3',
+                '\u0BC7',
+                '\u0BC8',
+                '\u0BCB',
+                '\u0BCC',
                 ]
 
 SouthVowelSignMap = [
-                    '\u0B47\u02D8',
-                    '\u0B4B\u02D8',
+                    '\u0BC6',
+                    '\u0BCA',
                     ]
 
 ModernVowelSignMap =[
-                    '\u0B47\u02BC',
-                    '\u0B3E\u02BC']
+                    '\u0BC6\u02BC',
+                    '\u0BBE\u02BC']
 
 SinhalaVowelSignMap = [
-                      '\u0B47\u02C7'
+                      '\u0BC7\u02C7'
                       ]
 
 AyogavahaMap = [
-               '\u0B01',
-               '\u0B02',
-               '\u0B03'
+               '\u0981',
+               '\u0982',
+               '\u0983'
                ]
-    
+
 ViramaMap =  [
-             '\u0B4D'
+             '\u0BCD'
              ]
 
 ConsonantMap =  [
-                '\u0B15',
-                '\u0B16',
-                '\u0B17',
-                '\u0B18',
-                '\u0B19',
-                
-                '\u0B1A',
-                '\u0B1B',
-                '\u0B1C',
-                '\u0B1D',
-                '\u0B1E',
-                
-                '\u0B1F',
-                '\u0B20',
-                '\u0B21',
-                '\u0B22',
-                '\u0B23',
-                
-                '\u0B24',
-                '\u0B25',
-                '\u0B26',
-                '\u0B27',
-                '\u0B28',
-                
-                '\u0B2A',
-                '\u0B2B',
-                '\u0B2C',
-                '\u0B2D',
-                '\u0B2E',
-                
-                '\u0B2F',
-                '\u0B30',
-                '\u0B32',
-                '\u0B71',
-                
-                '\u0B36',
-                '\u0B37',
-                '\u0B38',
-                '\u0B39'
+                '\u0B95',
+                '\u0996',
+                '\u0997',
+                '\u0998',
+                '\u0B99',
+
+                '\u0B9A',
+                '\u099B',
+                '\u0B9C',
+                '\u099D',
+                '\u0B9E',
+
+                '\u0B9F',
+                '\u09A0',
+                '\u09A1',
+                '\u09A2',
+                '\u0BA3',
+
+                '\u0BA4',
+                '\u09A5',
+                '\u09A6',
+                '\u09A7',
+                '\u0BA8',
+
+                '\u0BAA',
+                '\u09AB',
+                '\u09AC',
+                '\u09AD',
+                '\u0BAE',
+
+                '\u0BAF',
+                '\u0BB0',
+                '\u0BB2',
+                '\u0BB5',
+
+                '\u0BB6',
+                '\u0BB7',
+                '\u0BB8',
+                '\u0BB9'
                 ]
 
 SouthConsonantMap = [
-                    '\u0B33',
-                    '\u0B33\u0B3C',
-                    '\u0B30\u0B3C',
-                    '\u0B28\u0B3C'
+                    '\u0BB3',
+                    '\u0BB4',
+                    '\u0BB1',
+                    '\u0BA9'
                     ]
 
 NuktaConsonantMap =  [
-                     '\u0B15\u0B3C',
-                     '\u0B16\u0B3C',
-                     '\u0B17\u0B3C',
-                     '\u0B1C\u0B3C',
-                     '\u0B5C',
-                     '\u0B5D',
-                     '\u0B2B\u0B3C',
-                     '\u0B5F'
+                     '\u0B95\u09BC',
+                     '\u0996\u09BC',
+                     '\u0997\u09BC',
+                     '\u0B9C\u09BC',
+                     '\u09A1\u09BC',
+                     '\u09A2\u09BC',
+                     '\u09AB\u09BC',
+                     '\u0BAF\u09BC'
                      ]
 
 SinhalaConsonantMap =[
-                     '\u0B01\u02C6\u0B17',
-                     '\u0B01\u02C6\u0B1C',
-                     '\u0B01\u02C6\u0B21',
-                     '\u0B01\u02C6\u0B26',
-                     '\u0B01\u02C6\u0B2C',
+                     '\u0B99\u0BCD\u02C6\u0997',
+                     '\u0B9E\u0BCD\u02C6\u0B9C',
+                     '\u0BA3\u0BCD\u02C6\u09A1',
+                     '\u0BA8\u0BCD\u02C6\u09A6',
+                     '\u0BAE\u0BCD\u02C6\u09AC',
                       ]
 
 NuktaMap = [
-           '\u0B3C'
+           '\u09BC'
            ]
-    
+
 OmMap = [
-        '\u0B13\u0B01'
+        '\u0BD0'
         ]
 
 SignMap =[
-         '\u0B3D',
+         '\u09BD',
          '\u0964',
          '\u0965'
          ]
 
 Aytham =[AyogavahaMap[2]+'\u02BC']
 
 NumeralMap = [
-             '\u0B66',
-             '\u0B67',
-             '\u0B68',
-             '\u0B69',
-             '\u0B6A',
-             '\u0B6B',
-             '\u0B6C',
-             '\u0B6D',
-             '\u0B6E',
-             '\u0B6F'
+             '\u09E6',
+             '\u09E7',
+             '\u09E8',
+             '\u09E9',
+             '\u09EA',
+             '\u09EB',
+             '\u09EC',
+             '\u09ED',
+             '\u09EE',
+             '\u09EF'
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/Ranjana.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/SyriacMalayalam.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 # Script Mapping for Devanagari
 
 VowelMap =  [
-            '\u0905',
-            '\u0906',
+            'ܐܲ',
+            'ܐܵ',
             '\u0907',
             '\u0908',
             '\u0909',
             '\u090A',
             '\u090B',
             '\u0960',
             '\u090C',
@@ -16,25 +16,25 @@
             '\u090F',
             '\u0910',
             '\u0913',
             '\u0914',
             ]
 
 SouthVowelMap = [
-                '\u090F\u02BD',
-                '\u0913\u02BD',
+                '\u090E',
+                '\u0912',
                 ]
 
 ModernVowelMap = [
-                '\u090F\u02BD',
-                '\u0906\u02BD',
+                 '\u090D',
+                 '\u0911',
                  ]
 
 SinhalaVowelMap = [
-                '\u090F\u02BD',
+                  'एॕ'
                   ]
 
 VowelSignMap =  [
                 '\u093E',
                 '\u093F',
                 '\u0940',
                 '\u0941',
@@ -46,25 +46,24 @@
                 '\u0947',
                 '\u0948',
                 '\u094B',
                 '\u094C',
                 ]
 
 SouthVowelSignMap = [
-                    '\u0947\u02BD',
-                    '\u094B\u02BD',
+                    '\u0946',
+                    '\u094A',
                     ]
 
 ModernVowelSignMap =[
-                    '\u0947\u02BD',
-                    '\u093E\u02BD',
-                    ]
+                    '\u0945',
+                    '\u0949']
 
 SinhalaVowelSignMap = [
-                    '\u0947\u02BD',
+                      'ॕ'
                       ]
 
 AyogavahaMap = [
                '\u0901',
                '\u0902',
                '\u0903'
                ]
@@ -112,37 +111,37 @@
                 '\u0936',
                 '\u0937',
                 '\u0938',
                 '\u0939'
                 ]
 
 SouthConsonantMap = [
-                    'ल\u02BD',
-                    'ल\u02BD',
-                    '\u0930\u02BD',
-                    '\u0928\u02BD'
+                    '\u0933',
+                    '\u0934',
+                    '\u0931',
+                    '\u0929'
                     ]
 
 NuktaConsonantMap =  [
-                    '\u0915\u02BD',
-                    '\u0916\u02BD',
-                    '\u0917\u02BD',
-                     '\u091C\u02BD',
-                '\u0921\u02BD',
-                '\u0922\u02BD',
-                     '\u092B\u02BD',
-                     '\u092F\u02BD'
+                     '\u0958',
+                     '\u0959',
+                     '\u095A',
+                     '\u095B',
+                     '\u095C',
+                     '\u095D',
+                     '\u095E',
+                     '\u095F'
                      ]
 
 SinhalaConsonantMap =[
-                     '\u0901\u02BD\u0917',
-                     '\u0901\u02BD\u091C',
-                     '\u0901\u02BD\u0921',
-                     '\u0901\u02BD\u0926',
-                     '\u0901\u02BD\u092C',
+                     '\u0901\u02C6\u0917',
+                     '\u0901\u02C6\u091C',
+                     '\u0901\u02C6\u0921',
+                     '\u0901\u02C6\u0926',
+                     '\u0901\u02C6\u092C',
                       ]
 
 NuktaMap = [
            '\u093C'
            ]
 
 OmMap = [
@@ -151,21 +150,27 @@
 
 SignMap =[
          '\u093D',
          '\u0964',
          '\u0965'
          ]
 
-Aytham =[AyogavahaMap[2]+'\u02BD']
+Aytham =[AyogavahaMap[2]+'\u02BC']
 
 NumeralMap = [
              '\u0966',
              '\u0967',
              '\u0968',
              '\u0969',
              '\u096A',
              '\u096B',
              '\u096C',
              '\u096D',
              '\u096E',
              '\u096F'
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/Saurashtra.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/SylotiNagri.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,171 +1,177 @@
 # -*- coding: utf-8 -*-
 
 # Script Mapping for Devanagari
 
 VowelMap =  [
-            '\uA882',
-            '\uA883',
-            '\uA884',
-            '\uA885',
-            '\uA886',
-            '\uA887',
-            '\uA888',
-            '\uA889',
-            '\uA88A',
-            '\uA88B',
-            '\uA88D',
-            '\uA88E',
-            '\uA890',
-            '\uA891',
+            '\uA805',
+            '\uA800',
+            '\uA801',
+            '\uA801\u02BD',
+            '\uA803',
+            '\uA803\u02BD',
+            'ꠞꠤ\u02BD',
+            'ꠞꠤ\u02BD',
+            'ꠟꠤ\u02BD',
+            'ꠟꠤ\u02BD',
+            '\uA804',
+            '\uA805\uA802',
+            '\uA805\u02BD',
+            '\uA805\uA803',
             ]
 
 SouthVowelMap = [
-                '\uA88C',
-                '\uA88F',
+                '\uA804\u02BD',
+                '\uA805\u02BD',
                 ]
 
 ModernVowelMap = [
-                 '\uA88C\u02BD',
-                 '\uA883\u02BD',
+                 '\uA804\u02BD',
+                 '\uA800\u02BD',
                  ]
 
 SinhalaVowelMap = [
-                  '\uA88C\u02BD'
+                  '\uA804\u02BD'
                   ]
 
 VowelSignMap =  [
-                '\uA8B5',
-                '\uA8B6',
-                '\uA8B7',
-                '\uA8B8',
-                '\uA8B9',
-                '\uA8BA',
-                '\uA8BB',
-                '\uA8BC',
-                '\uA8BD',
-                '\uA8BF',
-                '\uA8C0',
-                '\uA8C2',
-                '\uA8C3',
+                '\uA823',
+                '\uA824',
+                '\uA824\u02BD',
+                '\uA825',
+                '\uA825\u02BD',
+                '\uA806ꠞꠤ\u02BD',
+                '\uA806ꠞꠤ\u02BD',
+                '\uA806ꠟꠤ\u02BD',
+                '\uA806ꠟꠤ\u02BD',
+                '\uA826',
+                '\uA802',
+                '\uA827',
+                '\uA803\u02BD\u02BD',
                 ]
 
 SouthVowelSignMap = [
-                    '\uA8BE',
-                    '\uA8C1',
+                    '\uA826\u02BD',
+                    '\uA827\u02BD',
                     ]
 
 ModernVowelSignMap =[
-                    '\uA8BE\u02BD',
-                    '\uA8B5\u02BD']
+                    '\uA826\u02BD',
+                    '\uA823\u02BD']
 
 SinhalaVowelSignMap = [
-                      '\uA8BF\u02BD'
+                      '\uA826\u02BD'
                       ]
 
 AyogavahaMap = [
-               '\uA8C5',
-               '\uA880',
-               '\uA881'
+               '\uA80B\u02BD',
+               '\uA80B',
+               'ꠢ꠆\u02BD'
                ]
 
 ViramaMap =  [
-             '\uA8C4'
+             '\uA806'
              ]
 
 ConsonantMap =  [
-                '\uA892',
-                '\uA893',
-                '\uA894',
-                '\uA895',
-                '\uA896',
-
-                '\uA897',
-                '\uA898',
-                '\uA899',
-                '\uA89A',
-                '\uA89B',
-
-                '\uA89C',
-                '\uA89D',
-                '\uA89E',
-                '\uA89F',
-                '\uA8A0',
-
-                '\uA8A1',
-                '\uA8A2',
-                '\uA8A3',
-                '\uA8A4',
-                '\uA8A5',
-
-                '\uA8A6',
-                '\uA8A7',
-                '\uA8A8',
-                '\uA8A9',
-                '\uA8AA',
-
-                '\uA8AB',
-                '\uA8AC',
-                '\uA8AD',
-                '\uA8AE',
-
-                '\uA8AF',
-                '\uA8B0',
-                '\uA8B1',
-                '\uA8B2'
+                '\uA807',
+                '\uA808',
+                '\uA809',
+                '\uA80A',
+                '\uA818\u02BD',
+
+                '\uA80C',
+                '\uA80D',
+                '\uA80E',
+                '\uA80F',
+                '\uA818\u02BD',
+
+                '\uA810',
+                '\uA811',
+                '\uA812',
+                '\uA813',
+                '\uA818\u02BD',
+
+                '\uA814',
+                '\uA815',
+                '\uA816',
+                '\uA817',
+                '\uA818',
+
+                '\uA819',
+                '\uA81A',
+                '\uA81B',
+                '\uA81C',
+                '\uA81D',
+
+                'ꠎ\u02BD',
+                '\uA81E',
+                '\uA81F',
+                'ꠛ\u02BD',
+
+                '\uA821\u02BD',
+                '\uA821\u02BD',
+                '\uA821',
+                '\uA822',
                 ]
 
 SouthConsonantMap = [
-                    '\uA8B3',
-                    '\uA8B3\u02BD',
-                    '\uA8AC\u02BD',
-                    '\uA8A5\u02BD'
+                    '\uA81F\u02BD',
+                    '\uA81F\u02BD',
+                    '\uA81E\u02BD',
+                    '\uA818\u02BD',
                     ]
 
 NuktaConsonantMap =  [
-                     '\uA892\u02BD',
-                     '\uA893\u02BD',
-                     '\uA894\u02BD',
-                     '\uA899\u02BD',
-                     '\uA89E\u02BD',
-                     '\uA89F\u02BD',
-                     '\uA8A7\u02BD',
-                     '\uA8AB\u02BD'
+                     'ꠇ\u02BD',
+                     'ꠈ\u02BD',
+                     'ꠉ\u02BD',
+                     'ꠎ\u02BD',
+                     'ꠠ',
+                     'ꠓ\u02BD',
+                     'ꠚ\u02BD',
+                     'ꠎ\u02BD'
                      ]
 
 SinhalaConsonantMap =[
-                     '\uA880\u02BD\uA894',
-                     '\uA880\u02BD\uA899',
-                     '\uA880\u02BD\uA89E',
-                     '\uA880\u02BD\uA8A3',
-                     '\uA880\u02BD\uA8A8',
+                     'ꠋꠉ\u02BD',
+                     'ꠋꠎ\u02BD',
+                     'ꠋꠒ\u02BD',
+                     'ꠋꠖ\u02BD',
+                     'ꠋꠛ\u02BD',
                       ]
 
 NuktaMap = [
-           '\u02BD\u02BD\u02BD\u02BD'
+           '\u02BD\u02BD\u02BD'
            ]
 
 OmMap = [
-        '\uA890\uA880'
+        'ꠅꠋ'
         ]
 
 SignMap =[
-         '\u0C3D',
-         '\uA8CE',
-         '\uA8CF'
+         '\u09BD',
+         '\u0964',
+         '\u0965'
          ]
 
-Aytham =[AyogavahaMap[2]+'\u02BC']
+Aytham =[AyogavahaMap[2]+'\u02BD']
 
 
 NumeralMap = [
-             '\uA8D0',
-             '\uA8D1',
-             '\uA8D2',
-             '\uA8D3',
-             '\uA8D4',
-             '\uA8D5',
-             '\uA8D6',
-             '\uA8D7',
-             '\uA8D8',
-             '\uA8D9'
+             '\u09E6',
+             '\u09E7',
+             '\u09E8',
+             '\u09E9',
+             '\u09EA',
+             '\u09EB',
+             '\u09EC',
+             '\u09ED',
+             '\u09EE',
+             '\u09EF'
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/Shahmukhi.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Shahmukhi.py`

 * *Files 18% similar despite different names*

```diff
@@ -166,7 +166,13 @@
              '\u06F4',
              '\u06F5',
              '\u06F6',
              '\u06F7',
              '\u06F8',
              '\u06F9',
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/Sharada.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Sharada.py`

 * *Files 11% similar despite different names*

```diff
@@ -165,7 +165,13 @@
              '\U000111D4',
              '\U000111D5',
              '\U000111D6',
              '\U000111D7',
              '\U000111D8',
              '\U000111D9'
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/SiddhamDevanagari.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/NonIndic/Hebrew.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,171 +1,176 @@
 # -*- coding: utf-8 -*-
 
-# Script Mapping for Devanagari
+# Script Mapping for ISO
 
 VowelMap =  [
-            '\u0905',
-            '\u0906',
-            '\u0907',
-            '\u0908',
-            '\u0909',
-            '\u090A',
-            '\u090B',
-            '\u0960',
-            '\u090C',
-            '\u0961',
-            '\u090F',
-            '\u0910',
-            '\u0913',
-            '\u0914',
+            'א' + '\u05B7',
+            'א' + '\u05B8',
+            'א' + '\u05B4',
+            'א' + '\u05B4\u05D9',
+            'א' + '\u05BB',
+            'א' + 'וּ' + '',
+            'רֻ' + '\u02BD',
+            'רוּ' + '\u02BD',
+            'לֻ' + '\u02BD',
+            'לוּ' + '\u02BD',
+            'א' + '\u05B5',
+            'א' + '\u05B7' + 'ײ' + '\u05B0' + '\u02BD',
+            'א' + '\u05D5\u05B9'  + '',
+            'א' + '\u05B7' + 'ו'  + '\u05B0' + '\u02BD',
             ]
 
 SouthVowelMap = [
-                '\u090F\u02BD',
-                '\u0913\u02BD',
+            'א' + '\u05B6',
+            'א' + '\u05B9',
                 ]
 
 ModernVowelMap = [
-                '\u090F\u02BD',
-                '\u0906\u02BD',
+            'א' + '\u05B8\u02BD',
+            'א' + '\u05B9\u02BD',
                  ]
 
 SinhalaVowelMap = [
-                '\u090F\u02BD',
+            'א' + '\u05B5\u02BD',
                   ]
 
 VowelSignMap =  [
-                '\u093E',
-                '\u093F',
-                '\u0940',
-                '\u0941',
-                '\u0942',
-                '\u0943',
-                '\u0944',
-                '\u0962',
-                '\u0963',
-                '\u0947',
-                '\u0948',
-                '\u094B',
-                '\u094C',
+                '\u05B8',
+                '\u05B4',
+                '\u05B4\u05D9',
+                '\u05BB',
+                'וּ',
+                '\u05B0' + 'רֻ' + '\u02BD',
+                '\u05B0' + 'רוּ' + '\u02BD',
+                '\u05B0' + 'לֻ' + '\u02BD',
+                '\u05B0' 'לוּ' + '\u02BD',
+                '\u05B5',
+                '\u05B7' + 'ײ' + '\u05B0' + '\u02BD',
+                '\u05D5\u05B9',
+                '\u05B7' + 'ו' + '\u05B0' + '\u02BD',
                 ]
 
 SouthVowelSignMap = [
-                    '\u0947\u02BD',
-                    '\u094B\u02BD',
+                    '\u05B6',
+                    '\u05B9',
                     ]
 
 ModernVowelSignMap =[
-                    '\u0947\u02BD',
-                    '\u093E\u02BD',
-                    ]
+                    '\u05B8\u02BD',
+                    '\u05B9\u02BD']
 
 SinhalaVowelSignMap = [
-                    '\u0947\u02BD',
+                      '\u05B5\u02BD'
                       ]
 
 AyogavahaMap = [
-               '\u0901',
-               '\u0902',
-               '\u0903'
+               'מְ' + '\u02BC',
+               'מְ' + '\u02BC',
+               'הְּ'  + '\u02BD'
                ]
 
 ViramaMap =  [
-             '\u094D'
+             '\u05B0'
              ]
 
 ConsonantMap =  [
-                '\u0915',
-                '\u0916',
-                '\u0917',
-                '\u0918',
-                '\u0919',
-
-                '\u091A',
-                '\u091B',
-                '\u091C',
-                '\u091D',
-                '\u091E',
-
-                '\u091F',
-                '\u0920',
-                '\u0921',
-                '\u0922',
-                '\u0923',
-
-                '\u0924',
-                '\u0925',
-                '\u0926',
-                '\u0927',
-                '\u0928',
-
-                '\u092A',
-                '\u092B',
-                '\u092C',
-                '\u092D',
-                '\u092E',
-
-                '\u092F',
-                '\u0930',
-                '\u0932',
-                '\u0935',
-
-                '\u0936',
-                '\u0937',
-                '\u0938',
-                '\u0939'
+                'כּ',
+                'כ\u02BD',
+                'ג',
+                'ג\u02BD',
+                'נ\u02BD',
+
+                'צ׳',
+                'צ׳\u02BD',
+                'ג׳',
+                'ג׳\u02BD',
+                'נ\u02BD',
+
+                'ט\u02BD',
+                'ט\u02BD',
+                'ד\u02BD',
+                'ד\u02BD',
+                'נ\u02BD',
+
+                'ט',
+                'ט\u02BD',
+                'ד',
+                'ד\u02BD',
+                'נ',
+
+                'פּ',
+                'פּ\u02BD',
+                'בּ',
+                'בּ\u02BD',
+                'מ',
+
+                'ײ',
+                'ר',
+                'ל',
+                'װ',
+
+                'שׁ\u02BD',
+                'שׁ',
+                'ס',
+                'ה',
                 ]
 
 SouthConsonantMap = [
-                    'ल़',
-                    'ष़',
-                    '\u0931',
-                    '\u0929'
+                    'ל\u02BD',
+                    'ל\u02BD',
+                    'ר\u02BD',
+                    'נ\u02BD'
                     ]
 
 NuktaConsonantMap =  [
-                     '\u0958',
-                     '\u0959',
-                     '\u095A',
-                     '\u095B',
-                     '\u095C',
-                     '\u095D',
-                     '\u095E',
-                     '\u095F'
+                     'ק',
+                     'כ',
+                     'גּ',
+                     'ז',
+                     'ד\u02BD',
+                     'ד\u02BD',
+                     'פ',
+                     'ײ\u02BD'
                      ]
 
 SinhalaConsonantMap =[
-                     '\u0901\u02BD\u0917',
-                     '\u0901\u02BD\u091C',
-                     '\u0901\u02BD\u0921',
-                     '\u0901\u02BD\u0926',
-                     '\u0901\u02BD\u092C',
+                     'נְגַ\u02BD',
+                     'נְגַ׳\u02BD',
+                     'נְדַ\u02BD',
+                     'נְדַ\u02BD',
+                     'מְבַּ\u02BD',
                       ]
 
 NuktaMap = [
-           '\u093C'
+           '\u02BE'
            ]
 
 OmMap = [
-        '\u0950'
+        'א' + 'וֹמְ'  + '\u02BD'
         ]
 
 SignMap =[
-         '\u093D',
-         '\u0964',
-         '\u0965'
+         '\u0027\u02BD',
+         '\u002E',
+         '\u002E\u002E'
          ]
 
-Aytham =[AyogavahaMap[2]+'\u02BD']
+Aytham =['הְ' + '\u02BD']
 
 NumeralMap = [
-             '\u0966',
-             '\u0967',
-             '\u0968',
-             '\u0969',
-             '\u096A',
-             '\u096B',
-             '\u096C',
-             '\u096D',
-             '\u096E',
-             '\u096F'
+             '\u0030',
+             '\u0031',
+             '\u0032',
+             '\u0033',
+             '\u0034',
+             '\u0035',
+             '\u0036',
+             '\u0037',
+             '\u0038',
+             '\u0039',
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/Sinhala.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/ShanLoCRomanLoC.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,170 +1,155 @@
 # -*- coding: utf-8 -*-
 
-# Script Mapping for Devanagari
+# Script Mapping for ISO
 
 VowelMap =  [
-            '\u0D85',
-            '\u0D86',
-            '\u0D89',
-            '\u0D8A',
-            '\u0D8B',
-            '\u0D8C',
-            '\u0D8D',
-            '\u0D8E',
-            '\u0D8F',
-            '\u0D90',
-            '\u0D92',
-            '\u0D93',
-            '\u0D95',
-            '\u0D96',
+            '\u0061',
+            '\u0101',
+            '\u0069',
+            '\u012B',
+            '\u0075',
+            '\u016B',
+            '\u1E5B',
+            '\u1E5D',
+            '\u1E37',
+            '\u1E39',
+            '\u0065',
+            '\u0061\u0069',
+            '\u006F',
+            '\u0061\u0075'
             ]
 
 SouthVowelMap = [
-                '\u0D91',
-                '\u0D94',
+                '\u0115',
+                '\u014F',
                 ]
 
 ModernVowelMap = [
-                 '\u0D87',
-                 '\u0D86\u02BC',
+                 'è',
+                 '\u00F4',
                  ]
 
 SinhalaVowelMap = [
-                  '\u0D88'
+                  '\u01E3'
                   ]
-    
-VowelSignMap =  [
-                '\u0DCF',
-                '\u0DD2',
-                '\u0DD3',
-                '\u0DD4',
-                '\u0DD6',
-                '\u0DD8',
-                '\u0DF2',
-                '\u0DDF',
-                '\u0DF3',
-                '\u0DDA',
-                '\u0DDB',
-                '\u0DDD',
-                '\u0DDE',
-                ]
 
-SouthVowelSignMap = [
-                    '\u0DD9',
-                    '\u0DDC',
-                    ]
+VowelSignMap =  VowelMap[1:]
 
-ModernVowelSignMap =[
-                    '\u0DD0',
-                    '\u0DCF\u02BC']
+SouthVowelSignMap = SouthVowelMap[:]
 
-SinhalaVowelSignMap = [
-                      '\u0DD1'
-                      ]
+ModernVowelSignMap = ModernVowelMap[:]
+
+SinhalaVowelSignMap = SinhalaVowelMap[:]
 
 AyogavahaMap = [
-               '\u0D82\u02BC',
-               '\u0D82',
-               '\u0D83'
+               '\u006D\u0310\u02BD',
+               '\u1E43',
+               'ʺ'
                ]
-    
+
 ViramaMap =  [
-             '\u0DCA'
+             '\u00D7'
              ]
 
 ConsonantMap =  [
-                '\u0D9A',
-                '\u0D9B',
-                '\u0D9C',
-                '\u0D9D',
-                '\u0D9E',
-                
-                '\u0DA0',
-                '\u0DA1',
-                '\u0DA2',
-                '\u0DA3',
-                '\u0DA4',
-                
-                '\u0DA7',
-                '\u0DA8',
-                '\u0DA9',
-                '\u0DAA',
-                '\u0DAB',
-                
-                '\u0DAD',
-                '\u0DAE',
-                '\u0DAF',
-                '\u0DB0',
-                '\u0DB1',
-                
-                '\u0DB4',
-                '\u0DB5',
-                '\u0DB6',
-                '\u0DB7',
-                '\u0DB8',
-                
-                '\u0DBA',
-                '\u0DBB',
-                '\u0DBD',
-                '\u0DC0',
-                
-                '\u0DC1',
-                '\u0DC2',
-                '\u0DC3',
-                '\u0DC4'
+                '\u006B',
+                '\u006B\u0068',
+                '\u0067',
+                '\u0067\u0068',
+                '\u1E45',
+
+                '\u0063',
+                '\u0063\u0068',
+                'z',
+                '\u006A\u0068',
+                '\u00F1',
+
+                '\u1E6D',
+                '\u1E6D\u0068',
+                '\u1E0D',
+                '\u1E0D\u0068',
+                '\u1E47',
+
+                '\u0074',
+                '\u0074\u0068',
+                '\u0064',
+                '\u0064\u0068',
+                '\u006E',
+
+                '\u0070',
+                '\u0070\u0068',
+                '\u0062',
+                '\u0062\u0068',
+                '\u006D',
+
+                '\u0079',
+                '\u0072',
+                '\u006C',
+                '\u0076',
+
+                '\u015B',
+                '\u1E63',
+                '\u0073',
+                '\u0068',
                 ]
 
 SouthConsonantMap = [
-                    '\u0DC5',
-                    '\u0DC5\u00B7',
-                    '\u0DBB\u00B7',
-                    '\u0DB1\u00B7'
+                    'ḷ',
+                    '\u1E3B',
+                    '\u1E5F',
+                    '\u1E49'
                     ]
 
 NuktaConsonantMap =  [
-                     '\u0D9A\u00B7',
-                     '\u0D9B\u00B7',
-                     '\u0D9C\u00B7',
-                     '\u0DA2\u00B7',
-                     '\u0DA9\u00B7',
-                     '\u0DAA\u00B7',
-                     '\u0DC6',
-                     '\u0DBA\u00B7'
+                     '\u0071',
+                     '\u006B\u035F\u0068',
+                     '\u0121',
+                     '\u007A',
+                     '\u0072\u0324',
+                     '\u0072\u0324\u0068',
+                     '\u0066',
+                     '\u1E8F'
                      ]
 
 SinhalaConsonantMap =[
-                     '\u0D9F',
-                     '\u0DA6',
-                     '\u0DAC',
-                     '\u0DB3',
-                     '\u0DB9' 
+                     '\u006E\u0306\u0067',
+                     '\u006E\u0306\u006A',
+                     '\u006E\u0306\u1E0D',
+                     '\u006E\u0306\u0064',
+                     '\u006D\u0306\u0062',
                       ]
 
 NuktaMap = [
-           '\u00B7'
+           '\u0308'
            ]
-    
+
 OmMap = [
-        '\u0D95\u0D82'
+        '\u006F\u1E43'
         ]
 
 SignMap =[
-         '\u0028\u0D85\u0029',
-         '\u002E',
-         '\u002E\u002E'
+         '\u0027',
+         ',',
+         '.'
          ]
 
-Aytham =[AyogavahaMap[2]+'\u02BC']
+Aytham =['\u1E35']
 
 NumeralMap = [
              '\u0030',
              '\u0031',
              '\u0032',
              '\u0033',
              '\u0034',
              '\u0035',
              '\u0036',
              '\u0037',
              '\u0038',
              '\u0039',
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/SyriacMalayalam.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/EastIndic/TibetanLoC.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,170 +1,176 @@
 # -*- coding: utf-8 -*-
 
 # Script Mapping for Devanagari
 
 VowelMap =  [
-            'ܐܲ',
-            'ܐܵ',
-            '\u0907',
-            '\u0908',
-            '\u0909',
-            '\u090A',
-            '\u090B',
-            '\u0960',
-            '\u090C',
-            '\u0961',
-            '\u090F',
-            '\u0910',
-            '\u0913',
-            '\u0914',
+            '\u0F68',
+            '\u0F68\u0F71',
+            '\u0F68\u0F72',
+            '\u0F68\u0F71\u0F72',
+            '\u0F68\u0F74',
+            '\u0F68\u0F71\u0F74',
+            '\u0F62\u0F80',
+            '\u0F62\u0F71\u0F80',
+            '\u0F63\u0F80',
+            '\u0F63\u0F71\u0F80',
+            '\u0F68\u0F7A',
+            '\u0F68\u0F7B',
+            '\u0F68\u0F7C',
+            '\u0F68\u0F7D',
             ]
 
 SouthVowelMap = [
-                '\u090E',
-                '\u0912',
+                '\u0F68\u0F7A\u02BD',
+                '\u0F68\u0F7C\u02BD',
                 ]
 
 ModernVowelMap = [
-                 '\u090D',
-                 '\u0911',
+                 '\u0F68\u0F7A\u02BD',
+                 '\u0F68\u0F71\u02BD',
                  ]
 
 SinhalaVowelMap = [
-                  'एॕ'
+                  '\u0F68\u0F7A\u02BD'
                   ]
 
 VowelSignMap =  [
-                '\u093E',
-                '\u093F',
-                '\u0940',
-                '\u0941',
-                '\u0942',
-                '\u0943',
-                '\u0944',
-                '\u0962',
-                '\u0963',
-                '\u0947',
-                '\u0948',
-                '\u094B',
-                '\u094C',
+                 '\u0F71',
+                 '\u0F72',
+                 '\u0F71\u0F72',
+                 '\u0F74',
+                 '\u0F71\u0F74',
+                 '\u0FB2\u0F80',
+                 '\u0FB2\u0F71\u0F80',
+                 '\u0FB3\u0F80',
+                 '\u0FB3\u0F71\u0F80',
+                 '\u0F7A',
+                 '\u0F7B',
+                 '\u0F7C',
+                 '\u0F7D',
                 ]
 
 SouthVowelSignMap = [
-                    '\u0946',
-                    '\u094A',
+                    '\u0F7A\u02BD',
+                    '\u0F7C\u02BD',
                     ]
 
 ModernVowelSignMap =[
-                    '\u0945',
-                    '\u0949']
+                    '\u0F7A\u02BD',
+                    '\u0F71\u02BD']
 
 SinhalaVowelSignMap = [
-                      'ॕ'
+                      '\u0F7A\u02BD'
                       ]
 
 AyogavahaMap = [
-               '\u0901',
-               '\u0902',
-               '\u0903'
+               '\u0F83',
+               '\u0F7E',
+               '\u0F7F'
                ]
 
 ViramaMap =  [
-             '\u094D'
+             '\u0F84'
              ]
 
 ConsonantMap =  [
-                '\u0915',
-                '\u0916',
-                '\u0917',
-                '\u0918',
-                '\u0919',
-
-                '\u091A',
-                '\u091B',
-                '\u091C',
-                '\u091D',
-                '\u091E',
-
-                '\u091F',
-                '\u0920',
-                '\u0921',
-                '\u0922',
-                '\u0923',
-
-                '\u0924',
-                '\u0925',
-                '\u0926',
-                '\u0927',
-                '\u0928',
-
-                '\u092A',
-                '\u092B',
-                '\u092C',
-                '\u092D',
-                '\u092E',
-
-                '\u092F',
-                '\u0930',
-                '\u0932',
-                '\u0935',
-
-                '\u0936',
-                '\u0937',
-                '\u0938',
-                '\u0939'
+                '\u0F40',
+                '\u0F41',
+                '\u0F42',
+                '\u0F43',
+                '\u0F44',
+
+                'ཅ',
+                'ཆ',
+                'ཇ',
+                'ཇྷ',
+                '\u0F49',
+
+                '\u0F4A',
+                '\u0F4B',
+                '\u0F4C',
+                '\u0F4D',
+                '\u0F4E',
+
+                '\u0F4F',
+                '\u0F50',
+                '\u0F51',
+                '\u0F52',
+                '\u0F53',
+
+                '\u0F54',
+                '\u0F55',
+                '\u0F56',
+                '\u0F57',
+                '\u0F58',
+
+                '\u0F61',
+                '\u0F62',
+                '\u0F63',
+                '\u0F5D',
+
+                '\u0F64',
+                '\u0F65',
+                '\u0F66',
+                '\u0F67'
                 ]
 
 SouthConsonantMap = [
-                    '\u0933',
-                    '\u0934',
-                    '\u0931',
-                    '\u0929'
+                    '\u0F63\u0F39',
+                    '\u0F65\u0F39',
+                    '\u0F62\u0F39',
+                    '\u0F53\u0F39'
                     ]
 
 NuktaConsonantMap =  [
-                     '\u0958',
-                     '\u0959',
-                     '\u095A',
-                     '\u095B',
-                     '\u095C',
-                     '\u095D',
-                     '\u095E',
-                     '\u095F'
+                     'ཙ',
+                     'ཚ',
+                     'ཛ',
+                     'ཛྷ',
+                     'འ',
+                     'ཞ',
+                     'ཟ',
+                     '\u0F61༹'
                      ]
 
 SinhalaConsonantMap =[
-                     '\u0901\u02C6\u0917',
-                     '\u0901\u02C6\u091C',
-                     '\u0901\u02C6\u0921',
-                     '\u0901\u02C6\u0926',
-                     '\u0901\u02C6\u092C',
+                     '\u0F83\u0F40\u02BD',
+                     '\u0F83\u0F5B\u02BD',
+                     '\u0F83\u0F4C\u02BD',
+                     '\u0F83\u0F51\u02BD',
+                     '\u0F83\u0F56\u02BD',
                       ]
 
 NuktaMap = [
-           '\u093C'
+           '༹'
            ]
 
 OmMap = [
-        '\u0950'
+        '\u0F00'
         ]
 
 SignMap =[
-         '\u093D',
-         '\u0964',
-         '\u0965'
+         '\u0F85',
+         '\u0F0D',
+         '\u0F0E'
          ]
 
-Aytham =[AyogavahaMap[2]+'\u02BC']
+Aytham =[AyogavahaMap[2]+'\u02BD']
 
 NumeralMap = [
-             '\u0966',
-             '\u0967',
-             '\u0968',
-             '\u0969',
-             '\u096A',
-             '\u096B',
-             '\u096C',
-             '\u096D',
-             '\u096E',
-             '\u096F'
+             '\u0F20',
+             '\u0F21',
+             '\u0F22',
+             '\u0F23',
+             '\u0F24',
+             '\u0F25',
+             '\u0F26',
+             '\u0F27',
+             '\u0F28',
+             '\u0F29'
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/Takri.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Takri.py`

 * *Files 15% similar despite different names*

```diff
@@ -165,7 +165,13 @@
              '\U000116C4',
              '\U000116C5',
              '\U000116C6',
              '\U000116C7',
              '\U000116C8',
              '\U000116C9'
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/Tamil.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Tamil.py`

 * *Files 18% similar despite different names*

```diff
@@ -164,7 +164,13 @@
              '\u0BEA',
              '\u0BEB',
              '\u0BEC',
              '\u0BED',
              '\u0BEE',
              '\u0BEF'
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/TamilBrahmi.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/TamilBrahmi.py`

 * *Files 14% similar despite different names*

```diff
@@ -165,7 +165,13 @@
              '\u0034',
              '\u0035',
              '\u0036',
              '\u0037',
              '\u0038',
              '\u0039',
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/TamilExtended.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/GreekModern.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,170 +1,155 @@
 # -*- coding: utf-8 -*-
 
-# Script Mapping for Devanagari
+# Script Mapping for ISO
 
 VowelMap =  [
-            '\u0D05',
-            '\u0D06',
-            '\u0D07',
-            '\u0D08',
-            '\u0D09',
-            '\u0D0A',
-            '\u0D0B',
-            '\u0D60',
-            '\u0D0C',
-            '\u0D61',
-            '\u0D0F',
-            '\u0D10',
-            '\u0D13',
-            '\u0D14',
+            '\u0061',
+            '\u0041',
+            '\u0069',
+            '\u0049',
+            '\u0075',
+            '\u0055',
+            '\u0052',
+            '\u0052\u0052',
+            '\u006C\u0052',
+            '\u006C\u0052\u0052',
+            '\u0065',
+            '\u0061\u0069',
+            '\u006F',
+            '\u0061\u0075'
             ]
 
 SouthVowelMap = [
-                '\u0D0E',
-                '\u0D12',
+                '\u0045',
+                '\u004F',
                 ]
 
 ModernVowelMap = [
-                 '\u0D0E\u02BC',
-                 '\u0D06\u02BC',
+                 '\u0061\u0045',
+                 '\u0061\u004F',
                  ]
 
 SinhalaVowelMap = [
-                  '\u0D0F\u02C7'
+                  '\u0041\u0045'
                   ]
 
-VowelSignMap =  [
-                '\u0D3E',
-                '\u0D3F',
-                '\u0D40',
-                '\u0D41',
-                '\u0D42',
-                '\u0D43',
-                '\u0D44',
-                '\u0D62',
-                '\u0D63',
-                '\u0D47',
-                '\u0D48',
-                '\u0D4B',
-                '\u0D57',
-                ]
+VowelSignMap =  VowelMap[1:]
 
-SouthVowelSignMap = [
-                    '\u0D46',
-                    '\u0D4A',
-                    ]
+SouthVowelSignMap = SouthVowelMap[:]
 
-ModernVowelSignMap =[
-                    '\u0D46\u02BC',
-                    '\u0D3E\u02BC']
+ModernVowelSignMap = ModernVowelMap[:]
 
-SinhalaVowelSignMap = [
-                      '\u0D47\u02C7'
-                      ]
+SinhalaVowelSignMap = SinhalaVowelMap[:]
 
 AyogavahaMap = [
-               '\u0D01',
-               '\u0D02',
-               '\u0D03'
+               '\u007E',
+               '\u004D',
+               '\u0048'
                ]
 
 ViramaMap =  [
-             '\u0D4D\u200C'
+             '\u00D7'
              ]
 
 ConsonantMap =  [
-                '\u0D15',
-                '\u0D16',
-                '\u0D17',
-                '\u0D18',
-                '\u0D19',
-
-                '\u0D1A',
-                '\u0D1B',
-                '\u0D1C',
-                '\u0D1D',
-                '\u0D1E',
-
-                '\u0D1F',
-                '\u0D20',
-                '\u0D21',
-                '\u0D22',
-                '\u0D23',
-
-                '\u0D24',
-                '\u0D25',
-                '\u0D26',
-                '\u0D27',
-                '\u0D28',
-
-                '\u0D2A',
-                '\u0D2B',
-                '\u0D2C',
-                '\u0D2D',
-                '\u0D2E',
-
-                '\u0D2F',
-                '\u0D30',
-                '\u0D32',
-                '\u0D35',
-
-                '\u0D36',
-                '\u0D37',
-                '\u0D38',
-                '\u0D39'
+                '\u006B',
+                '\u006B\u0068',
+                '\u0067',
+                '\u0067\u0068',
+                '\u0047',
+
+                '\u0063',
+                '\u0063\u0068',
+                '\u006A',
+                '\u006A\u0068',
+                '\u004A',
+
+                '\u0054',
+                '\u0054\u0068',
+                '\u0044',
+                '\u0044\u0068',
+                '\u004E',
+
+                '\u0074',
+                '\u0074\u0068',
+                '\u0064',
+                '\u0064\u0068',
+                '\u006E',
+
+                '\u0070',
+                '\u0070\u0068',
+                '\u0062',
+                '\u0062\u0068',
+                '\u006D',
+
+                '\u0079',
+                '\u0072',
+                '\u006C',
+                '\u0076',
+
+                '\u007A',
+                '\u0053',
+                '\u0073',
+                '\u0068',
                 ]
 
 SouthConsonantMap = [
-                    '\u0D33',
-                    '\u0D34',
-                    '\u0D31',
-                    '\u0D29'
+                    '\u004C',
+                    '\u005A',
+                    '\u0072\u0032',
+                    '\u006E\u0032'
                     ]
 
 NuktaConsonantMap =  [
-                     '\u0D15\u00B7',
-                     '\u0D16\u00B7',
-                     '\u0D17\u00B7',
-                     '\u0D1C\u00B7',
-                     '\u0D21\u00B7',
-                     '\u0D22\u00B7',
-                     '\u0D2B\u00B7',
-                     '\u0D2F\u00B7'
+                     '\u0071',
+                     '\u0071\u0068',
+                     '\u0067\u0032',
+                     '\u007A\u0032',
+                     '\u0072\u0033',
+                     '\u0072\u0033\u0068',
+                     '\u0066',
+                     '\u0059'
                      ]
 
 SinhalaConsonantMap =[
-                     '\u0D02\u02C6\u0D17',
-                     '\u0D02\u02C6\u0D1C',
-                     '\u0D02\u02C6\u0D21',
-                     '\u0D02\u02C6\u0D26',
-                     '\u0D02\u02C6\u0D2C',
+                     '\u006E\u002A\u0067',
+                     '\u006E\u002A\u006A',
+                     '\u006E\u002A\u0044',
+                     '\u006E\u002A\u0064',
+                     '\u006D\u002A\u0062',
                       ]
 
 NuktaMap = [
-           '\u00B7'
+           '\u0051'
            ]
 
 OmMap = [
-        '\u0BD0'
+        '\u006F\u004D'
         ]
 
 SignMap =[
-         '\u0D3D',
-         '.',
-         '..'
+         '\u0027',
+         '\u002E',
+         '\u002E\u002E'
          ]
 
-Aytham =['\u0B83']
+Aytham =['\u004B']
 
 NumeralMap = [
-             '0',
-             '1',
-             '2',
-             '3',
-             '4',
-             '5',
-             '6',
-             '7',
-             '8',
-             '9'
+             '\u0030',
+             '\u0031',
+             '\u0032',
+             '\u0033',
+             '\u0034',
+             '\u0035',
+             '\u0036',
+             '\u0037',
+             '\u0038',
+             '\u0039',
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/TamilGrantha.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/Velthuis.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,170 +1,155 @@
 # -*- coding: utf-8 -*-
 
-# Script Mapping for Devanagari
+# Script Mapping for ISO
 
 VowelMap =  [
-            '\u0B85',
-            '\u0B86',
-            '\u0B87',
-            '\u0B88',
-            '\u0B89',
-            '\u0B8A',
-            '\u098B',
-            '\u09E0',
-            '\u098C',
-            '\u09E1',
-            '\u0B8F',
-            '\u0B90',
-            '\u0B93',
-            '\u0B94',
+            '\u0061',
+            '\u0061\u0061',
+            '\u0069',
+            '\u0069\u0069',
+            '\u0075',
+            '\u0075\u0075',
+            '\u002E\u0072',
+            '\u002E\u0052',
+            '\u002E\u006C',
+            '\u002E\u004C',
+            '\u0065',
+            '\u0061\u0069',
+            '\u006F',
+            '\u0061\u0075'
             ]
 
 SouthVowelMap = [
-                '\u0B8E',
-                '\u0B92',
+                '\u0045',
+                '\u004F',
                 ]
 
 ModernVowelMap = [
-                 '\u0B8E\u02BC',
-                 '\u0B86\u02BC',
+                 '\u0061\u0045',
+                 '\u0061\u004F',
                  ]
 
 SinhalaVowelMap = [
-                  '\u0B8F\u02C7'
+                  '\u0041\u0045'
                   ]
-    
-VowelSignMap =  [
-                '\u0BBE',
-                '\u0BBF',
-                '\u0BC0',
-                '\u0BC1',
-                '\u0BC2',
-                '\u09C3',
-                '\u09C4',
-                '\u09E2',
-                '\u09E3',
-                '\u0BC7',
-                '\u0BC8',
-                '\u0BCB',
-                '\u0BCC',
-                ]
 
-SouthVowelSignMap = [
-                    '\u0BC6',
-                    '\u0BCA',
-                    ]
+VowelSignMap =  VowelMap[1:]
 
-ModernVowelSignMap =[
-                    '\u0BC6\u02BC',
-                    '\u0BBE\u02BC']
+SouthVowelSignMap = SouthVowelMap[:]
 
-SinhalaVowelSignMap = [
-                      '\u0BC7\u02C7'
-                      ]
+ModernVowelSignMap = ModernVowelMap[:]
+
+SinhalaVowelSignMap = SinhalaVowelMap[:]
 
 AyogavahaMap = [
-               '\u0981',
-               '\u0982',
-               '\u0983'
+               '\u007E\u006D',
+               '\u002E\u006D',
+               '\u002E\u0068'
                ]
-    
+
 ViramaMap =  [
-             '\u0BCD'
+             '\u00D7'
              ]
 
 ConsonantMap =  [
-                '\u0B95',
-                '\u0996',
-                '\u0997',
-                '\u0998',
-                '\u0B99',
-                
-                '\u0B9A',
-                '\u099B',
-                '\u0B9C',
-                '\u099D',
-                '\u0B9E',
-                
-                '\u0B9F',
-                '\u09A0',
-                '\u09A1',
-                '\u09A2',
-                '\u0BA3',
-                
-                '\u0BA4',
-                '\u09A5',
-                '\u09A6',
-                '\u09A7',
-                '\u0BA8',
-                
-                '\u0BAA',
-                '\u09AB',
-                '\u09AC',
-                '\u09AD',
-                '\u0BAE',
-                
-                '\u0BAF',
-                '\u0BB0',
-                '\u0BB2',
-                '\u0BB5',
-                
-                '\u0BB6',
-                '\u0BB7',
-                '\u0BB8',
-                '\u0BB9'
+                '\u006B',
+                '\u006B\u0068',
+                '\u0067',
+                '\u0067\u0068',
+                '\u0022\u006E',
+
+                '\u0063',
+                '\u0063\u0068',
+                '\u006A',
+                '\u006A\u0068',
+                '\u007E\u006E',
+
+                '\u002E\u0074',
+                '\u002E\u0074\u0068',
+                '\u002E\u0064',
+                '\u002E\u0064\u0068',
+                '\u002E\u006E',
+
+                '\u0074',
+                '\u0074\u0068',
+                '\u0064',
+                '\u0064\u0068',
+                '\u006E',
+
+                '\u0070',
+                '\u0070\u0068',
+                '\u0062',
+                '\u0062\u0068',
+                '\u006D',
+
+                '\u0079',
+                '\u0072',
+                '\u006C',
+                '\u0076',
+
+                '\u0022\u0073',
+                '\u002E\u0073',
+                '\u0073',
+                '\u0068',
                 ]
 
 SouthConsonantMap = [
-                    '\u0BB3',
-                    '\u0BB4',
-                    '\u0BB1',
-                    '\u0BA9'
-                    ]                   
+                    '\u002E\u002E\u006C',
+                    '\u005F\u006C',
+                    '\u005F\u0072',
+                    '\u005F\u006E'
+                    ]
 
 NuktaConsonantMap =  [
-                     '\u0B95\u09BC',
-                     '\u0996\u09BC',
-                     '\u0997\u09BC',
-                     '\u0B9C\u09BC',
-                     '\u09A1\u09BC',
-                     '\u09A2\u09BC',
-                     '\u09AB\u09BC',
-                     '\u0BAF\u09BC'
+                     '\u0071',
+                     '\u005F\u006B\u0068',
+                     '\u002E\u0067',
+                     '\u007A',
+                     '\u002E\u002E\u0072',
+                     '\u002E\u002E\u0072\u0068',
+                     '\u0066',
+                     '\u002E\u0079'
                      ]
 
 SinhalaConsonantMap =[
-                     '\u0B99\u0BCD\u02C6\u0997',
-                     '\u0B9E\u0BCD\u02C6\u0B9C',
-                     '\u0BA3\u0BCD\u02C6\u09A1',
-                     '\u0BA8\u0BCD\u02C6\u09A6',
-                     '\u0BAE\u0BCD\u02C6\u09AC',
+                     '\u006E\u002A\u0067',
+                     '\u006E\u002A\u006A',
+                     '\u006E\u002A\u002E\u0064',
+                     '\u006E\u002A\u0064',
+                     '\u006D\u002A\u0062',
                       ]
 
 NuktaMap = [
-           '\u09BC'
+           '\u0051'
            ]
-    
+
 OmMap = [
-        '\u0BD0'
+        'o.m'
         ]
 
 SignMap =[
-         '\u09BD',
-         '\u0964',
-         '\u0965'
+         '\u002E\u0061',
+         '\u002E',
+         '\u002E\u002E'
          ]
 
-Aytham =[AyogavahaMap[2]+'\u02BC']
+Aytham =['\u005F\u006B']
 
 NumeralMap = [
-             '\u09E6',
-             '\u09E7',
-             '\u09E8',
-             '\u09E9',
-             '\u09EA',
-             '\u09EB',
-             '\u09EC',
-             '\u09ED',
-             '\u09EE',
-             '\u09EF'
+             '\u0030',
+             '\u0031',
+             '\u0032',
+             '\u0033',
+             '\u0034',
+             '\u0035',
+             '\u0036',
+             '\u0037',
+             '\u0038',
+             '\u0039',
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/Telugu.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Telugu.py`

 * *Files 10% similar despite different names*

```diff
@@ -165,7 +165,13 @@
              '\u0C6A',
              '\u0C6B',
              '\u0C6C',
              '\u0C6D',
              '\u0C6E',
              '\u0C6F'
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/Tirhuta.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Khudawadi.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,171 +1,177 @@
 # -*- coding: utf-8 -*-
 
 # Script Mapping for Devanagari
 
 VowelMap =  [
-            '\U00011481',
-            '\U00011482',
-            '\U00011483',
-            '\U00011484',
-            '\U00011485',
-            '\U00011486',
-            '\U00011487',
-            '\U00011488',
-            '\U00011489',
-            '\U0001148A',
-            '\U0001148B',
-            '\U0001148C',
-            '\U0001148D',
-            '\U0001148E',
+            '\U000112B0',
+            '\U000112B1',
+            '\U000112B2',
+            '\U000112B3',
+            '\U000112B4',
+            '\U000112B5',
+            '𑋙𑋡\u02BD',
+            '𑋙𑋢\u02BD',
+            '𑋚𑋡\u02BD',
+            '𑋚𑋢\u02BD',
+            '\U000112B6',
+            '\U000112B7',
+            '\U000112B8',
+            '\U000112B9',
             ]
 
 SouthVowelMap = [
-                '\U00011481\U000114BA',
-                '\U00011481\U000114BD',
+                '\U000112B6\u02BD',
+                '\U000112B8\u02BD',
                 ]
 
 ModernVowelMap = [
-                 '\U0001148B\u02BD',
-                 '\U00011482\u02BD',
+                 '\U000112B6\u02BD',
+                 '\U000112B1\u02BD',
                  ]
 
 SinhalaVowelMap = [
-                  '\U0001148B\u02BD'
+                  '\U000112B6\u02BD'
                   ]
 
 VowelSignMap =  [
-                '\U000114B0',
-                '\U000114B1',
-                '\U000114B2',
-                '\U000114B3',
-                '\U000114B4',
-                '\U000114B5',
-                '\U000114B6',
-                '\U000114B7',
-                '\U000114B8',
-                '\U000114B9',
-                '\U000114BB',
-                '\U000114BC',
-                '\U000114BE',
+                '\U000112E0',
+                '\U000112E1',
+                '\U000112E2',
+                '\U000112E3',
+                '\U000112E4',
+                '𑋪𑋙𑋡\u02BD',
+                '𑋪𑋙𑋢\u02BD',
+                '𑋪𑋚𑋡\u02BD',
+                '𑋪𑋚𑋢\u02BD',
+                '\U000112E5',
+                '\U000112E6',
+                '\U000112E7',
+                '\U000112E8',
                 ]
 
 SouthVowelSignMap = [
-                    '\U000114BA',
-                    '\U000114BD',
+                    '\U000112E5\u02BD',
+                    '\U000112E7\u02BD',
                     ]
 
 ModernVowelSignMap =[
-                    '\U000114B9\u02BD',
-                    '\U000114B0\u02BD'
+                    '\U000112E5\u02BD',
+                    '\U000112E0\u02BD'
                     ]
 
 SinhalaVowelSignMap = [
-                      '\U000114B9\u02BD'
+                      '\U000112E5\u02BD'
                       ]
 
 AyogavahaMap = [
-               '\U000114BF',
-               '\U000114C0',
-               '\U000114C1'
+               '\U000112DF\u02BD',
+               '\U000112DF',
+               '𑋞𑋪\u02BD'
                ]
 
 ViramaMap =  [
-             '\U000114C2'
+             '\U000112EA'
              ]
 
 ConsonantMap =  [
-                '\U0001148F',
-                '\U00011490',
-                '\U00011491',
-                '\U00011492',
-                '\U00011493',
-
-                '\U00011494',
-                '\U00011495',
-                '\U00011496',
-                '\U00011497',
-                '\U00011498',
-
-                '\U00011499',
-                '\U0001149A',
-                '\U0001149B',
-                '\U0001149C',
-                '\U0001149D',
-
-                '\U0001149E',
-                '\U0001149F',
-                '\U000114A0',
-                '\U000114A1',
-                '\U000114A2',
-
-                '\U000114A3',
-                '\U000114A4',
-                '\U000114A5',
-                '\U000114A6',
-                '\U000114A7',
-
-                '\U000114A8',
-                '\U000114A9',
-                '\U000114AA',
-                '\U000114AB',
-
-                '\U000114AC',
-                '\U000114AD',
-                '\U000114AE',
-                '\U000114AF'
+                '\U000112BA',
+                '\U000112BB',
+                '\U000112BC',
+                '\U000112BE',
+                '\U000112BF',
+
+                '\U000112C0',
+                '\U000112C1',
+                '\U000112C2',
+                '\U000112C4',
+                '\U000112C5',
+
+                '\U000112C6',
+                '\U000112C7',
+                '\U000112C8',
+                '\U000112CB',
+                '\U000112CC',
+
+                '\U000112CD',
+                '\U000112CE',
+                '\U000112CF',
+                '\U000112D0',
+                '\U000112D1',
+
+                '\U000112D2',
+                '\U000112D3',
+                '\U000112D4',
+                '\U000112D6',
+                '\U000112D7',
+
+                '\U000112D8',
+                '\U000112D9',
+                '\U000112DA',
+                '\U000112DB',
+
+                '\U000112DC',
+                '\U000112DC𑋩',
+                '\U000112DD',
+                '\U000112DE'
                 ]
 
 SouthConsonantMap = [
-                    '𑒝𑓃',
-                    '𑒭𑓃',
-                    '𑒩\u02BD',
-                    '𑒪𑓃'
+                    '𑋚𑋩',
+                    '𑋚𑋩\u02BD',
+                    '𑋙𑋩',
+                    '𑋑𑋩'
                     ]
 
 NuktaConsonantMap =  [
-                     '\U0001148F\U000114C3',
-                     '\U00011490\U000114C3',
-                     '\U00011491\U000114C3',
-                     '\U00011496\U000114C3',
-                     '\U0001149B\U000114C3',
-                     '\U0001149C\U000114C3',
-                     '\U000114A4\U000114C3',
-                     '\U000114A8\U000114C3'
+                     '𑊺𑋩',
+                     '𑊻𑋩',
+                     '𑊼𑋩',
+                     '𑋂𑋩',
+                     '𑋊',
+                     '𑋋𑋩',
+                     '𑋓𑋩',
+                     '𑋘𑋩'
                      ]
 
 SinhalaConsonantMap =[
-                     '\U000114BF𑒑\u02BD',
-                     '\U000114BF𑒖\u02BD',
-                     '\U000114BF𑒛\u02BD',
-                     '\U000114BF𑒠\u02BD',
-                     '\U000114BF𑒥\u02BD',
+                     '𑋟𑊼\u02BD',
+                     '𑋟𑋂\u02BD',
+                     '𑋟𑋈\u02BD',
+                     '𑋟𑋏\u02BD',
+                     '𑋟𑋔\u02BD',
                       ]
 
 NuktaMap = [
-           '\U000114C3'
+           '𑋩'
            ]
 
 OmMap = [
-        '𑓇'
+        '𑊸𑋟'
         ]
 
 SignMap =[
-         '𑓄',
+         '\u093D',
          '।',
          '॥'
          ]
 
 Aytham =[AyogavahaMap[2]+'\u02BD']
 
 NumeralMap = [
-             '\U000114D0',
-             '\U000114D1',
-             '\U000114D2',
-             '\U000114D3',
-             '\U000114D4',
-             '\U000114D5',
-             '\U000114D6',
-             '\U000114D7',
-             '\U000114D8',
-             '\U000114D9'
+             '\U000112F0',
+             '\U000112F1',
+             '\U000112F2',
+             '\U000112F3',
+             '\U000112F4',
+             '\U000112F5',
+             '\U000112F6',
+             '\U000112F7',
+             '\U000112F8',
+             '\U000112F9',
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/Urdu.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Urdu.py`

 * *Files 24% similar despite different names*

```diff
@@ -166,7 +166,13 @@
              '\u06F4',
              '\u06F5',
              '\u06F6',
              '\u06F7',
              '\u06F8',
              '\u06F9',
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/MainIndic/Vatteluttu.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/MainIndic/Sinhala.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,170 +1,176 @@
 # -*- coding: utf-8 -*-
 
 # Script Mapping for Devanagari
 
 VowelMap =  [
-            '\u0B85',
-            '\u0B86',
-            '\u0B87',
-            '\u0B88',
-            '\u0B89',
-            '\u0B8A',
-            '\u0BB0\u0BC1\u02BD',
-            '\u0BB0\u0BC2\u02BD',
-            '\u0BB2\u0BC1\u02BD',
-            '\u0BB2\u0BC2\u02BD',
-            '\u0B8F',
-            '\u0B90',
-            '\u0B93',
-            '\u0B94',
+            '\u0D85',
+            '\u0D86',
+            '\u0D89',
+            '\u0D8A',
+            '\u0D8B',
+            '\u0D8C',
+            '\u0D8D',
+            '\u0D8E',
+            '\u0D8F',
+            '\u0D90',
+            '\u0D92',
+            '\u0D93',
+            '\u0D95',
+            '\u0D96',
             ]
 
 SouthVowelMap = [
-                '\u0B8E',
-                '\u0B92',
+                '\u0D91',
+                '\u0D94',
                 ]
 
 ModernVowelMap = [
-                 '\u0B8E\u02BD',
-                 '\u0B86\u02BD',
+                 '\u0D87',
+                 '\u0D86\u02BC',
                  ]
 
 SinhalaVowelMap = [
-                  '\u0B8F\u02BD'
+                  '\u0D88'
                   ]
 
 VowelSignMap =  [
-                '\u0BBE',
-                '\u0BBF',
-                '\u0BC0',
-                '\u0BC1',
-                '\u0BC2',
-                '\u0BCD\u0BB0\u0BC1\u02BD',
-                '\u0BCD\u0BB0\u0BC2\u02BD',
-                '\u0BCD\u0BB2\u0BC1\u02BD',
-                '\u0BCD\u0BB2\u0BC2\u02BD',
-                '\u0BC7',
-                '\u0BC8',
-                '\u0BCB',
-                '\u0BCC',
+                '\u0DCF',
+                '\u0DD2',
+                '\u0DD3',
+                '\u0DD4',
+                '\u0DD6',
+                '\u0DD8',
+                '\u0DF2',
+                '\u0DDF',
+                '\u0DF3',
+                '\u0DDA',
+                '\u0DDB',
+                '\u0DDD',
+                '\u0DDE',
                 ]
 
 SouthVowelSignMap = [
-                    '\u0BC6',
-                    '\u0BCA',
+                    '\u0DD9',
+                    '\u0DDC',
                     ]
 
 ModernVowelSignMap =[
-                    '\u0BC6\u02BD',
-                    '\u0BBE\u02BD']
+                    '\u0DD0',
+                    '\u0DCF\u02BC']
 
 SinhalaVowelSignMap = [
-                      '\u0BC7\u02BD'
+                      '\u0DD1'
                       ]
 
 AyogavahaMap = [
-               '\u0BAE\u0BCD\u02BD',
-               '\u0BAE\u0BCD\u02BD',
-               '꞉' # Modifying letter colon for Visarga
+               '\u0D81',
+               '\u0D82',
+               '\u0D83'
                ]
 
 ViramaMap =  [
-             '\u0BCD'
+             '\u0DCA'
              ]
 
 ConsonantMap =  [
-                '\u0B95',
-                '\u0B95\u02BD',
-                '\u0B95\u02BD',
-                '\u0B95\u02BD',
-                '\u0B99',
-
-                '\u0B9A',
-                '\u0B9A\u02BD',
-                '\u0B9A\u02BD',
-                '\u0B9A\u02BD',
-                '\u0B9E',
-
-                '\u0B9F',
-                '\u0B9F\u02BD',
-                '\u0B9F\u02BD',
-                '\u0B9F\u02BD',
-                '\u0BA3',
-
-                '\u0BA4',
-                '\u0BA4\u02BD',
-                '\u0BA4\u02BD',
-                '\u0BA4\u02BD',
-                '\u0BA8',
-
-                '\u0BAA',
-                '\u0BAA\u02BD',
-                '\u0BAA\u02BD',
-                '\u0BAA\u02BD',
-                '\u0BAE',
-
-                '\u0BAF',
-                '\u0BB0',
-                '\u0BB2',
-                '\u0BB5',
-
-                '\u0B9A\u02BD',
-                '\u0B9A\u02BD',
-                '\u0B9A\u02BD',
-                '\u0B95\u02BD'
+                '\u0D9A',
+                '\u0D9B',
+                '\u0D9C',
+                '\u0D9D',
+                '\u0D9E',
+
+                '\u0DA0',
+                '\u0DA1',
+                '\u0DA2',
+                '\u0DA3',
+                '\u0DA4',
+
+                '\u0DA7',
+                '\u0DA8',
+                '\u0DA9',
+                '\u0DAA',
+                '\u0DAB',
+
+                '\u0DAD',
+                '\u0DAE',
+                '\u0DAF',
+                '\u0DB0',
+                '\u0DB1',
+
+                '\u0DB4',
+                '\u0DB5',
+                '\u0DB6',
+                '\u0DB7',
+                '\u0DB8',
+
+                '\u0DBA',
+                '\u0DBB',
+                '\u0DBD',
+                '\u0DC0',
+
+                '\u0DC1',
+                '\u0DC2',
+                '\u0DC3',
+                '\u0DC4'
                 ]
 
 SouthConsonantMap = [
-                    '\u0BB3',
-                    '\u0BB4',
-                    '\u0BB1',
-                    '\u0BA9'
+                    '\u0DC5',
+                    '\u0DC5\u00B7',
+                    '\u0DBB\u00B7',
+                    '\u0DB1\u00B7'
                     ]
 
 NuktaConsonantMap =  [
-                     '\u02BD\u0B95',
-                     '\u02BD\u0B95',
-                     '\u02BD\u0B95',
-                     '\u02BD\u0B9A',
-                     '\u02BD\u0B9F',
-                     '\u02BD\u0B9F',
-                     '\u02BD\u0BAA',
-                     '\u02BD\u0BAF'
+                     '\u0D9A\u00B7',
+                     '\u0D9B\u00B7',
+                     '\u0D9C\u00B7',
+                     '\u0DA2\u00B7',
+                     '\u0DA9\u00B7',
+                     '\u0DAA\u00B7',
+                     '\u0DC6',
+                     '\u0DBA\u00B7'
                      ]
 
 SinhalaConsonantMap =[
-                     '\u0B99\u0BCD\u02BD\u0B95',
-                     '\u0B9E\u0BCD\u02BD\u0B9A',
-                     '\u0BA3\u0BCD\u02BD\u0B9F',
-                     '\u0BA8\u0BCD\u02BD\u0BA4',
-                     '\u0BAE\u0BCD\u02BD\u0BAA',
+                     '\u0D9F',
+                     '\u0DA6',
+                     '\u0DAC',
+                     '\u0DB3',
+                     '\u0DB9'
                       ]
 
 NuktaMap = [
-           '\u02BD\u02BD'
+           '\u00B7'
            ]
 
 OmMap = [
-        'ஓம்'
+        '\u0D95\u0D82'
         ]
 
 SignMap =[
-         '\u02BD\u02BD',
-         '.',
-         '..'
+         '\u0028\u0D85\u0029',
+         '\u002E',
+         '\u002E\u002E'
          ]
 
-Aytham =['\u0B83']
+Aytham =[AyogavahaMap[2]+'\u02BC']
 
 NumeralMap = [
-             '0',
-             '1',
-             '2',
-             '3',
-             '4',
-             '5',
-             '6',
-             '7',
-             '8',
-             '9'
-            ]
+             '\u0DE6',
+             '\u0DE7',
+             '\u0DE8',
+             '\u0DE9',
+             '\u0DEA',
+             '\u0DEB',
+             '\u0DEC',
+             '\u0DED',
+             '\u0DEE',
+             '\u0DEF',
+             ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/NonIndic/OldPersian.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/NonIndic/OldPersian.py`

 * *Files 11% similar despite different names*

```diff
@@ -157,7 +157,13 @@
              '\u0034',
              '\u0035',
              '\u0036',
              '\u0037',
              '\u0038',
              '\u0039',
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/NonIndic/kana2roman.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/NonIndic/kana2roman.py`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/Roman/Aksharaa.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/Aksharaa.py`

 * *Files 3% similar despite different names*

```diff
@@ -143,7 +143,13 @@
              '\u0034',
              '\u0035',
              '\u0036',
              '\u0037',
              '\u0038',
              '\u0039',
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/Roman/Ariyaka.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/JavaneseSimpleRomanLoC.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,149 +1,154 @@
 # -*- coding: utf-8 -*-
 
 # Script Mapping for ISO
 
 VowelMap =  [
-            'a',
-            'A',
-            'i',
-            'I',
-            'u',
-            'U',
-            'ru\u02BD',
-            'rU\u02BD',
-            'lu\u02BD',
-            'lU\u02BD',
+            '\u0061',
+            'a\u02BD',
+            '\u0069',
+            'i\u02BD',
+            '\u0075',
+            'u\u02BD',
+            'rĕ',
+            'rĕ\u02BD',
+            'lĕ',
+            'lĕ\u02BD',
             'e',
-            'ai',
+            'e\u02BD',
             'o',
-            'au'
+            'o\u02BD'
             ]
 
 SouthVowelMap = [
-                'e\u02BD',
-                'o\u02BD',
+                '\u0065\u02BD',
+                '\u006F\u02BD',
                 ]
 
 ModernVowelMap = [
-                'e\u02BD',
-                'A',
+                 'ĕ',
+                 '\u00F4',
                  ]
 
 SinhalaVowelMap = [
-                'e\u02BD',
+                  'ĕ'
                   ]
 
 VowelSignMap =  VowelMap[1:]
 
 SouthVowelSignMap = SouthVowelMap[:]
 
 ModernVowelSignMap = ModernVowelMap[:]
 
 SinhalaVowelSignMap = SinhalaVowelMap[:]
 
 AyogavahaMap = [
-               'M\u02BD',
-               'M',
+               'ng',
+               'ng',
                'h'
                ]
 
 ViramaMap =  [
              '\u00D7'
              ]
 
 ConsonantMap =  [
-                'k',
-                'K',
-                'g',
-                'G',
-                '~',
-
-                'c',
-                'C',
-                'j',
-                'J',
-                'Y',
-
-                'T',
-                'F',
-                'D',
-                'V',
-                'N',
-
-                't',
-                'f',
-                'd',
-                '@',
+                '\u006B',
+                '\u006B\u02BD',
+                '\u0067',
+                '\u0067\u02BD',
+                'ng',
+
+                '\u0063',
+                '\u0063\u02BD',
+                '\u006A',
+                '\u006A\u02BD',
+                'ny',
+
+                'th',
+                'th\u02BD',
+                'dh',
+                'dh\u02BD',
                 'n',
 
-                'p',
-                'P',
-                'b',
-                'B',
-                'm',
-
-                'y',
-                'r',
-                'l',
-                'v',
+                '\u0074',
+                '\u0074\u02BD',
+                '\u0064',
+                '\u0064\u02BD',
+                '\u006E',
+
+                '\u0070',
+                '\u0070\u02BD',
+                '\u0062',
+                '\u0062\u02BD',
+                '\u006D',
+
+                '\u0079',
+                '\u0072',
+                '\u006C',
+                'w',
 
                 's\u02BD',
                 's\u02BD',
-                's',
-                'h',
+                '\u0073',
+                '\u0068',
                 ]
 
 SouthConsonantMap = [
-                    'L',
-                    'L\u02BD',
-                    'r\u02BD',
-                    'n\u02BD'
+                    '\u1E37',
+                    '\u1E3B',
+                    '\u1E5F',
+                    '\u1E49'
                     ]
 
 NuktaConsonantMap =  [
-                     'k\u02BD',
-                     'K\u02BD',
-                     'g\u02BD',
-                     'j\u02BD',
-                    'D\u02BD',
-                    'V\u02BD',
-                     'P\u02BD',
-                     'y\u02BD'
+                     'kh\u02BD',
+                     '\u006B\u035F\u0068',
+                     'gh\u02BD',
+                     '\u007A',
+                     '\u1E5B',
+                     '\u1E5B\u0068',
+                     '\u0066',
+                     '\u1E8F'
                      ]
 
 SinhalaConsonantMap =[
-                     'Mg\u02BD',
-                     'Mj\u02BD',
-                     'MD\u02BD',
-                     'Md\u02BD',
-                     'Mb\u02BD',
+                     '\u006E\u0306\u0067',
+                     '\u006E\u0306\u006A',
+                     '\u006E\u0306\u1E0D',
+                     '\u006E\u0306\u0064',
+                     '\u006D\u0306\u0062',
                       ]
-
 NuktaMap = [
-           '\u02BD\u02BD'
+           '\u0308'
            ]
 
 OmMap = [
-        'oM'
+        '\u014D\u1E41'
         ]
 
+Aytham =['\u1E35']
+
 SignMap =[
-         '\u0027',
+         '’',
          '\u002E',
          '\u002E\u002E'
          ]
 
-Aytham =['h\u02BD']
-
 NumeralMap = [
              '\u0030',
              '\u0031',
              '\u0032',
              '\u0033',
              '\u0034',
              '\u0035',
              '\u0036',
              '\u0037',
              '\u0038',
              '\u0039',
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/Roman/Avestan.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/Avestan.py`

 * *Files 8% similar despite different names*

```diff
@@ -144,7 +144,13 @@
              '\u0034',
              '\u0035',
              '\u0036',
              '\u0037',
              '\u0038',
              '\u0039',
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/Roman/BarahaNorth.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/BarahaNorth.py`

 * *Files 14% similar despite different names*

```diff
@@ -142,7 +142,13 @@
              '\u0034',
              '\u0035',
              '\u0036',
              '\u0037',
              '\u0038',
              '\u0039',
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/Roman/BarahaSouth.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/BarahaSouth.py`

 * *Files 14% similar despite different names*

```diff
@@ -142,7 +142,13 @@
              '\u0034',
              '\u0035',
              '\u0036',
              '\u0037',
              '\u0038',
              '\u0039',
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/Roman/GreekModern.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/BalineseRomanLoC.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,78 +1,78 @@
 # -*- coding: utf-8 -*-
 
 # Script Mapping for ISO
 
 VowelMap =  [
             '\u0061',
-            '\u0041',
+            '\u0101',
             '\u0069',
-            '\u0049',
+            '\u012B',
             '\u0075',
-            '\u0055',
-            '\u0052',
-            '\u0052\u0052',
-            '\u006C\u0052',
-            '\u006C\u0052\u0052',
-            '\u0065',
+            '\u016B',
+            'rĕ',
+            'rö',
+            'lĕ',
+            'lö',
+            'e',
             '\u0061\u0069',
-            '\u006F',
+            'o',
             '\u0061\u0075'
             ]
 
 SouthVowelMap = [
-                '\u0045',
-                '\u004F',
+                'ĕ\u02BD',
+                'ŏ\u02BD',
                 ]
 
 ModernVowelMap = [
-                 '\u0061\u0045',
-                 '\u0061\u004F',
+                 'ĕ',
+                 '\u00F4',
                  ]
 
 SinhalaVowelMap = [
-                  '\u0041\u0045'
+                  'ö'
                   ]
 
 VowelSignMap =  VowelMap[1:]
 
 SouthVowelSignMap = SouthVowelMap[:]
 
 ModernVowelSignMap = ModernVowelMap[:]
 
 SinhalaVowelSignMap = SinhalaVowelMap[:]
 
 AyogavahaMap = [
-               '\u007E',
-               '\u004D',
-               '\u0048'
+               'ng',
+               'ng',
+               'h'
                ]
 
 ViramaMap =  [
              '\u00D7'
              ]
 
 ConsonantMap =  [
                 '\u006B',
                 '\u006B\u0068',
                 '\u0067',
                 '\u0067\u0068',
-                '\u0047',
+                'ng',
 
                 '\u0063',
                 '\u0063\u0068',
                 '\u006A',
                 '\u006A\u0068',
-                '\u004A',
+                '\u00F1',
 
-                '\u0054',
-                '\u0054\u0068',
-                '\u0044',
-                '\u0044\u0068',
-                '\u004E',
+                '\u1E6D',
+                '\u1E6D\u0068',
+                '\u1E0D',
+                '\u1E0D\u0068',
+                '\u1E47',
 
                 '\u0074',
                 '\u0074\u0068',
                 '\u0064',
                 '\u0064\u0068',
                 '\u006E',
 
@@ -81,69 +81,74 @@
                 '\u0062',
                 '\u0062\u0068',
                 '\u006D',
 
                 '\u0079',
                 '\u0072',
                 '\u006C',
-                '\u0076',
+                'w',
 
-                '\u007A',
-                '\u0053',
+                '\u015B',
+                '\u1E63',
                 '\u0073',
                 '\u0068',
                 ]
 
 SouthConsonantMap = [
-                    '\u004C',
-                    '\u005A',
-                    '\u0072\u0032',
-                    '\u006E\u0032'
+                    '\u1E37',
+                    '\u1E3B',
+                    '\u1E5F',
+                    '\u1E49'
                     ]
 
 NuktaConsonantMap =  [
-                     '\u0071',
-                     '\u0071\u0068',
-                     '\u0067\u0032',
-                     '\u007A\u0032',
-                     '\u0072\u0033',
-                     '\u0072\u0033\u0068',
+                     'kh\u02BD',
+                     '\u006B\u035F\u0068',
+                     'gh\u02BD',
+                     '\u007A',
+                     '\u1E5B',
+                     '\u1E5B\u0068',
                      '\u0066',
-                     '\u0059'
+                     '\u1E8F'
                      ]
 
 SinhalaConsonantMap =[
-                     '\u006E\u002A\u0067',
-                     '\u006E\u002A\u006A',
-                     '\u006E\u002A\u0044',
-                     '\u006E\u002A\u0064',
-                     '\u006D\u002A\u0062',
+                     '\u006E\u0306\u0067',
+                     '\u006E\u0306\u006A',
+                     '\u006E\u0306\u1E0D',
+                     '\u006E\u0306\u0064',
+                     '\u006D\u0306\u0062',
                       ]
-
 NuktaMap = [
-           '\u0051'
+           '\u0308'
            ]
 
 OmMap = [
-        '\u006F\u004D'
+        '\u014D\u1E41'
         ]
 
+Aytham =['\u1E35']
+
 SignMap =[
-         '\u0027',
+         '’',
          '\u002E',
          '\u002E\u002E'
          ]
 
-Aytham =['\u004B']
-
 NumeralMap = [
              '\u0030',
              '\u0031',
              '\u0032',
              '\u0033',
              '\u0034',
              '\u0035',
              '\u0036',
              '\u0037',
              '\u0038',
              '\u0039',
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/Roman/HK.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/RomanReadable.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,149 +1,155 @@
 # -*- coding: utf-8 -*-
 
 # Script Mapping for ISO
 
 VowelMap =  [
             '\u0061',
-            '\u0041',
+            'aa',
             '\u0069',
-            '\u0049',
+            'ee',
             '\u0075',
-            '\u0055',
-            '\u0052',
-            '\u0052\u0052',
-            '\u006C\u0052',
-            '\u006C\u0052\u0052',
-            '\u0065',
-            '\u0061\u0069',
-            '\u006F',
-            '\u0061\u0075'
+            'oo',
+            'ri\'',
+            'ree\'',
+            'li\'',
+            'lee\'',
+            'e',
+            'ai',
+            'o',
+            'au'
             ]
 
 SouthVowelMap = [
-                '\u0045',
-                '\u004F',
+                'e\'',
+                'o\'',
                 ]
 
 ModernVowelMap = [
-                 '\u0061\u0045',
-                 '\u0061\u004F',
+                 'a',
+                 'o',
                  ]
 
 SinhalaVowelMap = [
-                  '\u0041\u0045'
+                  'e'
                   ]
 
 VowelSignMap =  VowelMap[1:]
 
 SouthVowelSignMap = SouthVowelMap[:]
 
 ModernVowelSignMap = ModernVowelMap[:]
 
 SinhalaVowelSignMap = SinhalaVowelMap[:]
 
 AyogavahaMap = [
-               '\u007E',
                '\u004D',
-               '\u0048'
+               '\u004D',
+               'h\''
                ]
 
 ViramaMap =  [
              '\u00D7'
              ]
 
 ConsonantMap =  [
                 '\u006B',
                 '\u006B\u0068',
                 '\u0067',
                 '\u0067\u0068',
-                '\u0047',
+                'ng',
 
-                '\u0063',
-                '\u0063\u0068',
+                'ch',
+                'chh',
                 '\u006A',
                 '\u006A\u0068',
-                '\u004A',
+                'nj',
 
-                '\u0054',
-                '\u0054\u0068',
-                '\u0044',
-                '\u0044\u0068',
-                '\u004E',
-
-                '\u0074',
-                '\u0074\u0068',
-                '\u0064',
-                '\u0064\u0068',
+                't\'',
+                't\'h',
+                'd\'',
+                'd\'h',
+                'n',
+
+                't',
+                'th',
+                'd',
+                'dh',
                 '\u006E',
 
                 '\u0070',
                 '\u0070\u0068',
                 '\u0062',
                 '\u0062\u0068',
                 '\u006D',
 
                 '\u0079',
                 '\u0072',
                 '\u006C',
                 '\u0076',
 
-                '\u007A',
-                '\u0053',
+                'sh',
+                'sh',
                 '\u0073',
                 '\u0068',
                 ]
 
 SouthConsonantMap = [
-                    '\u004C',
-                    '\u005A',
-                    '\u0072\u0032',
-                    '\u006E\u0032'
+                    'l\'',
+                    'zh',
+                    'r\'',
+                    'n'
                     ]
 
 NuktaConsonantMap =  [
-                     '\u0071',
-                     '\u0071\u0068',
-                     '\u0067\u0032',
-                     '\u007A\u0032',
-                     '\u0072\u0033',
-                     '\u0072\u0033\u0068',
-                     '\u0066',
-                     '\u0059'
+                     'q',
+                     'kh',
+                     'g',
+                     'z',
+                     'r',
+                     'rh',
+                     'f',
+                     'y'
                      ]
 
 SinhalaConsonantMap =[
-                     '\u006E\u002A\u0067',
-                     '\u006E\u002A\u006A',
-                     '\u006E\u002A\u0044',
-                     '\u006E\u002A\u0064',
-                     '\u006D\u002A\u0062',
+                     'ng',
+                     'nj',
+                     'nd\'',
+                     'nd',
+                     'mb',
                       ]
 
 NuktaMap = [
-           '\u0051'
+           '\u02BD\u02BD'
            ]
 
 OmMap = [
-        '\u006F\u004D'
+        'om'
         ]
 
 SignMap =[
-         '\u0027',
+         '\'',
          '\u002E',
          '\u002E\u002E'
          ]
 
-Aytham =['\u004B']
+Aytham =['g']
 
 NumeralMap = [
              '\u0030',
              '\u0031',
              '\u0032',
              '\u0033',
              '\u0034',
              '\u0035',
              '\u0036',
              '\u0037',
              '\u0038',
              '\u0039',
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/Roman/HanifiRohingya.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/HanifiRohingya.py`

 * *Files 17% similar despite different names*

```diff
@@ -143,7 +143,13 @@
              '\U00010D34',
              '\U00010D35',
              '\U00010D36',
              '\U00010D37',
              '\U00010D38',
              '\U00010D39',
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/Roman/IAST.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/HK.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,78 +1,78 @@
 # -*- coding: utf-8 -*-
 
 # Script Mapping for ISO
 
 VowelMap =  [
             '\u0061',
-            '\u0101',
+            '\u0041',
             '\u0069',
-            '\u012B',
+            '\u0049',
             '\u0075',
-            '\u016B',
-            '\u1E5B',
-            '\u1E5D',
-            '\u1E37',
-            '\u1E39',
+            '\u0055',
+            '\u0052',
+            '\u0052\u0052',
+            '\u006C\u0052',
+            '\u006C\u0052\u0052',
             '\u0065',
             '\u0061\u0069',
             '\u006F',
             '\u0061\u0075'
             ]
 
 SouthVowelMap = [
-                '\u0115',
-                '\u014F',
+                '\u0045',
+                '\u004F',
                 ]
 
 ModernVowelMap = [
-                 '\u00E6',
-                 '\u00F4',
+                 '\u0061\u0045',
+                 '\u0061\u004F',
                  ]
 
 SinhalaVowelMap = [
-                  '\u01E3'
+                  '\u0041\u0045'
                   ]
 
 VowelSignMap =  VowelMap[1:]
 
 SouthVowelSignMap = SouthVowelMap[:]
 
 ModernVowelSignMap = ModernVowelMap[:]
 
 SinhalaVowelSignMap = SinhalaVowelMap[:]
 
 AyogavahaMap = [
-               '\u006D\u0310',
-               '\u1E43',
-               '\u1E25'
+               '\u007E',
+               '\u004D',
+               '\u0048'
                ]
 
 ViramaMap =  [
              '\u00D7'
              ]
 
 ConsonantMap =  [
                 '\u006B',
                 '\u006B\u0068',
                 '\u0067',
                 '\u0067\u0068',
-                '\u1E45',
+                '\u0047',
 
                 '\u0063',
                 '\u0063\u0068',
                 '\u006A',
                 '\u006A\u0068',
-                '\u00F1',
+                '\u004A',
 
-                '\u1E6D',
-                '\u1E6D\u0068',
-                '\u1E0D',
-                '\u1E0D\u0068',
-                '\u1E47',
+                '\u0054',
+                '\u0054\u0068',
+                '\u0044',
+                '\u0044\u0068',
+                '\u004E',
 
                 '\u0074',
                 '\u0074\u0068',
                 '\u0064',
                 '\u0064\u0068',
                 '\u006E',
 
@@ -83,67 +83,73 @@
                 '\u006D',
 
                 '\u0079',
                 '\u0072',
                 '\u006C',
                 '\u0076',
 
-                '\u015B',
-                '\u1E63',
+                '\u007A',
+                '\u0053',
                 '\u0073',
                 '\u0068',
                 ]
 
 SouthConsonantMap = [
-                    '\u006C\u0324',
-                    '\u1E3B',
-                    '\u1E5F',
-                    '\u1E49'
+                    '\u004C',
+                    '\u005A',
+                    '\u0072\u0032',
+                    '\u006E\u0032'
                     ]
 
 NuktaConsonantMap =  [
                      '\u0071',
-                     '\u006B\u035F\u0068',
-                     '\u0121',
-                     '\u007A',
-                     '\u0072\u0324',
-                     '\u0072\u0324\u0068',
+                     '\u0071\u0068',
+                     '\u0067\u0032',
+                     '\u007A\u0032',
+                     '\u0072\u0033',
+                     '\u0072\u0033\u0068',
                      '\u0066',
-                     '\u1E8F'
+                     '\u0059'
                      ]
 
 SinhalaConsonantMap =[
-                     '\u006E\u0306\u0067',
-                     '\u006E\u0306\u006A',
-                     '\u006E\u0306\u1E0D',
-                     '\u006E\u0306\u0064',
-                     '\u006D\u0306\u0062',
+                     '\u006E\u002A\u0067',
+                     '\u006E\u002A\u006A',
+                     '\u006E\u002A\u0044',
+                     '\u006E\u002A\u0064',
+                     '\u006D\u002A\u0062',
                       ]
 
 NuktaMap = [
-           '\u0308'
+           '\u0051'
            ]
 
 OmMap = [
-        '\u006F\u1E43'
+        '\u006F\u004D'
         ]
 
 SignMap =[
          '\u0027',
          '\u002E',
          '\u002E\u002E'
          ]
 
-Aytham =['\u1E35']
+Aytham =['\u004B']
 
 NumeralMap = [
              '\u0030',
              '\u0031',
              '\u0032',
              '\u0033',
              '\u0034',
              '\u0035',
              '\u0036',
              '\u0037',
              '\u0038',
              '\u0039',
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/Roman/IASTLOC.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/IAST.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,16 +7,16 @@
             '\u0101',
             '\u0069',
             '\u012B',
             '\u0075',
             '\u016B',
             '\u1E5B',
             '\u1E5D',
-            '\u006C\u0324',
-            '\u006C\u0324\u0304',
+            '\u1E37',
+            '\u1E39',
             '\u0065',
             '\u0061\u0069',
             '\u006F',
             '\u0061\u0075'
             ]
 
 SouthVowelMap = [
@@ -90,15 +90,15 @@
                 '\u015B',
                 '\u1E63',
                 '\u0073',
                 '\u0068',
                 ]
 
 SouthConsonantMap = [
-                    'ḷ',
+                    '\u006C\u0324',
                     '\u1E3B',
                     '\u1E5F',
                     '\u1E49'
                     ]
 
 NuktaConsonantMap =  [
                      '\u0071',
@@ -143,7 +143,13 @@
              '\u0034',
              '\u0035',
              '\u0036',
              '\u0037',
              '\u0038',
              '\u0039',
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/Roman/IASTPali.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/IASTPali.py`

 * *Files 18% similar despite different names*

```diff
@@ -143,7 +143,13 @@
              '\u0034',
              '\u0035',
              '\u0036',
              '\u0037',
              '\u0038',
              '\u0039',
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/Roman/IPA.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/IPA.py`

 * *Files 18% similar despite different names*

```diff
@@ -144,7 +144,13 @@
              '\u0034',
              '\u0035',
              '\u0036',
              '\u0037',
              '\u0038',
              '\u0039',
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/Roman/ISO.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/BurmeseRomanLoC.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,27 +5,27 @@
 VowelMap =  [
             '\u0061',
             '\u0101',
             '\u0069',
             '\u012B',
             '\u0075',
             '\u016B',
-            '\u0072\u0325',
-            '\u0072\u0325\u0304',
-            '\u006C\u0325',
-            '\u006C\u0325\u0304',
-            '\u0113',
+            '\u1E5B',
+            '\u1E5D',
+            '\u006C\u0324',
+            '\u006C\u0324\u0304',
+            '\u0065',
             '\u0061\u0069',
-            '\u014D',
+            '\u006F',
             '\u0061\u0075'
             ]
 
 SouthVowelMap = [
-                '\u0065',
-                '\u006F',
+                '\u0115',
+                '\u014F',
                 ]
 
 ModernVowelMap = [
                  '\u00E6',
                  '\u00F4',
                  ]
 
@@ -39,15 +39,15 @@
 
 ModernVowelSignMap = ModernVowelMap[:]
 
 SinhalaVowelSignMap = SinhalaVowelMap[:]
 
 AyogavahaMap = [
                '\u006D\u0310',
-               '\u1E41',
+               '\u1E43',
                '\u1E25'
                ]
 
 ViramaMap =  [
              '\u00D7'
              ]
 
@@ -90,59 +90,66 @@
                 '\u015B',
                 '\u1E63',
                 '\u0073',
                 '\u0068',
                 ]
 
 SouthConsonantMap = [
-                    '\u1E37',
+                    'ḷ',
                     '\u1E3B',
                     '\u1E5F',
                     '\u1E49'
                     ]
 
 NuktaConsonantMap =  [
                      '\u0071',
                      '\u006B\u035F\u0068',
                      '\u0121',
                      '\u007A',
-                     '\u1E5B',
-                     '\u1E5B\u0068',
+                     '\u0072\u0324',
+                     '\u0072\u0324\u0068',
                      '\u0066',
                      '\u1E8F'
                      ]
 
 SinhalaConsonantMap =[
                      '\u006E\u0306\u0067',
                      '\u006E\u0306\u006A',
                      '\u006E\u0306\u1E0D',
                      '\u006E\u0306\u0064',
                      '\u006D\u0306\u0062',
                       ]
+
 NuktaMap = [
            '\u0308'
            ]
 
 OmMap = [
-        '\u014D\u1E41'
+        '\u006F\u1E43'
         ]
 
-Aytham =['\u1E35']
-
 SignMap =[
-         '’',
+         '\u0027',
          '\u002E',
          '\u002E\u002E'
          ]
 
+Aytham =['\u1E35']
+
 NumeralMap = [
              '\u0030',
              '\u0031',
              '\u0032',
              '\u0033',
              '\u0034',
              '\u0035',
              '\u0036',
              '\u0037',
              '\u0038',
              '\u0039',
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/Roman/ISOPali.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/ThamLoCRomanLoC.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 VowelMap =  [
             '\u0061',
             '\u0101',
             '\u0069',
             '\u012B',
             '\u0075',
             '\u016B',
-            '\u0072\u0325',
-            '\u0072\u0325\u0304',
-            '\u006C\u0325',
-            '\u006C\u0325\u0304',
+            '\u1E5B',
+            '\u1E5D',
+            '\u006C\u0324',
+            '\u006C\u0324\u0304',
             '\u0065',
             '\u0061\u0069',
             '\u006F',
             '\u0061\u0075'
             ]
 
 SouthVowelMap = [
@@ -39,15 +39,15 @@
 
 ModernVowelSignMap = ModernVowelMap[:]
 
 SinhalaVowelSignMap = SinhalaVowelMap[:]
 
 AyogavahaMap = [
                '\u006D\u0310',
-               '\u1E41',
+               '\u1E43',
                '\u1E25'
                ]
 
 ViramaMap =  [
              '\u00D7'
              ]
 
@@ -90,59 +90,66 @@
                 '\u015B',
                 '\u1E63',
                 '\u0073',
                 '\u0068',
                 ]
 
 SouthConsonantMap = [
-                    '\u1E37',
+                    'ḷ',
                     '\u1E3B',
                     '\u1E5F',
                     '\u1E49'
                     ]
 
 NuktaConsonantMap =  [
                      '\u0071',
                      '\u006B\u035F\u0068',
                      '\u0121',
                      '\u007A',
-                     '\u1E5B',
-                     '\u1E5B\u0068',
+                     '\u0072\u0324',
+                     '\u0072\u0324\u0068',
                      '\u0066',
                      '\u1E8F'
                      ]
 
 SinhalaConsonantMap =[
                      '\u006E\u0306\u0067',
                      '\u006E\u0306\u006A',
                      '\u006E\u0306\u1E0D',
                      '\u006E\u0306\u0064',
                      '\u006D\u0306\u0062',
                       ]
+
 NuktaMap = [
            '\u0308'
            ]
 
 OmMap = [
-        '\u014D\u1E41'
+        '\u006F\u1E43'
         ]
 
-Aytham =['\u1E35']
-
 SignMap =[
-         '’\u02BD',
+         '\'\u02BD',
          '\u002E',
          '\u002E\u002E'
          ]
 
+Aytham =['\u1E35']
+
 NumeralMap = [
              '\u0030',
              '\u0031',
              '\u0032',
              '\u0033',
              '\u0034',
              '\u0035',
              '\u0036',
              '\u0037',
              '\u0038',
              '\u0039',
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/Roman/Itrans.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/JavaneseRomanLoC.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,78 +1,78 @@
 # -*- coding: utf-8 -*-
 
 # Script Mapping for ISO
 
 VowelMap =  [
             '\u0061',
-            '\u0041',
+            'a\u02BD',
             '\u0069',
-            '\u0049',
+            'i\u02BD',
             '\u0075',
-            '\u0055',
-            '\u0052\u005E\u0069',
-            '\u0052\u005E\u0049',
-            '\u004C\u005E\u0069',
-            '\u004C\u005E\u0049',
-            '\u0065',
-            '\u0061\u0069',
-            '\u006F',
-            '\u0061\u0075'
+            'u\u02BD',
+            'rĕ',
+            'rĕ\u02BD',
+            'lĕ',
+            'lĕ\u02BD',
+            'e',
+            'e\u02BD',
+            'o',
+            'o\u02BD'
             ]
 
 SouthVowelMap = [
-                '^e',
-                '^o',
+                '\u0065\u02BD',
+                '\u006F\u02BD',
                 ]
 
 ModernVowelMap = [
-                 'e.c',
-                 'A.c',
+                 'ĕ',
+                 '\u00F4',
                  ]
 
 SinhalaVowelMap = [
-                  '\u0061\u002E\u0043'
+                  'ĕ'
                   ]
 
 VowelSignMap =  VowelMap[1:]
 
 SouthVowelSignMap = SouthVowelMap[:]
 
 ModernVowelSignMap = ModernVowelMap[:]
 
 SinhalaVowelSignMap = SinhalaVowelMap[:]
 
 AyogavahaMap = [
-               '\u002E\u004E',
-               '\u004D',
-               '\u0048'
+               'ng',
+               'ng',
+               'h'
                ]
 
 ViramaMap =  [
              '\u00D7'
              ]
 
 ConsonantMap =  [
                 '\u006B',
                 '\u006B\u0068',
                 '\u0067',
                 '\u0067\u0068',
-                '\u007E\u004E',
+                'ng',
 
+                '\u0063',
                 '\u0063\u0068',
-                '\u0043\u0068',
                 '\u006A',
                 '\u006A\u0068',
-                '\u007E\u006E',
+                'ny',
 
-                '\u0054',
-                '\u0054\u0068',
-                '\u0044',
-                '\u0044\u0068',
-                '\u004E',
+                'th',
+                'thh',
+                'dh',
+                'dhh',
+                '\u1E47',
 
                 '\u0074',
                 '\u0074\u0068',
                 '\u0064',
                 '\u0064\u0068',
                 '\u006E',
 
@@ -81,69 +81,74 @@
                 '\u0062',
                 '\u0062\u0068',
                 '\u006D',
 
                 '\u0079',
                 '\u0072',
                 '\u006C',
-                '\u0076',
+                'w',
 
-                '\u0073\u0068',
-                '\u0053\u0068',
+                '\u015B',
+                '\u1E63',
                 '\u0073',
                 '\u0068',
                 ]
 
 SouthConsonantMap = [
-                    'L',
-                    'zh',
-                    'R',
-                    '\u005E\u006E'
+                    '\u1E37',
+                    '\u1E3B',
+                    '\u1E5F',
+                    '\u1E49'
                     ]
 
 NuktaConsonantMap =  [
-                     '\u0071',
-                     '\u004B',
-                     '\u0047',
+                     'kh\u02BD',
+                     '\u006B\u035F\u0068',
+                     'gh\u02BD',
                      '\u007A',
-                     '\u002E\u0044',
-                     '\u002E\u0044\u0068',
+                     '\u1E5B',
+                     '\u1E5B\u0068',
                      '\u0066',
-                     '\u0059'
+                     '\u1E8F'
                      ]
 
 SinhalaConsonantMap =[
-                     '\u006E\u002A\u0067',
-                     '\u006E\u002A\u006A',
-                     '\u006E\u002A\u0044',
-                     '\u006E\u002A\u0064',
-                     '\u006D\u002A\u0062',
+                     '\u006E\u0306\u0067',
+                     '\u006E\u0306\u006A',
+                     '\u006E\u0306\u1E0D',
+                     '\u006E\u0306\u0064',
+                     '\u006D\u0306\u0062',
                       ]
-
 NuktaMap = [
-           '\u0051'
+           '\u0308'
            ]
 
 OmMap = [
-        'oM'
+        '\u014D\u1E41'
         ]
 
+Aytham =['\u1E35']
+
 SignMap =[
-         '\u002E\u0061',
+         '’',
          '\u002E',
          '\u002E\u002E'
          ]
 
-Aytham =['\u004B\u005E']
-
 NumeralMap = [
              '\u0030',
              '\u0031',
              '\u0032',
              '\u0033',
              '\u0034',
              '\u0035',
              '\u0036',
              '\u0037',
              '\u0038',
              '\u0039',
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/Roman/Mongolian.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/Mongolian.py`

 * *Files 16% similar despite different names*

```diff
@@ -143,7 +143,13 @@
              '\u1814',
              '\u1815',
              '\u1816',
              '\u1817',
              '\u1818',
              '\u1819',
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/Roman/Mro.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/Mro.py`

 * *Files 18% similar despite different names*

```diff
@@ -143,7 +143,13 @@
              '\U00016A64',
              '\U00016A65',
              '\U00016A66',
              '\U00016A67',
              '\U00016A68',
              '\U00016A69',
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/Roman/RomanColloquial.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/RomanColloquial.py`

 * *Files 16% similar despite different names*

```diff
@@ -38,16 +38,16 @@
 SouthVowelSignMap = SouthVowelMap[:]
 
 ModernVowelSignMap = ModernVowelMap[:]
 
 SinhalaVowelSignMap = SinhalaVowelMap[:]
 
 AyogavahaMap = [
-               'm\'',
-               'm\'',
+               '\u004D',
+               '\u004D',
                'h'
                ]
 
 ViramaMap =  [
              '\u00D7'
              ]
 
@@ -143,7 +143,13 @@
              '\u0034',
              '\u0035',
              '\u0036',
              '\u0037',
              '\u0038',
              '\u0039',
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/Roman/RomanKana.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/RomanKana.py`

 * *Files 23% similar despite different names*

```diff
@@ -143,7 +143,13 @@
              '\u0034',
              '\u0035',
              '\u0036',
              '\u0037',
              '\u0038',
              '\u0039',
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/Roman/RomanReadable.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/DevanagariRomanLoC.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,149 +1,154 @@
 # -*- coding: utf-8 -*-
 
 # Script Mapping for ISO
 
 VowelMap =  [
             '\u0061',
-            'aa',
+            '\u0101',
             '\u0069',
-            'ee',
+            '\u012B',
             '\u0075',
-            'oo',
-            'ri\'',
-            'ree\'',
-            'li\'',
-            'lee\'',
-            'e',
-            'ai',
-            'o',
-            'au'
+            '\u016B',
+            '\u0072\u0325',
+            '\u0072\u0325\u0304',
+            '\u006C\u0325',
+            '\u006C\u0325\u0304',
+            '\u0065',
+            '\u0061\u0069',
+            '\u006F',
+            '\u0061\u0075'
             ]
 
 SouthVowelMap = [
-                'e\'',
-                'o\'',
+                '\u0115',
+                '\u014F',
                 ]
 
 ModernVowelMap = [
-                 'a',
-                 'o',
+                 'ê',
+                 '\u00F4',
                  ]
 
 SinhalaVowelMap = [
-                  'e'
+                  '\u01E3'
                   ]
 
 VowelSignMap =  VowelMap[1:]
 
 SouthVowelSignMap = SouthVowelMap[:]
 
 ModernVowelSignMap = ModernVowelMap[:]
 
 SinhalaVowelSignMap = SinhalaVowelMap[:]
 
 AyogavahaMap = [
-               'm\'',
-               '\u004D',
-               'h\''
+               '\u006D\u0310',
+               'ṃ',
+               '\u1E25'
                ]
 
 ViramaMap =  [
              '\u00D7'
              ]
 
 ConsonantMap =  [
                 '\u006B',
                 '\u006B\u0068',
                 '\u0067',
                 '\u0067\u0068',
-                'ng',
+                '\u1E45',
 
-                'ch',
-                'chh',
+                '\u0063',
+                '\u0063\u0068',
                 '\u006A',
                 '\u006A\u0068',
-                'nj',
+                '\u00F1',
 
-                't\'',
-                't\'h',
-                'd\'',
-                'd\'h',
-                'n',
-
-                't',
-                'th',
-                'd',
-                'dh',
+                '\u1E6D',
+                '\u1E6D\u0068',
+                '\u1E0D',
+                '\u1E0D\u0068',
+                '\u1E47',
+
+                '\u0074',
+                '\u0074\u0068',
+                '\u0064',
+                '\u0064\u0068',
                 '\u006E',
 
                 '\u0070',
                 '\u0070\u0068',
                 '\u0062',
                 '\u0062\u0068',
                 '\u006D',
 
                 '\u0079',
                 '\u0072',
                 '\u006C',
                 '\u0076',
 
-                'sh',
-                'sh',
+                '\u015B',
+                '\u1E63',
                 '\u0073',
                 '\u0068',
                 ]
 
 SouthConsonantMap = [
-                    'l\'',
-                    'zh',
-                    'r\'',
-                    'n'
+                    'ḻ',
+                    'l̳',
+                    '\u1E5F',
+                    '\u1E49'
                     ]
 
 NuktaConsonantMap =  [
-                     'q',
-                     'kh',
-                     'g',
-                     'z',
-                     'r',
-                     'rh',
-                     'f',
-                     'y'
+                     '\u0071',
+                     '\u006B\u035F\u0068',
+                     'g͟h',
+                     '\u007A',
+                     '\u1E5B',
+                     '\u1E5B\u0068',
+                     '\u0066',
+                     '\u1E8F'
                      ]
 
 SinhalaConsonantMap =[
-                     'ng',
-                     'nj',
-                     'nd\'',
-                     'nd',
-                     'mb',
+                     '\u006E\u0306\u0067',
+                     '\u006E\u0306\u006A',
+                     '\u006E\u0306\u1E0D',
+                     '\u006E\u0306\u0064',
+                     '\u006D\u0306\u0062',
                       ]
-
 NuktaMap = [
-           '\u02BD\u02BD'
+           '\u0308'
            ]
 
 OmMap = [
-        'om'
+        'oṃ'
         ]
 
+Aytham =['\u1E35']
+
 SignMap =[
-         '\'',
+         '’',
          '\u002E',
          '\u002E\u002E'
          ]
 
-Aytham =['g']
-
 NumeralMap = [
              '\u0030',
              '\u0031',
              '\u0032',
              '\u0033',
              '\u0034',
              '\u0035',
              '\u0036',
              '\u0037',
              '\u0038',
              '\u0039',
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/Roman/RomanSemitic.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/BalineseSimpleRomanLoC.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,165 +1,154 @@
 # -*- coding: utf-8 -*-
 
 # Script Mapping for ISO
 
 VowelMap =  [
-            'â',
-            'ā̂', # A
-            'î', #i
-            'ī̂', #I
-            'û', # u
-            'ū̂', # U
-            'ru\u02BD',
-            'rū\u02BD',
-            'lu\u02BD',
-            'lū\u02BD',
-            'ē̂', #e
-            'âŷ', #ai
-            'ō̂', #o
-            'âŵ' #au
+            '\u0061',
+            '\u0101',
+            '\u0069',
+            '\u012B',
+            '\u0075',
+            '\u016B',
+            'rĕ',
+            'rö',
+            'lĕ',
+            'lö',
+            'e',
+            '\u0061\u0069',
+            'o',
+            '\u0061\u0075'
             ]
 
 SouthVowelMap = [
-                'ê',
-                'ô'
+                'ĕ\u02BD',
+                'ŏ\u02BD',
                 ]
 
 ModernVowelMap = [
-                 'ē̂\u02BD',
-                 'ā̂\u02BD'
+                 'ĕ',
+                 '\u00F4',
                  ]
 
 SinhalaVowelMap = [
-                  'ê\u02BD'
+                  'ö'
                   ]
 
-VowelSignMap =  [
-            'ā', # A
-            'i', #i
-            'ī', #I
-            'u', # u
-            'ū', # U
-            '\u033Dru\u02BD',
-            '\u033Drū\u02BD',
-            '\u033Dru\u02BD',
-            '\u033Drū\u02BD',
-            'ē', #e
-            'aŷ', #ai
-            'ō', #o
-            'aŵ' #au
-]
+VowelSignMap =  VowelMap[1:]
 
-SouthVowelSignMap = ['e','o']
+SouthVowelSignMap = SouthVowelMap[:]
 
-ModernVowelSignMap = ['e\u02BD','ā\u02BD']
+ModernVowelSignMap = ModernVowelMap[:]
 
-SinhalaVowelSignMap = [
-                  'ē\u02BD'
-                  ]
+SinhalaVowelSignMap = SinhalaVowelMap[:]
 
 AyogavahaMap = [
-               'ₘ',
-               'ₘ', ## Check nasalization
-               'h\u033D\u02BD'
+               'ng',
+               'ng',
+               'h'
                ]
 
 ViramaMap =  [
-             '\u033D'
+             '\u00D7'
              ]
 
 ConsonantMap =  [
-                'k',
-                'kʰ',
-                'g',
-                'gʰ',
-                'n\u02BD',
-
-                'č',
-                'čʰ',
-                'j',
-                'jʰ',
-                'ɲ',
-
-                'ʈ',
-                'ʈʰ',
-                'ɖ',
-                'ɖʰ',
-                'ɳ',
-
-                't',
-                'tʰ',
-                'd',
-                'dʰ',
+                '\u006B',
+                'k\u02BD',
+                '\u0067',
+                'g\u0068',
+                'ng',
+
+                '\u0063',
+                '\u0063\u02BD',
+                '\u006A',
+                '\u006A\u02BD',
+                '\u00F1',
+
+                '\u1E6D',
+                '\u1E6D\u02BD',
+                '\u1E0D',
+                '\u1E0D\u02BD',
                 'n',
 
-                'p',
-                'pʰ',
-                'b',
-                'bʰ',
-                'm',
-
-                'y',
-                'r',
-                'l',
-                'v',
+                '\u0074',
+                '\u0074\u02BD',
+                '\u0064',
+                '\u0064\u0068',
+                '\u006E',
+
+                '\u0070',
+                '\u0070\u02BD',
+                '\u0062',
+                '\u0062\u02BD',
+                '\u006D',
+
+                '\u0079',
+                '\u0072',
+                '\u006C',
+                'w',
 
-                'š',
-                'ʂ',
                 's',
-                'h',
+                's',
+                '\u0073',
+                '\u0068',
                 ]
 
 SouthConsonantMap = [
-                    'ɭ',
-                    'ɭ\u02BD',
-                    'r\u02BD',
-                    'n\u02BD'
+                    '\u1E37',
+                    '\u1E3B',
+                    '\u1E5F',
+                    '\u1E49'
                     ]
 
 NuktaConsonantMap =  [
-                     'q',
-                     'ḫ',
-                     'ġ',
-                     'z',
-                     'ɽ',
-                     'ɽʰ',
-                     'f',
-                     'y\u02BD'
+                     'kh\u02BD',
+                     '\u006B\u035F\u0068',
+                     'gh\u02BD',
+                     '\u007A',
+                     '\u1E5B',
+                     '\u1E5B\u0068',
+                     '\u0066',
+                     '\u1E8F'
                      ]
 
 SinhalaConsonantMap =[
-                     'n\u033Dg\u02BD',
-                     'n\u033Dj\u02BD',
-                     'n\u033Dd\u02BD',
-                     'n\u033Dd\u02BD',
-                     'm\u033Db\u02BD',
+                     '\u006E\u0306\u0067',
+                     '\u006E\u0306\u006A',
+                     '\u006E\u0306\u1E0D',
+                     '\u006E\u0306\u0064',
+                     '\u006D\u0306\u0062',
                       ]
-
 NuktaMap = [
-           'Q'
+           '\u0308'
            ]
 
 OmMap = [
-        'ō̂m\u033D\u02BD'
+        '\u014D\u1E41'
         ]
 
+Aytham =['\u1E35']
+
 SignMap =[
-         '\u02BD\u02BD\u02BD\u02BD',
-         '.',
-         '..'
+         '’',
+         '\u002E',
+         '\u002E\u002E'
          ]
 
-Aytham =['h\u033D\u02BD']
-
 NumeralMap = [
              '\u0030',
              '\u0031',
              '\u0032',
              '\u0033',
              '\u0034',
              '\u0035',
              '\u0036',
              '\u0037',
              '\u0038',
              '\u0039',
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/Roman/RussianCyrillic.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/RussianCyrillic.py`

 * *Files 27% similar despite different names*

```diff
@@ -143,7 +143,13 @@
              '\u0034',
              '\u0035',
              '\u0036',
              '\u0037',
              '\u0038',
              '\u0039',
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/Roman/SLP1.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/SLP1.py`

 * *Files 24% similar despite different names*

```diff
@@ -143,7 +143,13 @@
              '\u0034',
              '\u0035',
              '\u0036',
              '\u0037',
              '\u0038',
              '\u0039',
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/Roman/Santali.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/Santali.py`

 * *Files 15% similar despite different names*

```diff
@@ -143,7 +143,13 @@
              '\u1C54',
              '\u1C55',
              '\u1C56',
              '\u1C57',
              '\u1C58',
              '\u1C59',
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/Roman/SoraSompeng.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/SoraSompeng.py`

 * *Files 24% similar despite different names*

```diff
@@ -146,7 +146,13 @@
              '\U000110F4',
              '\U000110F5',
              '\U000110F6',
              '\U000110F7',
              '\U000110F8',
              '\U000110F9',
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/Roman/Titus.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/ISOPali.py`

 * *Files 12% similar despite different names*

```diff
@@ -39,51 +39,51 @@
 
 ModernVowelSignMap = ModernVowelMap[:]
 
 SinhalaVowelSignMap = SinhalaVowelMap[:]
 
 AyogavahaMap = [
                '\u006D\u0310',
-               '\u1E43',
+               '\u1E41',
                '\u1E25'
                ]
 
 ViramaMap =  [
              '\u00D7'
              ]
 
 ConsonantMap =  [
                 '\u006B',
-                '\u006B\u02B0',
+                '\u006B\u0068',
                 '\u0067',
-                '\u0067\u02B0',
+                '\u0067\u0068',
                 '\u1E45',
 
                 '\u0063',
-                '\u0063\u02B0',
+                '\u0063\u0068',
                 '\u006A',
-                '\u006A\u02B0',
+                '\u006A\u0068',
                 '\u00F1',
 
                 '\u1E6D',
-                '\u1E6D\u02B0',
+                '\u1E6D\u0068',
                 '\u1E0D',
-                '\u1E0D\u02B0',
+                '\u1E0D\u0068',
                 '\u1E47',
 
                 '\u0074',
-                '\u0074\u02B0',
+                '\u0074\u0068',
                 '\u0064',
-                '\u0064\u02B0',
+                '\u0064\u0068',
                 '\u006E',
 
                 '\u0070',
-                '\u0070\u02B0',
+                '\u0070\u0068',
                 '\u0062',
-                '\u0062\u02B0',
+                '\u0062\u0068',
                 '\u006D',
 
                 '\u0079',
                 '\u0072',
                 '\u006C',
                 '\u0076',
 
@@ -98,52 +98,57 @@
                     '\u1E3B',
                     '\u1E5F',
                     '\u1E49'
                     ]
 
 NuktaConsonantMap =  [
                      '\u0071',
-                     '\u006B\u035F\u02B0',
+                     '\u006B\u035F\u0068',
                      '\u0121',
                      '\u007A',
                      '\u1E5B',
-                     '\u1E5B\u02B0',
+                     '\u1E5B\u0068',
                      '\u0066',
                      '\u1E8F'
                      ]
 
+SinhalaConsonantMap =[
+                     '\u006E\u0306\u0067',
+                     '\u006E\u0306\u006A',
+                     '\u006E\u0306\u1E0D',
+                     '\u006E\u0306\u0064',
+                     '\u006D\u0306\u0062',
+                      ]
 NuktaMap = [
            '\u0308'
            ]
 
 OmMap = [
-        '\u006F\u1E43'
+        '\u006F\u1E41'
         ]
 
+Aytham =['\u1E35']
+
 SignMap =[
-         '\u0027',
+         '’\u02BD',
          '\u002E',
          '\u002E\u002E'
          ]
 
-SinhalaConsonantMap =[
-                     '\u006E\u0306\u0067',
-                     '\u006E\u0306\u006A',
-                     '\u006E\u0306\u1E0D',
-                     '\u006E\u0306\u0064',
-                     '\u006D\u0306\u0062',
-                      ]
-
-Aytham =['\u1E35']
-
 NumeralMap = [
              '\u0030',
              '\u0031',
              '\u0032',
              '\u0033',
              '\u0034',
              '\u0035',
              '\u0036',
              '\u0037',
              '\u0038',
              '\u0039',
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/Roman/TolongSiki.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/TolongSiki.py`

 * *Files 13% similar despite different names*

```diff
@@ -147,7 +147,13 @@
              '\u00A4',
              '\u00A5',
              '\u00A6',
              '\u00A7',
              '\u00A8',
              '\u00A9',
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/Roman/Velthuis.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/GurmukhiLoCRomanLoC.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,149 +1,154 @@
 # -*- coding: utf-8 -*-
 
 # Script Mapping for ISO
 
 VowelMap =  [
             '\u0061',
-            '\u0061\u0061',
+            '\u0101',
             '\u0069',
-            '\u0069\u0069',
+            '\u012B',
             '\u0075',
-            '\u0075\u0075',
-            '\u002E\u0072',
-            '\u002E\u0052',
-            '\u002E\u006C',
-            '\u002E\u004C',
+            '\u016B',
+            '\u0072\u0325',
+            '\u0072\u0325\u0304',
+            '\u006C\u0325',
+            '\u006C\u0325\u0304',
             '\u0065',
             '\u0061\u0069',
             '\u006F',
             '\u0061\u0075'
             ]
 
 SouthVowelMap = [
-                '\u0045',
-                '\u004F',
+                '\u0115',
+                '\u014F',
                 ]
 
 ModernVowelMap = [
-                 '\u0061\u0045',
-                 '\u0061\u004F',
+                 'ê',
+                 '\u00F4',
                  ]
 
 SinhalaVowelMap = [
-                  '\u0041\u0045'
+                  '\u01E3'
                   ]
-    
+
 VowelSignMap =  VowelMap[1:]
-               
+
 SouthVowelSignMap = SouthVowelMap[:]
 
 ModernVowelSignMap = ModernVowelMap[:]
 
 SinhalaVowelSignMap = SinhalaVowelMap[:]
 
 AyogavahaMap = [
-               '\u007E\u006D',
-               '\u002E\u006D',
-               '\u002E\u0068'
+               'm̆',
+               'ṃ',
+               '\u1E25'
                ]
-    
+
 ViramaMap =  [
              '\u00D7'
              ]
 
 ConsonantMap =  [
                 '\u006B',
                 '\u006B\u0068',
                 '\u0067',
                 '\u0067\u0068',
-                '\u0022\u006E',
-                
+                '\u1E45',
+
                 '\u0063',
                 '\u0063\u0068',
                 '\u006A',
                 '\u006A\u0068',
-                '\u007E\u006E',
-                
-                '\u002E\u0074',
-                '\u002E\u0074\u0068',
-                '\u002E\u0064',
-                '\u002E\u0064\u0068',
-                '\u002E\u006E',
-                
+                '\u00F1',
+
+                '\u1E6D',
+                '\u1E6D\u0068',
+                '\u1E0D',
+                '\u1E0D\u0068',
+                '\u1E47',
+
                 '\u0074',
                 '\u0074\u0068',
                 '\u0064',
                 '\u0064\u0068',
                 '\u006E',
-                
+
                 '\u0070',
                 '\u0070\u0068',
                 '\u0062',
                 '\u0062\u0068',
                 '\u006D',
-                
+
                 '\u0079',
                 '\u0072',
                 '\u006C',
-                '\u0076',
-                
-                '\u0022\u0073',
-                '\u002E\u0073',
+                'w',
+
+                'sh',
+                '\u1E63',
                 '\u0073',
                 '\u0068',
                 ]
 
 SouthConsonantMap = [
-                    '\u002E\u002E\u006C',
-                    '\u005F\u006C',
-                    '\u005F\u0072',
-                    '\u005F\u006E'
+                    'ḷ',
+                    'l̳',
+                    '\u1E5F',
+                    '\u1E49'
                     ]
 
 NuktaConsonantMap =  [
                      '\u0071',
-                     '\u005F\u006B\u0068',
-                     '\u002E\u0067',
+                     '\u006B\u035F\u0068',
+                     'g͟h',
                      '\u007A',
-                     '\u002E\u002E\u0072',
-                     '\u002E\u002E\u0072\u0068',
+                     '\u1E5B',
+                     '\u1E5B\u0068',
                      '\u0066',
-                     '\u002E\u0079'
+                     '\u1E8F'
                      ]
 
 SinhalaConsonantMap =[
-                     '\u006E\u002A\u0067',
-                     '\u006E\u002A\u006A',
-                     '\u006E\u002A\u002E\u0064',
-                     '\u006E\u002A\u0064',
-                     '\u006D\u002A\u0062',
-                      ] 
-
+                     '\u006E\u0306\u0067',
+                     '\u006E\u0306\u006A',
+                     '\u006E\u0306\u1E0D',
+                     '\u006E\u0306\u0064',
+                     '\u006D\u0306\u0062',
+                      ]
 NuktaMap = [
-           '\u0051'
+           '\u0308'
            ]
-    
+
 OmMap = [
-        'o.m'
+        'o\u1E41'
         ]
 
+Aytham =['\u1E35']
+
 SignMap =[
-         '\u002E\u0061',
+         '’',
          '\u002E',
          '\u002E\u002E'
          ]
 
-Aytham =['\u005F\u006B']
-
 NumeralMap = [
              '\u0030',
              '\u0031',
              '\u0032',
              '\u0033',
              '\u0034',
              '\u0035',
              '\u0036',
              '\u0037',
              '\u0038',
              '\u0039',
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/Roman/WX.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/Ariyaka.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,149 +1,155 @@
 # -*- coding: utf-8 -*-
 
 # Script Mapping for ISO
 
 VowelMap =  [
-            '\u0061',
-            '\u0041',
-            '\u0069',
-            '\u0049',
-            '\u0075',
-            '\u0055',
-            '\u0071',
-            '\u0071\u0056',
-            '\u004C',
-            '\u004C\u0056',
-            '\u0065',
-            '\u0045',
-            '\u006F',
-            '\u004F'
+            'a',
+            'A',
+            'i',
+            'I',
+            'u',
+            'U',
+            'ru\u02BD',
+            'rU\u02BD',
+            'lu\u02BD',
+            'lU\u02BD',
+            'e',
+            'ai',
+            'o',
+            'au'
             ]
 
 SouthVowelMap = [
-                '\u0065\u0056',
-                '\u006F\u0056',
+                'e\u02BD',
+                'o\u02BD',
                 ]
 
 ModernVowelMap = [
-                 '\u0061\u0045\u0056',
-                 '\u0061\u004F\u0056',
+                'e\u02BD',
+                'A',
                  ]
 
 SinhalaVowelMap = [
-                  '\u0041\u0045\u0056'
+                'e\u02BD',
                   ]
 
 VowelSignMap =  VowelMap[1:]
 
 SouthVowelSignMap = SouthVowelMap[:]
 
 ModernVowelSignMap = ModernVowelMap[:]
 
 SinhalaVowelSignMap = SinhalaVowelMap[:]
 
 AyogavahaMap = [
-               '\u007A',
-               '\u004D',
-               '\u0048'
+               'M\u02BD',
+               'M',
+               'h'
                ]
 
 ViramaMap =  [
              '\u00D7'
              ]
 
 ConsonantMap =  [
-                '\u006B',
-                '\u004B',
-                '\u0067',
-                '\u0047',
-                '\u0066',
-
-                '\u0063',
-                '\u0043',
-                '\u006A',
-                '\u004A',
-                '\u0046',
-
-                '\u0074',
-                '\u0054',
-                '\u0064',
-                '\u0044',
-                '\u004E',
-
-                '\u0077',
-                '\u0057',
-                '\u0078',
-                '\u0058',
-                '\u006E',
-
-                '\u0070',
-                '\u0050',
-                '\u0062',
-                '\u0042',
-                '\u006D',
-
-                '\u0079',
-                '\u0072',
-                '\u006C',
-                '\u0076',
-
-                '\u0053',
-                '\u0052',
-                '\u0073',
-                '\u0068',
+                'k',
+                'K',
+                'g',
+                'G',
+                '~',
+
+                'c',
+                'C',
+                'j',
+                'J',
+                'Y',
+
+                'T',
+                'F',
+                'D',
+                'V',
+                'N',
+
+                't',
+                'f',
+                'd',
+                '@',
+                'n',
+
+                'p',
+                'P',
+                'b',
+                'B',
+                'm',
+
+                'y',
+                'r',
+                'l',
+                'v',
+
+                's\u02BD',
+                's\u02BD',
+                's',
+                'h',
                 ]
 
 SouthConsonantMap = [
-                    '\u006C\u0059',
-                    '\u006C\u0059\u0059',
-                    '\u0072\u0059',
-                    '\u006E\u0059'
+                    'L',
+                    'L\u02BD',
+                    'r\u02BD',
+                    'n\u02BD'
                     ]
 
 NuktaConsonantMap =  [
-                     '\u006B\u0059',
-                     '\u004B\u0059',
-                     '\u0047\u0059',
-                     '\u007A\u0059',
-                     '\u0064\u0059',
-                     '\u0044\u0059',
-                     '\u0050\u0059',
-                     '\u0079\u0059'
+                     'k\u02BD',
+                     'K\u02BD',
+                     'g\u02BD',
+                     'j\u02BD',
+                    'D\u02BD',
+                    'V\u02BD',
+                     'P\u02BD',
+                     'y\u02BD'
                      ]
 
 SinhalaConsonantMap =[
-                     '\u006E\u0059\u0059\u0067',
-                     '\u006E\u0059\u0059\u006A',
-                     '\u006E\u0059\u0059\u0064',
-                     '\u006E\u0059\u0059\u0078',
-                     '\u006D\u0059\u0059\u0062',
+                     'Mg\u02BD',
+                     'Mj\u02BD',
+                     'MD\u02BD',
+                     'Md\u02BD',
+                     'Mb\u02BD',
                       ]
 
 NuktaMap = [
-           '\u0051'
+           '\u02BD\u02BD'
            ]
 
 OmMap = [
-        '\u006F\u004D'
+        'oM'
         ]
 
 SignMap =[
-         'Z',
+         '\u0027',
          '\u002E',
          '\u002E\u002E'
          ]
 
-Aytham =['\u006B\u0059\u0059']
+Aytham =['h\u02BD']
 
 NumeralMap = [
              '\u0030',
              '\u0031',
              '\u0032',
              '\u0033',
              '\u0034',
              '\u0035',
              '\u0036',
              '\u0037',
              '\u0038',
              '\u0039',
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/ScriptMap/Roman/WarangCiti.py` & `aksharamukha-2.2.1/aksharamukha/ScriptMap/Roman/WarangCiti.py`

 * *Files 8% similar despite different names*

```diff
@@ -146,7 +146,13 @@
              '\U000118E4',
              '\U000118E5',
              '\U000118E6',
              '\U000118E7',
              '\U000118E8',
              '\U000118E9',
              ]
+
+from ... import GeneralMap as GM
+
+import os
+GM.add_additional_chars(dict([(charlist, globals()[charlist]) for charlist in GM.CharmapLists]),
+                        os.path.splitext(__file__)[0].split(os.path.sep)[-1])
```

### Comparing `aksharamukha-2.1.2/aksharamukha/gimeltra.py` & `aksharamukha-2.2.1/aksharamukha/gimeltra.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,29 +91,30 @@
         #if sc != 'Latn':
             # chars_missing = set(list(self.db[sc]["Latn"].values())) - set(chars)
 
         #if sc == 'Latn':
             #chars_missing = set(self.db_simplify) -  set(chars) #set(list(self.db[to_sc]["Latn"].values()))
             #print(chars)
 
-        chars_missing = sorted(list(set(self.db_simplify) -  set(chars)), key=len, reverse=True)
+        chars_missing = [x for x in self.db_simplify if x not in chars]
         #chars_missing = list(set(self.db_simplify) -  set(chars))
 
         for char in chars_missing:
             if char in self.db_simplify:
                 #print(char, self.db_simplify[char])
                 ## if Virama is misssing and characts has virama remove virama
                 if '\u033D' in chars_missing and '\u033D' in self.db_simplify[char]:
                     #print('here removing vriama')
                     #print(char, self.db_simplify[char])
                     text = text.replace(char, self.db_simplify[char])
                     text = text.replace('\u033D', self.db_simplify['\u033D'])
                 else:
                     text = text.replace(char, self.db_simplify[char])
 
+
         for char in chars:
             #print(text)
             #print(char + " " + self.db["Latn"][to_sc][char])
             text = text.replace(char, self.db["Latn"][to_sc][char])
             #print(text)
 
         return text
```

### Comparing `aksharamukha-2.1.2/aksharamukha/json/gimeltra_data.json` & `aksharamukha-2.2.1/aksharamukha/json/gimeltra_data.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999997040719697%*

 * *Differences: {"'ssub'": "{'Latn': {'Arab-Fa': {'v': 'و'}}}"}*

```diff
@@ -919,14 +919,15 @@
                 "p": "\u067e",
                 "q": "\u0642",
                 "r": "\u0631",
                 "s": "\u0633",
                 "t": "\u062a",
                 "u": "\u064f",
                 "u\u207f": "\u064c",
+                "v": "\u0648",
                 "w": "\u0648",
                 "y": "\u06cc",
                 "z": "\u0632",
                 "\u00e2": "\u0627\u064e",
                 "\u00e2\u0175": "\u0627\u064e\u0648\u0652",
                 "\u00e2\u0177": "\u0627\u064e\u06cc\u0652",
                 "\u00ea": "\u0627\u0650",
```

### Comparing `aksharamukha-2.1.2/aksharamukha/transliterate.py` & `aksharamukha-2.2.1/aksharamukha/transliterate.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,792 +1,872 @@
-from aksharamukha import GeneralMap
-import re
-
-from aksharamukha.gimeltra import Transliterator
-from . import Convert,PostOptions,PostProcess,PreProcess
-from . import ConvertFix
-import json
-import requests
-import html
-import itertools
-from collections import Counter
-import unicodedata
-import io
-import collections
-import yaml
-import warnings
-import langcodes
-from inspect import getmembers, isfunction
-
-#import sys
-#sys.stdout = None
-
-def removeA(a):
-    if a.count('a') == 1:
-        return a.replace('a', '')
-
-def unique_everseen(iterable, key=None):
-    "List unique elements, preserving order. Remember all elements ever seen."
-    # unique_everseen('AAAABBBCCDAABBB') --> A B C D
-    # unique_everseen('ABBCcAD', str.lower) --> A B C D
-    seen = set()
-    seen_add = seen.add
-    if key is None:
-        for element in itertools.filterfalse(seen.__contains__, iterable):
-            seen_add(element)
-            yield element
-    else:
-        for element in iterable:
-            k = key(element)
-            if k not in seen:
-                seen_add(k)
-                yield element
-
-def auto_detect(text, plugin = False):
-    scripts = []
-
-    for uchar in text:
-        try:
-            script_name = unicodedata.name(uchar).split(' ')[0].lower()
-            if script_name != 'old':
-                scripts.append(script_name)
-            else:
-                scripts.append(unicodedata.name(uchar).split(' ')[1].lower())
-        except ValueError:
-            pass
-            # print('Script not found')
-
-    counts = Counter(scripts)
-    script_percent = []
-
-    for script, count  in counts.items():
-        percent = count/len(scripts) * 100
-        script_percent.append((percent, script))
-
-    #print(sorted(script_percent))
-
-    if not plugin:
-        if len(script_percent) > 0:
-            script = sorted(script_percent)[-1][1]
-        else:
-            script = ''
-    else:
-        #print('here')
-        if len(script_percent) > 0:
-            if sorted(script_percent)[-1][1] == 'latin':
-                script = sorted(script_percent)[-2][1]
-            else:
-                script = sorted(script_percent)[-1][1]
-        else:
-            script = ''
-
-    inputScript = script[0].upper() + script[1:]
-
-    laoPali = ['ຆ', 'ຉ', 'ຌ', 'ຎ', 'ຏ', 'ຐ', 'ຑ', 'ຒ', 'ຓ', 'ຘ', 'ຠ', 'ຨ', 'ຩ', 'ຬ', '຺']
-
-    if inputScript == 'Bengali':
-        if 'ৰ' in text or 'ৱ' in text:
-            inputScript = 'Assamese'
-    elif inputScript == 'Lao':
-        if any(char in text for char in laoPali):
-            inputScript = 'LaoPali'
-    elif inputScript == 'Batak':
-        inputScript = 'BatakKaro'
-    elif inputScript == 'Myanmar':
-        inputScript = 'Burmese'
-
-        mon = ['ၚ', 'ၛ', '္ည', 'ၞ', 'ၟ', 'ၠ', 'ဳ', 'ဨ']
-        if any([char in text for char in mon]):
-            inputScript = 'Mon'
-
-        countSub = {'Shan': 0, 'TaiLaing': 0, 'KhamtiShan': 0}
-
-        text = text.replace('ႃ', '')
-
-        for uchar in text:
-            try:
-                char = unicodedata.name(uchar).lower()
-            except:
-                pass
-            if 'shan' in char:
-                countSub['Shan'] += 1
-            elif 'tai laing' in char:
-                countSub['TaiLaing'] += 1
-            elif 'khamti' in char:
-                countSub['KhamtiShan'] += 1
-
-        import operator
-        sorted_x = sorted(countSub.items(), key=operator.itemgetter(1))
-
-        if countSub['Shan'] > 0 or countSub['TaiLaing'] > 0 or countSub['KhamtiShan'] > 0:
-            inputScript = sorted_x[-1][0]
-
-
-        #shan = ['ႃ', '\u1086', '\u1084', 'ၵ', 'ၶ', 'ၷ', 'ꧠ', 'ၸ', 'ꧡ', 'ꩡ', 'ꧢ', 'ၺ', 'ꩦ', 'ꩧ', 'ꩨ', 'ꩩ', 'ꧣ', 'ၻ', 'ꩪ', 'ၼ','ၽ', 'ꧤ', 'ႁ', 'ꩮ', 'ၹ', 'ၾ']
-        #if any([char in text for char in shan]):
-            #inputScript = 'Shan'
-
-    elif inputScript == 'Meetei':
-        inputScript = 'MeeteiMayek'
-    elif inputScript == 'Persian':
-        inputScript = 'OldPersian'
-    elif inputScript == 'Phags-pa':
-        inputScript = 'PhagsPa'
-    elif inputScript == 'Ol':
-        inputScript = 'Santali'
-    elif inputScript == 'Sora':
-        inputScript = 'SoraSompeng'
-    elif inputScript == 'Syloti':
-        inputScript = 'SylotiNagri'
-    elif inputScript == 'Tai':
-        inputScript = 'TaiTham'
-    elif inputScript == 'Warang':
-        inputScript = 'WarangCiti'
-    elif inputScript == 'Siddham':
-        preOptions = 'siddhamUnicode'
-    elif inputScript == 'Cyrillic':
-        inputScript = 'RussianCyrillic'
-    elif inputScript == 'Zanabazar':
-        inputScript = 'ZanabazarSquare'
-    elif inputScript == 'Syriac':
-        inputScript = 'Syre'
-        eastern_dia = 'ܲ ܵ ܝܼ ܘܼ ܸ ܹ ܘܿ'.split(' ')
-        if any(char in text for char in eastern_dia):
-            inputScript = 'Syrn'
-        western_dia = 'ܰ ܺ ܶ ّ ܽ'.split(' ')
-        if any(char in text for char in western_dia):
-            inputScript = 'Syrj'
-    elif inputScript == 'Arabic':
-        inputScript = 'Arab'
-        persian_char = 'چ گ ژ پ هٔ'.split(' ')
-        if any(char in text for char in persian_char):
-            inputScript = 'Arab-Fa'
-        urdu_char = 'ڈ ٹ ڑ ھ'.split(' ')
-        if any(char in text for char in urdu_char):
-            inputScript = 'Urdu'
-        shahmukh_char = 'ݨ لؕ مھ نھ یھ رھ لھ وھ'.split(" ")
-        if any(char in text for char in shahmukh_char):
-            inputScript = 'Shahmukhi'
-    elif inputScript == 'Latin':
-        diacritics = ['ā', 'ī', 'ū', 'ṃ', 'ḥ', 'ś', 'ṣ', 'ṇ', 'ṛ', 'ṝ', 'ḷ', 'ḹ', 'ḻ', 'ṉ', 'ṟ', 'ṭ', 'ḍ', 'ṅ', 'ñ']
-        Itrans = ['R^i', 'R^I', 'L^i', 'L^I', '.N', '~N', '~n', 'Ch', 'sh', 'Sh']
-        semitic = ['ʾ', 'ʿ', 'š', 'w']
-        BurmeseLOC = ['´', '˝', 'ʻ']
-        if 'ʰ' in text:
-            inputScript = 'Titus'
-        elif any(char in text for char in semitic):
-            inputScript = 'Latn'
-        elif any(char in text for char in BurmeseLOC):
-            inputScript = 'IASTLOC' ## Change for other LoC schemese
-        elif any(char in text for char in diacritics):
-            if 'ē' in text or 'ō' in text or 'r̥' in text:
-                inputScript = 'ISO'
-            else:
-                inputScript = 'IAST'
-        elif any(char in text for char in Itrans):
-            inputScript = 'Itrans'
-        else:
-            inputScript = 'HK'
-    elif inputScript in GeneralMap.IndicScripts or inputScript in GeneralMap.LatinScripts or inputScript in ['Hiragana', 'Katakana']:
-        pass
-    else:
-        from . import gimeltra
-        tr = gimeltra.Transliterator()
-        inputScript = tr.auto_script(text)
-
-    return inputScript
-
-# Cross check with inded convert() funciton within autodetect
-# scripts available here must be added there
-def detect_preoptions(text, inputScript):
-    preoptions = []
-    if inputScript == 'Thai':
-        textNew = text.replace('ห์', '')
-        if '\u035C' in text or '\u0325' in text or 'งํ' in text or '\u0E47' in text:
-            preoptions = ['ThaiPhonetic']
-        elif '์' in textNew and ('ะ' in text):
-            preoptions = ['ThaiSajjhayawithA']
-        elif '์' in textNew:
-            preoptions = ['ThaiSajjhayaOrthography']
-        elif 'ะ' in text or 'ั' in text:
-            preoptions =  ['ThaiOrthography']
-    elif inputScript == 'Lao' or inputScript == 'LaoPali':
-        textNew = text.replace('ຫ໌', '')
-        if '໌' in textNew and ('ະ' in text):
-            preoptions = ['LaoSajhayaOrthographywithA']
-        elif '໌' in textNew:
-            preoptions = ['LaoSajhayaOrthography']
-        elif 'ະ' in text or 'ັ' in text:
-            preoptions = ['LaoTranscription']
-    elif inputScript == 'Urdu':
-            preoptions = ['UrduShortNotShown']
-
-    return preoptions
-
-def convert(src, tgt, txt, nativize, preoptions, postoptions):
-    tgtOld = ""
-
-    ## ALA-LC Romanizations
-    ## If associated script of LoC is not in Source, convert source into that script. The convert it to the actual target
-    ## Text (non-Burmese) -> Burmese -> LoC
-    if tgt == 'IASTLOC' and src != 'Burmese':
-        txt = convert(src, "Burmese", txt, nativize, preoptions, postoptions)
-        src = 'Burmese'
-
-    ## process as follows, if source is associated with LoC script
-    if tgt == 'IASTLOC' and src == 'Burmese':
-        # the below order for preoptions is important
-        preoptions = preoptions + [tgt + src + 'Target']
-        postoptions =  [tgt + src + 'Target'] + postoptions
-        nativize = False
-
-    ## if target is associated with the loc Script
-    if src == 'IASTLOC' and tgt == 'Burmese':
-        preoptions = [src + tgt + 'Source'] + preoptions
-        postoptions =  [src + tgt + 'Source'] + postoptions
-        nativize = False
-
-    ## else convert the Loc input into the associated script and then convert it into Loc
-    ## Text (Loc) -> Burmese -> non-Burmese
-    if src == 'IASTLOC' and tgt != 'Burmese':
-        txt = convert(src, "Burmese", txt, nativize, preoptions, postoptions)
-        src = 'Burmese'
-
-    ## Semitic ISO Standards
-    ### same as below use intermediates to convert non-associated input/output
-    if tgt in GeneralMap.semiticISO.keys():
-        if GeneralMap.semiticISO[tgt] != src:
-            txt = convert(src, GeneralMap.semiticISO[tgt], txt, nativize, preoptions, postoptions)
-            src = GeneralMap.semiticISO[tgt]
-
-        if GeneralMap.semiticISO[tgt] == src:
-            preoptions = [tgt + 'Target'] + preoptions
-            postoptions =  [tgt + 'Target'] + postoptions
-            nativize = False
-            tgt = 'Latn'
-
-    if src in GeneralMap.semiticISO.keys():
-        if GeneralMap.semiticISO[src] == tgt:
-            #print('here1')
-            preoptions = [src + 'Source'] + preoptions
-            postoptions = [src + 'Source'] + postoptions
-            src = 'Latn'
-        else:
-            #print('here2')
-            txt = convert(src, GeneralMap.semiticISO[src], txt, nativize, preoptions, postoptions)
-            src = GeneralMap.semiticISO[src]
-
-    if src == "Itrans" and '##' in txt:
-        textNew = [[i,word] for i, word in enumerate(txt.split("##")) if (i%2 == 0)]
-        textRest = [(i,word) for i, word in enumerate(txt.split("##")) if (i%2 == 1)]
-
-        txt = json.dumps(textNew).replace("\\n", "\n")
-
-    if tgt == "" or tgt == "Ignore":
-        return txt
-    if preoptions == [] and postoptions == [] and nativize == False and src == tgt:
-        return txt
-
-    ## Semitic Switches - Add Shahmukhi/Sindhi later
-    IndicSemiticMapping = { 'Hebrew': 'Hebr', 'Thaana': 'Thaa', 'Urdu': 'Arab-Ur', 'Shahmukhi': 'Arab-Pa'}
-
-    if (tgt in GeneralMap.SemiticScripts or tgt in GeneralMap.semiticISO.keys()) and src in IndicSemiticMapping.keys():
-        src = IndicSemiticMapping[src]
-    if (src in GeneralMap.SemiticScripts or src in GeneralMap.semiticISO.keys()) and tgt in IndicSemiticMapping.keys():
-        tgt = IndicSemiticMapping[tgt]
-    if src in IndicSemiticMapping.keys() and tgt in IndicSemiticMapping.keys():
-        src = IndicSemiticMapping[src]
-        tgt = IndicSemiticMapping[tgt]
-
-    # preserve semitic pattern
-    if not nativize and src == 'Hebrew':
-        src = 'Hebr'
-    if not nativize and src == 'Urdu':
-        src = 'Arab-Ur'
-    if not nativize and src == 'Shahmukhi':
-        src = 'Arab-Pa'
-    if not nativize and src == 'Thaana':
-        src = 'Thaa'
-
-    if src in ['Arab-Ur', 'Arab-Pa'] and tgt in GeneralMap.IndicScripts:
-        txt += '\u05CD'
-
-    ## Semitic to Urdu this is not needed
-    #if src in GeneralMap.SemiticScripts and src not in ['Arab-Fa', 'Arab', 'Latn'] and (tgt in ['Urdu', 'Shahmukhi']):
-    #    tgt = 'Arab-Fa'
-
-    ## recheck this the logic is missing :: This is not required
-    """if src in ['Urdu', 'Shahmukhi'] and tgt == 'Arab':
-        #print('Semiticizing Urdu')
-        txt = PreProcess.semiticizeUrdu(txt)
-        txt = PreProcess.ArabizePersian(txt)
-        src = "Arab-Fa"
-        tgt = "Arab"
-
-    if src in ['Urdu', 'Shahmukhi'] and tgt == 'Arab-Fa':
-        txt = PreProcess.semiticizeUrdu(txt)
-        src = "none"
-        tgt = "none"
-
-    if src == 'Arab-Fa' and tgt == 'Arab':
-        txt = PreProcess.ArabizePersian(txt)
-        #src = "none"
-        #tgt = "none"
-
-    if src  == 'Arab' and tgt == 'Arab-Fa':
-        txt = PreProcess.perisanizeArab(txt)
-        src = "none"
-        tgt = "none"
-
-    if src  == 'Arab' and tgt in ['Urdu', 'Shahmukhi']:
-        txt = PreProcess.perisanizeArab(txt)
-        src = "none"
-        tgt = "Arab-Fa"
-
-    if src in 'Arab-Fa' and tgt in ['Urdu', 'Shahmukhi']:
-        src = "none"
-        tgt = "none" """
-
-    ## Semitic Naivization : remove pesky Nuktas
-    if nativize:
-        if src in GeneralMap.SemiticScripts and tgt in GeneralMap.IndicScripts:
-            txt += "\u05CC"
-
-    if src == tgt and (src != 'Hiragana' and src != 'Katakana') and src not in GeneralMap.SemiticScripts:
-        tgtOld = tgt
-        tgt = "Devanagari"
-
-    txt = PreProcess.PreProcess(txt,src,tgt)
-
-    if 'siddhammukta' in postoptions and tgt == 'Siddham':
-        tgt = 'SiddhamDevanagari'
-    if 'siddhamap' in postoptions and tgt == 'Siddham':
-        tgt = 'SiddhamDevanagari'
-    if 'siddhammukta' in preoptions and src == 'Siddham':
-        src = 'SiddhamDevanagari'
-    if 'LaoNative' in postoptions and tgt == 'Lao':
-        tgt = 'Lao2'
-    if 'egrantamil' in preoptions and src == 'Grantha':
-        src = 'GranthaGrantamil'
-    if 'egrantamil' in postoptions and tgt == 'Grantha':
-        tgt = 'GranthaGrantamil'
-    if 'nepaldevafont' in postoptions and tgt == 'Newa':
-        tgt = 'Devanagari'
-    if 'ranjanalantsa' in postoptions and tgt == 'Ranjana':
-        tgt = 'Tibetan'
-        nativize = False
-    if 'ranjanawartu' in postoptions and tgt == 'Ranjana':
-        tgt = 'Tibetan'
-        nativize = False
-    if 'SoyomboFinals' in postoptions and tgt == 'Soyombo':
-        txt = '\u02BE' + txt
-    #if src not in GeneralMap.SemiticScripts and tgt == 'Arab' and not nativize:
-        #postoptions.append('arabicRemoveAdditionsPhonetic')
-
-    for options in preoptions:
-      txt = getattr(PreProcess, options)(txt)
-
-    ### Semitic Switches
-    if 'novowelshebrew' in preoptions and src == 'Hebr':
-        txt = txt.replace('\u05B7', '')
-
-    srcOld = ""
-
-    ### retain Latin ###
-    if (src != 'Latn'and src != 'Type' and src in GeneralMap.SemiticScripts) or \
-        (src in GeneralMap.IndicScripts and tgt in GeneralMap.SemiticScripts and src not in GeneralMap.LatinScripts) or \
-            (src in ['Hiragana', 'Katakana']):
-        txt = PreProcess.retainLatin(txt)
-
-    if src == 'Hiragana' or src == 'Katakana':
-        txt = PreProcess.JapanesePreProcess(src, txt, preoptions)
-        srcOld = 'Japanese'
-        src = 'ISO'
-
-    if tgt == 'Hiragana' or tgt == 'Katakana':
-        txt = PostProcess.JapanesePostProcess(src, tgt, txt, nativize, postoptions)
-
-    if src == "Oriya" and tgt == "IPA":
-        txt = ConvertFix.OriyaIPAFixPre(txt)
-
-    if src == "Itrans" and '##' in txt:
-        #print('I am here tyring to do things')
-        transliteration = ''
-        for i, word in enumerate(txt.split("##")):
-            if (i%2 == 0):
-                transliteration += Convert.convertScript(word, src, tgt)
-            else:
-                transliteration += word
-    else:
-        transliteration = Convert.convertScript(txt, src, tgt)
-
-    #print(transliteration)
-
-    if srcOld == 'Japanese' and tgt != 'Devanagari' and 'siddhammukta' not in postoptions:
-        transliteration = Convert.convertScript(transliteration, "Devanagari", "ISO")
-
-    if src == tgtOld:
-        tgt = tgtOld
-        transliteration = Convert.convertScript(transliteration, "Devanagari", tgt)
-
-    ## apply phonetic mapping for Arabic beforehand if not semitic source
-    if (src not in GeneralMap.SemiticScripts and tgt == 'Arab' and nativize) or 'arabicRemoveAdditionsPhonetic' in postoptions:
-        transliteration = getattr(PostProcess, 'arabicRemoveAdditionsPhonetic')(transliteration)
-
-    #print(transliteration)
-
-    if nativize:
-      transliteration =  PostOptions.ApplyScriptDefaults(transliteration, src, tgt, postoptions)
-      if tgt != 'Latn':
-        if tgt != 'Tamil':
-            transliteration = PostProcess.RemoveDiacritics(transliteration)
-        else:
-            transliteration = PostProcess.RemoveDiacriticsTamil(transliteration)
-
-    #print(transliteration)
-
-    if 'RemoveDiacritics' in postoptions:
-      if tgt == 'Tamil':
-        postoptions = map(lambda x: 'RemoveDiacriticsTamil' if x == 'RemoveDiacritics' else x, postoptions)
-
-    for options in postoptions:
-      transliteration = getattr(PostProcess, options)(transliteration)
-
-    if src == "Tamil" and tgt == "IPA":
-        r = requests.get("http://anunaadam.appspot.com/api?text=" + txt + "&method=2")
-        r.encoding = r.apparent_encoding
-        transliteration = r.text
-
-    if src == "Oriya" and tgt == "IPA":
-        transliteration = ConvertFix.OriyaIPAFix(transliteration)
-
-    if src == "Itrans" and '##' in txt:
-        textConv = {**dict(list(json.loads(transliteration.replace("\n", "\\n")))), ** dict(textRest)}
-        textConv = collections.OrderedDict(sorted(textConv.items()))
-        transliteration = "".join(textConv.values())
-
-    ### return Latin ###
-    transliteration = PreProcess.retainLatin(transliteration, reverse=True)
-
-    #print(transliteration)
-
-    return transliteration
-
-def process(src, tgt, txt, nativize = True, post_options = [], pre_options = [], param="default"):
-    if param == "default":
-        return process_default(src, tgt, txt, nativize, post_options, pre_options)
-
-    if param == "script_code":
-        return process_script_tag(src, tgt, txt, nativize, post_options, pre_options)
-
-    if param == "lang_code":
-        return process_lang_tag(src, tgt, txt, nativize, post_options, pre_options)
-
-    if param == "lang_name":
-        return process_lang_name(src, tgt, txt, nativize, post_options, pre_options)
-
-import functools
-
-@functools.cache
-def _load_data(file_path):
-    import os
-    dir_path = os.path.dirname(os.path.realpath(__file__))
-    with open(dir_path + file_path, 'r', encoding='utf8') as stream:
-        data_loaded = yaml.safe_load(stream)
-    return data_loaded
-
-def convert_default(src, tgt, txt, nativize = True, post_options = [], pre_options = []):
-    data_loaded = _load_data("/yaml/aksharamukha-scripts.yaml")
-
-    scriptList = GeneralMap.IndicScripts + GeneralMap.LatinScripts + GeneralMap.SemiticScripts
-
-    preOptionList = list(map(lambda x: x[0], getmembers(PreProcess, isfunction)))
-    preOptionListLower = list(map(lambda x: x.lower(), preOptionList))
-
-    postOptionList = list(map(lambda x: x[0], getmembers(PostProcess, isfunction)))
-    postOptionListLower = list(map(lambda x: x.lower(), postOptionList))
-
-    post_options = [option_id for option in post_options for option_id in postOptionList if option.lower() == option_id.lower()]
-    pre_options = [option_id for option in pre_options for option_id in preOptionList if option.lower() == option_id.lower()]
-
-    # font hack warning
-    font_hack_warning = tgt + ' uses an hacked font to display the script. In the absence of this font, you text may appear different. \n See: https://aksharamukha.appspot.com/describe/' + tgt + ' for the font used'
-
-    if tgt in data_loaded and 'font_hack' in data_loaded[tgt]:
-        warnings.warn(font_hack_warning)
-
-    if src not in scriptList:
-        script_not_found = 'Source script: ' + src + ' not found in the list of scripts supported. The text will not be transliterated.'
-        warnings.warn(script_not_found)
-
-    if tgt not in scriptList:
-        script_not_found = 'Target script: ' + tgt + ' not found in the list of scripts supported. The text will not be transliterated.'
-        warnings.warn(script_not_found)
-
-    return convert(src, tgt, txt, nativize, pre_options, post_options)
-
-def process_default(src, tgt, txt, nativize, post_options, pre_options):
-    scriptList = GeneralMap.IndicScripts + GeneralMap.LatinScripts
-    scriptListLower = list(map(lambda x: x.lower(), scriptList))
-
-    if src == 'autodetect':
-        src = auto_detect(txt)
-        #print('The autodetection is ' + src)
-        pre_options = detect_preoptions(txt, src)
-    elif src.lower() in scriptListLower:
-        src = [script_id for script_id in scriptList if src.lower() == script_id.lower()][0]
-
-    if tgt.lower() in scriptListLower:
-        tgt = [script_id for script_id in scriptList if tgt.lower() == script_id.lower()][0]
-
-    return convert_default(src, tgt, txt, nativize, post_options, pre_options)
-
-
-def process_script_tag(src_tag, tgt_tag, txt, nativize, post_options, pre_options):
-    # Read YAML file
-    data_loaded = _load_data("/yaml/aksharamukha-scripts.yaml")
-
-    data_loaded_wiki = _load_data("/yaml/wikitra2-data.yaml")
-
-    src = []
-    tgt = []
-
-    if src_tag == 'Syrc':
-        src_tag = 'Syre'
-        warnings.warn("Please specify the variety of Syriac script for the source: Estrangelo (Syre), Eastern (Syrn) or Wester (Syrj). Defaulting to Syre")
-    if tgt_tag == 'Syrc':
-        tgt_tag = 'Syre'
-        warnings.warn("Please specify the variety of Syriac script for the target: Estrangelo (Syre), Eastern (Syrn) or Wester (Syrj). Defaulting to Syre")
-
-    # loop through yaml to find match
-    for scrpt in data_loaded.keys():
-        scrpt_tag = data_loaded[scrpt]['script']
-
-        # get the popuation of each language of the script
-        if 'lang' in data_loaded[scrpt].keys():
-            lang_tag = data_loaded[scrpt]['lang'].split(',')[0]
-            lang = list(map(lambda x: x.lower(), data_loaded[scrpt]['lang'].split(',')))
-        else:
-            population = 0
-            lang = ''
-
-        #print(scrpt_tag, lang_tag)
-        if scrpt_tag in data_loaded_wiki.keys() and lang_tag in data_loaded_wiki[scrpt_tag].keys():
-            population = data_loaded_wiki[scrpt_tag][lang_tag]['population']
-        else:
-            population = 0
-
-        # find the match in the file
-        if '-' not in src_tag and data_loaded[scrpt]['script'].lower() == src_tag.lower():
-            src.append((population, scrpt))
-
-        if '-' not in tgt_tag and data_loaded[scrpt]['script'].lower() == tgt_tag.lower():
-            tgt.append((population, scrpt))
-
-        #print(population)
-        # if hypthenated find the exact match
-        if '-' in tgt_tag:
-            lang_part = tgt_tag.split('-')[0].lower()
-            script_part = tgt_tag.split('-')[1].lower()
-
-            if scrpt_tag.lower() == script_part.lower() and 'lang' in data_loaded[scrpt].keys() and lang_part.lower() in lang:
-                tgt.append((0, scrpt))
-
-        if '-' in src_tag:
-            lang_part = src_tag.split('-')[0].lower()
-            script_part = src_tag.split('-')[1].lower()
-
-            if scrpt_tag.lower() == script_part.lower() and 'lang' in data_loaded[scrpt].keys() and lang_part.lower() in lang:
-                src.append((0, scrpt))
-
-    if src_tag.lower() in ['latn', 'en', 'eng']:
-        warn = "Latin has multiple transcription schemes. 'ISO 15919' has been selected by default"
-        warn += "\n Please use a transcription format e.g. la-IAST or la-HK to select a particular scheme"
-        warnings.warn(warn)
-
-        src = [(0, 'ISO')]
-
-    if tgt_tag.lower() in ['latn', 'en', 'eng']:
-        warn = "Latin has multiple transcription schemes. 'ISO 15919' has been selected by default"
-        warn += "\n Please use a transcription format e.g. la-IAST or la-HK to select a particular scheme"
-        warnings.warn(warn)
-
-        tgt = [(0, 'ISO')]
-
-    # if latin ignore la and get the following part
-    if '-' in src_tag and src_tag.split('-')[0].lower() in ['latn', 'en', 'eng']:
-        src = [(0, src_tag.split('-')[1])]
-
-    if '-' in tgt_tag and tgt_tag.split('-')[0].lower() in ['latn', 'en', 'eng']:
-        tgt = [(0, tgt_tag.split('-')[1])]
-
-    if src_tag == 'autodetect':
-        src = [(0, auto_detect(txt))]
-        pre_options = detect_preoptions(txt, src)
-
-    if len(src) > 0:
-        src_pop = sorted(src, reverse=True)[0][1]
-    elif src_tag in GeneralMap.SemiticScripts:
-            src_pop = src_tag
-    else:
-        raise Exception('Source script code: ' + src_tag + ' not found')
-
-    if len(tgt) > 0:
-        tgt_pop = sorted(tgt, reverse=True)[0][1]
-    elif tgt_tag in GeneralMap.SemiticScripts:
-        tgt_pop = tgt_tag
-    else:
-        raise Exception('Target script code: ' + tgt_tag + ' not found')
-
-    if len(src) > 1:
-        warn = "Multiple orthographies, " + ','.join(map(lambda x: x[1], src)) + ", are associated with the input script. The most popular '" + src_pop + "' has been selected"
-        warn += "\n Please use the format lang_code-script_code e.g. ur-Arab or pa-Arab to select a particular orthography"
-
-        warnings.warn(warn)
-    if len(tgt) > 1:
-        warn = "Multiple orthographies: " + ', '.join(map(lambda x: x[1], tgt)) + " are associated with the target script. The most popular '" + tgt_pop + "' has been selected"
-        warn += "\n Please use the format lang_code-script_code e.g. ur-Arab or pa-Arab to select a particular orthography"
-        warnings.warn(warn)
-
-    return process_default(src_pop, tgt_pop, txt, nativize, post_options, pre_options)
-
-def process_lang_tag(src_tag, tgt_tag, txt, nativize, post_options, pre_options):
-    # Read YAML file
-    data_loaded = _load_data("/yaml/aksharamukha-scripts.yaml")
-
-    data_loaded_wiki = _load_data("/yaml/wikitra2-data.yaml")
-
-    src = []
-    tgt = []
-
-    # iterate through the yaml file
-    for scrpt in data_loaded.keys():
-        if 'lang' in data_loaded[scrpt].keys():
-            lang = list(map(lambda x: x.lower(), data_loaded[scrpt]['lang'].split(',')))
-        else:
-            lang = ''
-
-        scrpt_tag = data_loaded[scrpt]['script']
-
-        # try to get the popular script from wiktionary file
-        if scrpt_tag in data_loaded_wiki.keys():
-            script_count = len(data_loaded_wiki[scrpt_tag])
-        else:
-            script_count = 1
-
-        # trying to find the match in the yaml file
-        if src_tag.lower() in lang:
-            src.append((script_count, scrpt))
-
-        if tgt_tag.lower() in lang:
-            tgt.append((script_count, scrpt))
-
-        if '-' in tgt_tag:
-            lang_part = tgt_tag.split('-')[0].lower()
-            script_part = tgt_tag.split('-')[1].lower()
-
-            if scrpt_tag.lower() == script_part and lang_part in lang:
-                tgt.append((0, scrpt))
-
-        if '-' in src_tag:
-            lang_part = src_tag.split('-')[0].lower()
-            script_part = src_tag.split('-')[1].lower()
-
-            if scrpt_tag.lower() == script_part and lang_part in lang:
-                src.append((0, scrpt))
-
-    if src_tag.lower() in ['sa','san', 'pi', 'pli']:
-        warn = "The input language: " + src_tag + " is script-agnostic and can be written in multiple scripts. The most popular 'Devanagari' has been selected"
-        warn += "\n Please use the format lang_code-script_code e.g. sa-Gran or sa-Sidd to select a particular script"
-        warnings.warn(warn)
-
-        src = [(0, 'Devanagari')]
-
-    if tgt_tag.lower() in ['sa','san', 'pi', 'pli']:
-        warn = "The ouptput language: " + tgt_tag + " is script-agnostic and can be written in multiple scripts. The most popular 'Devanagari' has been selected"
-        warn += "\n Please use the format lang_code-script_code e.g. sa-Gran or sa-Sidd to select a particular script"
-        warnings.warn(warn)
-
-        tgt = [(0, 'Devanagari')]
-
-    # if sa-deva ignore sanskrita and only get deva
-    if '-' in src_tag and src_tag.split('-')[0].lower() in ['sa','san', 'pi', 'pli']:
-        for scrpt in data_loaded.keys():
-            scrpt_tag = data_loaded[scrpt]['script']
-
-            if scrpt_tag.lower() == src_tag.split('-')[1].lower():
-                src = [(0, scrpt)]
-
-    if '-' in tgt_tag and tgt_tag.split('-')[0].lower() in ['sa','san', 'pi', 'pli']:
-        for scrpt in data_loaded.keys():
-            scrpt_tag = data_loaded[scrpt]['script']
-
-            if scrpt_tag.lower() == tgt_tag.split('-')[1].lower():
-                tgt = [(0, scrpt)]
-
-    if src_tag.lower() in ['la', 'en', 'eng']:
-        warn = "Latin has multiple transcription schemes. 'ISO 15919' has been selected by default"
-        warn += "\n Please use a transcription format e.g. Latn-IAST or Latn-HK to select a particular scheme"
-        warnings.warn(warn)
-
-        src = [(0, 'ISO')]
-
-    if tgt_tag.lower() in ['la', 'en', 'eng']:
-        warn = "Latin has multiple transcription schemes. 'ISO 15919' has been selected by default"
-        warn += "\n Please use a transcription format e.g. Latn-IAST or Latn-HK to select a particular scheme"
-        warnings.warn(warn)
-
-        tgt = [(0, 'ISO')]
-
-    # if latin ignore la and get the following part
-    if '-' in src_tag and src_tag.split('-')[0].lower() in ['la', 'en', 'eng']:
-        src = [(0, src_tag.split('-')[1])]
-
-    if '-' in tgt_tag and tgt_tag.split('-')[0].lower() in ['la', 'en', 'eng']:
-        tgt = [(0, tgt_tag.split('-')[1])]
-
-    if src_tag == 'autodetect':
-        src = [(0,auto_detect(txt))]
-        pre_options = detect_preoptions(txt, src)
-
-    if len(src) > 0:
-        src_pop = sorted(src, reverse=True)[0][1]
-    else:
-        raise Exception('Source language code: ' + src_tag + ' not found')
-
-    if len(tgt) > 0:
-        tgt_pop = sorted(tgt, reverse=True)[0][1]
-    else:
-        raise Exception('Target language code: ' + tgt_tag + ' not found')
-
-    if len(src) > 1:
-        warn = "Multiple scripts " + ','.join(map(lambda x: x[1], src)) + " associated with the input language. The most popular '" + src_pop + "' has been selected"
-        warn += "\n Please use the format lang_code-script_code e.g. pa-Guru or pa-Arab to select a particular script"
-        warnings.warn(warn)
-    if len(tgt) > 1:
-        warn = "Multiple scripts " + ','.join(map(lambda x: x[1], tgt)) + " associated with the target language. The most popular '" + tgt_pop + "' has been selected"
-        warn += "\n Please use the format lang_code-script_code e.g. pa-Guru or pa-Arab to select a particular script"
-        warnings.warn(warn)
-
-    return process_default(src_pop, tgt_pop, txt, nativize, post_options, pre_options)
-
-def process_lang_name(src_name, tgt_name, txt, nativize, post_options, pre_options):
-    if src_name == 'autodetect':
-        src = auto_detect(txt)
-        pre_options = detect_preoptions(txt, src)
-    else:
-        src = str(langcodes.find(src_name))
-
-    tgt = str(langcodes.find(tgt_name))
-
-    return process_lang_tag(src, tgt, txt, nativize, post_options, pre_options)
-
-@functools.cache
-def get_semitic_json():
-    from pathlib import Path
-    cwd = Path(Path(__file__).parent)
-    with open(Path(cwd, "json/gimeltra_data.json"), "r", encoding="utf-8") as f:
-        data = json.load(f)
-
-    return data
-
+from aksharamukha import GeneralMap
+from aksharamukha.gimeltra import Transliterator
+from . import Convert,PostOptions,PostProcess,PreProcess
+from . import ConvertFix
+import json
+import requests
+import html
+import itertools
+from collections import Counter
+import unicodedata
+import collections
+import yaml
+import warnings
+import langcodes
+import os
+from inspect import getmembers, isfunction
+
+#import sys
+#sys.stdout = None
+
+def removeA(a):
+    if a.count('a') == 1:
+        return a.replace('a', '')
+
+def unique_everseen(iterable, key=None):
+    "List unique elements, preserving order. Remember all elements ever seen."
+    # unique_everseen('AAAABBBCCDAABBB') --> A B C D
+    # unique_everseen('ABBCcAD', str.lower) --> A B C D
+    seen = set()
+    seen_add = seen.add
+    if key is None:
+        for element in itertools.filterfalse(seen.__contains__, iterable):
+            seen_add(element)
+            yield element
+    else:
+        for element in iterable:
+            k = key(element)
+            if k not in seen:
+                seen_add(k)
+                yield element
+
+def auto_detect(text, plugin = False):
+    scripts = []
+
+    for uchar in text:
+        try:
+            script_name = unicodedata.name(uchar).split(' ')[0].lower()
+            if script_name != 'old':
+                scripts.append(script_name)
+            else:
+                scripts.append(unicodedata.name(uchar).split(' ')[1].lower())
+        except ValueError:
+            pass
+            # print('Script not found')
+
+    counts = Counter(scripts)
+    script_percent = []
+
+    for script, count  in counts.items():
+        percent = count/len(scripts) * 100
+        script_percent.append((percent, script))
+
+    #print(sorted(script_percent))
+
+    if not plugin:
+        if len(script_percent) > 0:
+            script = sorted(script_percent)[-1][1]
+        else:
+            script = ''
+    else:
+        #print('here')
+        if len(script_percent) > 0:
+            if sorted(script_percent)[-1][1] == 'latin':
+                script = sorted(script_percent)[-2][1]
+            else:
+                script = sorted(script_percent)[-1][1]
+        else:
+            script = ''
+
+    inputScript = script[0].upper() + script[1:]
+
+    laoPali = ['ຆ', 'ຉ', 'ຌ', 'ຎ', 'ຏ', 'ຐ', 'ຑ', 'ຒ', 'ຓ', 'ຘ', 'ຠ', 'ຨ', 'ຩ', 'ຬ', '຺']
+
+    if inputScript == 'Bengali':
+        if 'ৰ' in text or 'ৱ' in text:
+            inputScript = 'Assamese'
+    elif inputScript == 'Lao':
+        if any(char in text for char in laoPali):
+            inputScript = 'LaoPali'
+    elif inputScript == 'Batak':
+        inputScript = 'BatakKaro'
+    elif inputScript == 'Myanmar':
+        inputScript = 'Burmese'
+
+        mon = ['ၚ', 'ၛ', '္ည', 'ၞ', 'ၟ', 'ၠ', 'ဳ', 'ဨ']
+        if any([char in text for char in mon]):
+            inputScript = 'Mon'
+
+        countSub = {'Shan': 0, 'TaiLaing': 0, 'KhamtiShan': 0}
+
+        text = text.replace('ႃ', '')
+
+        for uchar in text:
+            try:
+                char = unicodedata.name(uchar).lower()
+            except:
+                pass
+            if 'shan' in char:
+                countSub['Shan'] += 1
+            elif 'tai laing' in char:
+                countSub['TaiLaing'] += 1
+            elif 'khamti' in char:
+                countSub['KhamtiShan'] += 1
+
+        import operator
+        sorted_x = sorted(countSub.items(), key=operator.itemgetter(1))
+
+        if countSub['Shan'] > 0 or countSub['TaiLaing'] > 0 or countSub['KhamtiShan'] > 0:
+            inputScript = sorted_x[-1][0]
+
+
+        #shan = ['ႃ', '\u1086', '\u1084', 'ၵ', 'ၶ', 'ၷ', 'ꧠ', 'ၸ', 'ꧡ', 'ꩡ', 'ꧢ', 'ၺ', 'ꩦ', 'ꩧ', 'ꩨ', 'ꩩ', 'ꧣ', 'ၻ', 'ꩪ', 'ၼ','ၽ', 'ꧤ', 'ႁ', 'ꩮ', 'ၹ', 'ၾ']
+        #if any([char in text for char in shan]):
+            #inputScript = 'Shan'
+
+    elif inputScript == 'Meetei':
+        inputScript = 'MeeteiMayek'
+    elif inputScript == 'Dives':
+        inputScript = 'DivesAkuru'
+    elif inputScript == 'Persian':
+        inputScript = 'OldPersian'
+    elif inputScript == 'Phags-pa':
+        inputScript = 'PhagsPa'
+    elif inputScript == 'Ol':
+        inputScript = 'Santali'
+    elif inputScript == 'Sora':
+        inputScript = 'SoraSompeng'
+    elif inputScript == 'Syloti':
+        inputScript = 'SylotiNagri'
+    elif inputScript == 'Tai':
+        inputScript = 'TaiTham'
+    elif inputScript == 'Warang':
+        inputScript = 'WarangCiti'
+    elif inputScript == 'Siddham':
+        preOptions = 'siddhamUnicode'
+    elif inputScript == 'Cyrillic':
+        inputScript = 'RussianCyrillic'
+    elif inputScript == 'Zanabazar':
+        inputScript = 'ZanabazarSquare'
+    elif inputScript == 'Syriac':
+        inputScript = 'Syre'
+        eastern_dia = 'ܲ ܵ ܝܼ ܘܼ ܸ ܹ ܘܿ'.split(' ')
+        if any(char in text for char in eastern_dia):
+            inputScript = 'Syrn'
+        western_dia = 'ܰ ܺ ܶ ّ ܽ'.split(' ')
+        if any(char in text for char in western_dia):
+            inputScript = 'Syrj'
+    elif inputScript == 'Arabic':
+        inputScript = 'Arab'
+        persian_char = 'چ گ ژ پ هٔ'.split(' ')
+        if any(char in text for char in persian_char):
+            inputScript = 'Arab-Fa'
+        urdu_char = 'ڈ ٹ ڑ ھ'.split(' ')
+        if any(char in text for char in urdu_char):
+            inputScript = 'Urdu'
+        shahmukh_char = 'ݨ لؕ مھ نھ یھ رھ لھ وھ'.split(" ")
+        if any(char in text for char in shahmukh_char):
+            inputScript = 'Shahmukhi'
+    elif inputScript == 'Latin':
+        diacritics = ['ā', 'ī', 'ū', 'ṃ', 'ḥ', 'ś', 'ṣ', 'ṇ', 'ṛ', 'ṝ', 'ḷ', 'ḹ', 'ḻ', 'ṉ', 'ṟ', 'ṭ', 'ḍ', 'ṅ', 'ñ']
+        Itrans = ['R^i', 'R^I', 'L^i', 'L^I', '.N', '~N', '~n', 'Ch', 'sh', 'Sh']
+        semitic = ['ʾ', 'ʿ', 'š', 'w']
+        BurmeseRomanLoC = ['´', '˝', 'ʻ']
+        if 'ʰ' in text:
+            inputScript = 'Titus'
+        elif any(char in text for char in semitic):
+            inputScript = 'Latn'
+        elif any(char in text for char in BurmeseRomanLoC):
+            inputScript = 'BurmeseRomanLoC' ## Change for other LoC schemese
+        elif any(char in text for char in diacritics):
+            if 'ē' in text or 'ō' in text or 'r̥' in text:
+                inputScript = 'ISO'
+            else:
+                inputScript = 'IAST'
+        elif any(char in text for char in Itrans):
+            inputScript = 'Itrans'
+        else:
+            inputScript = 'HK'
+    elif inputScript in GeneralMap.IndicScripts or inputScript in GeneralMap.LatinScripts or inputScript in ['Hiragana', 'Katakana']:
+        pass
+    else:
+        from . import gimeltra
+        tr = gimeltra.Transliterator()
+        inputScript = tr.auto_script(text)
+
+    return inputScript
+
+# Cross check with inded convert() funciton within autodetect
+# scripts available here must be added there
+def detect_preoptions(text, inputScript):
+    preoptions = []
+    if inputScript == 'Thai':
+        textNew = text.replace('ห์', '')
+        if '\u035C' in text or '\u0325' in text or 'งํ' in text or '\u0E47' in text:
+            preoptions = ['ThaiPhonetic']
+        elif '์' in textNew and ('ะ' in text):
+            preoptions = ['ThaiSajjhayawithA']
+        elif '์' in textNew:
+            preoptions = ['ThaiSajjhayaOrthography']
+        elif 'ะ' in text or 'ั' in text:
+            preoptions =  ['ThaiOrthography']
+    elif inputScript == 'Lao' or inputScript == 'LaoPali':
+        textNew = text.replace('ຫ໌', '')
+        if '໌' in textNew and ('ະ' in text):
+            preoptions = ['LaoSajhayaOrthographywithA']
+        elif '໌' in textNew:
+            preoptions = ['LaoSajhayaOrthography']
+        elif 'ະ' in text or 'ັ' in text:
+            preoptions = ['LaoTranscription']
+    elif inputScript == 'Urdu':
+            preoptions = ['UrduShortNotShown']
+
+    return preoptions
+
+def convert(src, tgt, txt, nativize, preoptions, postoptions):
+    tgtOld = ""
+
+    ## ALA-LC Romanizations
+    ## process as follows, if source is associated with LoC script
+    if tgt == 'RomanLoC' and src in GeneralMap.LoCScripts:
+    ### swtiches for Source scripts
+        if src in GeneralMap.LoCSrcMap:
+            src = src + 'LoC'
+        elif 'Tham' in src:
+            src = 'ThamLoC'
+
+        if src in GeneralMap.LoCTgtMap:
+            tgt = src + tgt
+        elif src in GeneralMap.LoCTgtISO:
+            tgt = 'ISO'
+
+        # the below order for preoptions is important
+        #special for east-asian scripts
+        if src in GeneralMap.LocPostPre:
+            preoptions = preoptions + [tgt + 'Target']
+            postoptions =  [tgt + 'Target'] + postoptions
+            nativize = False
+
+            if src in ['KhmerLoC']:
+                preoptions =  preoptions + ['SchwaFinalKhmerLoC']
+        #read from GeneralMap
+        else:
+            if src in GeneralMap.LoCTgtPostOptions.keys():
+                postoptions =  GeneralMap.LoCTgtPostOptions[src] + postoptions
+            if src in GeneralMap.LoCTgtPreOptions.keys():
+                preoptions =  preoptions + GeneralMap.LoCTgtPreOptions[src]
+
+    ## if source is not associated with LoC script
+    if tgt == 'RomanLoC' and src not in GeneralMap.LoCScripts:
+        if src in GeneralMap.SemiticScripts:
+            tgt = 'ISO233'
+        else:
+            tgt = 'ISO'
+
+    ## Switches for Target scripts
+    ## if target is associated with the loc Script
+    if src == 'RomanLoC' and tgt in GeneralMap.LoCScripts:
+        if tgt in GeneralMap.LoCSrcMap:
+            tgt = tgt + 'LoC'
+        elif 'Tham' in tgt:
+            tgt = 'ThamLoC'
+
+        if tgt in GeneralMap.LoCTgtMap:
+            src = tgt + src
+        elif tgt in GeneralMap.LoCTgtISO:
+            src = 'ISO'
+
+        if tgt in GeneralMap.LocPostPre:
+            preoptions = [src + 'Source'] + preoptions
+            postoptions =  [src + 'Source'] + postoptions
+            nativize = False
+        #read from GeneralMap
+        else:
+            if tgt in GeneralMap.LoCSrcPostOptions.keys():
+                postoptions =  GeneralMap.LoCSrcPostOptions[tgt] + postoptions
+            if tgt in GeneralMap.LoCSrcPreOptions.keys():
+                preoptions =  preoptions + GeneralMap.LoCSrcPreOptions[tgt]
+
+    ## if target is not associated with the loc Script
+    if src == 'RomanLoC' and tgt not in GeneralMap.LoCScripts:
+        if tgt in GeneralMap.SemiticScripts:
+            src = 'ISO233'
+        else:
+            src = 'ISO'
+
+    ## LoC Romanizattion ends here
+    ## else convert the Loc input into the associated script and then convert it into Loc
+    ## Text (Loc) -> Burmese -> non-Burmese
+    #if src == 'BurmeseRomanLoC' and tgt != 'Burmese':
+    #    txt = convert(src, "Burmese", txt, nativize, preoptions, postoptions)
+    #    src = 'Burmese'
+
+    ## Semitic ISO Standards
+    ### same as below use intermediates to convert non-associated input/output
+    if tgt in GeneralMap.semiticISO.keys():
+        if GeneralMap.semiticISO[tgt] != src:
+            txt = convert(src, GeneralMap.semiticISO[tgt], txt, nativize, preoptions, postoptions)
+            src = GeneralMap.semiticISO[tgt]
+
+        if GeneralMap.semiticISO[tgt] == src:
+            preoptions = [tgt + 'Target'] + preoptions
+            postoptions =  [tgt + 'Target'] + postoptions
+            nativize = False
+            tgt = 'Latn'
+
+    if src in GeneralMap.semiticISO.keys():
+        if GeneralMap.semiticISO[src] == tgt:
+            #print('here1')
+            preoptions = [src + 'Source'] + preoptions
+            postoptions = [src + 'Source'] + postoptions
+            src = 'Latn'
+        else:
+            #print('here2')
+            txt = convert(src, GeneralMap.semiticISO[src], txt, nativize, preoptions, postoptions)
+            src = GeneralMap.semiticISO[src]
+
+    '''if src == "Itrans" and '##' in txt:
+        textNew = [[i,word] for i, word in enumerate(txt.split("##")) if (i%2 == 0)]
+        textRest = [(i,word) for i, word in enumerate(txt.split("##")) if (i%2 == 1)]
+
+        txt = json.dumps(textNew).replace("\\n", "\n")'''
+
+    if tgt == "" or tgt == "Ignore":
+        return txt
+    if preoptions == [] and postoptions == [] and nativize == False and src == tgt:
+        return txt
+
+    ## Semitic Switches - Add Shahmukhi/Sindhi later
+    IndicSemiticMapping = { 'Hebrew': 'Hebr', 'Thaana': 'Thaa', 'Urdu': 'Arab-Ur', 'Shahmukhi': 'Arab-Pa'}
+
+    if (tgt in GeneralMap.SemiticScripts or tgt in GeneralMap.semiticISO.keys()) and src in IndicSemiticMapping.keys():
+        src = IndicSemiticMapping[src]
+    if (src in GeneralMap.SemiticScripts or src in GeneralMap.semiticISO.keys()) and tgt in IndicSemiticMapping.keys():
+        tgt = IndicSemiticMapping[tgt]
+    if src in IndicSemiticMapping.keys() and tgt in IndicSemiticMapping.keys():
+        src = IndicSemiticMapping[src]
+        tgt = IndicSemiticMapping[tgt]
+
+    # preserve semitic pattern
+    if not nativize and src == 'Hebrew':
+        src = 'Hebr'
+    if not nativize and src == 'Urdu':
+        src = 'Arab-Ur'
+    if not nativize and src == 'Shahmukhi':
+        src = 'Arab-Pa'
+    if not nativize and src == 'Thaana':
+        src = 'Thaa'
+
+    if src in ['Arab-Ur', 'Arab-Pa'] and tgt in GeneralMap.IndicScripts:
+        txt += '\u05CD'
+
+    ## Semitic to Urdu this is not needed
+    #if src in GeneralMap.SemiticScripts and src not in ['Arab-Fa', 'Arab', 'Latn'] and (tgt in ['Urdu', 'Shahmukhi']):
+    #    tgt = 'Arab-Fa'
+
+    ## recheck this the logic is missing :: This is not required
+    """if src in ['Urdu', 'Shahmukhi'] and tgt == 'Arab':
+        #print('Semiticizing Urdu')
+        txt = PreProcess.semiticizeUrdu(txt)
+        txt = PreProcess.ArabizePersian(txt)
+        src = "Arab-Fa"
+        tgt = "Arab"
+
+    if src in ['Urdu', 'Shahmukhi'] and tgt == 'Arab-Fa':
+        txt = PreProcess.semiticizeUrdu(txt)
+        src = "none"
+        tgt = "none"
+
+    if src == 'Arab-Fa' and tgt == 'Arab':
+        txt = PreProcess.ArabizePersian(txt)
+        #src = "none"
+        #tgt = "none"
+
+    if src  == 'Arab' and tgt == 'Arab-Fa':
+        txt = PreProcess.perisanizeArab(txt)
+        src = "none"
+        tgt = "none"
+
+    if src  == 'Arab' and tgt in ['Urdu', 'Shahmukhi']:
+        txt = PreProcess.perisanizeArab(txt)
+        src = "none"
+        tgt = "Arab-Fa"
+
+    if src in 'Arab-Fa' and tgt in ['Urdu', 'Shahmukhi']:
+        src = "none"
+        tgt = "none" """
+
+    ## Semitic Naivization : remove pesky Nuktas
+    if nativize:
+        if src in GeneralMap.SemiticScripts and tgt in GeneralMap.IndicScripts:
+            txt += "\u05CC"
+
+    if src == tgt and (src != 'Hiragana' and src != 'Katakana') and src not in GeneralMap.SemiticScripts:
+        tgtOld = tgt
+        tgt = "Devanagari"
+
+    ## this has to be before preprocess.preprocess
+    if 'indicDandas' in postoptions:
+        if src in GeneralMap.pipeScripts and '|' in txt:
+            txt = PreProcess.RetainPipeDanda(txt)
+        elif GeneralMap.CrunchList('SignMap', src)[1] == '।':
+            preoptions = preoptions + ['RetainDevangariDanda']
+        else:
+            if tgt not in GeneralMap.Transliteration:
+                postoptions = postoptions + ['Dot2Dandas']
+            else:
+                postoptions = postoptions + ['Dot2Pipes']
+
+    txt = PreProcess.PreProcess(txt,src,tgt,postoptions,preoptions)
+
+    if 'siddhammukta' in postoptions and tgt == 'Siddham':
+        tgt = 'SiddhamDevanagari'
+    if 'siddhamap' in postoptions and tgt == 'Siddham':
+        tgt = 'SiddhamDevanagari'
+    if 'siddhammukta' in preoptions and src == 'Siddham':
+        src = 'SiddhamDevanagari'
+    if 'LaoNative' in postoptions and tgt == 'Lao':
+        tgt = 'Lao2'
+    if 'egrantamil' in preoptions and src == 'Grantha':
+        src = 'GranthaGrantamil'
+    if 'egrantamil' in postoptions and tgt == 'Grantha':
+        tgt = 'GranthaGrantamil'
+    if 'nepaldevafont' in postoptions and tgt == 'Newa':
+        tgt = 'Devanagari'
+    if 'ranjanalantsa' in postoptions and tgt == 'Ranjana':
+        tgt = 'Tibetan'
+        nativize = False
+    if 'ranjanawartu' in postoptions and tgt == 'Ranjana':
+        tgt = 'Tibetan'
+        nativize = False
+    if 'BengaliRaBa' in postoptions and tgt == 'Bengali':
+        tgt = 'BengaliRaBa'
+        nativize = False
+    if 'SoyomboFinals' in postoptions and tgt == 'Soyombo':
+        txt = '\u02BE' + txt
+    if  'BalineseSimplified' in postoptions and src == 'Balinese':
+        tgt = 'BalineseSimpleRomanLoC'
+    if  'JavaneseSimplified' in postoptions and src == 'Javanese':
+        tgt = 'JavaneseSimpleRomanLoC'
+
+    #if src not in GeneralMap.SemiticScripts and tgt == 'Arab' and not nativize:
+        #postoptions.append('arabicRemoveAdditionsPhonetic')
+
+    for options in preoptions:
+      txt = getattr(PreProcess, options)(txt)
+
+    ### Semitic Switches
+    if 'novowelshebrew' in preoptions and src == 'Hebr':
+        txt = txt.replace('\u05B7', '')
+
+    srcOld = ""
+
+    ### retain Latin ###
+    if (src != 'Latn'and src != 'Type' and src in GeneralMap.SemiticScripts) or \
+        (src in GeneralMap.IndicScripts and tgt in GeneralMap.SemiticScripts and src not in GeneralMap.LatinScripts) or \
+            (src in ['Hiragana', 'Katakana']):
+        txt = PreProcess.retainLatin(txt)
+
+    if src == 'Hiragana' or src == 'Katakana':
+        txt = PreProcess.JapanesePreProcess(src, txt, preoptions)
+        srcOld = 'Japanese'
+        src = 'ISO'
+
+    if tgt == 'Hiragana' or tgt == 'Katakana':
+        txt = PostProcess.JapanesePostProcess(src, tgt, txt, nativize, postoptions)
+
+    if src == "Oriya" and tgt == "IPA":
+        txt = ConvertFix.OriyaIPAFixPre(txt)
+
+    if src == "Itrans" and '##' in txt:
+        #print('I am here tyring to do things')
+        transliteration = ''
+        for i, word in enumerate(txt.split("##")):
+            if (i%2 == 0):
+                transliteration += Convert.convertScript(word, src, tgt)
+            else:
+                transliteration += word
+    else:
+        transliteration = Convert.convertScript(txt, src, tgt)
+
+    #print(transliteration)
+
+    if srcOld == 'Japanese' and tgt != 'Devanagari' and 'siddhammukta' not in postoptions:
+        transliteration = Convert.convertScript(transliteration, "Devanagari", "ISO")
+        # print(transliteration)
+
+    if src == tgtOld:
+        tgt = tgtOld
+        transliteration = Convert.convertScript(transliteration, "Devanagari", tgt)
+
+    ## apply phonetic mapping for Arabic beforehand if not semitic source
+    if (src not in GeneralMap.SemiticScripts and tgt == 'Arab' and nativize) or 'arabicRemoveAdditionsPhonetic' in postoptions:
+        transliteration = getattr(PostProcess, 'arabicRemoveAdditionsPhonetic')(transliteration)
+
+    #print(transliteration)
+
+    if nativize:
+      transliteration =  PostOptions.ApplyScriptDefaults(transliteration, src, tgt, postoptions)
+      if tgt != 'Latn':
+        if tgt != 'Tamil':
+            transliteration = PostProcess.RemoveDiacritics(transliteration)
+        else:
+            transliteration = PostProcess.RemoveDiacriticsTamil(transliteration)
+
+    #print(transliteration)
+
+    if 'RemoveDiacritics' in postoptions:
+      if tgt == 'Tamil':
+        postoptions = map(lambda x: 'RemoveDiacriticsTamil' if x == 'RemoveDiacritics' else x, postoptions)
+
+    for options in postoptions:
+      transliteration = getattr(PostProcess, options)(transliteration)
+
+    if src == "Tamil" and tgt == "IPA":
+        r = requests.get("http://anunaadam.appspot.com/api?text=" + txt + "&method=2")
+        r.encoding = r.apparent_encoding
+        transliteration = r.text
+
+    if src == "Oriya" and tgt == "IPA":
+        transliteration = ConvertFix.OriyaIPAFix(transliteration)
+
+    '''if src == "Itrans" and '##' in txt:
+        textConv = {**dict(list(json.loads(transliteration.replace("\n", "\\n")))), ** dict(textRest)}
+        textConv = collections.OrderedDict(sorted(textConv.items()))
+        transliteration = "".join(textConv.values())'''
+
+    ### return Latin ###
+    transliteration = PreProcess.retainLatin(transliteration, reverse=True)
+
+    ## DefaultPostProcess ##
+
+    transliteration = PostProcess.defaultPost(src, tgt, transliteration, nativize, preoptions, postoptions)
+
+    return transliteration
+
+def process(src, tgt, txt, nativize = True, post_options = [], pre_options = [], param="default"):
+    if param == "default":
+        return process_default(src, tgt, txt, nativize, post_options, pre_options)
+
+    if param == "script_code":
+        return process_script_tag(src, tgt, txt, nativize, post_options, pre_options)
+
+    if param == "lang_code":
+        return process_lang_tag(src, tgt, txt, nativize, post_options, pre_options)
+
+    if param == "lang_name":
+        return process_lang_name(src, tgt, txt, nativize, post_options, pre_options)
+
+import functools
+
+@functools.lru_cache(maxsize=None)
+def _load_data(file_path):
+    import os
+    dir_path = os.path.dirname(os.path.realpath(__file__))
+    with open(dir_path + file_path, 'r', encoding='utf8') as stream:
+        data_loaded = yaml.safe_load(stream)
+    return data_loaded
+
+def convert_default(src, tgt, txt, nativize = True, post_options = [], pre_options = []):
+    data_loaded = _load_data("/yaml/aksharamukha-scripts.yaml")
+
+    scriptList = GeneralMap.IndicScripts + GeneralMap.LatinScripts + GeneralMap.SemiticScripts
+
+    preOptionList = list(map(lambda x: x[0], getmembers(PreProcess, isfunction)))
+    preOptionListLower = list(map(lambda x: x.lower(), preOptionList))
+
+    postOptionList = list(map(lambda x: x[0], getmembers(PostProcess, isfunction)))
+    postOptionListLower = list(map(lambda x: x.lower(), postOptionList))
+
+    post_options = [option_id for option in post_options for option_id in postOptionList if option.lower() == option_id.lower()]
+    pre_options = [option_id for option in pre_options for option_id in preOptionList if option.lower() == option_id.lower()]
+
+    # font hack warning
+    font_hack_warning = tgt + ' uses an hacked font to display the script. In the absence of this font, you text may appear different. \n See: https://www.aksharamukha.com/describe/' + tgt + ' for the font used'
+
+    if tgt in data_loaded and 'font_hack' in data_loaded[tgt]:
+        warnings.warn(font_hack_warning)
+
+    if src not in scriptList:
+        script_not_found = 'Source script: ' + src + ' not found in the list of scripts supported. The text will not be transliterated.'
+        warnings.warn(script_not_found)
+
+    if tgt not in scriptList:
+        script_not_found = 'Target script: ' + tgt + ' not found in the list of scripts supported. The text will not be transliterated.'
+        warnings.warn(script_not_found)
+
+    if (tgt == 'RomanLoC' and src not in GeneralMap.LoCScripts):
+        script_not_found = 'The LoC romanization of ' + src + ' is not yet supported. The output text will be rendered using ISO 233 if Semitic else ISO 15919. See: https://www.aksharamukha.com/loc'
+        warnings.warn(script_not_found)
+
+    if (src == 'RomanLoC' and tgt not in GeneralMap.LoCScripts):
+        script_not_found = 'The LoC romanization of ' + tgt + ' is not yet supported. The input text will be treated as if it was ISO 233 if Semitic else ISO 15919.. See: https://www.aksharamukha.com/loc'
+        warnings.warn(script_not_found)
+
+    return convert(src, tgt, txt, nativize, pre_options, post_options)
+
+def process_default(src, tgt, txt, nativize, post_options, pre_options):
+    scriptList = GeneralMap.IndicScripts + GeneralMap.LatinScripts
+    scriptListLower = list(map(lambda x: x.lower(), scriptList))
+
+    if src == 'autodetect':
+        src = auto_detect(txt)
+        #print('The autodetection is ' + src)
+        pre_options = detect_preoptions(txt, src)
+    elif src.lower() in scriptListLower:
+        src = [script_id for script_id in scriptList if src.lower() == script_id.lower()][0]
+
+    if tgt.lower() in scriptListLower:
+        tgt = [script_id for script_id in scriptList if tgt.lower() == script_id.lower()][0]
+
+    return convert_default(src, tgt, txt, nativize, post_options, pre_options)
+
+
+def process_script_tag(src_tag, tgt_tag, txt, nativize, post_options, pre_options):
+    # Read YAML file
+    data_loaded = _load_data("/yaml/aksharamukha-scripts.yaml")
+
+    data_loaded_wiki = _load_data("/yaml/wikitra2-data.yaml")
+
+    src = []
+    tgt = []
+
+    if src_tag == 'Syrc':
+        src_tag = 'Syre'
+        warnings.warn("Please specify the variety of Syriac script for the source: Estrangelo (Syre), Eastern (Syrn) or Wester (Syrj). Defaulting to Syre")
+    if tgt_tag == 'Syrc':
+        tgt_tag = 'Syre'
+        warnings.warn("Please specify the variety of Syriac script for the target: Estrangelo (Syre), Eastern (Syrn) or Wester (Syrj). Defaulting to Syre")
+
+    # loop through yaml to find match
+    for scrpt in data_loaded.keys():
+        scrpt_tag = data_loaded[scrpt]['script']
+
+        # get the popuation of each language of the script
+        if 'lang' in data_loaded[scrpt].keys():
+            lang_tag = data_loaded[scrpt]['lang'].split(',')[0]
+            lang = list(map(lambda x: x.lower(), data_loaded[scrpt]['lang'].split(',')))
+        else:
+            population = 0
+            lang = ''
+
+        #print(scrpt_tag, lang_tag)
+        if scrpt_tag in data_loaded_wiki.keys() and lang_tag in data_loaded_wiki[scrpt_tag].keys():
+            population = data_loaded_wiki[scrpt_tag][lang_tag]['population']
+        else:
+            population = 0
+
+        # find the match in the file
+        if '-' not in src_tag and data_loaded[scrpt]['script'].lower() == src_tag.lower():
+            src.append((population, scrpt))
+
+        if '-' not in tgt_tag and data_loaded[scrpt]['script'].lower() == tgt_tag.lower():
+            tgt.append((population, scrpt))
+
+        #print(population)
+        # if hypthenated find the exact match
+        if '-' in tgt_tag:
+            lang_part = tgt_tag.split('-')[0].lower()
+            script_part = tgt_tag.split('-')[1].lower()
+
+            if scrpt_tag.lower() == script_part.lower() and 'lang' in data_loaded[scrpt].keys() and lang_part.lower() in lang:
+                tgt.append((0, scrpt))
+
+        if '-' in src_tag:
+            lang_part = src_tag.split('-')[0].lower()
+            script_part = src_tag.split('-')[1].lower()
+
+            if scrpt_tag.lower() == script_part.lower() and 'lang' in data_loaded[scrpt].keys() and lang_part.lower() in lang:
+                src.append((0, scrpt))
+
+    if src_tag.lower() in ['latn', 'en', 'eng']:
+        warn = "Latin has multiple transcription schemes. 'ISO 15919' has been selected by default"
+        warn += "\n Please use a transcription format e.g. la-IAST or la-HK to select a particular scheme"
+        warnings.warn(warn)
+
+        src = [(0, 'ISO')]
+
+    if tgt_tag.lower() in ['latn', 'en', 'eng']:
+        warn = "Latin has multiple transcription schemes. 'ISO 15919' has been selected by default"
+        warn += "\n Please use a transcription format e.g. la-IAST or la-HK to select a particular scheme"
+        warnings.warn(warn)
+
+        tgt = [(0, 'ISO')]
+
+    # if latin ignore la and get the following part
+    if '-' in src_tag and src_tag.split('-')[0].lower() in ['latn', 'en', 'eng']:
+        src = [(0, src_tag.split('-')[1])]
+
+    if '-' in tgt_tag and tgt_tag.split('-')[0].lower() in ['latn', 'en', 'eng']:
+        tgt = [(0, tgt_tag.split('-')[1])]
+
+    if src_tag == 'autodetect':
+        src = [(0, auto_detect(txt))]
+        pre_options = detect_preoptions(txt, src)
+
+    if len(src) > 0:
+        src_pop = sorted(src, reverse=True)[0][1]
+    elif src_tag in GeneralMap.SemiticScripts:
+            src_pop = src_tag
+    else:
+        raise Exception('Source script code: ' + src_tag + ' not found')
+
+    if len(tgt) > 0:
+        tgt_pop = sorted(tgt, reverse=True)[0][1]
+    elif tgt_tag in GeneralMap.SemiticScripts:
+        tgt_pop = tgt_tag
+    else:
+        raise Exception('Target script code: ' + tgt_tag + ' not found')
+
+    if len(src) > 1:
+        warn = "Multiple orthographies, " + ','.join(map(lambda x: x[1], src)) + ", are associated with the input script. The most popular '" + src_pop + "' has been selected"
+        warn += "\n Please use the format lang_code-script_code e.g. ur-Arab or pa-Arab to select a particular orthography"
+
+        warnings.warn(warn)
+    if len(tgt) > 1:
+        warn = "Multiple orthographies: " + ', '.join(map(lambda x: x[1], tgt)) + " are associated with the target script. The most popular '" + tgt_pop + "' has been selected"
+        warn += "\n Please use the format lang_code-script_code e.g. ur-Arab or pa-Arab to select a particular orthography"
+        warnings.warn(warn)
+
+    return process_default(src_pop, tgt_pop, txt, nativize, post_options, pre_options)
+
+def process_lang_tag(src_tag, tgt_tag, txt, nativize, post_options, pre_options):
+    # Read YAML file
+    data_loaded = _load_data("/yaml/aksharamukha-scripts.yaml")
+
+    data_loaded_wiki = _load_data("/yaml/wikitra2-data.yaml")
+
+    src = []
+    tgt = []
+
+    # iterate through the yaml file
+    for scrpt in data_loaded.keys():
+        if 'lang' in data_loaded[scrpt].keys():
+            lang = list(map(lambda x: x.lower(), data_loaded[scrpt]['lang'].split(',')))
+        else:
+            lang = ''
+
+        scrpt_tag = data_loaded[scrpt]['script']
+
+        # try to get the popular script from wiktionary file
+        if scrpt_tag in data_loaded_wiki.keys():
+            script_count = len(data_loaded_wiki[scrpt_tag])
+        else:
+            script_count = 1
+
+        # trying to find the match in the yaml file
+        if src_tag.lower() in lang:
+            src.append((script_count, scrpt))
+
+        if tgt_tag.lower() in lang:
+            tgt.append((script_count, scrpt))
+
+        if '-' in tgt_tag:
+            lang_part = tgt_tag.split('-')[0].lower()
+            script_part = tgt_tag.split('-')[1].lower()
+
+            if scrpt_tag.lower() == script_part and lang_part in lang:
+                tgt.append((0, scrpt))
+
+        if '-' in src_tag:
+            lang_part = src_tag.split('-')[0].lower()
+            script_part = src_tag.split('-')[1].lower()
+
+            if scrpt_tag.lower() == script_part and lang_part in lang:
+                src.append((0, scrpt))
+
+    if src_tag.lower() in ['sa','san', 'pi', 'pli']:
+        warn = "The input language: " + src_tag + " is script-agnostic and can be written in multiple scripts. The most popular 'Devanagari' has been selected"
+        warn += "\n Please use the format lang_code-script_code e.g. sa-Gran or sa-Sidd to select a particular script"
+        warnings.warn(warn)
+
+        src = [(0, 'Devanagari')]
+
+    if tgt_tag.lower() in ['sa','san', 'pi', 'pli']:
+        warn = "The ouptput language: " + tgt_tag + " is script-agnostic and can be written in multiple scripts. The most popular 'Devanagari' has been selected"
+        warn += "\n Please use the format lang_code-script_code e.g. sa-Gran or sa-Sidd to select a particular script"
+        warnings.warn(warn)
+
+        tgt = [(0, 'Devanagari')]
+
+    # if sa-deva ignore sanskrita and only get deva
+    if '-' in src_tag and src_tag.split('-')[0].lower() in ['sa','san', 'pi', 'pli']:
+        for scrpt in data_loaded.keys():
+            scrpt_tag = data_loaded[scrpt]['script']
+
+            if scrpt_tag.lower() == src_tag.split('-')[1].lower():
+                src = [(0, scrpt)]
+
+    if '-' in tgt_tag and tgt_tag.split('-')[0].lower() in ['sa','san', 'pi', 'pli']:
+        for scrpt in data_loaded.keys():
+            scrpt_tag = data_loaded[scrpt]['script']
+
+            if scrpt_tag.lower() == tgt_tag.split('-')[1].lower():
+                tgt = [(0, scrpt)]
+
+    if src_tag.lower() in ['la', 'en', 'eng']:
+        warn = "Latin has multiple transcription schemes. 'ISO 15919' has been selected by default"
+        warn += "\n Please use a transcription format e.g. Latn-IAST or Latn-HK to select a particular scheme"
+        warnings.warn(warn)
+
+        src = [(0, 'ISO')]
+
+    if tgt_tag.lower() in ['la', 'en', 'eng']:
+        warn = "Latin has multiple transcription schemes. 'ISO 15919' has been selected by default"
+        warn += "\n Please use a transcription format e.g. Latn-IAST or Latn-HK to select a particular scheme"
+        warnings.warn(warn)
+
+        tgt = [(0, 'ISO')]
+
+    # if latin ignore la and get the following part
+    if '-' in src_tag and src_tag.split('-')[0].lower() in ['la', 'en', 'eng']:
+        src = [(0, src_tag.split('-')[1])]
+
+    if '-' in tgt_tag and tgt_tag.split('-')[0].lower() in ['la', 'en', 'eng']:
+        tgt = [(0, tgt_tag.split('-')[1])]
+
+    if src_tag == 'autodetect':
+        src = [(0,auto_detect(txt))]
+        pre_options = detect_preoptions(txt, src)
+
+    if len(src) > 0:
+        src_pop = sorted(src, reverse=True)[0][1]
+    else:
+        raise Exception('Source language code: ' + src_tag + ' not found')
+
+    if len(tgt) > 0:
+        tgt_pop = sorted(tgt, reverse=True)[0][1]
+    else:
+        raise Exception('Target language code: ' + tgt_tag + ' not found')
+
+    if len(src) > 1:
+        warn = "Multiple scripts " + ','.join(map(lambda x: x[1], src)) + " associated with the input language. The most popular '" + src_pop + "' has been selected"
+        warn += "\n Please use the format lang_code-script_code e.g. pa-Guru or pa-Arab to select a particular script"
+        warnings.warn(warn)
+    if len(tgt) > 1:
+        warn = "Multiple scripts " + ','.join(map(lambda x: x[1], tgt)) + " associated with the target language. The most popular '" + tgt_pop + "' has been selected"
+        warn += "\n Please use the format lang_code-script_code e.g. pa-Guru or pa-Arab to select a particular script"
+        warnings.warn(warn)
+
+    return process_default(src_pop, tgt_pop, txt, nativize, post_options, pre_options)
+
+def process_lang_name(src_name, tgt_name, txt, nativize, post_options, pre_options):
+    if src_name == 'autodetect':
+        src = auto_detect(txt)
+        pre_options = detect_preoptions(txt, src)
+    else:
+        src = str(langcodes.find(src_name))
+
+    tgt = str(langcodes.find(tgt_name))
+
+    return process_lang_tag(src, tgt, txt, nativize, post_options, pre_options)
+
+@functools.lru_cache(maxsize=None)
+def get_semitic_json():
+    from pathlib import Path
+    cwd = Path(Path(__file__).parent)
+    with open(Path(cwd, "json/gimeltra_data.json"), "r", encoding="utf-8") as f:
+        data = json.load(f)
+
+    return data
+
 ## add the new libraries to requiesments.txt in both folders
```

### Comparing `aksharamukha-2.1.2/aksharamukha/yaml/aksharamukha-scripts.yaml` & `aksharamukha-2.2.1/aksharamukha/yaml/aksharamukha-scripts.yaml`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.1.2/aksharamukha/yaml/wikitra2-data.yaml` & `aksharamukha-2.2.1/aksharamukha/yaml/wikitra2-data.yaml`

 * *Files identical despite different names*

### Comparing `aksharamukha-2.1.2/aksharamukha.egg-info/PKG-INFO` & `aksharamukha-2.2.1/aksharamukha.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aksharamukha
-Version: 2.1.2
+Version: 2.2.1
 Summary: Provides script conversion (a.k.a transliteration) between various scripts
 Home-page: https://github.com/virtualvinodh/aksharamukha-python
 Author: Vinodh Rajan
 Author-email: vinodh@virtualvindh.com
 License: GNU AGPL 3.0
 Keywords: unicode semitic arabic syriac hebrew indic indian language script brahmi brahmic asian transliteration conversion writing alphabet romanization
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `aksharamukha-2.1.2/aksharamukha.egg-info/SOURCES.txt` & `aksharamukha-2.2.1/aksharamukha.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,90 +1,100 @@
 README.md
 setup.cfg
 setup.py
 aksharamukha/Convert.py
 aksharamukha/ConvertFix.py
+aksharamukha/FallBack.py
 aksharamukha/GeneralMap.py
 aksharamukha/PostOptions.py
 aksharamukha/PostProcess.py
 aksharamukha/PreOptions.py
 aksharamukha/PreProcess.py
 aksharamukha/__init__.py
+aksharamukha/demo.py
 aksharamukha/gimeltra.py
 aksharamukha/transliterate.py
+aksharamukha/transliterate_file.py
 aksharamukha.egg-info/PKG-INFO
 aksharamukha.egg-info/SOURCES.txt
 aksharamukha.egg-info/dependency_links.txt
 aksharamukha.egg-info/requires.txt
 aksharamukha.egg-info/top_level.txt
-aksharamukha/ScriptMap/FallBack.py
 aksharamukha/ScriptMap/__init__.py
 aksharamukha/ScriptMap/EastIndic/Balinese.py
 aksharamukha/ScriptMap/EastIndic/BatakKaro.py
 aksharamukha/ScriptMap/EastIndic/BatakManda.py
 aksharamukha/ScriptMap/EastIndic/BatakPakpak.py
 aksharamukha/ScriptMap/EastIndic/BatakSima.py
 aksharamukha/ScriptMap/EastIndic/BatakToba.py
 aksharamukha/ScriptMap/EastIndic/Buginese.py
 aksharamukha/ScriptMap/EastIndic/Buhid.py
 aksharamukha/ScriptMap/EastIndic/Burmese.py
 aksharamukha/ScriptMap/EastIndic/Cham.py
+aksharamukha/ScriptMap/EastIndic/DivesAkuru.py
 aksharamukha/ScriptMap/EastIndic/Hanunoo.py
 aksharamukha/ScriptMap/EastIndic/Javanese.py
 aksharamukha/ScriptMap/EastIndic/Kawi.py
 aksharamukha/ScriptMap/EastIndic/KhamtiShan.py
 aksharamukha/ScriptMap/EastIndic/Khmer.py
+aksharamukha/ScriptMap/EastIndic/KhmerLoC.py
 aksharamukha/ScriptMap/EastIndic/KhomThai.py
 aksharamukha/ScriptMap/EastIndic/KhuenTham.py
 aksharamukha/ScriptMap/EastIndic/Lao.py
 aksharamukha/ScriptMap/EastIndic/Lao2.py
 aksharamukha/ScriptMap/EastIndic/LaoPali.py
 aksharamukha/ScriptMap/EastIndic/LaoTham.py
 aksharamukha/ScriptMap/EastIndic/LueTham.py
 aksharamukha/ScriptMap/EastIndic/Makasar.py
 aksharamukha/ScriptMap/EastIndic/Marchen.py
 aksharamukha/ScriptMap/EastIndic/Mon.py
 aksharamukha/ScriptMap/EastIndic/Pallava.py
 aksharamukha/ScriptMap/EastIndic/PhagsPa.py
 aksharamukha/ScriptMap/EastIndic/Rejang.py
 aksharamukha/ScriptMap/EastIndic/Shan.py
+aksharamukha/ScriptMap/EastIndic/ShanLoC.py
 aksharamukha/ScriptMap/EastIndic/Siddham.py
 aksharamukha/ScriptMap/EastIndic/SiddhamRanjana.py
 aksharamukha/ScriptMap/EastIndic/Soyombo.py
 aksharamukha/ScriptMap/EastIndic/Sundanese.py
 aksharamukha/ScriptMap/EastIndic/Tagalog.py
 aksharamukha/ScriptMap/EastIndic/Tagbanwa.py
 aksharamukha/ScriptMap/EastIndic/TaiLaing.py
 aksharamukha/ScriptMap/EastIndic/TaiTham.py
 aksharamukha/ScriptMap/EastIndic/Thaana.py
 aksharamukha/ScriptMap/EastIndic/Thai.py
+aksharamukha/ScriptMap/EastIndic/ThamLoC.py
 aksharamukha/ScriptMap/EastIndic/Tibetan.py
+aksharamukha/ScriptMap/EastIndic/TibetanLoC.py
 aksharamukha/ScriptMap/EastIndic/ZanabazarSquare.py
 aksharamukha/ScriptMap/EastIndic/__init__.py
 aksharamukha/ScriptMap/MainIndic/Ahom.py
 aksharamukha/ScriptMap/MainIndic/Assamese.py
 aksharamukha/ScriptMap/MainIndic/Bengali.py
+aksharamukha/ScriptMap/MainIndic/BengaliRaBa.py
 aksharamukha/ScriptMap/MainIndic/Bhaiksuki.py
 aksharamukha/ScriptMap/MainIndic/Brahmi.py
 aksharamukha/ScriptMap/MainIndic/Chakma.py
 aksharamukha/ScriptMap/MainIndic/Devanagari.py
 aksharamukha/ScriptMap/MainIndic/Dogra.py
 aksharamukha/ScriptMap/MainIndic/Grantha.py
 aksharamukha/ScriptMap/MainIndic/GranthaGrantamil.py
 aksharamukha/ScriptMap/MainIndic/GranthaPandya.py
 aksharamukha/ScriptMap/MainIndic/Gujarati.py
 aksharamukha/ScriptMap/MainIndic/GunjalaGondi.py
 aksharamukha/ScriptMap/MainIndic/Gurmukhi.py
+aksharamukha/ScriptMap/MainIndic/GurmukhiLoC.py
 aksharamukha/ScriptMap/MainIndic/Kaithi.py
 aksharamukha/ScriptMap/MainIndic/Kannada.py
 aksharamukha/ScriptMap/MainIndic/Kharoshthi.py
 aksharamukha/ScriptMap/MainIndic/Khojki.py
 aksharamukha/ScriptMap/MainIndic/Khudawadi.py
 aksharamukha/ScriptMap/MainIndic/Lepcha.py
 aksharamukha/ScriptMap/MainIndic/Limbu.py
+aksharamukha/ScriptMap/MainIndic/LimbuLoC.py
 aksharamukha/ScriptMap/MainIndic/Mahajani.py
 aksharamukha/ScriptMap/MainIndic/Malayalam.py
 aksharamukha/ScriptMap/MainIndic/MasaramGondi.py
 aksharamukha/ScriptMap/MainIndic/MeeteiMayek.py
 aksharamukha/ScriptMap/MainIndic/Modi.py
 aksharamukha/ScriptMap/MainIndic/Multani.py
 aksharamukha/ScriptMap/MainIndic/Nandinagari.py
@@ -110,42 +120,68 @@
 aksharamukha/ScriptMap/MainIndic/__init__.py
 aksharamukha/ScriptMap/NonIndic/Hebrew.py
 aksharamukha/ScriptMap/NonIndic/OldPersian.py
 aksharamukha/ScriptMap/NonIndic/__init__.py
 aksharamukha/ScriptMap/NonIndic/kana2roman.py
 aksharamukha/ScriptMap/Roman/Aksharaa.py
 aksharamukha/ScriptMap/Roman/Ariyaka.py
+aksharamukha/ScriptMap/Roman/AssameseRomanLoC.py
 aksharamukha/ScriptMap/Roman/Avestan.py
+aksharamukha/ScriptMap/Roman/BalineseRomanLoC.py
+aksharamukha/ScriptMap/Roman/BalineseSimpleRomanLoC.py
 aksharamukha/ScriptMap/Roman/BarahaNorth.py
 aksharamukha/ScriptMap/Roman/BarahaSouth.py
+aksharamukha/ScriptMap/Roman/BengaliRomanLoC.py
+aksharamukha/ScriptMap/Roman/BurmeseRomanLoC.py
+aksharamukha/ScriptMap/Roman/DevanagariRomanLoC.py
 aksharamukha/ScriptMap/Roman/GreekModern.py
+aksharamukha/ScriptMap/Roman/GujaratiRomanLoC.py
+aksharamukha/ScriptMap/Roman/GurmukhiLoCRomanLoC.py
 aksharamukha/ScriptMap/Roman/HK.py
 aksharamukha/ScriptMap/Roman/HanifiRohingya.py
 aksharamukha/ScriptMap/Roman/IAST.py
-aksharamukha/ScriptMap/Roman/IASTLOC.py
 aksharamukha/ScriptMap/Roman/IASTPali.py
 aksharamukha/ScriptMap/Roman/IPA.py
 aksharamukha/ScriptMap/Roman/ISO.py
 aksharamukha/ScriptMap/Roman/ISOPali.py
 aksharamukha/ScriptMap/Roman/Inter.py
 aksharamukha/ScriptMap/Roman/Itrans.py
+aksharamukha/ScriptMap/Roman/JavaneseRomanLoC.py
+aksharamukha/ScriptMap/Roman/JavaneseSimpleRomanLoC.py
+aksharamukha/ScriptMap/Roman/KannadaRomanLoC.py
+aksharamukha/ScriptMap/Roman/KhmerLoCRomanLoC.py
+aksharamukha/ScriptMap/Roman/LimbuLoCRomanLoC.py
 aksharamukha/ScriptMap/Roman/Mongolian.py
 aksharamukha/ScriptMap/Roman/Mro.py
+aksharamukha/ScriptMap/Roman/OriyaRomanLoC.py
 aksharamukha/ScriptMap/Roman/RomanColloquial.py
 aksharamukha/ScriptMap/Roman/RomanKana.py
 aksharamukha/ScriptMap/Roman/RomanReadable.py
 aksharamukha/ScriptMap/Roman/RomanSemitic.py
 aksharamukha/ScriptMap/Roman/RussianCyrillic.py
 aksharamukha/ScriptMap/Roman/SLP1.py
 aksharamukha/ScriptMap/Roman/Santali.py
+aksharamukha/ScriptMap/Roman/ShanLoCRomanLoC.py
+aksharamukha/ScriptMap/Roman/SinhalaRomanLoC.py
 aksharamukha/ScriptMap/Roman/SoraSompeng.py
+aksharamukha/ScriptMap/Roman/TeluguRomanLoC.py
+aksharamukha/ScriptMap/Roman/ThamLoCRomanLoC.py
+aksharamukha/ScriptMap/Roman/TibetanLoCRomanLoC.py
 aksharamukha/ScriptMap/Roman/Titus.py
 aksharamukha/ScriptMap/Roman/TolongSiki.py
 aksharamukha/ScriptMap/Roman/Velthuis.py
 aksharamukha/ScriptMap/Roman/WX-kok.py
 aksharamukha/ScriptMap/Roman/WX.py
 aksharamukha/ScriptMap/Roman/Wancho.py
 aksharamukha/ScriptMap/Roman/WarangCiti.py
 aksharamukha/ScriptMap/Roman/__init__.py
 aksharamukha/json/gimeltra_data.json
+aksharamukha/test/__init__.py
+aksharamukha/test/loc_burmese_test_cases.py
+aksharamukha/test/loc_indic_test_cases.py
+aksharamukha/test/loc_khmer_test_cases.py
+aksharamukha/test/loc_shan_test_cases.py
+aksharamukha/test/loc_tham_test_cases.py
+aksharamukha/test/test_file_generator.py
+aksharamukha/test/testsuite.py
 aksharamukha/yaml/aksharamukha-scripts.yaml
 aksharamukha/yaml/wikitra2-data.yaml
```

### Comparing `aksharamukha-2.1.2/setup.py` & `aksharamukha-2.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 setup(
   name='aksharamukha',
 
   # Versions should comply with PEP440.  For a discussion on single-sourcing
   # the version across setup.py and the project code, see
   # https://packaging.python.org/en/latest/single_source_version.html
-  version='2.1.2',
+  version='2.2.1',
 
   description='Provides script conversion (a.k.a transliteration) between various scripts',
   long_description=long_description,
   long_description_content_type='text/markdown',
 
   # The project's main homepage.
   url='https://github.com/virtualvinodh/aksharamukha-python',
```

