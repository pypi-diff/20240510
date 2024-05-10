# Comparing `tmp/pygramcore-1.0.2.tar.gz` & `tmp/pygramcore-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygramcore-1.0.2.tar", last modified: Thu May  9 18:34:55 2024, max compression
+gzip compressed data, was "pygramcore-1.0.3.tar", last modified: Fri May 10 14:48:06 2024, max compression
```

## Comparing `pygramcore-1.0.2.tar` & `pygramcore-1.0.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 18:34:55.028375 pygramcore-1.0.2/
--rw-rw-rw-   0        0        0     1089 2024-05-05 17:27:36.000000 pygramcore-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     3865 2024-05-09 18:34:55.027377 pygramcore-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     3149 2024-05-09 18:34:13.000000 pygramcore-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-09 18:34:54.999376 pygramcore-1.0.2/pygramcore/
--rw-rw-rw-   0        0        0       54 2024-05-09 13:07:12.000000 pygramcore-1.0.2/pygramcore/__init__.py
--rw-rw-rw-   0        0        0      266 2024-05-09 13:07:12.000000 pygramcore-1.0.2/pygramcore/constants.py
-drwxrwxrwx   0        0        0        0 2024-05-09 18:34:55.017877 pygramcore-1.0.2/pygramcore/elements/
--rw-rw-rw-   0        0        0       48 2024-05-09 13:07:12.000000 pygramcore-1.0.2/pygramcore/elements/__init__.py
--rw-rw-rw-   0        0        0     9663 2024-05-09 16:17:22.000000 pygramcore-1.0.2/pygramcore/elements/post.py
--rw-rw-rw-   0        0        0    14390 2024-05-09 16:20:10.000000 pygramcore-1.0.2/pygramcore/elements/user.py
-drwxrwxrwx   0        0        0        0 2024-05-09 18:34:55.023376 pygramcore-1.0.2/pygramcore/exceptions/
--rw-rw-rw-   0        0        0        0 2024-05-09 12:49:58.000000 pygramcore-1.0.2/pygramcore/exceptions/__init__.py
--rw-rw-rw-   0        0        0      148 2024-05-09 17:13:14.000000 pygramcore-1.0.2/pygramcore/exceptions/auth.py
--rw-rw-rw-   0        0        0      238 2024-05-09 17:07:39.000000 pygramcore-1.0.2/pygramcore/exceptions/format.py
--rw-rw-rw-   0        0        0      494 2024-05-09 13:07:12.000000 pygramcore-1.0.2/pygramcore/exceptions/post.py
--rw-rw-rw-   0        0        0      638 2024-05-09 13:07:12.000000 pygramcore-1.0.2/pygramcore/exceptions/user.py
--rw-rw-rw-   0        0        0     8945 2024-05-09 17:16:12.000000 pygramcore-1.0.2/pygramcore/pygram.py
-drwxrwxrwx   0        0        0        0 2024-05-09 18:34:55.025378 pygramcore-1.0.2/pygramcore/utils/
--rw-rw-rw-   0        0        0       21 2024-05-09 13:07:12.000000 pygramcore-1.0.2/pygramcore/utils/__init__.py
--rw-rw-rw-   0        0        0      977 2024-05-09 13:07:12.000000 pygramcore-1.0.2/pygramcore/utils/misc.py
-drwxrwxrwx   0        0        0        0 2024-05-09 18:34:55.026377 pygramcore-1.0.2/pygramcore.egg-info/
--rw-rw-rw-   0        0        0     3865 2024-05-09 18:34:54.000000 pygramcore-1.0.2/pygramcore.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      561 2024-05-09 18:34:54.000000 pygramcore-1.0.2/pygramcore.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 18:34:54.000000 pygramcore-1.0.2/pygramcore.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2024-05-09 18:34:54.000000 pygramcore-1.0.2/pygramcore.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-09 18:34:54.000000 pygramcore-1.0.2/pygramcore.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-09 18:34:55.028375 pygramcore-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1174 2024-05-09 18:34:44.000000 pygramcore-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-10 14:48:06.116293 pygramcore-1.0.3/
+-rw-rw-rw-   0        0        0     1089 2024-05-05 17:27:36.000000 pygramcore-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     4405 2024-05-10 14:48:06.115293 pygramcore-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3684 2024-05-09 20:03:27.000000 pygramcore-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-10 14:48:06.085795 pygramcore-1.0.3/pygramcore/
+-rw-rw-rw-   0        0        0       54 2024-05-09 13:07:12.000000 pygramcore-1.0.3/pygramcore/__init__.py
+-rw-rw-rw-   0        0        0      266 2024-05-09 13:07:12.000000 pygramcore-1.0.3/pygramcore/constants.py
+drwxrwxrwx   0        0        0        0 2024-05-10 14:48:06.105792 pygramcore-1.0.3/pygramcore/elements/
+-rw-rw-rw-   0        0        0       48 2024-05-09 13:07:12.000000 pygramcore-1.0.3/pygramcore/elements/__init__.py
+-rw-rw-rw-   0        0        0     9598 2024-05-10 14:46:19.000000 pygramcore-1.0.3/pygramcore/elements/post.py
+-rw-rw-rw-   0        0        0    14556 2024-05-10 14:46:25.000000 pygramcore-1.0.3/pygramcore/elements/user.py
+drwxrwxrwx   0        0        0        0 2024-05-10 14:48:06.111292 pygramcore-1.0.3/pygramcore/exceptions/
+-rw-rw-rw-   0        0        0        0 2024-05-09 12:49:58.000000 pygramcore-1.0.3/pygramcore/exceptions/__init__.py
+-rw-rw-rw-   0        0        0      148 2024-05-09 17:13:14.000000 pygramcore-1.0.3/pygramcore/exceptions/auth.py
+-rw-rw-rw-   0        0        0      238 2024-05-09 17:07:39.000000 pygramcore-1.0.3/pygramcore/exceptions/format.py
+-rw-rw-rw-   0        0        0      494 2024-05-09 13:07:12.000000 pygramcore-1.0.3/pygramcore/exceptions/post.py
+-rw-rw-rw-   0        0        0      638 2024-05-09 13:07:12.000000 pygramcore-1.0.3/pygramcore/exceptions/user.py
+-rw-rw-rw-   0        0        0     8945 2024-05-09 17:16:12.000000 pygramcore-1.0.3/pygramcore/pygram.py
+drwxrwxrwx   0        0        0        0 2024-05-10 14:48:06.113292 pygramcore-1.0.3/pygramcore/utils/
+-rw-rw-rw-   0        0        0       21 2024-05-09 13:07:12.000000 pygramcore-1.0.3/pygramcore/utils/__init__.py
+-rw-rw-rw-   0        0        0      977 2024-05-09 13:07:12.000000 pygramcore-1.0.3/pygramcore/utils/misc.py
+drwxrwxrwx   0        0        0        0 2024-05-10 14:48:06.114291 pygramcore-1.0.3/pygramcore.egg-info/
+-rw-rw-rw-   0        0        0     4405 2024-05-10 14:48:05.000000 pygramcore-1.0.3/pygramcore.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      561 2024-05-10 14:48:06.000000 pygramcore-1.0.3/pygramcore.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 14:48:05.000000 pygramcore-1.0.3/pygramcore.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2024-05-10 14:48:05.000000 pygramcore-1.0.3/pygramcore.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-10 14:48:05.000000 pygramcore-1.0.3/pygramcore.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-10 14:48:06.116293 pygramcore-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1174 2024-05-10 14:47:31.000000 pygramcore-1.0.3/setup.py
```

### Comparing `pygramcore-1.0.2/LICENSE` & `pygramcore-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pygramcore-1.0.2/PKG-INFO` & `pygramcore-1.0.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygramcore
-Version: 1.0.2
+Version: 1.0.3
 Summary: A simple-to-use Instagram Python interface using Selenium.
 Author: Joel Taylor
 Author-email: contact@joeltaylor.business
 License: MIT
 Keywords: instagram,instagram bot,selenium,automation,bot
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -48,25 +48,25 @@
 
 <div id="key-features"></div>
 
 ## 🔑 Key Features
 
 - **Modular Elements**: Easily use and customize modular elements such as Posts, Comments, and Users.
 
