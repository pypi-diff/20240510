# Comparing `tmp/youqu-2.5.4.tar.gz` & `tmp/youqu-2.5.5.tar.gz`

## Comparing `youqu-2.5.4.tar` & `youqu-2.5.5.tar`

### file list

```diff
@@ -1,228 +1,228 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/CURRENT
--rw-r--r--   0        0        0    41974 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/conftest.py
--rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/env.sh
--rw-r--r--   0        0        0     3703 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/manage.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/pytest.ini
--rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/ruff.toml
--rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/startproject.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/apps/__init__.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/setting/__init__.py
--rw-r--r--   0        0        0     4354 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/setting/_env_base.sh
--rwxr-xr-x   0        0        0     3272 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/setting/env_dev.sh
--rw-r--r--   0        0        0     5447 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/setting/env_vir.sh
--rw-r--r--   0        0        0    11023 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/setting/globalconfig.ini
--rw-r--r--   0        0        0    11361 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/setting/globalconfig.py
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/setting/playbook.toml
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/setting/pmsmark.ini
--rw-r--r--   0        0        0    20451 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/setting/pylintrc.cfg
--rw-r--r--   0        0        0     2365 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/setting/skipif.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/setting/sleepx.ini
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/setting/subcmd.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/setting/template/ci.json
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/setting/template/language.ini
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/setting/template/app_template/${app_name}_assert.py-tpl
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/setting/template/app_template/.gitignore-tpl
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/setting/template/app_template/__init__.py-tpl
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/setting/template/app_template/config.ini-tpl
--rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/setting/template/app_template/config.py-tpl
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/setting/template/app_template/conftest.py-tpl
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/setting/template/app_template/control-tpl
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/setting/template/app_template/mycase.csv-tpl
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/setting/template/app_template/case/__init__.py-tpl
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/setting/template/app_template/case/base_case.py-tpl
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/setting/template/app_template/case/test_mycase_001.py-tpl
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/setting/template/app_template/case/test_mycase_002.py-tpl
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/setting/template/app_template/case/assert_res/readme
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/setting/template/app_template/widget/${app_name}_widget.py-tpl
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/setting/template/app_template/widget/__init__.py-tpl
--rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/setting/template/app_template/widget/base_widget.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/setting/template/app_template/widget/other.ini-tpl
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/setting/template/app_template/widget/other_widget.py-tpl
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/setting/template/app_template/widget/ui.ini-tpl
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/setting/template/app_template/widget/case_res/readme
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/setting/template/app_template/widget/pic_res/readme
--rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/__init__.py
--rw-r--r--   0        0        0    18200 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/assert_common.py
--rw-r--r--   0        0        0    26398 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/button_center.py
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/calculate.py
--rw-r--r--   0        0        0     7990 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/cmdctl.py
--rw-r--r--   0        0        0     6975 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/csvctl.py
--rw-r--r--   0        0        0     5006 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/custom_exception.py
--rw-r--r--   0        0        0     2921 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/dbus_utils.py
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/desktop.py
--rw-r--r--   0        0        0     7644 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/dogtail_utils.py
--rw-r--r--   0        0        0    10856 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/filectl.py
--rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/filter_image.py
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/image_utils.py
--rw-r--r--   0        0        0    14377 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/mouse_key.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/ocr_utils.py
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/pinyin.py
--rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/read_csv.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/read_toml.py
--rw-r--r--   0        0        0     3672 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/recording_screen.py
--rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/requestx.py
--rw-r--r--   0        0        0    15481 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/shortcut.py
--rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/singleton.py
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/sleepx.py
--rw-r--r--   0        0        0     4348 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/startapp.py
--rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/startproject.py
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/video_utils.py
--rw-r--r--   0        0        0     5039 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/wayland_wininfo.py
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/webui.py
--rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/ydotool.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/__init__.py
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/cfonts/__init__.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/cfonts/__version__.py
--rw-r--r--   0        0        0     4783 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/cfonts/cli.py
--rw-r--r--   0        0        0     6451 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/cfonts/colors.py
--rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/cfonts/consts.py
--rw-r--r--   0        0        0    12752 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/cfonts/core.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/cfonts/py.typed
--rw-r--r--   0        0        0    29547 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/cfonts/fonts/3d.json
--rw-r--r--   0        0        0    16516 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/cfonts/fonts/block.json
--rw-r--r--   0        0        0     4771 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/cfonts/fonts/chrome.json
--rw-r--r--   0        0        0    11811 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/cfonts/fonts/grid.json
--rw-r--r--   0        0        0    37089 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/cfonts/fonts/huge.json
--rw-r--r--   0        0        0    13028 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/cfonts/fonts/pallet.json
--rw-r--r--   0        0        0    15470 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/cfonts/fonts/shade.json
--rw-r--r--   0        0        0     3896 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/cfonts/fonts/simple.json
--rw-r--r--   0        0        0     8083 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/cfonts/fonts/simple3d.json
--rw-r--r--   0        0        0     7299 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/cfonts/fonts/simpleBlock.json
--rw-r--r--   0        0        0    13027 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/cfonts/fonts/slick.json
--rw-r--r--   0        0        0     2568 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/cfonts/fonts/tiny.json
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/colorama/__init__.py
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/colorama/ansi.py
--rw-r--r--   0        0        0    11128 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/colorama/ansitowin32.py
--rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/colorama/initialise.py
--rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/colorama/win32.py
--rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/colorama/winterm.py
--rw-r--r--   0        0        0    18011 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/dogtail/COPYING
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/dogtail/__init__.py
--rw-r--r--   0        0        0     7794 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/dogtail/config.py
--rw-r--r--   0        0        0    12153 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/dogtail/distro.py
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/dogtail/dump.py
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/dogtail/errors.py
--rw-r--r--   0        0        0     9448 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/dogtail/i18n.py
--rw-r--r--   0        0        0     7191 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/dogtail/logging.py
--rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/dogtail/path.py
--rw-r--r--   0        0        0    15256 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/dogtail/predicate.py
--rw-r--r--   0        0        0    13055 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/dogtail/procedural.py
--rw-r--r--   0        0        0     9565 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/dogtail/rawinput.py
--rw-r--r--   0        0        0    17581 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/dogtail/rawinput_wayland.py
--rw-r--r--   0        0        0     7063 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/dogtail/sessions.py
--rw-r--r--   0        0        0     7988 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/dogtail/tc.py
--rw-r--r--   0        0        0    48139 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/dogtail/tree.py
--rw-r--r--   0        0        0    16049 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/dogtail/utils.py
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/dogtail/version.py
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/dogtail/wrapped.py
--rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/dogtail/icons/dogtail-head-48.png
--rw-r--r--   0        0        0    55404 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/dogtail/icons/dogtail-head.svg
--rw-r--r--   0        0        0     2462 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/dogtail/icons/dogtail-tail-48.png
--rw-r--r--   0        0        0    29904 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/dogtail/icons/dogtail-tail.svg
--rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/pyautogui/LICENSE.txt
--rw-r--r--   0        0        0    78875 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/pyautogui/__init__.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/pyautogui/__main__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/pyautogui/_pyautogui_java.py
--rw-r--r--   0        0        0    14827 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/pyautogui/_pyautogui_osx.py
--rw-r--r--   0        0        0    17011 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/pyautogui/_pyautogui_wayland.py
--rw-r--r--   0        0        0    20065 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/pyautogui/_pyautogui_win.py
--rw-r--r--   0        0        0    15261 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/pyautogui/_pyautogui_x11.py
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/pygtkcompat/__init__.py
--rw-r--r--   0        0        0    14200 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/pygtkcompat/generictreemodel.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/pygtkcompat/meson.build
--rw-r--r--   0        0        0    20672 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/pygtkcompat/pygtkcompat.py
--rwxr-xr-x   0        0        0    30155 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/sniff/sniff
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/sniff/sniff.desktop
--rw-r--r--   0        0        0    20943 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/sniff/sniff.ui
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/sniff/icons/button.xpm
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/sniff/icons/checkbutton.xpm
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/sniff/icons/checkmenuitem.xpm
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/sniff/icons/colorselection.xpm
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/sniff/icons/combo.xpm
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/sniff/icons/dialog.xpm
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/sniff/icons/image.xpm
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/sniff/icons/label.xpm
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/sniff/icons/menubar.xpm
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/sniff/icons/menuitem.xpm
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/sniff/icons/notebook.xpm
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/sniff/icons/scrolledwindow.xpm
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/sniff/icons/spinbutton.xpm
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/sniff/icons/statusbar.xpm
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/sniff/icons/table.xpm
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/sniff/icons/text.xpm
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/sniff/icons/toolbar.xpm
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/sniff/icons/tree.xpm
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/sniff/icons/treeitem.xpm
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/sniff/icons/unknown.xpm
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/sniff/icons/viewport.xpm
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/sniff/icons/vscrollbar.xpm
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/sniff/icons/vseparator.xpm
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/sniff/icons/window.xpm
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/wayland_autotool/CMakeLists.txt
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/wayland_autotool/README.md
--rw-r--r--   0        0        0     9324 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/wayland_autotool/autotool.cpp
--rw-r--r--   0        0        0     2929 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/wayland_autotool/autotool.h
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/wayland_autotool/install.sh
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/wayland_autotool/main.cpp
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/ydotool/.editorconfig
--rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/ydotool/CMakeLists.txt
--rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/ydotool/LICENSE
--rw-r--r--   0        0        0     4536 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/ydotool/Client/tool_click.c
--rw-r--r--   0        0        0     4137 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/ydotool/Client/tool_key.c
--rw-r--r--   0        0        0     4174 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/ydotool/Client/tool_mousemove.c
--rw-r--r--   0        0        0     8344 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/ydotool/Client/tool_type.c
--rw-r--r--   0        0        0     4696 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/ydotool/Client/ydotool.c
--rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/ydotool/Client/ydotool.h
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/ydotool/Daemon/CMakeLists.txt
--rwxr-xr-x   0        0        0      223 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/ydotool/Daemon/ydotool.service-openrc.in
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/ydotool/Daemon/ydotool.service.in
--rw-r--r--   0        0        0    16544 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/ydotool/Daemon/ydotoold.c
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/ydotool/manpage/CMakeLists.txt
--rw-r--r--   0        0        0     3262 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/ydotool/manpage/ydotool.1.scd
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/depends/ydotool/manpage/ydotoold.8.scd
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/git/__init__.py
--rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/git/_cargo.py
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/git/check.py
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/git/clone.py
--rw-r--r--   0        0        0     8061 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/git/code_statistics.py
--rw-r--r--   0        0        0     2498 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/git/commit.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/plugins/__init__.py
--rw-r--r--   0        0        0     2272 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/plugins/allure_report_extend.py
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/plugins/emoji_hooks.py
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/plugins/mng.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/pms/__init__.py
--rw-r--r--   0        0        0     4725 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/pms/_base.py
--rw-r--r--   0        0        0     2741 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/pms/_cargo.py
--rw-r--r--   0        0        0     4403 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/pms/csv2pms.py
--rw-r--r--   0        0        0    11725 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/pms/pms2csv.py
--rw-r--r--   0        0        0     5574 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/pms/send2pms.py
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/pms/suite.py
--rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/pms/task.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/remotectl/__init__.py
--rw-r--r--   0        0        0     5000 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/remotectl/_base.py
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/remotectl/_remote_dogtail_ctl.py
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/remotectl/_remote_other_ctl.py
--rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/remotectl/remote.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/rtk/__init__.py
--rw-r--r--   0        0        0     3804 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/rtk/_base.py
--rw-r--r--   0        0        0    11436 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/rtk/_cargo.py
--rw-r--r--   0        0        0    16780 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/rtk/local_runner.py
--rw-r--r--   0        0        0     3149 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/rtk/playbook.py
--rw-r--r--   0        0        0    21570 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/rtk/remote_runner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/utils/__init__.py
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/utils/check_python_source.py
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/utils/command_complete.sh
--rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/utils/docs_env.sh
--rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/utils/opencv_rpc_server.py
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/utils/pylint.sh
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/utils/sslclone.sh
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/utils/sub_deb.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/utils/sub_depends.py
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/utils/sub_env_cut.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/utils/sub_remote.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/utils/sub_sources.py
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/utils/sub_webui.py
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/src/utils/vnc.sh
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 youqu-2.5.4/pyproject.toml
--rw-r--r--   0        0        0     7482 2020-02-02 00:00:00.000000 youqu-2.5.4/youqu/README.md
--rw-r--r--   0        0        0     7958 2020-02-02 00:00:00.000000 youqu-2.5.4/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/CURRENT
+-rw-r--r--   0        0        0    41974 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/conftest.py
+-rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/env.sh
+-rw-r--r--   0        0        0     3703 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/manage.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/pytest.ini
+-rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/ruff.toml
+-rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/startproject.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/apps/__init__.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/setting/__init__.py
+-rw-r--r--   0        0        0     4354 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/setting/_env_base.sh
+-rwxr-xr-x   0        0        0     3272 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/setting/env_dev.sh
+-rw-r--r--   0        0        0     5444 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/setting/env_vir.sh
+-rw-r--r--   0        0        0    11023 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/setting/globalconfig.ini
+-rw-r--r--   0        0        0    11361 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/setting/globalconfig.py
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/setting/playbook.toml
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/setting/pmsmark.ini
+-rw-r--r--   0        0        0    20451 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/setting/pylintrc.cfg
+-rw-r--r--   0        0        0     2365 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/setting/skipif.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/setting/sleepx.ini
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/setting/subcmd.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/setting/template/ci.json
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/setting/template/language.ini
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/setting/template/app_template/${app_name}_assert.py-tpl
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/setting/template/app_template/.gitignore-tpl
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/setting/template/app_template/__init__.py-tpl
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/setting/template/app_template/config.ini-tpl
+-rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/setting/template/app_template/config.py-tpl
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/setting/template/app_template/conftest.py-tpl
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/setting/template/app_template/control-tpl
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/setting/template/app_template/mycase.csv-tpl
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/setting/template/app_template/case/__init__.py-tpl
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/setting/template/app_template/case/base_case.py-tpl
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/setting/template/app_template/case/test_mycase_001.py-tpl
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/setting/template/app_template/case/test_mycase_002.py-tpl
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/setting/template/app_template/case/assert_res/readme
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/setting/template/app_template/widget/${app_name}_widget.py-tpl
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/setting/template/app_template/widget/__init__.py-tpl
+-rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/setting/template/app_template/widget/base_widget.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/setting/template/app_template/widget/other.ini-tpl
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/setting/template/app_template/widget/other_widget.py-tpl
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/setting/template/app_template/widget/ui.ini-tpl
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/setting/template/app_template/widget/case_res/readme
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/setting/template/app_template/widget/pic_res/readme
+-rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/__init__.py
+-rw-r--r--   0        0        0    18200 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/assert_common.py
+-rw-r--r--   0        0        0    26398 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/button_center.py
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/calculate.py
+-rw-r--r--   0        0        0     7990 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/cmdctl.py
+-rw-r--r--   0        0        0     6975 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/csvctl.py
+-rw-r--r--   0        0        0     5006 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/custom_exception.py
+-rw-r--r--   0        0        0     2921 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/dbus_utils.py
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/desktop.py
+-rw-r--r--   0        0        0     7644 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/dogtail_utils.py
+-rw-r--r--   0        0        0    10856 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/filectl.py
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/filter_image.py
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/image_utils.py
+-rw-r--r--   0        0        0    14377 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/mouse_key.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/ocr_utils.py
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/pinyin.py
+-rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/read_csv.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/read_toml.py
+-rw-r--r--   0        0        0     3672 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/recording_screen.py
+-rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/requestx.py
+-rw-r--r--   0        0        0    15481 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/shortcut.py
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/singleton.py
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/sleepx.py
+-rw-r--r--   0        0        0     4348 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/startapp.py
+-rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/startproject.py
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/video_utils.py
+-rw-r--r--   0        0        0     5039 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/wayland_wininfo.py
+-rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/webui.py
+-rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/ydotool.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/__init__.py
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/cfonts/__init__.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/cfonts/__version__.py
+-rw-r--r--   0        0        0     4783 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/cfonts/cli.py
+-rw-r--r--   0        0        0     6451 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/cfonts/colors.py
+-rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/cfonts/consts.py
+-rw-r--r--   0        0        0    12752 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/cfonts/core.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/cfonts/py.typed
+-rw-r--r--   0        0        0    29547 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/cfonts/fonts/3d.json
+-rw-r--r--   0        0        0    16516 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/cfonts/fonts/block.json
+-rw-r--r--   0        0        0     4771 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/cfonts/fonts/chrome.json
+-rw-r--r--   0        0        0    11811 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/cfonts/fonts/grid.json
+-rw-r--r--   0        0        0    37089 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/cfonts/fonts/huge.json
+-rw-r--r--   0        0        0    13028 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/cfonts/fonts/pallet.json
+-rw-r--r--   0        0        0    15470 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/cfonts/fonts/shade.json
+-rw-r--r--   0        0        0     3896 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/cfonts/fonts/simple.json
+-rw-r--r--   0        0        0     8083 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/cfonts/fonts/simple3d.json
+-rw-r--r--   0        0        0     7299 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/cfonts/fonts/simpleBlock.json
+-rw-r--r--   0        0        0    13027 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/cfonts/fonts/slick.json
+-rw-r--r--   0        0        0     2568 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/cfonts/fonts/tiny.json
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/colorama/__init__.py
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/colorama/ansi.py
+-rw-r--r--   0        0        0    11128 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/colorama/ansitowin32.py
+-rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/colorama/initialise.py
+-rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/colorama/win32.py
+-rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/colorama/winterm.py
+-rw-r--r--   0        0        0    18011 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/dogtail/COPYING
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/dogtail/__init__.py
+-rw-r--r--   0        0        0     7794 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/dogtail/config.py
+-rw-r--r--   0        0        0    12153 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/dogtail/distro.py
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/dogtail/dump.py
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/dogtail/errors.py
+-rw-r--r--   0        0        0     9448 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/dogtail/i18n.py
+-rw-r--r--   0        0        0     7191 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/dogtail/logging.py
+-rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/dogtail/path.py
+-rw-r--r--   0        0        0    15256 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/dogtail/predicate.py
+-rw-r--r--   0        0        0    13055 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/dogtail/procedural.py
+-rw-r--r--   0        0        0     9565 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/dogtail/rawinput.py
+-rw-r--r--   0        0        0    17581 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/dogtail/rawinput_wayland.py
+-rw-r--r--   0        0        0     7063 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/dogtail/sessions.py
+-rw-r--r--   0        0        0     7988 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/dogtail/tc.py
+-rw-r--r--   0        0        0    48139 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/dogtail/tree.py
+-rw-r--r--   0        0        0    16049 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/dogtail/utils.py
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/dogtail/version.py
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/dogtail/wrapped.py
+-rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/dogtail/icons/dogtail-head-48.png
+-rw-r--r--   0        0        0    55404 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/dogtail/icons/dogtail-head.svg
+-rw-r--r--   0        0        0     2462 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/dogtail/icons/dogtail-tail-48.png
+-rw-r--r--   0        0        0    29904 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/dogtail/icons/dogtail-tail.svg
+-rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/pyautogui/LICENSE.txt
+-rw-r--r--   0        0        0    78875 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/pyautogui/__init__.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/pyautogui/__main__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/pyautogui/_pyautogui_java.py
+-rw-r--r--   0        0        0    14827 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/pyautogui/_pyautogui_osx.py
+-rw-r--r--   0        0        0    17011 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/pyautogui/_pyautogui_wayland.py
+-rw-r--r--   0        0        0    20065 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/pyautogui/_pyautogui_win.py
+-rw-r--r--   0        0        0    15261 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/pyautogui/_pyautogui_x11.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/pygtkcompat/__init__.py
+-rw-r--r--   0        0        0    14200 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/pygtkcompat/generictreemodel.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/pygtkcompat/meson.build
+-rw-r--r--   0        0        0    20672 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/pygtkcompat/pygtkcompat.py
+-rwxr-xr-x   0        0        0    30155 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/sniff/sniff
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/sniff/sniff.desktop
+-rw-r--r--   0        0        0    20943 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/sniff/sniff.ui
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/sniff/icons/button.xpm
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/sniff/icons/checkbutton.xpm
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/sniff/icons/checkmenuitem.xpm
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/sniff/icons/colorselection.xpm
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/sniff/icons/combo.xpm
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/sniff/icons/dialog.xpm
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/sniff/icons/image.xpm
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/sniff/icons/label.xpm
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/sniff/icons/menubar.xpm
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/sniff/icons/menuitem.xpm
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/sniff/icons/notebook.xpm
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/sniff/icons/scrolledwindow.xpm
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/sniff/icons/spinbutton.xpm
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/sniff/icons/statusbar.xpm
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/sniff/icons/table.xpm
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/sniff/icons/text.xpm
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/sniff/icons/toolbar.xpm
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/sniff/icons/tree.xpm
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/sniff/icons/treeitem.xpm
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/sniff/icons/unknown.xpm
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/sniff/icons/viewport.xpm
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/sniff/icons/vscrollbar.xpm
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/sniff/icons/vseparator.xpm
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/sniff/icons/window.xpm
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/wayland_autotool/CMakeLists.txt
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/wayland_autotool/README.md
+-rw-r--r--   0        0        0     9324 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/wayland_autotool/autotool.cpp
+-rw-r--r--   0        0        0     2929 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/wayland_autotool/autotool.h
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/wayland_autotool/install.sh
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/wayland_autotool/main.cpp
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/ydotool/.editorconfig
+-rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/ydotool/CMakeLists.txt
+-rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/ydotool/LICENSE
+-rw-r--r--   0        0        0     4536 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/ydotool/Client/tool_click.c
+-rw-r--r--   0        0        0     4137 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/ydotool/Client/tool_key.c
+-rw-r--r--   0        0        0     4174 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/ydotool/Client/tool_mousemove.c
+-rw-r--r--   0        0        0     8344 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/ydotool/Client/tool_type.c
+-rw-r--r--   0        0        0     4696 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/ydotool/Client/ydotool.c
+-rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/ydotool/Client/ydotool.h
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/ydotool/Daemon/CMakeLists.txt
+-rwxr-xr-x   0        0        0      223 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/ydotool/Daemon/ydotool.service-openrc.in
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/ydotool/Daemon/ydotool.service.in
+-rw-r--r--   0        0        0    16544 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/ydotool/Daemon/ydotoold.c
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/ydotool/manpage/CMakeLists.txt
+-rw-r--r--   0        0        0     3262 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/ydotool/manpage/ydotool.1.scd
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/depends/ydotool/manpage/ydotoold.8.scd
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/git/__init__.py
+-rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/git/_cargo.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/git/check.py
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/git/clone.py
+-rw-r--r--   0        0        0     8061 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/git/code_statistics.py
+-rw-r--r--   0        0        0     2498 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/git/commit.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/plugins/__init__.py
+-rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/plugins/allure_report_extend.py
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/plugins/emoji_hooks.py
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/plugins/mng.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/pms/__init__.py
+-rw-r--r--   0        0        0     4725 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/pms/_base.py
+-rw-r--r--   0        0        0     2741 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/pms/_cargo.py
+-rw-r--r--   0        0        0     4403 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/pms/csv2pms.py
+-rw-r--r--   0        0        0    11725 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/pms/pms2csv.py
+-rw-r--r--   0        0        0     5574 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/pms/send2pms.py
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/pms/suite.py
+-rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/pms/task.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/remotectl/__init__.py
+-rw-r--r--   0        0        0     5000 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/remotectl/_base.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/remotectl/_remote_dogtail_ctl.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/remotectl/_remote_other_ctl.py
+-rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/remotectl/remote.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/rtk/__init__.py
+-rw-r--r--   0        0        0     3788 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/rtk/_base.py
+-rw-r--r--   0        0        0    11436 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/rtk/_cargo.py
+-rw-r--r--   0        0        0    16780 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/rtk/local_runner.py
+-rw-r--r--   0        0        0     3149 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/rtk/playbook.py
+-rw-r--r--   0        0        0    21570 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/rtk/remote_runner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/utils/__init__.py
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/utils/check_python_source.py
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/utils/command_complete.sh
+-rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/utils/docs_env.sh
+-rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/utils/opencv_rpc_server.py
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/utils/pylint.sh
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/utils/sslclone.sh
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/utils/sub_deb.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/utils/sub_depends.py
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/utils/sub_env_cut.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/utils/sub_remote.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/utils/sub_sources.py
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/utils/sub_webui.py
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/src/utils/vnc.sh
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 youqu-2.5.5/pyproject.toml
+-rw-r--r--   0        0        0     5252 2020-02-02 00:00:00.000000 youqu-2.5.5/youqu/README.md
+-rw-r--r--   0        0        0     5728 2020-02-02 00:00:00.000000 youqu-2.5.5/PKG-INFO
```

