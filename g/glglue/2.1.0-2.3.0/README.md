# Comparing `tmp/glglue-2.1.0.tar.gz` & `tmp/glglue-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glglue-2.1.0.tar", last modified: Tue May  7 09:57:17 2024, max compression
+gzip compressed data, was "glglue-2.3.0.tar", last modified: Fri May 10 11:00:43 2024, max compression
```

## Comparing `glglue-2.1.0.tar` & `glglue-2.3.0.tar`

### file list

```diff
@@ -1,122 +1,127 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 09:57:17.094121 glglue-2.1.0/
--rw-rw-rw-   0        0        0      321 2024-05-07 04:24:13.000000 glglue-2.1.0/.clang-format
-drwxrwxrwx   0        0        0        0 2024-05-07 09:57:17.022846 glglue-2.1.0/.github/
-drwxrwxrwx   0        0        0        0 2024-05-07 09:57:17.033918 glglue-2.1.0/.github/workflows/
--rw-rw-rw-   0        0        0     1321 2024-05-07 09:21:29.000000 glglue-2.1.0/.github/workflows/docusaurus.yml
--rw-rw-rw-   0        0        0     3318 2024-05-07 09:35:53.000000 glglue-2.1.0/.github/workflows/pypi.yml
--rw-rw-rw-   0        0        0       79 2024-05-07 04:24:13.000000 glglue-2.1.0/.gitignore
--rw-rw-rw-   0        0        0       75 2024-05-07 04:24:13.000000 glglue-2.1.0/.remarkrc
-drwxrwxrwx   0        0        0        0 2024-05-07 09:57:17.035936 glglue-2.1.0/.vscode/
--rw-rw-rw-   0        0        0     2791 2024-05-07 09:19:11.000000 glglue-2.1.0/.vscode/launch.json
--rw-rw-rw-   0        0        0      602 2024-05-07 04:24:13.000000 glglue-2.1.0/.vscode/settings.json
--rw-rw-rw-   0        0        0      555 2024-05-07 04:24:13.000000 glglue-2.1.0/.vscode/tasks.json
--rw-rw-rw-   0        0        0     1065 2024-05-07 04:24:13.000000 glglue-2.1.0/LICENSE
--rw-rw-rw-   0        0        0     1884 2024-05-07 09:57:17.093122 glglue-2.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1259 2024-05-07 09:19:11.000000 glglue-2.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-07 09:57:17.040936 glglue-2.1.0/docs/
--rw-rw-rw-   0        0        0      233 2024-05-07 09:19:11.000000 glglue-2.1.0/docs/.gitignore
--rw-rw-rw-   0        0        0      768 2024-05-07 09:19:11.000000 glglue-2.1.0/docs/README.md
--rw-rw-rw-   0        0        0       89 2024-05-07 09:19:11.000000 glglue-2.1.0/docs/babel.config.js
-drwxrwxrwx   0        0        0        0 2024-05-07 09:57:17.043936 glglue-2.1.0/docs/blog/
--rw-rw-rw-   0        0        0      389 2024-05-07 09:19:11.000000 glglue-2.1.0/docs/blog/2019-05-28-first-blog-post.md
--rw-rw-rw-   0        0        0     3116 2024-05-07 09:19:11.000000 glglue-2.1.0/docs/blog/2019-05-29-long-blog-post.md
--rw-rw-rw-   0        0        0      439 2024-05-07 09:19:11.000000 glglue-2.1.0/docs/blog/2021-08-01-mdx-blog-post.mdx
-drwxrwxrwx   0        0        0        0 2024-05-07 09:57:17.044936 glglue-2.1.0/docs/blog/2021-08-26-welcome/
--rw-rw-rw-   0        0        0    96122 2024-05-07 09:19:11.000000 glglue-2.1.0/docs/blog/2021-08-26-welcome/docusaurus-plushie-banner.jpeg
--rw-rw-rw-   0        0        0      783 2024-05-07 09:19:11.000000 glglue-2.1.0/docs/blog/2021-08-26-welcome/index.md
--rw-rw-rw-   0        0        0      447 2024-05-07 09:19:11.000000 glglue-2.1.0/docs/blog/authors.yml
-drwxrwxrwx   0        0        0        0 2024-05-07 09:57:17.044936 glglue-2.1.0/docs/docs/
--rw-rw-rw-   0        0        0      875 2024-05-07 09:19:11.000000 glglue-2.1.0/docs/docs/index.md
--rw-rw-rw-   0        0        0     3760 2024-05-07 09:19:11.000000 glglue-2.1.0/docs/docusaurus.config.ts
--rw-rw-rw-   0        0        0   570118 2024-05-07 09:19:11.000000 glglue-2.1.0/docs/package-lock.json
--rw-rw-rw-   0        0        0     1150 2024-05-07 09:19:11.000000 glglue-2.1.0/docs/package.json
--rw-rw-rw-   0        0        0      645 2024-05-07 09:19:11.000000 glglue-2.1.0/docs/sidebars.ts
-drwxrwxrwx   0        0        0        0 2024-05-07 09:57:17.026842 glglue-2.1.0/docs/src/
-drwxrwxrwx   0        0        0        0 2024-05-07 09:57:17.026842 glglue-2.1.0/docs/src/components/
-drwxrwxrwx   0        0        0        0 2024-05-07 09:57:17.045936 glglue-2.1.0/docs/src/components/HomepageFeatures/
--rw-rw-rw-   0        0        0     1889 2024-05-07 09:19:11.000000 glglue-2.1.0/docs/src/components/HomepageFeatures/index.tsx
--rw-rw-rw-   0        0        0      138 2024-05-07 09:19:11.000000 glglue-2.1.0/docs/src/components/HomepageFeatures/styles.module.css
-drwxrwxrwx   0        0        0        0 2024-05-07 09:57:17.046936 glglue-2.1.0/docs/src/css/
--rw-rw-rw-   0        0        0     1042 2024-05-07 09:19:11.000000 glglue-2.1.0/docs/src/css/custom.css
-drwxrwxrwx   0        0        0        0 2024-05-07 09:57:17.047936 glglue-2.1.0/docs/src/pages/
--rw-rw-rw-   0        0        0      365 2024-05-07 09:19:11.000000 glglue-2.1.0/docs/src/pages/index.module.css
--rw-rw-rw-   0        0        0     1343 2024-05-07 09:25:04.000000 glglue-2.1.0/docs/src/pages/index.tsx
--rw-rw-rw-   0        0        0      118 2024-05-07 09:19:11.000000 glglue-2.1.0/docs/src/pages/markdown-page.md
-drwxrwxrwx   0        0        0        0 2024-05-07 09:57:17.049584 glglue-2.1.0/docs/static/
--rw-rw-rw-   0        0        0        0 2024-05-07 09:19:11.000000 glglue-2.1.0/docs/static/.nojekyll
-drwxrwxrwx   0        0        0        0 2024-05-07 09:57:17.053603 glglue-2.1.0/docs/static/img/
--rw-rw-rw-   0        0        0    55746 2024-05-07 09:19:11.000000 glglue-2.1.0/docs/static/img/docusaurus-social-card.jpg
--rw-rw-rw-   0        0        0     5142 2024-05-07 09:19:11.000000 glglue-2.1.0/docs/static/img/docusaurus.png
--rw-rw-rw-   0        0        0     3626 2024-05-07 09:19:11.000000 glglue-2.1.0/docs/static/img/favicon.ico
--rw-rw-rw-   0        0        0     6438 2024-05-07 09:19:11.000000 glglue-2.1.0/docs/static/img/logo.svg
--rw-rw-rw-   0        0        0    31486 2024-05-07 09:19:11.000000 glglue-2.1.0/docs/static/img/undraw_docusaurus_mountain.svg
--rw-rw-rw-   0        0        0    36002 2024-05-07 09:19:11.000000 glglue-2.1.0/docs/static/img/undraw_docusaurus_react.svg
--rw-rw-rw-   0        0        0    11887 2024-05-07 09:19:11.000000 glglue-2.1.0/docs/static/img/undraw_docusaurus_tree.svg
--rw-rw-rw-   0        0        0      176 2024-05-07 09:19:11.000000 glglue-2.1.0/docs/tsconfig.json
-drwxrwxrwx   0        0        0        0 2024-05-07 09:57:17.056602 glglue-2.1.0/examples/
--rw-rw-rw-   0        0        0      533 2024-05-07 09:19:11.000000 glglue-2.1.0/examples/freeglut_sample.py
--rw-rw-rw-   0        0        0      394 2024-05-07 09:19:11.000000 glglue-2.1.0/examples/glfw_sample.py
--rw-rw-rw-   0        0        0      632 2024-05-07 04:24:13.000000 glglue-2.1.0/examples/gtk3_sample.py
--rw-rw-rw-   0        0        0      776 2024-05-07 04:24:13.000000 glglue-2.1.0/examples/gtk4_sample.py
--rw-rw-rw-   0        0        0      391 2024-05-07 09:19:11.000000 glglue-2.1.0/examples/pysdl2_sample.py
--rw-rw-rw-   0        0        0      591 2024-05-07 09:19:11.000000 glglue-2.1.0/examples/pyside6_sample.py
--rw-rw-rw-   0        0        0      657 2024-05-07 04:24:13.000000 glglue-2.1.0/examples/wgl_sample.py
--rw-rw-rw-   0        0        0      816 2024-05-07 09:19:11.000000 glglue-2.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-07 09:57:17.094121 glglue-2.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-07 09:57:17.028844 glglue-2.1.0/src/
-drwxrwxrwx   0        0        0        0 2024-05-07 09:57:17.068501 glglue-2.1.0/src/glglue/
--rw-rw-rw-   0        0        0       67 2024-05-07 09:19:11.000000 glglue-2.1.0/src/glglue/__init__.py
--rw-rw-rw-   0        0        0     1115 2024-05-07 09:19:11.000000 glglue-2.1.0/src/glglue/__main__.py
--rw-rw-rw-   0        0        0      427 2024-05-07 09:57:16.000000 glglue-2.1.0/src/glglue/_version.py
-drwxrwxrwx   0        0        0        0 2024-05-07 09:57:17.079502 glglue-2.1.0/src/glglue/assets/
--rw-rw-rw-   0        0        0   471984 2024-05-07 09:19:11.000000 glglue-2.1.0/src/glglue/assets/Utah_teapot_(solid).stl
--rw-rw-rw-   0        0        0       96 2024-05-07 09:19:11.000000 glglue-2.1.0/src/glglue/assets/mesh.fs
--rw-rw-rw-   0        0        0      406 2024-05-07 09:19:11.000000 glglue-2.1.0/src/glglue/assets/mesh.vs
-drwxrwxrwx   0        0        0        0 2024-05-07 09:57:17.083090 glglue-2.1.0/src/glglue/camera/
--rw-rw-rw-   0        0        0      279 2024-05-07 09:19:11.000000 glglue-2.1.0/src/glglue/camera/__init__.py
--rw-rw-rw-   0        0        0     7991 2024-05-07 09:19:11.000000 glglue-2.1.0/src/glglue/camera/camera.py
--rw-rw-rw-   0        0        0      823 2024-05-07 09:19:11.000000 glglue-2.1.0/src/glglue/camera/mouse_camera.py
--rw-rw-rw-   0        0        0     4730 2024-05-07 09:19:11.000000 glglue-2.1.0/src/glglue/camera/mouse_event.py
-drwxrwxrwx   0        0        0        0 2024-05-07 09:57:17.086121 glglue-2.1.0/src/glglue/drawable/
--rw-rw-rw-   0        0        0       55 2024-05-07 09:19:11.000000 glglue-2.1.0/src/glglue/drawable/__init__.py
--rw-rw-rw-   0        0        0     1400 2024-05-07 09:19:11.000000 glglue-2.1.0/src/glglue/drawable/cube.py
--rw-rw-rw-   0        0        0     1360 2024-05-07 09:19:11.000000 glglue-2.1.0/src/glglue/drawable/drawable.py
--rw-rw-rw-   0        0        0     2744 2024-05-07 09:19:11.000000 glglue-2.1.0/src/glglue/drawable/teapot.py
--rw-rw-rw-   0        0        0     1392 2024-05-07 09:19:11.000000 glglue-2.1.0/src/glglue/drawable/vertex_buffer.py
--rw-rw-rw-   0        0        0      509 2024-05-07 09:19:11.000000 glglue-2.1.0/src/glglue/frame_input.py
--rw-rw-rw-   0        0        0     5210 2024-05-07 09:19:11.000000 glglue-2.1.0/src/glglue/glfw.py
-drwxrwxrwx   0        0        0        0 2024-05-07 09:57:17.089121 glglue-2.1.0/src/glglue/glo/
--rw-rw-rw-   0        0        0      470 2024-05-07 09:19:11.000000 glglue-2.1.0/src/glglue/glo/__init__.py
--rw-rw-rw-   0        0        0     2461 2024-05-07 09:19:11.000000 glglue-2.1.0/src/glglue/glo/fbo.py
--rw-rw-rw-   0        0        0     5587 2024-05-07 09:19:11.000000 glglue-2.1.0/src/glglue/glo/shader.py
--rw-rw-rw-   0        0        0     1980 2024-05-07 09:19:11.000000 glglue-2.1.0/src/glglue/glo/texture.py
--rw-rw-rw-   0        0        0     1355 2024-05-07 09:19:11.000000 glglue-2.1.0/src/glglue/glo/vao.py
--rw-rw-rw-   0        0        0     2100 2024-05-07 09:19:11.000000 glglue-2.1.0/src/glglue/glo/vbo.py
--rw-rw-rw-   0        0        0     3630 2024-05-07 09:19:11.000000 glglue-2.1.0/src/glglue/glo/vertex_layout.py
--rw-rw-rw-   0        0        0     3144 2024-05-07 09:19:11.000000 glglue-2.1.0/src/glglue/glut.py
--rw-rw-rw-   0        0        0     2659 2024-05-07 09:19:11.000000 glglue-2.1.0/src/glglue/gtk3.py
--rw-rw-rw-   0        0        0     3156 2024-05-07 09:19:11.000000 glglue-2.1.0/src/glglue/gtk4.py
--rw-rw-rw-   0        0        0     3625 2024-05-07 09:19:11.000000 glglue-2.1.0/src/glglue/pysdl2.py
--rw-rw-rw-   0        0        0     3930 2024-05-07 09:19:11.000000 glglue-2.1.0/src/glglue/pyside6.py
--rw-rw-rw-   0        0        0     2443 2024-05-07 09:19:11.000000 glglue-2.1.0/src/glglue/qgl4.py
--rw-rw-rw-   0        0        0     2452 2024-05-07 09:19:11.000000 glglue-2.1.0/src/glglue/qgl5.py
-drwxrwxrwx   0        0        0        0 2024-05-07 09:57:17.090121 glglue-2.1.0/src/glglue/scene/
--rw-rw-rw-   0        0        0      185 2024-05-07 09:19:11.000000 glglue-2.1.0/src/glglue/scene/node.py
--rw-rw-rw-   0        0        0     1709 2024-05-07 09:19:11.000000 glglue-2.1.0/src/glglue/scene/sample.py
--rw-rw-rw-   0        0        0      962 2024-05-07 09:19:11.000000 glglue-2.1.0/src/glglue/sdl.py
--rw-rw-rw-   0        0        0     2885 2024-05-07 09:19:11.000000 glglue-2.1.0/src/glglue/togl.py
--rw-rw-rw-   0        0        0     1475 2024-05-07 09:19:11.000000 glglue-2.1.0/src/glglue/util.py
--rw-rw-rw-   0        0        0    21812 2024-05-07 09:19:11.000000 glglue-2.1.0/src/glglue/wgl.py
--rw-rw-rw-   0        0        0   122098 2024-05-07 09:19:11.000000 glglue-2.1.0/src/glglue/win32con.py
--rw-rw-rw-   0        0        0      529 2024-05-07 09:19:11.000000 glglue-2.1.0/src/glglue/windowconfig.py
--rw-rw-rw-   0        0        0     3190 2024-05-07 09:19:11.000000 glglue-2.1.0/src/glglue/wxglcanvas.py
-drwxrwxrwx   0        0        0        0 2024-05-07 09:57:17.092122 glglue-2.1.0/src/glglue.egg-info/
--rw-rw-rw-   0        0        0     1884 2024-05-07 09:57:16.000000 glglue-2.1.0/src/glglue.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2507 2024-05-07 09:57:17.000000 glglue-2.1.0/src/glglue.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 09:57:16.000000 glglue-2.1.0/src/glglue.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-05-07 09:57:16.000000 glglue-2.1.0/src/glglue.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-07 09:57:16.000000 glglue-2.1.0/src/glglue.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-07 09:57:17.092122 glglue-2.1.0/tests/
--rw-rw-rw-   0        0        0     1410 2024-05-07 04:24:13.000000 glglue-2.1.0/tests/test_numpy.py
--rw-rw-rw-   0        0        0      287 2024-05-07 09:19:11.000000 glglue-2.1.0/tests/test_py.py
--rw-rw-rw-   0        0        0      221 2024-05-07 09:19:11.000000 glglue-2.1.0/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-10 11:00:43.897657 glglue-2.3.0/
+-rw-rw-rw-   0        0        0      321 2024-05-07 04:24:13.000000 glglue-2.3.0/.clang-format
+drwxrwxrwx   0        0        0        0 2024-05-10 11:00:43.829623 glglue-2.3.0/.github/
+drwxrwxrwx   0        0        0        0 2024-05-10 11:00:43.840880 glglue-2.3.0/.github/workflows/
+-rw-rw-rw-   0        0        0     1321 2024-05-07 09:21:29.000000 glglue-2.3.0/.github/workflows/docusaurus.yml
+-rw-rw-rw-   0        0        0       86 2024-05-08 10:16:01.000000 glglue-2.3.0/.gitignore
+-rw-rw-rw-   0        0        0       75 2024-05-07 04:24:13.000000 glglue-2.3.0/.remarkrc
+drwxrwxrwx   0        0        0        0 2024-05-10 11:00:43.841879 glglue-2.3.0/.vscode/
+-rw-rw-rw-   0        0        0     2760 2024-05-08 10:28:17.000000 glglue-2.3.0/.vscode/launch.json
+-rw-rw-rw-   0        0        0      602 2024-05-07 04:24:13.000000 glglue-2.3.0/.vscode/settings.json
+-rw-rw-rw-   0        0        0      555 2024-05-07 04:24:13.000000 glglue-2.3.0/.vscode/tasks.json
+-rw-rw-rw-   0        0        0     1065 2024-05-07 04:24:13.000000 glglue-2.3.0/LICENSE
+-rw-rw-rw-   0        0        0     1884 2024-05-10 11:00:43.896872 glglue-2.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1259 2024-05-07 09:19:11.000000 glglue-2.3.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-10 11:00:43.849395 glglue-2.3.0/docs/
+-rw-rw-rw-   0        0        0      233 2024-05-07 09:19:11.000000 glglue-2.3.0/docs/.gitignore
+-rw-rw-rw-   0        0        0      768 2024-05-07 09:19:11.000000 glglue-2.3.0/docs/README.md
+-rw-rw-rw-   0        0        0       89 2024-05-07 09:19:11.000000 glglue-2.3.0/docs/babel.config.js
+drwxrwxrwx   0        0        0        0 2024-05-10 11:00:43.851394 glglue-2.3.0/docs/blog/
+-rw-rw-rw-   0        0        0      389 2024-05-07 09:19:11.000000 glglue-2.3.0/docs/blog/2019-05-28-first-blog-post.md
+-rw-rw-rw-   0        0        0     3116 2024-05-07 09:19:11.000000 glglue-2.3.0/docs/blog/2019-05-29-long-blog-post.md
+-rw-rw-rw-   0        0        0      439 2024-05-07 09:19:11.000000 glglue-2.3.0/docs/blog/2021-08-01-mdx-blog-post.mdx
+drwxrwxrwx   0        0        0        0 2024-05-10 11:00:43.852395 glglue-2.3.0/docs/blog/2021-08-26-welcome/
+-rw-rw-rw-   0        0        0    96122 2024-05-07 09:19:11.000000 glglue-2.3.0/docs/blog/2021-08-26-welcome/docusaurus-plushie-banner.jpeg
+-rw-rw-rw-   0        0        0      783 2024-05-07 09:19:11.000000 glglue-2.3.0/docs/blog/2021-08-26-welcome/index.md
+-rw-rw-rw-   0        0        0      447 2024-05-07 09:19:11.000000 glglue-2.3.0/docs/blog/authors.yml
+drwxrwxrwx   0        0        0        0 2024-05-10 11:00:43.853394 glglue-2.3.0/docs/docs/
+-rw-rw-rw-   0        0        0      875 2024-05-07 09:19:11.000000 glglue-2.3.0/docs/docs/index.md
+-rw-rw-rw-   0        0        0     3760 2024-05-07 09:19:11.000000 glglue-2.3.0/docs/docusaurus.config.ts
+-rw-rw-rw-   0        0        0   570118 2024-05-07 09:19:11.000000 glglue-2.3.0/docs/package-lock.json
+-rw-rw-rw-   0        0        0     1150 2024-05-07 09:19:11.000000 glglue-2.3.0/docs/package.json
+-rw-rw-rw-   0        0        0      645 2024-05-07 09:19:11.000000 glglue-2.3.0/docs/sidebars.ts
+drwxrwxrwx   0        0        0        0 2024-05-10 11:00:43.833417 glglue-2.3.0/docs/src/
+drwxrwxrwx   0        0        0        0 2024-05-10 11:00:43.832312 glglue-2.3.0/docs/src/components/
+drwxrwxrwx   0        0        0        0 2024-05-10 11:00:43.854480 glglue-2.3.0/docs/src/components/HomepageFeatures/
+-rw-rw-rw-   0        0        0     1889 2024-05-07 09:19:11.000000 glglue-2.3.0/docs/src/components/HomepageFeatures/index.tsx
+-rw-rw-rw-   0        0        0      138 2024-05-07 09:19:11.000000 glglue-2.3.0/docs/src/components/HomepageFeatures/styles.module.css
+drwxrwxrwx   0        0        0        0 2024-05-10 11:00:43.854480 glglue-2.3.0/docs/src/css/
+-rw-rw-rw-   0        0        0     1042 2024-05-07 09:19:11.000000 glglue-2.3.0/docs/src/css/custom.css
+drwxrwxrwx   0        0        0        0 2024-05-10 11:00:43.856480 glglue-2.3.0/docs/src/pages/
+-rw-rw-rw-   0        0        0      365 2024-05-07 09:19:11.000000 glglue-2.3.0/docs/src/pages/index.module.css
+-rw-rw-rw-   0        0        0     1343 2024-05-07 09:25:04.000000 glglue-2.3.0/docs/src/pages/index.tsx
+-rw-rw-rw-   0        0        0      118 2024-05-07 09:19:11.000000 glglue-2.3.0/docs/src/pages/markdown-page.md
+drwxrwxrwx   0        0        0        0 2024-05-10 11:00:43.856480 glglue-2.3.0/docs/static/
+-rw-rw-rw-   0        0        0        0 2024-05-07 09:19:11.000000 glglue-2.3.0/docs/static/.nojekyll
+drwxrwxrwx   0        0        0        0 2024-05-10 11:00:43.859500 glglue-2.3.0/docs/static/img/
+-rw-rw-rw-   0        0        0    55746 2024-05-07 09:19:11.000000 glglue-2.3.0/docs/static/img/docusaurus-social-card.jpg
+-rw-rw-rw-   0        0        0     5142 2024-05-07 09:19:11.000000 glglue-2.3.0/docs/static/img/docusaurus.png
+-rw-rw-rw-   0        0        0     3626 2024-05-07 09:19:11.000000 glglue-2.3.0/docs/static/img/favicon.ico
+-rw-rw-rw-   0        0        0     6438 2024-05-07 09:19:11.000000 glglue-2.3.0/docs/static/img/logo.svg
+-rw-rw-rw-   0        0        0    31486 2024-05-07 09:19:11.000000 glglue-2.3.0/docs/static/img/undraw_docusaurus_mountain.svg
+-rw-rw-rw-   0        0        0    36002 2024-05-07 09:19:11.000000 glglue-2.3.0/docs/static/img/undraw_docusaurus_react.svg
+-rw-rw-rw-   0        0        0    11887 2024-05-07 09:19:11.000000 glglue-2.3.0/docs/static/img/undraw_docusaurus_tree.svg
+-rw-rw-rw-   0        0        0      176 2024-05-07 09:19:11.000000 glglue-2.3.0/docs/tsconfig.json
+drwxrwxrwx   0        0        0        0 2024-05-10 11:00:43.834376 glglue-2.3.0/examples/
+drwxrwxrwx   0        0        0        0 2024-05-10 11:00:43.864011 glglue-2.3.0/examples/basic/
+-rw-rw-rw-   0        0        0      533 2024-05-07 09:19:11.000000 glglue-2.3.0/examples/basic/freeglut_sample.py
+-rw-rw-rw-   0        0        0      394 2024-05-07 09:19:11.000000 glglue-2.3.0/examples/basic/glfw_sample.py
+-rw-rw-rw-   0        0        0      632 2024-05-07 04:24:13.000000 glglue-2.3.0/examples/basic/gtk3_sample.py
+-rw-rw-rw-   0        0        0      776 2024-05-07 04:24:13.000000 glglue-2.3.0/examples/basic/gtk4_sample.py
+-rw-rw-rw-   0        0        0      391 2024-05-07 09:19:11.000000 glglue-2.3.0/examples/basic/pysdl2_sample.py
+-rw-rw-rw-   0        0        0      591 2024-05-07 09:19:11.000000 glglue-2.3.0/examples/basic/pyside6_sample.py
+-rw-rw-rw-   0        0        0      657 2024-05-07 04:24:13.000000 glglue-2.3.0/examples/basic/wgl_sample.py
+drwxrwxrwx   0        0        0        0 2024-05-10 11:00:43.865010 glglue-2.3.0/examples/gui/
+-rw-rw-rw-   0        0        0     2630 2024-05-08 11:56:08.000000 glglue-2.3.0/examples/gui/pyside6_gui.py
+-rw-rw-rw-   0        0        0      816 2024-05-07 09:19:11.000000 glglue-2.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-10 11:00:43.897657 glglue-2.3.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-10 11:00:43.835375 glglue-2.3.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-10 11:00:43.874369 glglue-2.3.0/src/glglue/
+-rw-rw-rw-   0        0        0       67 2024-05-07 09:19:11.000000 glglue-2.3.0/src/glglue/__init__.py
+-rw-rw-rw-   0        0        0      427 2024-05-10 11:00:43.000000 glglue-2.3.0/src/glglue/_version.py
+drwxrwxrwx   0        0        0        0 2024-05-10 11:00:43.884585 glglue-2.3.0/src/glglue/assets/
+-rw-rw-rw-   0        0        0   471984 2024-05-07 09:19:11.000000 glglue-2.3.0/src/glglue/assets/Utah_teapot_(solid).stl
+-rw-rw-rw-   0        0        0      103 2024-05-10 10:42:28.000000 glglue-2.3.0/src/glglue/assets/line.frag
+-rw-rw-rw-   0        0        0      261 2024-05-10 10:43:01.000000 glglue-2.3.0/src/glglue/assets/line.vert
+-rw-rw-rw-   0        0        0      103 2024-05-10 10:39:30.000000 glglue-2.3.0/src/glglue/assets/mesh.frag
+-rw-rw-rw-   0        0        0      462 2024-05-10 10:40:21.000000 glglue-2.3.0/src/glglue/assets/mesh.vert
+drwxrwxrwx   0        0        0        0 2024-05-10 11:00:43.886583 glglue-2.3.0/src/glglue/camera/
+-rw-rw-rw-   0        0        0      279 2024-05-07 09:19:11.000000 glglue-2.3.0/src/glglue/camera/__init__.py
+-rw-rw-rw-   0        0        0     7991 2024-05-07 09:19:11.000000 glglue-2.3.0/src/glglue/camera/camera.py
+-rw-rw-rw-   0        0        0      891 2024-05-08 09:14:56.000000 glglue-2.3.0/src/glglue/camera/mouse_camera.py
+-rw-rw-rw-   0        0        0     4730 2024-05-07 09:19:11.000000 glglue-2.3.0/src/glglue/camera/mouse_event.py
+drwxrwxrwx   0        0        0        0 2024-05-10 11:00:43.890790 glglue-2.3.0/src/glglue/drawable/
+-rw-rw-rw-   0        0        0       55 2024-05-07 09:19:11.000000 glglue-2.3.0/src/glglue/drawable/__init__.py
+-rw-rw-rw-   0        0        0     1097 2024-05-08 13:11:26.000000 glglue-2.3.0/src/glglue/drawable/axes.py
+-rw-rw-rw-   0        0        0     1398 2024-05-08 12:54:14.000000 glglue-2.3.0/src/glglue/drawable/cube.py
+-rw-rw-rw-   0        0        0     1374 2024-05-10 10:51:55.000000 glglue-2.3.0/src/glglue/drawable/drawable.py
+-rw-rw-rw-   0        0        0      892 2024-05-08 13:10:38.000000 glglue-2.3.0/src/glglue/drawable/grid.py
+-rw-rw-rw-   0        0        0     1045 2024-05-08 12:56:37.000000 glglue-2.3.0/src/glglue/drawable/line_builder.py
+-rw-rw-rw-   0        0        0     1699 2024-05-08 12:52:09.000000 glglue-2.3.0/src/glglue/drawable/mesh_builder.py
+-rw-rw-rw-   0        0        0     2815 2024-05-08 13:02:37.000000 glglue-2.3.0/src/glglue/drawable/teapot.py
+-rw-rw-rw-   0        0        0      509 2024-05-07 09:19:11.000000 glglue-2.3.0/src/glglue/frame_input.py
+-rw-rw-rw-   0        0        0     5210 2024-05-07 09:19:11.000000 glglue-2.3.0/src/glglue/glfw.py
+drwxrwxrwx   0        0        0        0 2024-05-10 11:00:43.893301 glglue-2.3.0/src/glglue/glo/
+-rw-rw-rw-   0        0        0      470 2024-05-07 09:19:11.000000 glglue-2.3.0/src/glglue/glo/__init__.py
+-rw-rw-rw-   0        0        0     2461 2024-05-07 09:19:11.000000 glglue-2.3.0/src/glglue/glo/fbo.py
+-rw-rw-rw-   0        0        0     6221 2024-05-10 10:41:35.000000 glglue-2.3.0/src/glglue/glo/shader.py
+-rw-rw-rw-   0        0        0     1980 2024-05-07 09:19:11.000000 glglue-2.3.0/src/glglue/glo/texture.py
+-rw-rw-rw-   0        0        0     1689 2024-05-10 08:05:17.000000 glglue-2.3.0/src/glglue/glo/vao.py
+-rw-rw-rw-   0        0        0     3140 2024-05-10 10:30:35.000000 glglue-2.3.0/src/glglue/glo/vbo.py
+-rw-rw-rw-   0        0        0     3755 2024-05-08 09:43:52.000000 glglue-2.3.0/src/glglue/glo/vertex_layout.py
+-rw-rw-rw-   0        0        0     3144 2024-05-07 09:19:11.000000 glglue-2.3.0/src/glglue/glut.py
+-rw-rw-rw-   0        0        0     2659 2024-05-07 09:19:11.000000 glglue-2.3.0/src/glglue/gtk3.py
+-rw-rw-rw-   0        0        0     3156 2024-05-07 09:19:11.000000 glglue-2.3.0/src/glglue/gtk4.py
+-rw-rw-rw-   0        0        0     3625 2024-05-07 09:19:11.000000 glglue-2.3.0/src/glglue/pysdl2.py
+-rw-rw-rw-   0        0        0     4672 2024-05-08 11:20:04.000000 glglue-2.3.0/src/glglue/pyside6.py
+-rw-rw-rw-   0        0        0     2443 2024-05-07 09:19:11.000000 glglue-2.3.0/src/glglue/qgl4.py
+-rw-rw-rw-   0        0        0     2452 2024-05-07 09:19:11.000000 glglue-2.3.0/src/glglue/qgl5.py
+drwxrwxrwx   0        0        0        0 2024-05-10 11:00:43.894301 glglue-2.3.0/src/glglue/scene/
+-rw-rw-rw-   0        0        0     2781 2024-05-08 13:09:20.000000 glglue-2.3.0/src/glglue/scene/sample.py
+-rw-rw-rw-   0        0        0      962 2024-05-07 09:19:11.000000 glglue-2.3.0/src/glglue/sdl.py
+-rw-rw-rw-   0        0        0     2885 2024-05-07 09:19:11.000000 glglue-2.3.0/src/glglue/togl.py
+-rw-rw-rw-   0        0        0     1475 2024-05-07 09:19:11.000000 glglue-2.3.0/src/glglue/util.py
+-rw-rw-rw-   0        0        0    21812 2024-05-07 09:19:11.000000 glglue-2.3.0/src/glglue/wgl.py
+-rw-rw-rw-   0        0        0   122098 2024-05-07 09:19:11.000000 glglue-2.3.0/src/glglue/win32con.py
+-rw-rw-rw-   0        0        0      529 2024-05-07 09:19:11.000000 glglue-2.3.0/src/glglue/windowconfig.py
+-rw-rw-rw-   0        0        0     3190 2024-05-07 09:19:11.000000 glglue-2.3.0/src/glglue/wxglcanvas.py
+drwxrwxrwx   0        0        0        0 2024-05-10 11:00:43.896369 glglue-2.3.0/src/glglue.egg-info/
+-rw-rw-rw-   0        0        0     1884 2024-05-10 11:00:43.000000 glglue-2.3.0/src/glglue.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2653 2024-05-10 11:00:43.000000 glglue-2.3.0/src/glglue.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-10 11:00:43.000000 glglue-2.3.0/src/glglue.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-10 11:00:43.000000 glglue-2.3.0/src/glglue.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-10 11:00:43.000000 glglue-2.3.0/src/glglue.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-10 11:00:43.895301 glglue-2.3.0/tests/
+-rw-rw-rw-   0        0        0     1410 2024-05-07 04:24:13.000000 glglue-2.3.0/tests/test_numpy.py
+-rw-rw-rw-   0        0        0      287 2024-05-07 09:19:11.000000 glglue-2.3.0/tests/test_py.py
+-rw-rw-rw-   0        0        0      221 2024-05-07 09:19:11.000000 glglue-2.3.0/tests/test_utils.py
```

### Comparing `glglue-2.1.0/.github/workflows/docusaurus.yml` & `glglue-2.3.0/.github/workflows/docusaurus.yml`

 * *Files identical despite different names*

### Comparing `glglue-2.1.0/.vscode/settings.json` & `glglue-2.3.0/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `glglue-2.1.0/.vscode/tasks.json` & `glglue-2.3.0/.vscode/tasks.json`

 * *Files identical despite different names*