-  - **Users**: Follow, download posts, direct message, and more.
+  - **Users**: Follow, direct message, get posts, and more.
 
-  - **Stories**: Like, download, reply and more.
+  - **Posts**: Like, comment, download, and more.
 
-  - **Posts**: Like, comment, save, download, and more.
+  - **Stories** (Coming soon...)
 
-  - **Comments**: Like, reply, and engage.
+  - **Comments** (Coming soon...)
 
 <div id="how-to-use"></div>
 
-## ❓ How To Use
+## 🔧 How To Use
 
 First of all, install the package using:
 
 ```bash
 pip install pygramcore
 ```
 
@@ -111,15 +111,20 @@
   urls = post.get_images()
 
   # Like & comment the post
   post.comment("Nice post!")
   post.like()
 ```
 
-Please refer to the docs for more.
+Please refer to the [docs](https://github.com/jtayped/pygramcore/tree/main/docs) for more.
 
 <div id="related"></div>
 
+## ❓ About the Project
+This Python package was created as a fun project to enhance my proficiency in writing "professional" Python code, building packages, implementing semantic versioning, and ensuring code maintainability.
+I am still a relatively new developer, and I welcome any contributions and feedback to help me improve.
+It is important to note that this project is not intended to replace essential packages such as [InstaPy](https://github.com/InstaPy/InstaPy), nor do I anticipate that it will.
+
 ## 🙋‍♂️ You may also like...
 
 - [✂️📱TikTok Manager](https://github.com/jtayped/tiktok-manager) - A script that manages MULTIPLE TikTok accounts by schedueling automatically generated videos from pre-selected YouTube channels to TikTok in advance.
 - [🧑‍💼My Portfolio](https://joeltaylor.business) - Check out my front-end and SEO skills on my Portfolio!
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pygramcore Version: 1.0.2 Summary: A simple-to-use
+Metadata-Version: 2.1 Name: pygramcore Version: 1.0.3 Summary: A simple-to-use
 Instagram Python interface using Selenium. Author: Joel Taylor Author-email:
 contact@joeltaylor.business License: MIT Keywords: instagram,instagram
 bot,selenium,automation,bot Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3.12 Classifier: Programming Language :: Python :: Implementation ::
 CPython Description-Content-Type: text/markdown License-File: LICENSE Requires-
 Dist: selenium Requires-Dist: selenium-stealth
@@ -11,30 +11,37 @@
                                 ?ð???· ppyyggrraammccoorree
                                      ************
              ****** AAnn eeaassyy--ttoo--uussee IInnssttaaggrraamm SSDDKK uussiinngg _SS_ee_ll_ee_nn_ii_uu_mm.. ******
     _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_p_y_g_r_a_m_c_o_r_e_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_]_[_L_i_c_e_n_s_e_]
                               _[_L_i_c_e_n_s_e_]_[_L_i_n_k_e_d_I_n_]
                     _K_e_y_ _F_e_a_t_u_r_e_s â¢ _H_o_w_ _T_o_ _U_s_e â¢ _R_e_l_a_t_e_d
 ## ð Key Features - **Modular Elements**: Easily use and customize modular
-elements such as Posts, Comments, and Users. - **Users**: Follow, download
-posts, direct message, and more. - **Stories**: Like, download, reply and more.
-- **Posts**: Like, comment, save, download, and more. - **Comments**: Like,
-reply, and engage.
-## â How To Use First of all, install the package using: ```bash pip install
+elements such as Posts, Comments, and Users. - **Users**: Follow, direct
+message, get posts, and more. - **Posts**: Like, comment, download, and more. -
+**Stories** (Coming soon...) - **Comments** (Coming soon...)
+## ð§ How To Use First of all, install the package using: ```bash pip install
 pygramcore ``` To take authenticated actions, initialize your Instagram account
 with your email/password and login: ```python from pygramcore import Account
 Account.login("youremail@email.com", "yourpassword123") Account.save_cookies
 ("path/to/file.pkl") ``` To initialize an account from cookies: ```python
 Account.load_cookies("path/to/file.pkl") ``` This will allow you to post
 images, comment on other peoples posts, send DMs, etc... ```python Account.post
 ("path/to/image.png", "Your very interesting caption") ``` To search for a user
 simply: ```python from pygramcore import User user = User("username123_") ```
 Here is an example of the usage of a user: ```python # Get a list of Post()
 objects posts = user.get_posts(limit=50) # Like the first 10 posts in the
 user's feed for post in posts[:10]: # Get URLs of the images in the post urls =
 post.get_images() # Like & comment the post post.comment("Nice post!")