### Comparing `youqu-2.5.4/youqu/conftest.py` & `youqu-2.5.5/youqu/conftest.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/env.sh` & `youqu-2.5.5/youqu/env.sh`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/manage.py` & `youqu-2.5.5/youqu/manage.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/ruff.toml` & `youqu-2.5.5/youqu/ruff.toml`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/startproject.py` & `youqu-2.5.5/youqu/startproject.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/setting/_env_base.sh` & `youqu-2.5.5/youqu/setting/_env_base.sh`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/setting/env_dev.sh` & `youqu-2.5.5/youqu/setting/env_dev.sh`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/setting/env_vir.sh` & `youqu-2.5.5/youqu/setting/env_vir.sh`

 * *Files 2% similar despite different names*

```diff
@@ -174,17 +174,17 @@
 rm -rf Pipfile
 echo "${python_virtualenv_path}"
 pipenv run pip list
 system_env
 
 echo 'pipenv run python "$@"' | sudo tee /usr/bin/youqu > /dev/null 2>&1
 echo "pipenv shell" | sudo tee /usr/bin/youqu-shell > /dev/null 2>&1
-echo "pipenv --rm" | sudo tee /usr/bin/youqu-shell-rm > /dev/null 2>&1
+echo "pipenv --rm" | sudo tee /usr/bin/youqu-rm > /dev/null 2>&1
 sudo chmod +x /usr/bin/youqu
 sudo chmod +x /usr/bin/youqu-shell
 sudo chmod +x /usr/bin/youqu-shell-rm
 
-cp --force ${ROOT_DIR}/src/utils/command_complete.sh ${HOME}/.config/
-echo "source ${HOME}/.config/command_complete.sh" >> $HOME/.bashrc
-source $HOME/.bashrc
+#cp --force ${ROOT_DIR}/src/utils/command_complete.sh ${HOME}/.config/
+#echo "source ${HOME}/.config/command_complete.sh" >> $HOME/.bashrc
+#source $HOME/.bashrc
 
 cd ${ROOT_DIR};youqu manage.py -h
```