### Comparing `glglue-2.1.0/LICENSE` & `glglue-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `glglue-2.1.0/PKG-INFO` & `glglue-2.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glglue
-Version: 2.1.0
+Version: 2.3.0
 Summary: The glue code which mediates between OpenGL and some GUI
 Author-email: ousttrue <ousttrue@gmail.com>
 Project-URL: HomePage, https://ousttrue.github.io/glglue/
 Project-URL: Repository, https://github.com/ousttrue/glglue/
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Multimedia :: Graphics :: 3D Modeling
```

### Comparing `glglue-2.1.0/README.md` & `glglue-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `glglue-2.1.0/docs/README.md` & `glglue-2.3.0/docs/README.md`

 * *Files identical despite different names*

### Comparing `glglue-2.1.0/docs/blog/2019-05-29-long-blog-post.md` & `glglue-2.3.0/docs/blog/2019-05-29-long-blog-post.md`

 * *Files identical despite different names*

### Comparing `glglue-2.1.0/docs/blog/2021-08-26-welcome/docusaurus-plushie-banner.jpeg` & `glglue-2.3.0/docs/blog/2021-08-26-welcome/docusaurus-plushie-banner.jpeg`

 * *Files identical despite different names*

### Comparing `glglue-2.1.0/docs/blog/2021-08-26-welcome/index.md` & `glglue-2.3.0/docs/blog/2021-08-26-welcome/index.md`

 * *Files identical despite different names*