-post.like() ``` Please refer to the docs for more.
-## ðââï¸ You may also like... - [âï¸ð±TikTok Manager](https://
-github.com/jtayped/tiktok-manager) - A script that manages MULTIPLE TikTok
-accounts by schedueling automatically generated videos from pre-selected
-YouTube channels to TikTok in advance. - [ð§âð¼My Portfolio](https://
-joeltaylor.business) - Check out my front-end and SEO skills on my Portfolio!
+post.like() ``` Please refer to the [docs](https://github.com/jtayped/
+pygramcore/tree/main/docs) for more.
+## â About the Project This Python package was created as a fun project to
+enhance my proficiency in writing "professional" Python code, building
+packages, implementing semantic versioning, and ensuring code maintainability.
+I am still a relatively new developer, and I welcome any contributions and
+feedback to help me improve. It is important to note that this project is not
+intended to replace essential packages such as [InstaPy](https://github.com/
+InstaPy/InstaPy), nor do I anticipate that it will. ## ðââï¸ You may
+also like... - [âï¸ð±TikTok Manager](https://github.com/jtayped/tiktok-
+manager) - A script that manages MULTIPLE TikTok accounts by schedueling
+automatically generated videos from pre-selected YouTube channels to TikTok in
+advance. - [ð§âð¼My Portfolio](https://joeltaylor.business) - Check out
+my front-end and SEO skills on my Portfolio!
```

### Comparing `pygramcore-1.0.2/README.md` & `pygramcore-1.0.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -31,25 +31,25 @@
 
 <div id="key-features"></div>
 
 ## 🔑 Key Features
 
 - **Modular Elements**: Easily use and customize modular elements such as Posts, Comments, and Users.
 
-  - **Users**: Follow, download posts, direct message, and more.
+  - **Users**: Follow, direct message, get posts, and more.
 
-  - **Stories**: Like, download, reply and more.
+  - **Posts**: Like, comment, download, and more.
 
-  - **Posts**: Like, comment, save, download, and more.
+  - **Stories** (Coming soon...)
 
-  - **Comments**: Like, reply, and engage.
+  - **Comments** (Coming soon...)
 
 <div id="how-to-use"></div>
 
-## ❓ How To Use
+## 🔧 How To Use
 
 First of all, install the package using:
 
 ```bash
 pip install pygramcore
 ```
 
@@ -94,15 +94,20 @@
   urls = post.get_images()
 
   # Like & comment the post
   post.comment("Nice post!")
   post.like()
 ```
 
-Please refer to the docs for more.
+Please refer to the [docs](https://github.com/jtayped/pygramcore/tree/main/docs) for more.
 
 <div id="related"></div>
 
+## ❓ About the Project
+This Python package was created as a fun project to enhance my proficiency in writing "professional" Python code, building packages, implementing semantic versioning, and ensuring code maintainability.
+I am still a relatively new developer, and I welcome any contributions and feedback to help me improve.
+It is important to note that this project is not intended to replace essential packages such as [InstaPy](https://github.com/InstaPy/InstaPy), nor do I anticipate that it will.
+
 ## 🙋‍♂️ You may also like...
 
 - [✂️📱TikTok Manager](https://github.com/jtayped/tiktok-manager) - A script that manages MULTIPLE TikTok accounts by schedueling automatically generated videos from pre-selected YouTube channels to TikTok in advance.
 - [🧑‍💼My Portfolio](https://joeltaylor.business) - Check out my front-end and SEO skills on my Portfolio!
```

#### html2text {}

```diff
@@ -3,30 +3,37 @@
                                 ?ð???· ppyyggrraammccoorree
                                      ************
              ****** AAnn eeaassyy--ttoo--uussee IInnssttaaggrraamm SSDDKK uussiinngg _SS_ee_ll_ee_nn_ii_uu_mm.. ******
     _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_p_y_g_r_a_m_c_o_r_e_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_]_[_L_i_c_e_n_s_e_]
                               _[_L_i_c_e_n_s_e_]_[_L_i_n_k_e_d_I_n_]
                     _K_e_y_ _F_e_a_t_u_r_e_s â¢ _H_o_w_ _T_o_ _U_s_e â¢ _R_e_l_a_t_e_d
 ## ð Key Features - **Modular Elements**: Easily use and customize modular
-elements such as Posts, Comments, and Users. - **Users**: Follow, download
-posts, direct message, and more. - **Stories**: Like, download, reply and more.
-- **Posts**: Like, comment, save, download, and more. - **Comments**: Like,
-reply, and engage.
-## â How To Use First of all, install the package using: ```bash pip install
+elements such as Posts, Comments, and Users. - **Users**: Follow, direct
+message, get posts, and more. - **Posts**: Like, comment, download, and more. -
+**Stories** (Coming soon...) - **Comments** (Coming soon...)
+## ð§ How To Use First of all, install the package using: ```bash pip install
 pygramcore ``` To take authenticated actions, initialize your Instagram account
 with your email/password and login: ```python from pygramcore import Account
 Account.login("youremail@email.com", "yourpassword123") Account.save_cookies
 ("path/to/file.pkl") ``` To initialize an account from cookies: ```python
 Account.load_cookies("path/to/file.pkl") ``` This will allow you to post
 images, comment on other peoples posts, send DMs, etc... ```python Account.post
 ("path/to/image.png", "Your very interesting caption") ``` To search for a user
 simply: ```python from pygramcore import User user = User("username123_") ```
 Here is an example of the usage of a user: ```python # Get a list of Post()
 objects posts = user.get_posts(limit=50) # Like the first 10 posts in the
 user's feed for post in posts[:10]: # Get URLs of the images in the post urls =
 post.get_images() # Like & comment the post post.comment("Nice post!")
-post.like() ``` Please refer to the docs for more.
-## ðââï¸ You may also like... - [âï¸ð±TikTok Manager](https://
-github.com/jtayped/tiktok-manager) - A script that manages MULTIPLE TikTok
-accounts by schedueling automatically generated videos from pre-selected
-YouTube channels to TikTok in advance. - [ð§âð¼My Portfolio](https://
-joeltaylor.business) - Check out my front-end and SEO skills on my Portfolio!
+post.like() ``` Please refer to the [docs](https://github.com/jtayped/
+pygramcore/tree/main/docs) for more.
+## â About the Project This Python package was created as a fun project to
+enhance my proficiency in writing "professional" Python code, building
+packages, implementing semantic versioning, and ensuring code maintainability.
+I am still a relatively new developer, and I welcome any contributions and
+feedback to help me improve. It is important to note that this project is not
+intended to replace essential packages such as [InstaPy](https://github.com/
+InstaPy/InstaPy), nor do I anticipate that it will. ## ðââï¸ You may
+also like... - [âï¸ð±TikTok Manager](https://github.com/jtayped/tiktok-
+manager) - A script that manages MULTIPLE TikTok accounts by schedueling
+automatically generated videos from pre-selected YouTube channels to TikTok in
+advance. - [ð§âð¼My Portfolio](https://joeltaylor.business) - Check out
+my front-end and SEO skills on my Portfolio!
```

### Comparing `pygramcore-1.0.2/pygramcore/elements/post.py` & `pygramcore-1.0.3/pygramcore/elements/post.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,15 +107,15 @@
 
         Returns:
             list[User]: List of Users.
 
         Raises:
             TooManyUsers: Raises when the limit is above 100.
         """
-        from elements import User
+        from .user import User
 
         if limit > 100:
             raise TooManyUsers()
 
         # Open likes dialog
         likes_element = self._driver.find_element(
             By.XPATH,
@@ -227,15 +227,14 @@
         Args:
             text (str): The comment.
 
         Raises:
             CannotComment: Whether you can comment.
             NotAuthenticated: Raises when the current account is not logged in.
         """
-        # TODO: when comment implementation done continue...
         if not self.can_comment():
             raise CannotComment()
 
         # Find form and write the comment text
         form_element = self._driver.find_element(By.TAG_NAME, "form")
 
         # The textarea changes when selecting it, triggering a "StaleElementReferenceException"
```

### Comparing `pygramcore-1.0.2/pygramcore/elements/user.py` & `pygramcore-1.0.3/pygramcore/elements/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,18 +104,18 @@
             "body > div.x1n2onr6.xzkaem6 > div.x9f619.x1n2onr6.x1ja2u2z > div > div.x1uvtmcs.x4k7w5x.x1h91t0o.x1beo9mf.xaigb6o.x12ejxvf.x3igimt.xarpa2k.xedcshv.x1lytzrv.x1t2pt76.x7ja8zs.x1n2onr6.x1qrby5j.x1jfb8zj > div > div > div > div > div.x7r02ix.xf1ldfh.x131esax.xdajt7p.xxfnqb6.xb88tzc.xw2csxc.x1odjw0f.x5fp0pe > div > div > div > div:nth-child(8)",
         )
         unfollow_btn.click()
 
     @check_authorization
     def is_following(self):
         """
-        Check whether you follow the user.
+        Check whether the account logged in follows the user.
 
         Returns:
-            bool: True if the user is followed, False if not.
+            bool: whether the account logged in follows the user.
 
         Raises:
             NotAuthenticated: Raises when the current account is not logged in.
         """
 
         self._driver.implicitly_wait(1)
 
@@ -308,14 +308,20 @@
         following_str = following_span.find_element(By.CSS_SELECTOR, "span").text
 
         # Remove the commas and convert to integer
         followers = int(following_str.replace(",", ""))
         return followers
 
     def send_dm(self, message: str) -> None:
+        """
+        Send a DM (direct message) to the user.
+
+        Args:
+            message (str): Message to send the user.
+        """
         # Enter the DMs
         message_btn = self._driver.find_element(By.XPATH, '//div[text()="Message"]')
         message_btn.click()
 
         # Write the the message
         message_input = self._driver.find_element(
             By.XPATH,
@@ -347,15 +353,15 @@
         posts = user.get_posts()
 
         # Like his first three posts
         for post in posts[:3]:
             post.like()
         ```
         """
-        from elements import Post
+        from .post import Post
 
         css_selector = "a[href^='/p/']"
         if reels:
             css_selector += ",a[href^='/reel/']"
 
         posts = []
```

### Comparing `pygramcore-1.0.2/pygramcore/exceptions/user.py` & `pygramcore-1.0.3/pygramcore/exceptions/user.py`

 * *Files identical despite different names*

### Comparing `pygramcore-1.0.2/pygramcore/pygram.py` & `pygramcore-1.0.3/pygramcore/pygram.py`

 * *Files identical despite different names*

### Comparing `pygramcore-1.0.2/pygramcore/utils/misc.py` & `pygramcore-1.0.3/pygramcore/utils/misc.py`

 * *Files identical despite different names*

### Comparing `pygramcore-1.0.2/pygramcore.egg-info/PKG-INFO` & `pygramcore-1.0.3/pygramcore.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygramcore
-Version: 1.0.2
+Version: 1.0.3
 Summary: A simple-to-use Instagram Python interface using Selenium.
 Author: Joel Taylor
 Author-email: contact@joeltaylor.business
 License: MIT
 Keywords: instagram,instagram bot,selenium,automation,bot
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -48,25 +48,25 @@
 
 <div id="key-features"></div>
 
 ## 🔑 Key Features
 
 - **Modular Elements**: Easily use and customize modular elements such as Posts, Comments, and Users.
 
-  - **Users**: Follow, download posts, direct message, and more.
+  - **Users**: Follow, direct message, get posts, and more.
 
-  - **Stories**: Like, download, reply and more.
+  - **Posts**: Like, comment, download, and more.
 
-  - **Posts**: Like, comment, save, download, and more.
+  - **Stories** (Coming soon...)
 
-  - **Comments**: Like, reply, and engage.
+  - **Comments** (Coming soon...)
 
 <div id="how-to-use"></div>
 
-## ❓ How To Use
+## 🔧 How To Use
 
 First of all, install the package using:
 
 ```bash
 pip install pygramcore
 ```
 
@@ -111,15 +111,20 @@
   urls = post.get_images()
 
   # Like & comment the post
   post.comment("Nice post!")
   post.like()
 ```
 
-Please refer to the docs for more.
+Please refer to the [docs](https://github.com/jtayped/pygramcore/tree/main/docs) for more.
 
 <div id="related"></div>
 
+## ❓ About the Project
+This Python package was created as a fun project to enhance my proficiency in writing "professional" Python code, building packages, implementing semantic versioning, and ensuring code maintainability.
+I am still a relatively new developer, and I welcome any contributions and feedback to help me improve.
+It is important to note that this project is not intended to replace essential packages such as [InstaPy](https://github.com/InstaPy/InstaPy), nor do I anticipate that it will.
+
 ## 🙋‍♂️ You may also like...
 
 - [✂️📱TikTok Manager](https://github.com/jtayped/tiktok-manager) - A script that manages MULTIPLE TikTok accounts by schedueling automatically generated videos from pre-selected YouTube channels to TikTok in advance.
 - [🧑‍💼My Portfolio](https://joeltaylor.business) - Check out my front-end and SEO skills on my Portfolio!
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pygramcore Version: 1.0.2 Summary: A simple-to-use
+Metadata-Version: 2.1 Name: pygramcore Version: 1.0.3 Summary: A simple-to-use
 Instagram Python interface using Selenium. Author: Joel Taylor Author-email:
 contact@joeltaylor.business License: MIT Keywords: instagram,instagram
 bot,selenium,automation,bot Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3.12 Classifier: Programming Language :: Python :: Implementation ::
 CPython Description-Content-Type: text/markdown License-File: LICENSE Requires-
 Dist: selenium Requires-Dist: selenium-stealth
@@ -11,30 +11,37 @@
                                 ?ð???· ppyyggrraammccoorree
                                      ************
              ****** AAnn eeaassyy--ttoo--uussee IInnssttaaggrraamm SSDDKK uussiinngg _SS_ee_ll_ee_nn_ii_uu_mm.. ******
     _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_p_y_g_r_a_m_c_o_r_e_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_]_[_L_i_c_e_n_s_e_]
                               _[_L_i_c_e_n_s_e_]_[_L_i_n_k_e_d_I_n_]
                     _K_e_y_ _F_e_a_t_u_r_e_s â¢ _H_o_w_ _T_o_ _U_s_e â¢ _R_e_l_a_t_e_d
 ## ð Key Features - **Modular Elements**: Easily use and customize modular
-elements such as Posts, Comments, and Users. - **Users**: Follow, download
-posts, direct message, and more. - **Stories**: Like, download, reply and more.
-- **Posts**: Like, comment, save, download, and more. - **Comments**: Like,
-reply, and engage.
-## â How To Use First of all, install the package using: ```bash pip install
+elements such as Posts, Comments, and Users. - **Users**: Follow, direct
+message, get posts, and more. - **Posts**: Like, comment, download, and more. -
+**Stories** (Coming soon...) - **Comments** (Coming soon...)
+## ð§ How To Use First of all, install the package using: ```bash pip install
 pygramcore ``` To take authenticated actions, initialize your Instagram account
 with your email/password and login: ```python from pygramcore import Account
 Account.login("youremail@email.com", "yourpassword123") Account.save_cookies
 ("path/to/file.pkl") ``` To initialize an account from cookies: ```python
 Account.load_cookies("path/to/file.pkl") ``` This will allow you to post
 images, comment on other peoples posts, send DMs, etc... ```python Account.post
 ("path/to/image.png", "Your very interesting caption") ``` To search for a user
 simply: ```python from pygramcore import User user = User("username123_") ```
 Here is an example of the usage of a user: ```python # Get a list of Post()
 objects posts = user.get_posts(limit=50) # Like the first 10 posts in the
 user's feed for post in posts[:10]: # Get URLs of the images in the post urls =
 post.get_images() # Like & comment the post post.comment("Nice post!")
-post.like() ``` Please refer to the docs for more.
-## ðââï¸ You may also like... - [âï¸ð±TikTok Manager](https://
-github.com/jtayped/tiktok-manager) - A script that manages MULTIPLE TikTok
-accounts by schedueling automatically generated videos from pre-selected
-YouTube channels to TikTok in advance. - [ð§âð¼My Portfolio](https://
-joeltaylor.business) - Check out my front-end and SEO skills on my Portfolio!
+post.like() ``` Please refer to the [docs](https://github.com/jtayped/
+pygramcore/tree/main/docs) for more.
+## â About the Project This Python package was created as a fun project to
+enhance my proficiency in writing "professional" Python code, building
+packages, implementing semantic versioning, and ensuring code maintainability.
+I am still a relatively new developer, and I welcome any contributions and
+feedback to help me improve. It is important to note that this project is not
+intended to replace essential packages such as [InstaPy](https://github.com/
+InstaPy/InstaPy), nor do I anticipate that it will. ## ðââï¸ You may
+also like... - [âï¸ð±TikTok Manager](https://github.com/jtayped/tiktok-
+manager) - A script that manages MULTIPLE TikTok accounts by schedueling
+automatically generated videos from pre-selected YouTube channels to TikTok in
+advance. - [ð§âð¼My Portfolio](https://joeltaylor.business) - Check out
+my front-end and SEO skills on my Portfolio!
```

### Comparing `pygramcore-1.0.2/pygramcore.egg-info/SOURCES.txt` & `pygramcore-1.0.3/pygramcore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pygramcore-1.0.2/setup.py` & `pygramcore-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 from codecs import open
 from os import path
 
 # Read version from VERSION file
 here = path.abspath(path.dirname(__file__))
 
-VERSION = "1.0.2"
+VERSION = "1.0.3"
 DESCRIPTION = "A simple-to-use Instagram Python interface using Selenium."
 
 # Get the long description from the README file
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     LONG_DESCRIPTION = f.read()
 
 setup(
```