### Comparing `youqu-2.5.4/youqu/setting/globalconfig.ini` & `youqu-2.5.5/youqu/setting/globalconfig.ini`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/setting/globalconfig.py` & `youqu-2.5.5/youqu/setting/globalconfig.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/setting/playbook.toml` & `youqu-2.5.5/youqu/setting/playbook.toml`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/setting/pylintrc.cfg` & `youqu-2.5.5/youqu/setting/pylintrc.cfg`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/setting/skipif.py` & `youqu-2.5.5/youqu/setting/skipif.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/setting/template/app_template/config.py-tpl` & `youqu-2.5.5/youqu/setting/template/app_template/config.py-tpl`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/setting/template/app_template/case/test_mycase_002.py-tpl` & `youqu-2.5.5/youqu/setting/template/app_template/case/test_mycase_002.py-tpl`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/setting/template/app_template/widget/base_widget.py-tpl` & `youqu-2.5.5/youqu/setting/template/app_template/widget/base_widget.py-tpl`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/setting/template/app_template/widget/ui.ini-tpl` & `youqu-2.5.5/youqu/setting/template/app_template/widget/ui.ini-tpl`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/__init__.py` & `youqu-2.5.5/youqu/src/__init__.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/assert_common.py` & `youqu-2.5.5/youqu/src/assert_common.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/button_center.py` & `youqu-2.5.5/youqu/src/button_center.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/calculate.py` & `youqu-2.5.5/youqu/src/calculate.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/cmdctl.py` & `youqu-2.5.5/youqu/src/cmdctl.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/csvctl.py` & `youqu-2.5.5/youqu/src/csvctl.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/custom_exception.py` & `youqu-2.5.5/youqu/src/custom_exception.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/dbus_utils.py` & `youqu-2.5.5/youqu/src/dbus_utils.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/desktop.py` & `youqu-2.5.5/youqu/src/desktop.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/dogtail_utils.py` & `youqu-2.5.5/youqu/src/dogtail_utils.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/filectl.py` & `youqu-2.5.5/youqu/src/filectl.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/filter_image.py` & `youqu-2.5.5/youqu/src/filter_image.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/image_utils.py` & `youqu-2.5.5/youqu/src/image_utils.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/mouse_key.py` & `youqu-2.5.5/youqu/src/mouse_key.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/ocr_utils.py` & `youqu-2.5.5/youqu/src/ocr_utils.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/pinyin.py` & `youqu-2.5.5/youqu/src/pinyin.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/read_csv.py` & `youqu-2.5.5/youqu/src/read_csv.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/recording_screen.py` & `youqu-2.5.5/youqu/src/recording_screen.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/requestx.py` & `youqu-2.5.5/youqu/src/requestx.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/shortcut.py` & `youqu-2.5.5/youqu/src/shortcut.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/singleton.py` & `youqu-2.5.5/youqu/src/singleton.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/sleepx.py` & `youqu-2.5.5/youqu/src/sleepx.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/startapp.py` & `youqu-2.5.5/youqu/src/startapp.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/startproject.py` & `youqu-2.5.5/youqu/src/startproject.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/video_utils.py` & `youqu-2.5.5/youqu/src/video_utils.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/wayland_wininfo.py` & `youqu-2.5.5/youqu/src/wayland_wininfo.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/webui.py` & `youqu-2.5.5/youqu/src/webui.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/ydotool.py` & `youqu-2.5.5/youqu/src/ydotool.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/cfonts/cli.py` & `youqu-2.5.5/youqu/src/depends/cfonts/cli.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/cfonts/colors.py` & `youqu-2.5.5/youqu/src/depends/cfonts/colors.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/cfonts/consts.py` & `youqu-2.5.5/youqu/src/depends/cfonts/consts.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/cfonts/core.py` & `youqu-2.5.5/youqu/src/depends/cfonts/core.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/cfonts/fonts/3d.json` & `youqu-2.5.5/youqu/src/depends/cfonts/fonts/3d.json`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/cfonts/fonts/block.json` & `youqu-2.5.5/youqu/src/depends/cfonts/fonts/block.json`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/cfonts/fonts/chrome.json` & `youqu-2.5.5/youqu/src/depends/cfonts/fonts/chrome.json`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/cfonts/fonts/grid.json` & `youqu-2.5.5/youqu/src/depends/cfonts/fonts/grid.json`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/cfonts/fonts/huge.json` & `youqu-2.5.5/youqu/src/depends/cfonts/fonts/huge.json`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/cfonts/fonts/pallet.json` & `youqu-2.5.5/youqu/src/depends/cfonts/fonts/pallet.json`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/cfonts/fonts/shade.json` & `youqu-2.5.5/youqu/src/depends/cfonts/fonts/shade.json`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/cfonts/fonts/simple.json` & `youqu-2.5.5/youqu/src/depends/cfonts/fonts/simple.json`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/cfonts/fonts/simple3d.json` & `youqu-2.5.5/youqu/src/depends/cfonts/fonts/simple3d.json`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/cfonts/fonts/simpleBlock.json` & `youqu-2.5.5/youqu/src/depends/cfonts/fonts/simpleBlock.json`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/cfonts/fonts/slick.json` & `youqu-2.5.5/youqu/src/depends/cfonts/fonts/slick.json`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/cfonts/fonts/tiny.json` & `youqu-2.5.5/youqu/src/depends/cfonts/fonts/tiny.json`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/colorama/ansi.py` & `youqu-2.5.5/youqu/src/depends/colorama/ansi.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/colorama/ansitowin32.py` & `youqu-2.5.5/youqu/src/depends/colorama/ansitowin32.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/colorama/initialise.py` & `youqu-2.5.5/youqu/src/depends/colorama/initialise.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/colorama/win32.py` & `youqu-2.5.5/youqu/src/depends/colorama/win32.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/colorama/winterm.py` & `youqu-2.5.5/youqu/src/depends/colorama/winterm.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/dogtail/COPYING` & `youqu-2.5.5/youqu/src/depends/dogtail/COPYING`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/dogtail/__init__.py` & `youqu-2.5.5/youqu/src/depends/dogtail/__init__.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/dogtail/config.py` & `youqu-2.5.5/youqu/src/depends/dogtail/config.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/dogtail/distro.py` & `youqu-2.5.5/youqu/src/depends/dogtail/distro.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/dogtail/dump.py` & `youqu-2.5.5/youqu/src/depends/dogtail/dump.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/dogtail/errors.py` & `youqu-2.5.5/youqu/src/depends/dogtail/errors.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/dogtail/i18n.py` & `youqu-2.5.5/youqu/src/depends/dogtail/i18n.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/dogtail/logging.py` & `youqu-2.5.5/youqu/src/depends/dogtail/logging.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/dogtail/path.py` & `youqu-2.5.5/youqu/src/depends/dogtail/path.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/dogtail/predicate.py` & `youqu-2.5.5/youqu/src/depends/dogtail/predicate.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/dogtail/procedural.py` & `youqu-2.5.5/youqu/src/depends/dogtail/procedural.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/dogtail/rawinput.py` & `youqu-2.5.5/youqu/src/depends/dogtail/rawinput.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/dogtail/rawinput_wayland.py` & `youqu-2.5.5/youqu/src/depends/dogtail/rawinput_wayland.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/dogtail/sessions.py` & `youqu-2.5.5/youqu/src/depends/dogtail/sessions.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/dogtail/tc.py` & `youqu-2.5.5/youqu/src/depends/dogtail/tc.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/dogtail/tree.py` & `youqu-2.5.5/youqu/src/depends/dogtail/tree.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/dogtail/utils.py` & `youqu-2.5.5/youqu/src/depends/dogtail/utils.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/dogtail/version.py` & `youqu-2.5.5/youqu/src/depends/dogtail/version.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/dogtail/wrapped.py` & `youqu-2.5.5/youqu/src/depends/dogtail/wrapped.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/dogtail/icons/dogtail-head-48.png` & `youqu-2.5.5/youqu/src/depends/dogtail/icons/dogtail-head-48.png`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/dogtail/icons/dogtail-head.svg` & `youqu-2.5.5/youqu/src/depends/dogtail/icons/dogtail-head.svg`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/dogtail/icons/dogtail-tail-48.png` & `youqu-2.5.5/youqu/src/depends/dogtail/icons/dogtail-tail-48.png`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/dogtail/icons/dogtail-tail.svg` & `youqu-2.5.5/youqu/src/depends/dogtail/icons/dogtail-tail.svg`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/pyautogui/LICENSE.txt` & `youqu-2.5.5/youqu/src/depends/pyautogui/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/pyautogui/__init__.py` & `youqu-2.5.5/youqu/src/depends/pyautogui/__init__.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/pyautogui/_pyautogui_osx.py` & `youqu-2.5.5/youqu/src/depends/pyautogui/_pyautogui_osx.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/pyautogui/_pyautogui_wayland.py` & `youqu-2.5.5/youqu/src/depends/pyautogui/_pyautogui_wayland.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/pyautogui/_pyautogui_win.py` & `youqu-2.5.5/youqu/src/depends/pyautogui/_pyautogui_win.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/pyautogui/_pyautogui_x11.py` & `youqu-2.5.5/youqu/src/depends/pyautogui/_pyautogui_x11.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/pygtkcompat/__init__.py` & `youqu-2.5.5/youqu/src/depends/pygtkcompat/__init__.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/pygtkcompat/generictreemodel.py` & `youqu-2.5.5/youqu/src/depends/pygtkcompat/generictreemodel.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/pygtkcompat/pygtkcompat.py` & `youqu-2.5.5/youqu/src/depends/pygtkcompat/pygtkcompat.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/sniff/sniff` & `youqu-2.5.5/youqu/src/depends/sniff/sniff`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/sniff/sniff.ui` & `youqu-2.5.5/youqu/src/depends/sniff/sniff.ui`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/sniff/icons/button.xpm` & `youqu-2.5.5/youqu/src/depends/sniff/icons/button.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/sniff/icons/checkbutton.xpm` & `youqu-2.5.5/youqu/src/depends/sniff/icons/checkbutton.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/sniff/icons/checkmenuitem.xpm` & `youqu-2.5.5/youqu/src/depends/sniff/icons/checkmenuitem.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/sniff/icons/colorselection.xpm` & `youqu-2.5.5/youqu/src/depends/sniff/icons/colorselection.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/sniff/icons/combo.xpm` & `youqu-2.5.5/youqu/src/depends/sniff/icons/combo.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/sniff/icons/dialog.xpm` & `youqu-2.5.5/youqu/src/depends/sniff/icons/dialog.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/sniff/icons/image.xpm` & `youqu-2.5.5/youqu/src/depends/sniff/icons/image.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/sniff/icons/label.xpm` & `youqu-2.5.5/youqu/src/depends/sniff/icons/label.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/sniff/icons/menubar.xpm` & `youqu-2.5.5/youqu/src/depends/sniff/icons/menubar.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/sniff/icons/menuitem.xpm` & `youqu-2.5.5/youqu/src/depends/sniff/icons/menuitem.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/sniff/icons/notebook.xpm` & `youqu-2.5.5/youqu/src/depends/sniff/icons/notebook.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/sniff/icons/scrolledwindow.xpm` & `youqu-2.5.5/youqu/src/depends/sniff/icons/scrolledwindow.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/sniff/icons/spinbutton.xpm` & `youqu-2.5.5/youqu/src/depends/sniff/icons/spinbutton.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/sniff/icons/statusbar.xpm` & `youqu-2.5.5/youqu/src/depends/sniff/icons/statusbar.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/sniff/icons/table.xpm` & `youqu-2.5.5/youqu/src/depends/sniff/icons/table.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/sniff/icons/text.xpm` & `youqu-2.5.5/youqu/src/depends/sniff/icons/text.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/sniff/icons/toolbar.xpm` & `youqu-2.5.5/youqu/src/depends/sniff/icons/toolbar.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/sniff/icons/tree.xpm` & `youqu-2.5.5/youqu/src/depends/sniff/icons/tree.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/sniff/icons/treeitem.xpm` & `youqu-2.5.5/youqu/src/depends/sniff/icons/treeitem.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/sniff/icons/unknown.xpm` & `youqu-2.5.5/youqu/src/depends/sniff/icons/unknown.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/sniff/icons/viewport.xpm` & `youqu-2.5.5/youqu/src/depends/sniff/icons/viewport.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/sniff/icons/vscrollbar.xpm` & `youqu-2.5.5/youqu/src/depends/sniff/icons/vscrollbar.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/sniff/icons/vseparator.xpm` & `youqu-2.5.5/youqu/src/depends/sniff/icons/vseparator.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/sniff/icons/window.xpm` & `youqu-2.5.5/youqu/src/depends/sniff/icons/window.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/wayland_autotool/CMakeLists.txt` & `youqu-2.5.5/youqu/src/depends/wayland_autotool/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/wayland_autotool/autotool.cpp` & `youqu-2.5.5/youqu/src/depends/wayland_autotool/autotool.cpp`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/wayland_autotool/autotool.h` & `youqu-2.5.5/youqu/src/depends/wayland_autotool/autotool.h`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/wayland_autotool/main.cpp` & `youqu-2.5.5/youqu/src/depends/wayland_autotool/main.cpp`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/ydotool/CMakeLists.txt` & `youqu-2.5.5/youqu/src/depends/ydotool/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/ydotool/LICENSE` & `youqu-2.5.5/youqu/src/depends/ydotool/LICENSE`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/ydotool/Client/tool_click.c` & `youqu-2.5.5/youqu/src/depends/ydotool/Client/tool_click.c`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/ydotool/Client/tool_key.c` & `youqu-2.5.5/youqu/src/depends/ydotool/Client/tool_key.c`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/ydotool/Client/tool_mousemove.c` & `youqu-2.5.5/youqu/src/depends/ydotool/Client/tool_mousemove.c`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/ydotool/Client/tool_type.c` & `youqu-2.5.5/youqu/src/depends/ydotool/Client/tool_type.c`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/ydotool/Client/ydotool.c` & `youqu-2.5.5/youqu/src/depends/ydotool/Client/ydotool.c`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/ydotool/Client/ydotool.h` & `youqu-2.5.5/youqu/src/depends/ydotool/Client/ydotool.h`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/ydotool/Daemon/ydotoold.c` & `youqu-2.5.5/youqu/src/depends/ydotool/Daemon/ydotoold.c`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/ydotool/manpage/ydotool.1.scd` & `youqu-2.5.5/youqu/src/depends/ydotool/manpage/ydotool.1.scd`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/depends/ydotool/manpage/ydotoold.8.scd` & `youqu-2.5.5/youqu/src/depends/ydotool/manpage/ydotoold.8.scd`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/git/_cargo.py` & `youqu-2.5.5/youqu/src/git/_cargo.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/git/clone.py` & `youqu-2.5.5/youqu/src/git/clone.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/git/code_statistics.py` & `youqu-2.5.5/youqu/src/git/code_statistics.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/git/commit.py` & `youqu-2.5.5/youqu/src/git/commit.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/plugins/allure_report_extend.py` & `youqu-2.5.5/youqu/src/plugins/allure_report_extend.py`

 * *Files 13% similar despite different names*