### Comparing `glglue-2.1.0/docs/docs/index.md` & `glglue-2.3.0/docs/docs/index.md`

 * *Files identical despite different names*

### Comparing `glglue-2.1.0/docs/docusaurus.config.ts` & `glglue-2.3.0/docs/docusaurus.config.ts`

 * *Files identical despite different names*

### Comparing `glglue-2.1.0/docs/package-lock.json` & `glglue-2.3.0/docs/package-lock.json`

 * *Files identical despite different names*

### Comparing `glglue-2.1.0/docs/package.json` & `glglue-2.3.0/docs/package.json`

 * *Files identical despite different names*

### Comparing `glglue-2.1.0/docs/sidebars.ts` & `glglue-2.3.0/docs/sidebars.ts`

 * *Files identical despite different names*

### Comparing `glglue-2.1.0/docs/src/components/HomepageFeatures/index.tsx` & `glglue-2.3.0/docs/src/components/HomepageFeatures/index.tsx`

 * *Files identical despite different names*

### Comparing `glglue-2.1.0/docs/src/css/custom.css` & `glglue-2.3.0/docs/src/css/custom.css`

 * *Files identical despite different names*

### Comparing `glglue-2.1.0/docs/src/pages/index.tsx` & `glglue-2.3.0/docs/src/pages/index.tsx`

 * *Files identical despite different names*