```diff
@@ -39,27 +39,31 @@
             w(f"PMS用例维度(总数/通过/失败/跳过)={py_case_info}")
             w(f"网络地址={GlobalConfig.USERNAME}@{GlobalConfig.HOST_IP}")
             w(f"工作目录={GlobalConfig.ROOT_DIR}")
             w(f"镜像版本={GlobalConfig.VERSION}")
 
             screen = Tk()
             w(f"分辨率={screen.winfo_screenwidth()}x{screen.winfo_screenheight()}")
-
             w(f"显示协议={GlobalConfig.DISPLAY_SERVER.title()}")
 
-            cpu_info = (
-                os.popen(
-                    f"echo '{GlobalConfig.PASSWORD}' | sudo -S dmidecode -s  processor-version"
+            try:
+                cpu_info = (
+                    os.popen(
+                        f"echo '{GlobalConfig.PASSWORD}' | sudo -S dmidecode -s  processor-version"
+                    )
+                    .readlines()[0]
+                    .strip("\n")
                 )
-                .readlines()[0]
-                .strip("\n")
-            )
-            w(f"CPU信息={cpu_info}")
+                w(f"CPU信息={cpu_info}")
+
 
-            mem_info = os.popen(
-                f'''echo '{GlobalConfig.PASSWORD}' | sudo -S dmidecode|grep -A16 'Memory Device' | grep -v "Memory Device Mapped Address" | grep "Range Size"'''
-            ).readlines()
-            MEM_TOTAL = sum([int(i.split(":")[1].rstrip(" GB\n").strip()) for i in mem_info])
-            w(f"内存信息={MEM_TOTAL}G")
+                mem_info = os.popen(
+                    f'''echo '{GlobalConfig.PASSWORD}' | sudo -S dmidecode|grep -A16 'Memory Device' | '''
+                    'grep -v "Memory Device Mapped Address" | grep "Range Size"'
+                ).readlines()
+                MEM_TOTAL = sum([int(i.split(":")[1].rstrip(" GB\n").strip()) for i in mem_info])
+                w(f"内存信息={MEM_TOTAL}G")
+            except IndexError:
+                ...
 
             os_info = os.popen("uname -a").read()
             w(f"内核信息={os_info}")
```

### Comparing `youqu-2.5.4/youqu/src/plugins/emoji_hooks.py` & `youqu-2.5.5/youqu/src/plugins/emoji_hooks.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/plugins/mng.py` & `youqu-2.5.5/youqu/src/plugins/mng.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/pms/_base.py` & `youqu-2.5.5/youqu/src/pms/_base.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/pms/_cargo.py` & `youqu-2.5.5/youqu/src/pms/_cargo.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/pms/csv2pms.py` & `youqu-2.5.5/youqu/src/pms/csv2pms.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/pms/pms2csv.py` & `youqu-2.5.5/youqu/src/pms/pms2csv.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/pms/send2pms.py` & `youqu-2.5.5/youqu/src/pms/send2pms.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/pms/suite.py` & `youqu-2.5.5/youqu/src/pms/suite.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/pms/task.py` & `youqu-2.5.5/youqu/src/pms/task.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/remotectl/_base.py` & `youqu-2.5.5/youqu/src/remotectl/_base.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/remotectl/_remote_dogtail_ctl.py` & `youqu-2.5.5/youqu/src/remotectl/_remote_dogtail_ctl.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/remotectl/_remote_other_ctl.py` & `youqu-2.5.5/youqu/src/remotectl/_remote_other_ctl.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/remotectl/remote.py` & `youqu-2.5.5/youqu/src/remotectl/remote.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/rtk/_base.py` & `youqu-2.5.5/youqu/src/rtk/_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,18 +83,17 @@
     raise NotADirectoryError(f"{app_name} 目录不存在")
 
 
 def collect_result(results):
     res = Counter([results.get(i).get("result") for i in results])
     total = sum(res.values())
     skiped = res.get("skip", 0)