### Comparing `glglue-2.1.0/docs/static/img/docusaurus-social-card.jpg` & `glglue-2.3.0/docs/static/img/docusaurus-social-card.jpg`

 * *Files identical despite different names*

### Comparing `glglue-2.1.0/docs/static/img/docusaurus.png` & `glglue-2.3.0/docs/static/img/docusaurus.png`

 * *Files identical despite different names*

### Comparing `glglue-2.1.0/docs/static/img/favicon.ico` & `glglue-2.3.0/docs/static/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `glglue-2.1.0/docs/static/img/logo.svg` & `glglue-2.3.0/docs/static/img/logo.svg`

 * *Files identical despite different names*

### Comparing `glglue-2.1.0/docs/static/img/undraw_docusaurus_mountain.svg` & `glglue-2.3.0/docs/static/img/undraw_docusaurus_mountain.svg`

 * *Files identical despite different names*

### Comparing `glglue-2.1.0/docs/static/img/undraw_docusaurus_react.svg` & `glglue-2.3.0/docs/static/img/undraw_docusaurus_react.svg`

 * *Files identical despite different names*

### Comparing `glglue-2.1.0/docs/static/img/undraw_docusaurus_tree.svg` & `glglue-2.3.0/docs/static/img/undraw_docusaurus_tree.svg`

 * *Files identical despite different names*