-    total = total - skiped
     passed = res.get("pass", 0)
     failed = total - passed
-    pass_rate = f"{round((passed / total) * 100, 1)}%" if passed else "0%"
+    pass_rate = f"{round((passed / (total - skiped)) * 100, 2)}%" if passed else "0%"
     return total, failed, passed, skiped, pass_rate
 
 
 def get_result(ci_result):
     with open(ci_result, "r", encoding="utf-8") as _f:
         results_dict = json.load(_f)
     return collect_result(results_dict)
```

### Comparing `youqu-2.5.4/youqu/src/rtk/_cargo.py` & `youqu-2.5.5/youqu/src/rtk/_cargo.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/rtk/local_runner.py` & `youqu-2.5.5/youqu/src/rtk/local_runner.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/rtk/playbook.py` & `youqu-2.5.5/youqu/src/rtk/playbook.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/rtk/remote_runner.py` & `youqu-2.5.5/youqu/src/rtk/remote_runner.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/utils/check_python_source.py` & `youqu-2.5.5/youqu/src/utils/check_python_source.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/utils/docs_env.sh` & `youqu-2.5.5/youqu/src/utils/docs_env.sh`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/utils/opencv_rpc_server.py` & `youqu-2.5.5/youqu/src/utils/opencv_rpc_server.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/utils/pylint.sh` & `youqu-2.5.5/youqu/src/utils/pylint.sh`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/utils/sslclone.sh` & `youqu-2.5.5/youqu/src/utils/sslclone.sh`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/utils/sub_deb.py` & `youqu-2.5.5/youqu/src/utils/sub_deb.py`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/youqu/src/utils/vnc.sh` & `youqu-2.5.5/youqu/src/utils/vnc.sh`

 * *Files identical despite different names*

### Comparing `youqu-2.5.4/pyproject.toml` & `youqu-2.5.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "youqu"
-version = "2.5.4"
+version = "2.5.5"
 authors = [
     { name = "mikigo", email = "huangmingqiang@uniontech.com" },
 ]
 
 description = "youqu"
 readme = "youqu/README.md"
 requires-python = ">=3.7"
```

### Comparing `youqu-2.5.4/PKG-INFO` & `youqu-2.5.5/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: youqu
-Version: 2.5.4
+Version: 2.5.5
 Summary: youqu
 Project-URL: Source, https://github.com/linuxdeepin/youqu
 Project-URL: Documentation, https://linuxdeepin.github.io/youqu
 Author-email: mikigo <huangmingqiang@uniontech.com>
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
@@ -41,58 +41,44 @@
 
 <a href="https://github.com/linuxdeepin/youqu" target="_blank">GitHub</a> | <a href="https://gitee.com/deepin-community/youqu" target="_blank">Gitee</a>
 
 <a href="https://linuxdeepin.github.io/youqu" target="_blank">在线文档</a>
 
 ---
 
-YouQu（有趣）是深度公司开源的一个用于 Linux 操作系统的自动化测试框架，支持多元化元素定位和断言、用例标签化管理和执行、强大的日志和报告输出等特色功能，同时完美兼容 X11、Wayland 显示协议，环境部署简单，操作易上手。
+YouQu（有趣）是深度公司开源的一个用于 Linux 操作系统的自动化测试框架，支持多元化元素定位和断言、用例标签化管理和执行、强大的日志和报告输出等特色功能，同时完美兼容 X11、Wayland 显示协议，环境部署简单，操作易上手。🔥
 
 ## YouQu（有趣）能做什么
 
-- [x] Linux 桌面应用 UI 自动化测试
-- [x] Linux 桌面应用 DBus/Gsettings 接口自动化测试
-- [x] 命令行自动化测试
-- [x] HTTP 接口自动化测试
-- [x] Web UI 自动化测试
-- [ ] Linux 桌面应用性能自动化测试
-
-<details>
-	<summary style="color: #FF9933">点击查看爱上 “有趣（YouQu）” 的 N 个理由</summary>
-	<ul>
-        <li>无处不在的代码补全，让编写自动化测试用例成为一种享受；</li>
-        <li>核心库提供了统一的接口，编写方法时只需要导入一个包就可以使用到核心库提供的所有功能；</li>
-        <li>除了常用的属性定位、图像识别以外，我们还提供基于 UI 的元素定位方案，其使用简单且高效，效果一定能惊讶到你；</li>
-        <li>对属性定位的方法进行了二次封装，将编写属性定位的方法变得简单而优雅；</li>
-        <li>对图像识别定位技术进行功能升级，除了支持单个坐标返回，还支持同一界面下多个相同元素返回多个坐标的功能；</li>
-        <li>提供用例标签化管理、批量跳过和批量条件跳过的功能，你想不到一个 csv 文件原来能干这么多事情；</li>
-        <li>提供了功能强大的执行器入口，让你可以方便的在本地执行任何用例集的用例，其丰富的自定义配置项，满足你对执行器所有的幻想；</li>
-        <li>提供远程执行的功能，可以控制多台机器并行跑，或者分布式跑，这种付费功能现在免费给你用；</li>
-        <li>提供自动输出日志的功能，你再也不用为每个方法单独写输出日志的代码，一切我们给你搞定了，日志输出不仅内容丰富，颜值也绝对在线，我们还自己设计了一款终端输出主题叫《五彩斑斓的黑》；</li>
-        <li>提供一键部署自动化测试环境的功能，让你再也不用为环境部署而烦恼；</li>
-        <li>提供自动生成多种报告的功能，你想输出什么报告形式都行，而且我们在报告中还加入了失败录屏和失败截图的功能；</li>
-        <li>对断言进行了二次封装，提供更友好化的错误提示，让定位问题精准高效；</li>
-        <li>不仅支持单条用例超时控制，而且还支持动态控制用例批量执行的总时间，确保 CI 环境下能顺畅运行；</li>
-        <li>支持本地文件测试套执行、PMS 测试套执行、标签化执行方案，满足你各种场景下的执行需求；</li>
-        <li>支持基于深度学习的 OCR 功能，可定位可断言，中文识别的天花板；</li>
-        <li>完美兼容 Wayland  和 X11，真正做到一套代码，随处执行；</li>
-        <li>支持多种方式的数据回填功能，其中异步回填的方案，完美解决了数据回填的耗时问题；</li>
-        <li>支持重启交互场景用例的执行，使用方法优雅简洁；</li>
-    </ul>
-</details>
+- [x] 💻 Linux 桌面应用 UI 自动化测试
+- [x] 🌏 Web UI 自动化测试
+- [x] 🚌 Linux DBus 接口自动化测试
+- [x] 🚀 命令行自动化测试
+- [x] 🕷️ HTTP 接口自动化测试
+- [ ] ⏲️ Linux 桌面应用性能自动化测试
 
 ## 安装
 
 从 PyPI 安装:
 
 
 ```shell
 $ sudo pip3 install youqu
 ```
 