### Comparing `glglue-2.1.0/examples/freeglut_sample.py` & `glglue-2.3.0/examples/basic/freeglut_sample.py`

 * *Files identical despite different names*

### Comparing `glglue-2.1.0/examples/gtk3_sample.py` & `glglue-2.3.0/examples/basic/gtk3_sample.py`

 * *Files identical despite different names*

### Comparing `glglue-2.1.0/examples/gtk4_sample.py` & `glglue-2.3.0/examples/basic/gtk4_sample.py`

 * *Files identical despite different names*

### Comparing `glglue-2.1.0/examples/pyside6_sample.py` & `glglue-2.3.0/examples/basic/pyside6_sample.py`

 * *Files identical despite different names*

### Comparing `glglue-2.1.0/examples/wgl_sample.py` & `glglue-2.3.0/examples/basic/wgl_sample.py`

 * *Files identical despite different names*

### Comparing `glglue-2.1.0/pyproject.toml` & `glglue-2.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `glglue-2.1.0/src/glglue/assets/Utah_teapot_(solid).stl` & `glglue-2.3.0/src/glglue/assets/Utah_teapot_(solid).stl`

 * *Files identical despite different names*

### Comparing `glglue-2.1.0/src/glglue/camera/camera.py` & `glglue-2.3.0/src/glglue/camera/camera.py`

 * *Files identical despite different names*

### Comparing `glglue-2.1.0/src/glglue/camera/mouse_camera.py` & `glglue-2.3.0/src/glglue/camera/mouse_camera.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 from .camera import Camera, ArcBall, ScreenShift
 from .mouse_event import MouseEvent
 from glglue.frame_input import FrameInput
 
 
 class MouseCamera:
-    def __init__(self, *, mouse_event=None, distance: float = 5, y: float = 0) -> None:
+    def __init__(
+        self,
+        *,
+        mouse_event: MouseEvent | None = None,
+        distance: float = 5,
+        y: float = 0,
+    ) -> None:
         self.camera = Camera(distance=distance, y=y)
         self.mouse_event = mouse_event if mouse_event else MouseEvent()
         self.mouse_event.bind_right_drag(
             ArcBall(self.camera.view, self.camera.projection)
         )
         self.middle_drag = ScreenShift(self.camera.view, self.camera.projection)
         self.mouse_event.bind_middle_drag(self.middle_drag)
```

### Comparing `glglue-2.1.0/src/glglue/camera/mouse_event.py` & `glglue-2.3.0/src/glglue/camera/mouse_event.py`

 * *Files identical despite different names*

### Comparing `glglue-2.1.0/src/glglue/drawable/cube.py` & `glglue-2.3.0/src/glglue/drawable/cube.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from typing import Tuple, NamedTuple, List
+from typing import NamedTuple
 import glm
 from glglue import glo