+<details> 
+<summary>不加 sudo ?</summary> 
+<pre>
+其实不加 sudo 也是可以的：<br>
+  pip3 install youqu<br>
+但某些情况下可能出现 youqu-startproject 命令无法使用，这是因为不加 sudo 时，安装包路径是在 $HOME/.local/lib/pythonX.X/site-packages，而此路径可能不在环境变量（PATH）中，您可以通过添加环境变量的方式使用 youqu-startproject 命令：<br>
+  export PATH=$PATH:$HOME/.local/lib/pythonX.X/site-packages<br>
+</pre>
+</details>
+
 ## 创建项目
 
 您可以在任意目录下，使用 `youqu-startproject` 命令创建一个项目：
 
 ```shell
 $ youqu-startproject my_project
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: youqu Version: 2.5.4 Summary: youqu Project-URL:
+Metadata-Version: 2.1 Name: youqu Version: 2.5.5 Summary: youqu Project-URL:
 Source, https://github.com/linuxdeepin/youqu Project-URL: Documentation, https:
 //linuxdeepin.github.io/youqu Author-email: mikigo
 uniontech.com> Classifier: License :: OSI Approved :: GNU General Public
 License v2 (GPLv2) Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3.7 Requires-Python: >=3.7 Description-
 Content-Type: text/markdown
                                     _[_Y_o_u_Q_u_]
@@ -23,46 +23,32 @@
 project/youqu) [![Downloads](https://static.pepy.tech/badge/youqu/month)]
 (https://pepy.tech/project/youqu) [![Downloads](https://static.pepy.tech/badge/
 youqu)](https://pepy.tech/project/youqu) [![Hits](https://hits.sh/github.com/
 linuxdeepin/youqu.svg?style=flat&label=Github_Hits&color=blue)](https://
 github.com/linuxdeepin/youqu) --- _G_i_t_H_u_b | _G_i_t_e_e _å__¨_ç_º_¿_æ___æ_¡_£ --
 - YouQuï¼æè¶£ï¼æ¯æ·±åº¦å¬å¸å¼æºçä¸ä¸ªç¨äº Linux
 æä½ç³»ç»çèªå¨åæµè¯æ¡æ¶ï¼æ¯æå¤åååç´ å®ä½åæ­è¨ãç¨ä¾æ ç­¾åç®¡çåæ§è¡ãå¼ºå¤§çæ¥å¿åæ¥åè¾åºç­ç¹è²åè½ï¼åæ¶å®ç¾å¼å®¹
-X11ãWayland æ¾ç¤ºåè®®ï¼ç¯å¢é¨ç½²ç®åï¼æä½æä¸æã ##
-YouQuï¼æè¶£ï¼è½åä»ä¹ - [x] Linux æ¡é¢åºç¨ UI èªå¨åæµè¯ - [x]
-Linux æ¡é¢åºç¨ DBus/Gsettings æ¥å£èªå¨åæµè¯ - [x]
-å½ä»¤è¡èªå¨åæµè¯ - [x] HTTP æ¥å£èªå¨åæµè¯ - [x] Web UI
-èªå¨åæµè¯ - [ ] Linux æ¡é¢åºç¨æ§è½èªå¨åæµè¯
-ç¹å»æ¥çç±ä¸ âæè¶£ï¼YouQuï¼â ç N ä¸ªçç±
-    * æ å¤ä¸å¨çä»£ç è¡¥å¨ï¼è®©ç¼åèªå¨åæµè¯ç¨ä¾æä¸ºä¸ç§äº«åï¼
-    * æ ¸å¿åºæä¾äºç»ä¸çæ¥å£ï¼ç¼åæ¹æ³æ¶åªéè¦å¯¼å¥ä¸ä¸ªåå°±å¯ä»¥ä½¿ç¨å°æ ¸å¿åºæä¾çææåè½ï¼
-    * é¤äºå¸¸ç¨çå±æ§å®ä½ãå¾åè¯å«ä»¥å¤ï¼æä»¬è¿æä¾åºäº
-      UI
-      çåç´ å®ä½æ¹æ¡ï¼å¶ä½¿ç¨ç®åä¸é«æï¼ææä¸å®è½æè®¶å°ä½ ï¼
-    * å¯¹å±æ§å®ä½çæ¹æ³è¿è¡äºäºæ¬¡å°è£ï¼å°ç¼åå±æ§å®ä½çæ¹æ³åå¾ç®åèä¼éï¼
-    * å¯¹å¾åè¯å«å®ä½ææ¯è¿è¡åè½åçº§ï¼é¤äºæ¯æåä¸ªåæ è¿åï¼è¿æ¯æåä¸çé¢ä¸å¤ä¸ªç¸ååç´ è¿åå¤ä¸ªåæ çåè½ï¼
-    * æä¾ç¨ä¾æ ç­¾åç®¡çãæ¹éè·³è¿åæ¹éæ¡ä»¶è·³è¿çåè½ï¼ä½ æ³ä¸å°ä¸ä¸ª
-      csv æä»¶åæ¥è½å¹²è¿ä¹å¤äºæï¼
-    * æä¾äºåè½å¼ºå¤§çæ§è¡å¨å¥å£ï¼è®©ä½ å¯ä»¥æ¹ä¾¿çå¨æ¬å°æ§è¡ä»»ä½ç¨ä¾éçç¨ä¾ï¼å¶ä¸°å¯çèªå®ä¹éç½®é¡¹ï¼æ»¡è¶³ä½ å¯¹æ§è¡å¨ææçå¹»æ³ï¼
-    * æä¾è¿ç¨æ§è¡çåè½ï¼å¯ä»¥æ§å¶å¤å°æºå¨å¹¶è¡è·ï¼æèåå¸å¼è·ï¼è¿ç§ä»è´¹åè½ç°å¨åè´¹ç»ä½ ç¨ï¼
-    * æä¾èªå¨è¾åºæ¥å¿çåè½ï¼ä½ åä¹ä¸ç¨ä¸ºæ¯ä¸ªæ¹æ³åç¬åè¾åºæ¥å¿çä»£ç ï¼ä¸åæä»¬ç»ä½ æå®äºï¼æ¥å¿è¾åºä¸ä»åå®¹ä¸°å¯ï¼é¢å¼ä¹ç»å¯¹å¨çº¿ï¼æä»¬è¿èªå·±è®¾è®¡äºä¸æ¬¾ç»ç«¯è¾åºä¸»é¢å«ãäºå½©ææçé»ãï¼
-    * æä¾ä¸é®é¨ç½²èªå¨åæµè¯ç¯å¢çåè½ï¼è®©ä½ åä¹ä¸ç¨ä¸ºç¯å¢é¨ç½²èç¦æ¼ï¼
-    * æä¾èªå¨çæå¤ç§æ¥åçåè½ï¼ä½ æ³è¾åºä»ä¹æ¥åå½¢å¼é½è¡ï¼èä¸æä»¬å¨æ¥åä¸­è¿å å¥äºå¤±è´¥å½å±åå¤±è´¥æªå¾çåè½ï¼
-    * å¯¹æ­è¨è¿è¡äºäºæ¬¡å°è£ï¼æä¾æ´åå¥½åçéè¯¯æç¤ºï¼è®©å®ä½é®é¢ç²¾åé«æï¼
-    * ä¸ä»æ¯æåæ¡ç¨ä¾è¶æ¶æ§å¶ï¼èä¸è¿æ¯æå¨ææ§å¶ç¨ä¾æ¹éæ§è¡çæ»æ¶é´ï¼ç¡®ä¿
-      CI ç¯å¢ä¸è½é¡ºçè¿è¡ï¼
-    * æ¯ææ¬å°æä»¶æµè¯å¥æ§è¡ãPMS
-      æµè¯å¥æ§è¡ãæ ç­¾åæ§è¡æ¹æ¡ï¼æ»¡è¶³ä½ åç§åºæ¯ä¸çæ§è¡éæ±ï¼
-    * æ¯æåºäºæ·±åº¦å­¦ä¹ ç OCR
-      åè½ï¼å¯å®ä½å¯æ­è¨ï¼ä¸­æè¯å«çå¤©è±æ¿ï¼
-    * å®ç¾å¼å®¹ Wayland å X11ï¼çæ­£åå°ä¸å¥ä»£ç ï¼éå¤æ§è¡ï¼
-    * æ¯æå¤ç§æ¹å¼çæ°æ®åå¡«åè½ï¼å¶ä¸­å¼æ­¥åå¡«çæ¹æ¡ï¼å®ç¾è§£å³äºæ°æ®åå¡«çèæ¶é®é¢ï¼
-    * æ¯æéå¯äº¤äºåºæ¯ç¨ä¾çæ§è¡ï¼ä½¿ç¨æ¹æ³ä¼éç®æ´ï¼
-## å®è£ ä» PyPI å®è£: ```shell $ sudo pip3 install youqu ``` ##
-åå»ºé¡¹ç® æ¨å¯ä»¥å¨ä»»æç®å½ä¸ï¼ä½¿ç¨ `youqu-startproject`
+X11ãWayland æ¾ç¤ºåè®®ï¼ç¯å¢é¨ç½²ç®åï¼æä½æä¸æãð¥ ##
+YouQuï¼æè¶£ï¼è½åä»ä¹ - [x] ð» Linux æ¡é¢åºç¨ UI èªå¨åæµè¯
+- [x] ð Web UI èªå¨åæµè¯ - [x] ð Linux DBus æ¥å£èªå¨åæµè¯ -
+[x] ð å½ä»¤è¡èªå¨åæµè¯ - [x] ð·ï¸ HTTP æ¥å£èªå¨åæµè¯ -
+[ ] â²ï¸ Linux æ¡é¢åºç¨æ§è½èªå¨åæµè¯ ## å®è£ ä» PyPI å®è£:
+```shell $ sudo pip3 install youqu ``` ä¸å  sudo ?
+å¶å®ä¸å  sudo ä¹æ¯å¯ä»¥çï¼
+
+  pip3 install youqu
+
+ä½æäºæåµä¸å¯è½åºç° youqu-startproject
+å½ä»¤æ æ³ä½¿ç¨ï¼è¿æ¯å ä¸ºä¸å  sudo æ¶ï¼å®è£åè·¯å¾æ¯å¨
+$HOME/.local/lib/pythonX.X/site-
+packagesï¼èæ­¤è·¯å¾å¯è½ä¸å¨ç¯å¢åéï¼PATHï¼ä¸­ï¼æ¨å¯ä»¥éè¿æ·»å ç¯å¢åéçæ¹å¼ä½¿ç¨
+youqu-startproject å½ä»¤ï¼
+
+  export PATH=$PATH:$HOME/.local/lib/pythonX.X/site-packages
+## åå»ºé¡¹ç® æ¨å¯ä»¥å¨ä»»æç®å½ä¸ï¼ä½¿ç¨ `youqu-startproject`
 å½ä»¤åå»ºä¸ä¸ªé¡¹ç®ï¼ ```shell $ youqu-startproject my_project ``` å¦æ
 `youqu-startproject` åé¢ä¸å åæ°ï¼é»è®¤çé¡¹ç®åç§°ä¸ºï¼`youqu`
 ï¼ ![](./docs/assets/install.gif) ## å®è£ä¾èµ å®è£é¨ç½² YouQu
 æ§è¡æéç¯å¢ï¼ ```shell $ cd my_project $ bash env.sh ``` ## åå»º APP
 å·¥ç¨ ä½¿ç¨ `startapp` å½ä»¤èªå¨åå»º APP å·¥ç¨ï¼ ```shell $ youqu
 manage.py startapp autotest_deepin_some ``` èªå¨åå»ºç APP
 å·¥ç¨éµå¾ªå®æ´ç PO
```