-from .vertex_buffer import MeshBuilder
+from .mesh_builder import MeshBuilder
 from .drawable import Drawable
 
 """
 OpenGL default is ccw
 
 +->
 |
@@ -31,38 +31,38 @@
     glm.vec3(S, S, -S),
     glm.vec3(S, S, S),
     glm.vec3(-S, S, S),
 ]
 
 
 class Face(NamedTuple):
-    indices: Tuple[int, int, int, int]
-    color: Tuple[float, float, float]
+    indices: tuple[int, int, int, int]
+    color: tuple[float, float, float]
 
 
 # CCW
 QUADS = [
     Face((7, 3, 2, 6), (0.5, 0.5, 1)),  # front
     Face((5, 1, 0, 4), (0.5, 0.5, 1)),  # back
     Face((6, 2, 1, 5), (1, 0.5, 0.5)),  # right
     Face((4, 0, 3, 7), (1, 0.5, 0.5)),  # left
     Face((4, 7, 6, 5), (0.5, 1, 0.5)),  # top
     Face((0, 1, 2, 3), (0.5, 1, 0.5)),  # bottom
 ]
 
 
-def create(shader: glo.Shader, props: List[glo.UniformUpdater]) -> Drawable:
+def create(shader: glo.Shader, props: list[glo.UniformUpdater]) -> Drawable:
     builder = MeshBuilder()
     for (i0, i1, i2, i3), rgb in QUADS:
         builder.push_quad(
             VERTICES[i0], VERTICES[i1], VERTICES[i2], VERTICES[i3], glm.vec3(*rgb)
         )
     vertices = builder.create_vertices()
 
     vbo = glo.Vbo()
-    vbo.set_vertices(vertices)
+    vbo.set_vertices(memoryview(vertices))
 
     vao = glo.Vao(vbo, glo.VertexLayout.create_list(shader.program))
 
     drawable = Drawable(vao)
     drawable.push_submesh(shader, len(vertices), props)
     return drawable
```

### Comparing `glglue-2.1.0/src/glglue/drawable/drawable.py` & `glglue-2.3.0/src/glglue/drawable/drawable.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,53 +1,49 @@
-from typing import List, Optional
-from OpenGL import GL
+from OpenGL import GL  # type: ignore
 from glglue.glo.shader import Shader, UniformUpdater
 from glglue.glo.vao import Vao
 
 
-def empty():
-    return []
-
-
 class Submesh:
     def __init__(
         self,
-        topology,
+        topology: int,
         *,
-        draw_count=0,
-        shader: Optional[Shader] = None,
-        props: List[UniformUpdater] = empty()
+        draw_count: int = 0,
+        shader: Shader | None = None,
+        props: list[UniformUpdater] | None = None,
     ) -> None:
         self.topology = topology
         self.draw_count = draw_count
-        assert (not shader) or isinstance(shader, Shader)
         self.shader = shader
-        self.properties = props
+        self.properties = props if props else []
 
 
 class Drawable:
     def __init__(self, vao: Vao) -> None:
         self.vao = vao
-        self.submeshes: List[Submesh] = []
+        self.submeshes: list[Submesh] = []
 
     def push_submesh(
         self,
         shader: Shader,
         draw_count: int,
-        properties: list,
+        properties: list[UniformUpdater],
         *,
-        topology=GL.GL_TRIANGLES
+        topology: int = GL.GL_TRIANGLES,  # type: ignore
     ):
         assert isinstance(shader, Shader)
         self.submeshes.append(
             Submesh(topology, shader=shader, draw_count=draw_count, props=properties)
         )
 
     def draw(self):
         self.vao.bind()
+        offset = 0
         for submesh in self.submeshes:
             if submesh.shader:
                 with submesh.shader:
                     for prop in submesh.properties:
                         prop()
-                    self.vao.draw(submesh.draw_count, topology=submesh.topology)
+                    self.vao.draw(submesh.draw_count, offset=offset)
+            offset += submesh.draw_count
         self.vao.unbind()
```

### Comparing `glglue-2.1.0/src/glglue/drawable/teapot.py` & `glglue-2.3.0/src/glglue/drawable/teapot.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import ctypes
 import struct
 import pkgutil
 from glglue import glo
-from .vertex_buffer import Float3, Vertex
+from .mesh_builder import Float3, Vertex
 from .drawable import Drawable
 
+
 WHITE = Float3(1, 1, 1)
 
 
 class StlTriangle(ctypes.Structure):
     _pack_ = 1
     _fields_ = [
         ("normal", Float3),
@@ -39,25 +40,25 @@
         return struct.unpack("I", data)[0]
 
     def read_float32(self) -> float:
         data = self.read(4)
         return struct.unpack("f", data)[0]
 
 
-def load_teapot() -> ctypes.Array:
+def load_teapot() -> ctypes.Array[Vertex]:
     # https://en.wikipedia.org/wiki/Utah_teapot#/media/File:Utah_teapot_(solid).stl
     data = pkgutil.get_data("glglue", "assets/Utah_teapot_(solid).stl")
     assert data
 
     # https://en.wikipedia.org/wiki/STL_%28file_format%29
     r = BinaryReader(data)
 
     # UINT8[80]    – Header                 -     80 bytes
     # UINT32       – Number of triangles    -      4 bytes
-    header = r.read(80)
+    _header = r.read(80)
     triangle_count = r.read_uint32()
 
     triangles_type = StlTriangle * triangle_count
     data = r.read(ctypes.sizeof(triangles_type))
     triangles = triangles_type.from_buffer_copy(data)
 
     vertices = (Vertex * (triangle_count * 3))()
@@ -85,18 +86,18 @@
 
     for i, t in enumerate(triangles):
         push_triangle(i * 3, t, 0.1)
 
     return vertices
 
 
-def create(shader, props):
+def create(shader: glo.Shader, props: list[glo.UniformUpdater]) -> Drawable:
     vertices = load_teapot()
 
     vbo = glo.Vbo()
-    vbo.set_vertices(vertices)
+    vbo.set_vertices(memoryview(vertices))
 
     vao = glo.Vao(vbo, glo.VertexLayout.create_list(shader.program))
 
     drawable = Drawable(vao)
     drawable.push_submesh(shader, len(vertices), props)
     return drawable
```

### Comparing `glglue-2.1.0/src/glglue/drawable/vertex_buffer.py` & `glglue-2.3.0/src/glglue/drawable/mesh_builder.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,46 +1,65 @@
 from typing import List
 import ctypes
 import glm
 
 
 class Float3(ctypes.Structure):
     _fields_ = [
-        ('x', ctypes.c_float),
-        ('y', ctypes.c_float),
-        ('z', ctypes.c_float),
+        ("x", ctypes.c_float),
+        ("y", ctypes.c_float),
+        ("z", ctypes.c_float),
     ]
 
     def __iter__(self):
         yield self.x
         yield self.y
         yield self.z
 
 
 class Vertex(ctypes.Structure):
     _fields_ = [
-        ('position', Float3),
-        ('normal', Float3),
-        ('color', Float3),
+        ("position", Float3),
+        ("normal", Float3),
+        ("color", Float3),
     ]
 
 
 class MeshBuilder:
     def __init__(self) -> None:
         self.vertices: List[Vertex] = []
 
-    def push_triangle(self, p0: glm.vec3, p1: glm.vec3, p2: glm.vec3, n: glm.vec3, color: glm.vec3):
+    def push_triangle(
+        self, p0: glm.vec3, p1: glm.vec3, p2: glm.vec3, n: glm.vec3, color: glm.vec3
+    ):
         self.vertices.append(
-            Vertex(Float3(p0.x, p0.y, p0.z), Float3(n.x, n.y, n.z), Float3(color.x, color.y, color.z)))
+            Vertex(
+                Float3(p0.x, p0.y, p0.z),
+                Float3(n.x, n.y, n.z),
+                Float3(color.x, color.y, color.z),
+            )
+        )
         self.vertices.append(
-            Vertex(Float3(p1.x, p1.y, p1.z), Float3(n.x, n.y, n.z), Float3(color.x, color.y, color.z)))
+            Vertex(
+                Float3(p1.x, p1.y, p1.z),
+                Float3(n.x, n.y, n.z),
+                Float3(color.x, color.y, color.z),
+            )
+        )
         self.vertices.append(
-            Vertex(Float3(p2.x, p2.y, p2.z), Float3(n.x, n.y, n.z), Float3(color.x, color.y, color.z)))
-
-    def push_quad(self, p0, p1, p2, p3, color):
-        n = glm.cross(glm.normalize(p0-p1), glm.normalize(p2-p1)) # type: ignore
+            Vertex(
+                Float3(p2.x, p2.y, p2.z),
+                Float3(n.x, n.y, n.z),
+                Float3(color.x, color.y, color.z),
+            )
+        )
+
+    def push_quad(
+        self, p0: glm.vec3, p1: glm.vec3, p2: glm.vec3, p3: glm.vec3, color: glm.vec3
+    ):
+        n = glm.cross(glm.normalize(p0 - p1), glm.normalize(p2 - p1))  # type: ignore
         self.push_triangle(p0, p1, p2, n, color)
         self.push_triangle(p2, p3, p0, n, color)
 
-    def create_vertices(self) -> ctypes.Array:
+    def create_vertices(self) -> ctypes.Array[Vertex]:
         vertices = (Vertex * len(self.vertices))(*self.vertices)
         return vertices
```

### Comparing `glglue-2.1.0/src/glglue/glfw.py` & `glglue-2.3.0/src/glglue/glfw.py`

 * *Files identical despite different names*

### Comparing `glglue-2.1.0/src/glglue/glo/fbo.py` & `glglue-2.3.0/src/glglue/glo/fbo.py`

 * *Files identical despite different names*

### Comparing `glglue-2.1.0/src/glglue/glo/shader.py` & `glglue-2.3.0/src/glglue/glo/shader.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,198 +1,213 @@
-from typing import NamedTuple, Optional, Union, Tuple, cast, List, Callable, TypeAlias
+from typing import (
+    NamedTuple,
+    Optional,
+    Union,
+    Tuple,
+    cast,
+    List,
+    Callable,
+    TypeAlias,
+    Protocol,
+)
 from OpenGL import GL
 import glm
 import logging
+from ..camera import Camera
 
 LOGGER = logging.getLogger(__name__)
 
 
-def GetGLErrorStr(err):
+def GetGLErrorStr(err: int):
     match (err):
-        case GL.GL_NO_ERROR:
+        case GL.GL_NO_ERROR:  # type: ignore
             return "No error"
-        case GL.GL_INVALID_ENUM:
+        case GL.GL_INVALID_ENUM:  # type: ignore
             return "Invalid enum"
-        case GL.GL_INVALID_VALUE:
+        case GL.GL_INVALID_VALUE:  # type: ignore
             return "Invalid value"
-        case GL.GL_INVALID_OPERATION:
+        case GL.GL_INVALID_OPERATION:  # type: ignore
             return "Invalid operation"
-        case GL.GL_STACK_OVERFLOW:
+        case GL.GL_STACK_OVERFLOW:  # type: ignore
             return "Stack overflow"
-        case GL.GL_STACK_UNDERFLOW:
+        case GL.GL_STACK_UNDERFLOW:  # type: ignore
             return "Stack underflow"
-        case GL.GL_OUT_OF_MEMORY:
+        case GL.GL_OUT_OF_MEMORY:  # type: ignore
             return "Out of memory"
         case _:
             return "Unknown error"
 
 
 def CheckGLError():
     while True:
-        err = GL.glGetError()
-        if GL.GL_NO_ERROR == err:
+        err: int = GL.glGetError()  # type: ignore
+        if GL.GL_NO_ERROR == err:  # type: ignore
             break
         LOGGER.error(f"GL Error: {GetGLErrorStr(err)}")
 
 
 class ShaderCompile:
-    def __init__(self, shader_type):
-        """
-        GL.GL_VERTEX_SHADER
-        GL.GL_FRAGMENT_SHADER
-        """
-        self.shader = GL.glCreateShader(shader_type)
+    def __init__(self, shader_type: GL.GL_VERTEX_SHADER | GL.GL_FRAGMENT_SHADER):  # type: ignore
+        self.shader: int = GL.glCreateShader(shader_type)  # type: ignore
 
     def compile(self, src: Union[str, bytes]) -> Tuple[bool, str]:
         GL.glShaderSource(self.shader, src, None)
-        GL.glCompileShader(self.shader)
-        result = GL.glGetShaderiv(self.shader, GL.GL_COMPILE_STATUS)
-        if result == GL.GL_TRUE:
+        GL.glCompileShader(self.shader)  # type: ignore
+        result = GL.glGetShaderiv(self.shader, GL.GL_COMPILE_STATUS)  # type: ignore
+        if result == GL.GL_TRUE:  # type: ignore
             return True, ""
         # error message
         info = GL.glGetShaderInfoLog(self.shader)
         return False, info.decode("ascii")
 
     def __del__(self):
-        GL.glDeleteShader(self.shader)
+        GL.glDeleteShader(self.shader)  # type: ignore
 
 
 UniformUpdater: TypeAlias = Callable[[], None]
 
 
+class Node(Protocol):
+    world_matrix: glm.mat4
+
+
 class Shader:
     def __init__(self) -> None:
         self.program = cast(int, GL.glCreateProgram())
 
     def __del__(self):
-        GL.glDeleteProgram(self.program)
+        GL.glDeleteProgram(self.program)  # type: ignore
 
     def __enter__(self):
         self.use()
 
-    def __exit__(self, exc_type, exc_value, traceback):
+    def __exit__(self, exc_type, exc_value, traceback):  # type: ignore
         self.unuse()
         if exc_type:
             LOGGER.warning(f"{exc_type}: {exc_value}: {traceback}")
 
-    def link(self, vs, fs) -> Tuple[bool, str]:
-        GL.glAttachShader(self.program, vs)
-        GL.glAttachShader(self.program, fs)
-        GL.glLinkProgram(self.program)
-        error = GL.glGetProgramiv(self.program, GL.GL_LINK_STATUS)
-        if error == GL.GL_TRUE:
+    def link(self, vs: int, fs: int) -> Tuple[bool, str]:
+        GL.glAttachShader(self.program, vs)  # type: ignore
+        GL.glAttachShader(self.program, fs)  # type: ignore
+        GL.glLinkProgram(self.program)  # type: ignore
+        error = GL.glGetProgramiv(self.program, GL.GL_LINK_STATUS)  # type: ignore
+        if error == GL.GL_TRUE:  # type: ignore
             return True, ""
 
         # error message
         info = GL.glGetProgramInfoLog(self.program)
         return False, info.decode("ascii")
 
     @staticmethod
     def load(
         vs_src: Union[str, bytes], fs_src: Union[str, bytes]
     ) -> Union["Shader", str]:
-        vs = ShaderCompile(GL.GL_VERTEX_SHADER)
+        vs = ShaderCompile(GL.GL_VERTEX_SHADER)  # type: ignore
         success, info = vs.compile(vs_src)
         if not success:
             return "vs: " + info
-        fs = ShaderCompile(GL.GL_FRAGMENT_SHADER)
+        fs = ShaderCompile(GL.GL_FRAGMENT_SHADER)  # type: ignore
         success, info = fs.compile(fs_src)
         if not success:
             return "fs: " + info
         shader = Shader()
         success, info = shader.link(vs.shader, fs.shader)
         if not success:
             return "link: " + info
         return shader
 
     @staticmethod
     def load_from_pkg(pkg: str, name: str) -> Optional["Shader"]:
         import pkgutil
 
-        vs = pkgutil.get_data(pkg, f"{name}.vs")
+        vs = pkgutil.get_data(pkg, f"{name}.vert")
         assert vs
-        fs = pkgutil.get_data(pkg, f"{name}.fs")
+        fs = pkgutil.get_data(pkg, f"{name}.frag")
         assert fs
         match Shader.load(vs, fs):
             case Shader() as shader:
                 return shader
             case str() as info:
                 LOGGER.error(f"{pkg}#{name}: {info}")
-            case _:
-                raise RuntimeError()
 
-    def create_props(self, camera, node=None) -> List[UniformUpdater]:
-        from .. import glo
+    def create_props(
+        self, camera: Camera, node: Node | None = None
+    ) -> List[UniformUpdater]:
 
         props: List[Callable[[], None]] = []
 
-        model = UniformLocation.create(self.program, "uModel")
+        model = UniformLocation.create(self.program, "u_model")
         if model:
             if node:
 
                 def update_model():
-                    model.set_mat4(glm.value_ptr(node.world_matrix))
+                    model.set_mat4(node.world_matrix)
 
             else:
                 identity = glm.mat4(1)
 
                 def update_model():
-                    model.set_mat4(glm.value_ptr(identity))
+                    model.set_mat4(identity)
 
             props.append(update_model)
 
-        view = UniformLocation.create(self.program, "uView")
+        view = UniformLocation.create(self.program, "u_view")
         if view:
 
             def update_view():
-                view.set_mat4(glm.value_ptr(camera.view.matrix))
+                view.set_mat4(camera.view.matrix)
 
             props.append(update_view)
 
-        projection = UniformLocation.create(self.program, "uProjection")
+        projection = UniformLocation.create(self.program, "u_projection")
         if projection:
 
             def update_projection():
-                projection.set_mat4(glm.value_ptr(camera.projection.matrix))
+                projection.set_mat4(camera.projection.matrix)
 
             props.append(update_projection)
 
         return props
 
-    def use(self):
-        GL.glUseProgram(self.program)
+    def use(self) -> None:
+        GL.glUseProgram(self.program)  # type: ignore
 
-    def unuse(self):
-        GL.glUseProgram(0)
+    def unuse(self) -> None:
+        GL.glUseProgram(0)  # type: ignore
 
 
 class UniformLocation(NamedTuple):
     name: str
     location: int
 
     @staticmethod
-    def create(program, name: str) -> "UniformLocation":
-        location = GL.glGetUniformLocation(program, name)
+    def create(program: int, name: str) -> "UniformLocation":
+        location: int = GL.glGetUniformLocation(program, name)
         if location == -1:
             LOGGER.warn(f"{name}: -1")
         return UniformLocation(name, location)
 
     def set_int(self, value: int):
-        GL.glUniform1i(self.location, value)
+        GL.glUniform1i(self.location, value)  # type: ignore
 
-    def set_float2(self, value):
+    def set_float2(self, value: tuple[float, float]):
         GL.glUniform2fv(self.location, 1, value)
 
-    def set_mat4(self, value, transpose: bool = False, count=1):
+    def set_mat4(
+        self,
+        value: glm.mat4,
+        transpose: bool = False,
+        count: int = 1,
+    ):
         GL.glUniformMatrix4fv(
-            self.location, count, GL.GL_TRUE if transpose else GL.GL_FALSE, value
+            self.location, count, GL.GL_TRUE if transpose else GL.GL_FALSE, glm.value_ptr(value)  # type: ignore
         )
 
 
 class UniformBlockIndex(NamedTuple):
     name: str
-    index: int
+    block_index: int
 
     @staticmethod
-    def create(program, name: str) -> "UniformBlockIndex":
-        index = GL.glGetUniformBlockIndex(program, name)
-        return UniformBlockIndex(name, index)
+    def create(program: int, name: str) -> "UniformBlockIndex":
+        block_index = cast(int, GL.glGetUniformBlockIndex(program, name))  # type: ignore
+        return UniformBlockIndex(name, block_index)
```

### Comparing `glglue-2.1.0/src/glglue/glo/texture.py` & `glglue-2.3.0/src/glglue/glo/texture.py`

 * *Files identical despite different names*

### Comparing `glglue-2.1.0/src/glglue/glo/vbo.py` & `glglue-2.3.0/src/glglue/glo/vbo.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,75 +3,104 @@
 import ctypes
 
 LOGGER = logging.getLogger(__name__)
 
 
 class Vbo:
     def __init__(self):
-        self.vbo = GL.glGenBuffers(1)
+        self.vbo: int = GL.glGenBuffers(1)
 
-    def __del__(self):
+    def __del__(self) -> None:
         LOGGER.debug(f"delete vbo: {self.vbo}")
         GL.glDeleteBuffers(1, [self.vbo])
 
-    def bind(self):
-        GL.glBindBuffer(GL.GL_ARRAY_BUFFER, self.vbo)
+    def bind(self) -> None:
+        GL.glBindBuffer(GL.GL_ARRAY_BUFFER, self.vbo)  # type: ignore
 
-    def unbind(self):
-        GL.glBindBuffer(GL.GL_ARRAY_BUFFER, 0)
+    def unbind(self) -> None:
+        GL.glBindBuffer(GL.GL_ARRAY_BUFFER, 0)  # type: ignore
 
-    def set_vertices(self, vertices, *, is_dynamic: bool = False):
+    def set_vertices(self, vertices: memoryview, *, is_dynamic: bool = False) -> None:
+        data = vertices.tobytes()
         self.bind()
-        GL.glBufferData(
-            GL.GL_ARRAY_BUFFER,
-            ctypes.sizeof(vertices),
-            vertices,
-            GL.GL_DYNAMIC_DRAW if is_dynamic else GL.GL_STATIC_DRAW,
+        GL.glBufferData(  # type: ignore
+            GL.GL_ARRAY_BUFFER,  # type: ignore
+            len(data),
+            data,
+            GL.GL_DYNAMIC_DRAW if is_dynamic else GL.GL_STATIC_DRAW,  # type: ignore
         )
         self.unbind()
 
-    def update(self, vertices, offset=0) -> None:
+    def update(self, vertices: memoryview, offset: int = 0) -> None:
+        data = vertices.tobytes()
         self.bind()
-        GL.glBufferSubData(
-            GL.GL_ARRAY_BUFFER, offset, ctypes.sizeof(vertices), vertices
+        GL.glBufferSubData(  # type: ignore
+            GL.GL_ARRAY_BUFFER, offset, len(data), data  # type: ignore
         )
         self.unbind()
 
 
 class Ibo:
     def __init__(self):
-        self.vbo = GL.glGenBuffers(1)
+        self.vbo: int = GL.glGenBuffers(1)
         self.format = 0
 
-    def __del__(self):
+    def __del__(self) -> None:
         LOGGER.debug(f"delete vbo: {self.vbo}")
         GL.glDeleteBuffers(1, [self.vbo])
 
-    def bind(self):
-        GL.glBindBuffer(GL.GL_ELEMENT_ARRAY_BUFFER, self.vbo)
+    def bind(self) -> None:
+        GL.glBindBuffer(GL.GL_ELEMENT_ARRAY_BUFFER, self.vbo)  # type: ignore
 
-    def unbind(self):
-        GL.glBindBuffer(GL.GL_ELEMENT_ARRAY_BUFFER, 0)
+    def unbind(self) -> None:
+        GL.glBindBuffer(GL.GL_ELEMENT_ARRAY_BUFFER, 0)  # type: ignore
 
-    def set_indices(self, indices: ctypes.Array, *, is_dynamic: bool = False):
-        match indices._type_:
-            case ctypes.c_ushort:
-                self.format = GL.GL_UNSIGNED_SHORT
-            case ctypes.c_uint:
-                self.format = GL.GL_UNSIGNED_INT
+    def set_bytes(
+        self,
+        indices: bytes,
+        stride: int,
+        *,
+        is_dynamic: bool = False,
+    ):
+        match stride:
+            case 2:
+                self.format = GL.GL_UNSIGNED_SHORT  # type: ignore
+            case 4:
+                self.format = GL.GL_UNSIGNED_INT  # type: ignore
             case _:
                 raise NotImplementedError()
         self.bind()
-        GL.glBufferData(
-            GL.GL_ELEMENT_ARRAY_BUFFER,
-            ctypes.sizeof(indices),
+        GL.glBufferData(  # type: ignore
+            GL.GL_ELEMENT_ARRAY_BUFFER,  # type: ignore
+            len(indices),  # bytesize
             indices,
-            GL.GL_DYNAMIC_DRAW if is_dynamic else GL.GL_STATIC_DRAW,
+            GL.GL_DYNAMIC_DRAW if is_dynamic else GL.GL_STATIC_DRAW,  # type: ignore
         )
         self.unbind()
 
-    def update(self, indices, offset=0) -> None:
+    def set_indices(
+        self,
+        indices: ctypes.Array[ctypes.c_ushort] | ctypes.Array[ctypes.c_uint],
+        *,
+        is_dynamic: bool = False,
+    ):
+        match indices._type_:
+            case ctypes.c_ushort:
+                self.set_bytes(bytes(indices), 2, is_dynamic=is_dynamic)
+            case ctypes.c_uint:
+                self.set_bytes(bytes(indices), 4, is_dynamic=is_dynamic)
+            case _:
+                raise NotImplementedError()
+
+    def update(
+        self,
+        indices: ctypes.Array[ctypes.c_ushort] | ctypes.Array[ctypes.c_uint],
+        offset: int = 0,
+    ) -> None:
         self.bind()
-        GL.glBufferSubData(
-            GL.GL_ELEMENT_ARRAY_BUFFER, offset, ctypes.sizeof(indices), indices
+        GL.glBufferSubData(  # type: ignore
+            GL.GL_ELEMENT_ARRAY_BUFFER,  # type: ignore
+            offset,
+            ctypes.sizeof(indices),  # bytesize
+            indices,  # type: ignore
         )
         self.unbind()
```

### Comparing `glglue-2.1.0/src/glglue/glo/vertex_layout.py` & `glglue-2.3.0/src/glglue/glo/vertex_layout.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from typing import NamedTuple, Iterable, List
+from typing import NamedTuple, cast, Any
 from OpenGL import GL
 import logging
 
 LOGGER = logging.getLogger(__name__)
 
 
 class AttributeLocation(NamedTuple):
     name: str
     location: int
 
     @staticmethod
-    def create(program, name: str) -> "AttributeLocation":
+    def create(program: int, name: str) -> "AttributeLocation":
         location = GL.glGetAttribLocation(program, name)
         assert location != -1
         return AttributeLocation(name, location)
 
 
-type_map = {
+type_map: dict[int, tuple[int, int]] = {
     GL.GL_FLOAT: (GL.GL_FLOAT, 1),
     GL.GL_FLOAT_VEC2: (GL.GL_FLOAT, 2),
     GL.GL_FLOAT_VEC3: (GL.GL_FLOAT, 3),
     GL.GL_FLOAT_VEC4: (GL.GL_FLOAT, 4),
     GL.GL_FLOAT_MAT2: (GL.GL_FLOAT, 4),
     GL.GL_FLOAT_MAT3: (GL.GL_FLOAT, 9),
     GL.GL_FLOAT_MAT4: (GL.GL_FLOAT, 16),
@@ -50,23 +50,23 @@
     GL.GL_DOUBLE_MAT3x2: (GL.GL_DOUBLE, 6),
     GL.GL_DOUBLE_MAT3x4: (GL.GL_DOUBLE, 12),
     GL.GL_DOUBLE_MAT4x2: (GL.GL_DOUBLE, 8),
     GL.GL_DOUBLE_MAT4x3: (GL.GL_DOUBLE, 12),
 }
 
 
-def byte_size(t, n):
+def byte_size(t: int, n: int):
     match t:
-        case GL.GL_FLOAT:
+        case GL.GL_FLOAT:  # type: ignore
             return 4 * n
         case _:
             raise NotImplemented()
 
 
-def to_str(src) -> str:
+def to_str(src: str | bytes | Any) -> str:
     match src:
         case str():
             return src
         case bytes():
             return src.decode("ascii")
         case _:
             data = bytes(src)
@@ -79,19 +79,19 @@
 class VertexLayout(NamedTuple):
     attribute: AttributeLocation
     item_count: int  # maybe float1, 2, 3, 4 and 16
     stride: int
     byte_offset: int
 
     @staticmethod
-    def create_list(program) -> List["VertexLayout"]:
-        count = GL.glGetProgramiv(program, GL.GL_ACTIVE_ATTRIBUTES)
+    def create_list(program: int) -> list["VertexLayout"]:
+        count = cast(int, GL.glGetProgramiv(program, GL.GL_ACTIVE_ATTRIBUTES))  # type: ignore
         LOGGER.debug(f"Active Attributes: {count}")
 
-        layouts: List[VertexLayout] = []
+        layouts: list[VertexLayout] = []
         stride = 0
         for i in range(count):
             name, size, type_ = GL.glGetActiveAttrib(program, i)
             # https://www.khronos.org/registry/OpenGL-Refpages/gl4/html/glGetActiveAttrib.xhtml
             attribute = AttributeLocation.create(program, to_str(name))
             match type_map.get(type_):
                 case (t, n):
@@ -99,15 +99,15 @@
                     layouts.append(VertexLayout(attribute, n, 0, size))
                     stride += size
                 case _:
                     raise RuntimeError()
         # not same with location order
         layouts.sort(key=lambda l: l.attribute.location)
 
-        result = []
+        result: list[VertexLayout] = []
         offset = 0
         for layout in layouts:
             result.append(
                 VertexLayout(layout.attribute, layout.item_count, stride, offset)
             )
             offset += layout.byte_offset
         return result
```

### Comparing `glglue-2.1.0/src/glglue/glut.py` & `glglue-2.3.0/src/glglue/glut.py`

 * *Files identical despite different names*

### Comparing `glglue-2.1.0/src/glglue/gtk3.py` & `glglue-2.3.0/src/glglue/gtk3.py`

 * *Files identical despite different names*

### Comparing `glglue-2.1.0/src/glglue/gtk4.py` & `glglue-2.3.0/src/glglue/gtk4.py`

 * *Files identical despite different names*

### Comparing `glglue-2.1.0/src/glglue/pysdl2.py` & `glglue-2.3.0/src/glglue/pysdl2.py`

 * *Files identical despite different names*

### Comparing `glglue-2.1.0/src/glglue/qgl4.py` & `glglue-2.3.0/src/glglue/qgl4.py`

 * *Files identical despite different names*

### Comparing `glglue-2.1.0/src/glglue/qgl5.py` & `glglue-2.3.0/src/glglue/qgl5.py`

 * *Files identical despite different names*

### Comparing `glglue-2.1.0/src/glglue/sdl.py` & `glglue-2.3.0/src/glglue/sdl.py`

 * *Files identical despite different names*

### Comparing `glglue-2.1.0/src/glglue/togl.py` & `glglue-2.3.0/src/glglue/togl.py`

 * *Files identical despite different names*

### Comparing `glglue-2.1.0/src/glglue/util.py` & `glglue-2.3.0/src/glglue/util.py`

 * *Files identical despite different names*

### Comparing `glglue-2.1.0/src/glglue/wgl.py` & `glglue-2.3.0/src/glglue/wgl.py`

 * *Files identical despite different names*

### Comparing `glglue-2.1.0/src/glglue/win32con.py` & `glglue-2.3.0/src/glglue/win32con.py`

 * *Files identical despite different names*

### Comparing `glglue-2.1.0/src/glglue/windowconfig.py` & `glglue-2.3.0/src/glglue/windowconfig.py`

 * *Files identical despite different names*

### Comparing `glglue-2.1.0/src/glglue/wxglcanvas.py` & `glglue-2.3.0/src/glglue/wxglcanvas.py`

 * *Files identical despite different names*

### Comparing `glglue-2.1.0/src/glglue.egg-info/PKG-INFO` & `glglue-2.3.0/src/glglue.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glglue
-Version: 2.1.0
+Version: 2.3.0
 Summary: The glue code which mediates between OpenGL and some GUI
 Author-email: ousttrue <ousttrue@gmail.com>
 Project-URL: HomePage, https://ousttrue.github.io/glglue/
 Project-URL: Repository, https://github.com/ousttrue/glglue/
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Multimedia :: Graphics :: 3D Modeling
```

### Comparing `glglue-2.1.0/src/glglue.egg-info/SOURCES.txt` & `glglue-2.3.0/src/glglue.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 .clang-format
 .gitignore
 .remarkrc
 LICENSE
 README.md
 pyproject.toml
 .github/workflows/docusaurus.yml
-.github/workflows/pypi.yml
 .vscode/launch.json
 .vscode/settings.json
 .vscode/tasks.json
 docs/.gitignore
 docs/README.md
 docs/babel.config.js
 docs/docusaurus.config.ts
@@ -34,23 +33,23 @@
 docs/static/img/docusaurus-social-card.jpg
 docs/static/img/docusaurus.png
 docs/static/img/favicon.ico
 docs/static/img/logo.svg
 docs/static/img/undraw_docusaurus_mountain.svg
 docs/static/img/undraw_docusaurus_react.svg
 docs/static/img/undraw_docusaurus_tree.svg
-examples/freeglut_sample.py
-examples/glfw_sample.py
-examples/gtk3_sample.py
-examples/gtk4_sample.py
-examples/pysdl2_sample.py
-examples/pyside6_sample.py
-examples/wgl_sample.py
+examples/basic/freeglut_sample.py
+examples/basic/glfw_sample.py
+examples/basic/gtk3_sample.py
+examples/basic/gtk4_sample.py
+examples/basic/pysdl2_sample.py
+examples/basic/pyside6_sample.py
+examples/basic/wgl_sample.py
+examples/gui/pyside6_gui.py
 src/glglue/__init__.py
-src/glglue/__main__.py
 src/glglue/_version.py
 src/glglue/frame_input.py
 src/glglue/glfw.py
 src/glglue/glut.py
 src/glglue/gtk3.py
 src/glglue/gtk4.py
 src/glglue/pysdl2.py
@@ -66,30 +65,34 @@
 src/glglue/wxglcanvas.py
 src/glglue.egg-info/PKG-INFO
 src/glglue.egg-info/SOURCES.txt
 src/glglue.egg-info/dependency_links.txt
 src/glglue.egg-info/requires.txt
 src/glglue.egg-info/top_level.txt
 src/glglue/assets/Utah_teapot_(solid).stl
-src/glglue/assets/mesh.fs
-src/glglue/assets/mesh.vs
+src/glglue/assets/line.frag
+src/glglue/assets/line.vert
+src/glglue/assets/mesh.frag
+src/glglue/assets/mesh.vert
 src/glglue/camera/__init__.py
 src/glglue/camera/camera.py
 src/glglue/camera/mouse_camera.py
 src/glglue/camera/mouse_event.py
 src/glglue/drawable/__init__.py
+src/glglue/drawable/axes.py
 src/glglue/drawable/cube.py
 src/glglue/drawable/drawable.py
+src/glglue/drawable/grid.py
+src/glglue/drawable/line_builder.py
+src/glglue/drawable/mesh_builder.py
 src/glglue/drawable/teapot.py
-src/glglue/drawable/vertex_buffer.py
 src/glglue/glo/__init__.py
 src/glglue/glo/fbo.py
 src/glglue/glo/shader.py
 src/glglue/glo/texture.py
 src/glglue/glo/vao.py
 src/glglue/glo/vbo.py
 src/glglue/glo/vertex_layout.py
-src/glglue/scene/node.py
 src/glglue/scene/sample.py
 tests/test_numpy.py
 tests/test_py.py
 tests/test_utils.py
```

### Comparing `glglue-2.1.0/tests/test_numpy.py` & `glglue-2.3.0/tests/test_numpy.py`

 * *Files identical despite different names*

