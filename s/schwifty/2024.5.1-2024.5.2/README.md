# Comparing `tmp/schwifty-2024.5.1.tar.gz` & `tmp/schwifty-2024.5.2.tar.gz`

## Comparing `schwifty-2024.5.1.tar` & `schwifty-2024.5.2.tar`

### file list

```diff
@@ -1,129 +1,129 @@
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 schwifty-2024.5.1/.envrc
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 schwifty-2024.5.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 schwifty-2024.5.1/.readthedocs.yml
--rw-r--r--   0        0        0    20764 2020-02-02 00:00:00.000000 schwifty-2024.5.1/CHANGELOG.rst
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 schwifty-2024.5.1/Makefile
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 schwifty-2024.5.1/devbox.json
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 schwifty-2024.5.1/devbox.lock
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 schwifty-2024.5.1/.github/workflows/lint-and-test.yml
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 schwifty-2024.5.1/.github/workflows/publish.yml
--rw-r--r--   0        0        0     7673 2020-02-02 00:00:00.000000 schwifty-2024.5.1/docs/Makefile
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 schwifty-2024.5.1/docs/requirements.txt
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 schwifty-2024.5.1/docs/source/api.rst
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 schwifty-2024.5.1/docs/source/changelog.rst
--rw-r--r--   0        0        0     6847 2020-02-02 00:00:00.000000 schwifty-2024.5.1/docs/source/conf.py
--rw-r--r--   0        0        0     7562 2020-02-02 00:00:00.000000 schwifty-2024.5.1/docs/source/examples.rst
--rw-r--r--   0        0        0   366898 2020-02-02 00:00:00.000000 schwifty-2024.5.1/docs/source/ilikewhatugot.png
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 schwifty-2024.5.1/docs/source/index.rst
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 schwifty-2024.5.1/docs/source/troubleshooting.rst
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/__init__.py
--rw-r--r--   0        0        0     8868 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bban.py
--rw-r--r--   0        0        0    16894 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bic.py
--rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/common.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/domain.py
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/exceptions.py
--rw-r--r--   0        0        0    14458 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/iban.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/py.typed
--rw-r--r--   0        0        0     3053 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/registry.py
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/README.md
--rw-r--r--   0        0        0   191535 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/generated_at.json
--rw-r--r--   0        0        0     4617 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/generated_ba.json
--rw-r--r--   0        0        0   134356 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/generated_be.json
--rw-r--r--   0        0        0   218276 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/generated_ch.json
--rw-r--r--   0        0        0    10930 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/generated_cz.json
--rw-r--r--   0        0        0  1064251 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/generated_de.json
--rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/generated_ee.json
--rw-r--r--   0        0        0   105235 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/generated_es.json
--rw-r--r--   0        0        0   123774 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/generated_fi.json
--rw-r--r--   0        0        0     3460 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/generated_ge.json
--rw-r--r--   0        0        0     4520 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/generated_hr.json
--rw-r--r--   0        0        0    31389 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/generated_hu.json
--rw-r--r--   0        0        0    59696 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/generated_it.json
--rw-r--r--   0        0        0    18148 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/generated_kz.json
--rw-r--r--   0        0        0    56450 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/generated_lt.json
--rw-r--r--   0        0        0     5308 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/generated_lv.json
--rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/generated_md.json
--rw-r--r--   0        0        0    14272 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/generated_nl.json
--rw-r--r--   0        0        0   406123 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/generated_no.json
--rw-r--r--   0        0        0   768164 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/generated_pl.json
--rw-r--r--   0        0        0     9274 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/generated_ro.json
--rw-r--r--   0        0        0     5101 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/generated_rs.json
--rw-r--r--   0        0        0     6024 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/generated_se.json
--rw-r--r--   0        0        0   145633 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/generated_si.json
--rw-r--r--   0        0        0     9331 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/generated_sk.json
--rw-r--r--   0        0        0  1752206 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/generated_ua.json
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/manual_ad.json
--rw-r--r--   0        0        0    10224 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/manual_ae.json
--rw-r--r--   0        0        0     4479 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/manual_bg.json
--rw-r--r--   0        0        0     4593 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/manual_cr.json
--rw-r--r--   0        0        0     8729 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/manual_cy.json
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/manual_dk.json
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/manual_es.json
--rw-r--r--   0        0        0    68361 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/manual_fr.json
--rw-r--r--   0        0        0     7604 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/manual_gb.json
--rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/manual_gr.json
--rw-r--r--   0        0        0     5493 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/manual_ie.json
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/manual_il.json
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/manual_is.json
--rw-r--r--   0        0        0    26893 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/manual_it.json
--rw-r--r--   0        0        0    21031 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/manual_lu.json
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/manual_mc.json
--rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/manual_me.json
--rw-r--r--   0        0        0    17257 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/manual_pt.json
--rw-r--r--   0        0        0    25035 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/manual_sa.json
--rw-r--r--   0        0        0    10797 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/manual_tr.json
--rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/checksum/__init__.py
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/checksum/albania.py
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/checksum/belgium.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/checksum/czech_republic.py
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/checksum/estonia.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/checksum/finland.py
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/checksum/france.py
--rw-r--r--   0        0        0    15549 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/checksum/germany.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/checksum/iceland.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/checksum/iso7064_mod97_10.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/checksum/iso7064_mod97_10_variant.py
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/checksum/italy.py
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/checksum/netherlands.py
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/checksum/norway.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/checksum/poland.py
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/checksum/registry.py
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/checksum/spain.py
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/iban_registry/README.md
--rw-r--r--   0        0        0    33306 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/iban_registry/generated.json
--rw-r--r--   0        0        0    16740 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/iban_registry/overwrite.json
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 schwifty-2024.5.1/scripts/Dockerfile_se
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 schwifty-2024.5.1/scripts/README.md
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 schwifty-2024.5.1/scripts/get_bank_registry_at.py
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 schwifty-2024.5.1/scripts/get_bank_registry_be.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 schwifty-2024.5.1/scripts/get_bank_registry_ch.py
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 schwifty-2024.5.1/scripts/get_bank_registry_cz.py
--rwxr-xr-x   0        0        0     2066 2020-02-02 00:00:00.000000 schwifty-2024.5.1/scripts/get_bank_registry_de.py
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 schwifty-2024.5.1/scripts/get_bank_registry_es.py
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 schwifty-2024.5.1/scripts/get_bank_registry_fi.py
--rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 schwifty-2024.5.1/scripts/get_bank_registry_hr.py
--rwxr-xr-x   0        0        0     1213 2020-02-02 00:00:00.000000 schwifty-2024.5.1/scripts/get_bank_registry_hu.py
--rw-r--r--   0        0        0     8112 2020-02-02 00:00:00.000000 schwifty-2024.5.1/scripts/get_bank_registry_it.py
--rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 schwifty-2024.5.1/scripts/get_bank_registry_lt.py
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 schwifty-2024.5.1/scripts/get_bank_registry_lv.py
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 schwifty-2024.5.1/scripts/get_bank_registry_nl.py
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 schwifty-2024.5.1/scripts/get_bank_registry_no.py
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 schwifty-2024.5.1/scripts/get_bank_registry_pl.py
--rwxr-xr-x   0        0        0     1110 2020-02-02 00:00:00.000000 schwifty-2024.5.1/scripts/get_bank_registry_ro.py
--rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 schwifty-2024.5.1/scripts/get_bank_registry_se.py
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 schwifty-2024.5.1/scripts/get_bank_registry_si.py
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 schwifty-2024.5.1/scripts/get_bank_registry_sk.py
--rw-r--r--   0        0        0     2483 2020-02-02 00:00:00.000000 schwifty-2024.5.1/scripts/get_bank_registry_ua.py
--rwxr-xr-x   0        0        0     3190 2020-02-02 00:00:00.000000 schwifty-2024.5.1/scripts/get_iban_registry.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 schwifty-2024.5.1/scripts/requirements.txt
--rwxr-xr-x   0        0        0      322 2020-02-02 00:00:00.000000 schwifty-2024.5.1/scripts/update-all.sh
--rw-r--r--   0        0        0     7669 2020-02-02 00:00:00.000000 schwifty-2024.5.1/tests/test_bic.py
--rw-r--r--   0        0        0     3480 2020-02-02 00:00:00.000000 schwifty-2024.5.1/tests/test_checksum.py
--rw-r--r--   0        0        0    15450 2020-02-02 00:00:00.000000 schwifty-2024.5.1/tests/test_iban.py
--rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 schwifty-2024.5.1/tests/test_registry.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 schwifty-2024.5.1/.gitignore
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 schwifty-2024.5.1/LICENSE
--rw-r--r--   0        0        0     3528 2020-02-02 00:00:00.000000 schwifty-2024.5.1/README.rst
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 schwifty-2024.5.1/hatch.toml
--rw-r--r--   0        0        0     2283 2020-02-02 00:00:00.000000 schwifty-2024.5.1/pyproject.toml
--rw-r--r--   0        0        0     4710 2020-02-02 00:00:00.000000 schwifty-2024.5.1/PKG-INFO
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 schwifty-2024.5.2/.envrc
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 schwifty-2024.5.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 schwifty-2024.5.2/.readthedocs.yml
+-rw-r--r--   0        0        0    21004 2020-02-02 00:00:00.000000 schwifty-2024.5.2/CHANGELOG.rst
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 schwifty-2024.5.2/Makefile
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 schwifty-2024.5.2/devbox.json
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 schwifty-2024.5.2/devbox.lock
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 schwifty-2024.5.2/.github/workflows/lint-and-test.yml
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 schwifty-2024.5.2/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     7673 2020-02-02 00:00:00.000000 schwifty-2024.5.2/docs/Makefile
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 schwifty-2024.5.2/docs/requirements.txt
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 schwifty-2024.5.2/docs/source/api.rst
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 schwifty-2024.5.2/docs/source/changelog.rst
+-rw-r--r--   0        0        0     6847 2020-02-02 00:00:00.000000 schwifty-2024.5.2/docs/source/conf.py
+-rw-r--r--   0        0        0     7562 2020-02-02 00:00:00.000000 schwifty-2024.5.2/docs/source/examples.rst
+-rw-r--r--   0        0        0   366898 2020-02-02 00:00:00.000000 schwifty-2024.5.2/docs/source/ilikewhatugot.png
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 schwifty-2024.5.2/docs/source/index.rst
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 schwifty-2024.5.2/docs/source/troubleshooting.rst
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 schwifty-2024.5.2/schwifty/__init__.py
+-rw-r--r--   0        0        0     8868 2020-02-02 00:00:00.000000 schwifty-2024.5.2/schwifty/bban.py
+-rw-r--r--   0        0        0    16894 2020-02-02 00:00:00.000000 schwifty-2024.5.2/schwifty/bic.py
+-rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 schwifty-2024.5.2/schwifty/common.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 schwifty-2024.5.2/schwifty/domain.py
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 schwifty-2024.5.2/schwifty/exceptions.py
+-rw-r--r--   0        0        0    14458 2020-02-02 00:00:00.000000 schwifty-2024.5.2/schwifty/iban.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 schwifty-2024.5.2/schwifty/py.typed
+-rw-r--r--   0        0        0     3053 2020-02-02 00:00:00.000000 schwifty-2024.5.2/schwifty/registry.py
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 schwifty-2024.5.2/schwifty/bank_registry/README.md
+-rw-r--r--   0        0        0   191535 2020-02-02 00:00:00.000000 schwifty-2024.5.2/schwifty/bank_registry/generated_at.json
+-rw-r--r--   0        0        0     4617 2020-02-02 00:00:00.000000 schwifty-2024.5.2/schwifty/bank_registry/generated_ba.json
+-rw-r--r--   0        0        0   134356 2020-02-02 00:00:00.000000 schwifty-2024.5.2/schwifty/bank_registry/generated_be.json
+-rw-r--r--   0        0        0   218276 2020-02-02 00:00:00.000000 schwifty-2024.5.2/schwifty/bank_registry/generated_ch.json
+-rw-r--r--   0        0        0    10930 2020-02-02 00:00:00.000000 schwifty-2024.5.2/schwifty/bank_registry/generated_cz.json
+-rw-r--r--   0        0        0  1064251 2020-02-02 00:00:00.000000 schwifty-2024.5.2/schwifty/bank_registry/generated_de.json
+-rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 schwifty-2024.5.2/schwifty/bank_registry/generated_ee.json
+-rw-r--r--   0        0        0   105235 2020-02-02 00:00:00.000000 schwifty-2024.5.2/schwifty/bank_registry/generated_es.json
+-rw-r--r--   0        0        0   123774 2020-02-02 00:00:00.000000 schwifty-2024.5.2/schwifty/bank_registry/generated_fi.json
+-rw-r--r--   0        0        0     3460 2020-02-02 00:00:00.000000 schwifty-2024.5.2/schwifty/bank_registry/generated_ge.json
+-rw-r--r--   0        0        0     4520 2020-02-02 00:00:00.000000 schwifty-2024.5.2/schwifty/bank_registry/generated_hr.json
+-rw-r--r--   0        0        0    31389 2020-02-02 00:00:00.000000 schwifty-2024.5.2/schwifty/bank_registry/generated_hu.json
+-rw-r--r--   0        0        0    59696 2020-02-02 00:00:00.000000 schwifty-2024.5.2/schwifty/bank_registry/generated_it.json
+-rw-r--r--   0        0        0    18148 2020-02-02 00:00:00.000000 schwifty-2024.5.2/schwifty/bank_registry/generated_kz.json
+-rw-r--r--   0        0        0    56450 2020-02-02 00:00:00.000000 schwifty-2024.5.2/schwifty/bank_registry/generated_lt.json
+-rw-r--r--   0        0        0     5308 2020-02-02 00:00:00.000000 schwifty-2024.5.2/schwifty/bank_registry/generated_lv.json
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 schwifty-2024.5.2/schwifty/bank_registry/generated_md.json
+-rw-r--r--   0        0        0    14272 2020-02-02 00:00:00.000000 schwifty-2024.5.2/schwifty/bank_registry/generated_nl.json
+-rw-r--r--   0        0        0   406123 2020-02-02 00:00:00.000000 schwifty-2024.5.2/schwifty/bank_registry/generated_no.json
+-rw-r--r--   0        0        0   768164 2020-02-02 00:00:00.000000 schwifty-2024.5.2/schwifty/bank_registry/generated_pl.json
+-rw-r--r--   0        0        0     9274 2020-02-02 00:00:00.000000 schwifty-2024.5.2/schwifty/bank_registry/generated_ro.json
+-rw-r--r--   0        0        0     5101 2020-02-02 00:00:00.000000 schwifty-2024.5.2/schwifty/bank_registry/generated_rs.json
+-rw-r--r--   0        0        0     6024 2020-02-02 00:00:00.000000 schwifty-2024.5.2/schwifty/bank_registry/generated_se.json
+-rw-r--r--   0        0        0   145633 2020-02-02 00:00:00.000000 schwifty-2024.5.2/schwifty/bank_registry/generated_si.json
+-rw-r--r--   0        0        0     9331 2020-02-02 00:00:00.000000 schwifty-2024.5.2/schwifty/bank_registry/generated_sk.json
+-rw-r--r--   0        0        0  1752206 2020-02-02 00:00:00.000000 schwifty-2024.5.2/schwifty/bank_registry/generated_ua.json
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 schwifty-2024.5.2/schwifty/bank_registry/manual_ad.json
+-rw-r--r--   0        0        0    10224 2020-02-02 00:00:00.000000 schwifty-2024.5.2/schwifty/bank_registry/manual_ae.json
+-rw-r--r--   0        0        0     4479 2020-02-02 00:00:00.000000 schwifty-2024.5.2/schwifty/bank_registry/manual_bg.json
+-rw-r--r--   0        0        0     4593 2020-02-02 00:00:00.000000 schwifty-2024.5.2/schwifty/bank_registry/manual_cr.json
+-rw-r--r--   0        0        0     8729 2020-02-02 00:00:00.000000 schwifty-2024.5.2/schwifty/bank_registry/manual_cy.json
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 schwifty-2024.5.2/schwifty/bank_registry/manual_dk.json
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 schwifty-2024.5.2/schwifty/bank_registry/manual_es.json
+-rw-r--r--   0        0        0    68361 2020-02-02 00:00:00.000000 schwifty-2024.5.2/schwifty/bank_registry/manual_fr.json
+-rw-r--r--   0        0        0     7604 2020-02-02 00:00:00.000000 schwifty-2024.5.2/schwifty/bank_registry/manual_gb.json
+-rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 schwifty-2024.5.2/schwifty/bank_registry/manual_gr.json
+-rw-r--r--   0        0        0     5493 2020-02-02 00:00:00.000000 schwifty-2024.5.2/schwifty/bank_registry/manual_ie.json
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 schwifty-2024.5.2/schwifty/bank_registry/manual_il.json
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 schwifty-2024.5.2/schwifty/bank_registry/manual_is.json
+-rw-r--r--   0        0        0    26893 2020-02-02 00:00:00.000000 schwifty-2024.5.2/schwifty/bank_registry/manual_it.json
+-rw-r--r--   0        0        0    21031 2020-02-02 00:00:00.000000 schwifty-2024.5.2/schwifty/bank_registry/manual_lu.json
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 schwifty-2024.5.2/schwifty/bank_registry/manual_mc.json
+-rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 schwifty-2024.5.2/schwifty/bank_registry/manual_me.json
+-rw-r--r--   0        0        0    17257 2020-02-02 00:00:00.000000 schwifty-2024.5.2/schwifty/bank_registry/manual_pt.json
+-rw-r--r--   0        0        0    25035 2020-02-02 00:00:00.000000 schwifty-2024.5.2/schwifty/bank_registry/manual_sa.json
+-rw-r--r--   0        0        0    10797 2020-02-02 00:00:00.000000 schwifty-2024.5.2/schwifty/bank_registry/manual_tr.json
+-rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 schwifty-2024.5.2/schwifty/checksum/__init__.py
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 schwifty-2024.5.2/schwifty/checksum/albania.py
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 schwifty-2024.5.2/schwifty/checksum/belgium.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 schwifty-2024.5.2/schwifty/checksum/czech_republic.py
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 schwifty-2024.5.2/schwifty/checksum/estonia.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 schwifty-2024.5.2/schwifty/checksum/finland.py
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 schwifty-2024.5.2/schwifty/checksum/france.py
+-rw-r--r--   0        0        0    15549 2020-02-02 00:00:00.000000 schwifty-2024.5.2/schwifty/checksum/germany.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 schwifty-2024.5.2/schwifty/checksum/iceland.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 schwifty-2024.5.2/schwifty/checksum/iso7064_mod97_10.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 schwifty-2024.5.2/schwifty/checksum/iso7064_mod97_10_variant.py
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 schwifty-2024.5.2/schwifty/checksum/italy.py
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 schwifty-2024.5.2/schwifty/checksum/netherlands.py
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 schwifty-2024.5.2/schwifty/checksum/norway.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 schwifty-2024.5.2/schwifty/checksum/poland.py
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 schwifty-2024.5.2/schwifty/checksum/registry.py
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 schwifty-2024.5.2/schwifty/checksum/spain.py
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 schwifty-2024.5.2/schwifty/iban_registry/README.md
+-rw-r--r--   0        0        0    33306 2020-02-02 00:00:00.000000 schwifty-2024.5.2/schwifty/iban_registry/generated.json
+-rw-r--r--   0        0        0    16740 2020-02-02 00:00:00.000000 schwifty-2024.5.2/schwifty/iban_registry/overwrite.json
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 schwifty-2024.5.2/scripts/Dockerfile_se
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 schwifty-2024.5.2/scripts/README.md
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 schwifty-2024.5.2/scripts/get_bank_registry_at.py
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 schwifty-2024.5.2/scripts/get_bank_registry_be.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 schwifty-2024.5.2/scripts/get_bank_registry_ch.py
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 schwifty-2024.5.2/scripts/get_bank_registry_cz.py
+-rwxr-xr-x   0        0        0     2066 2020-02-02 00:00:00.000000 schwifty-2024.5.2/scripts/get_bank_registry_de.py
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 schwifty-2024.5.2/scripts/get_bank_registry_es.py
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 schwifty-2024.5.2/scripts/get_bank_registry_fi.py
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 schwifty-2024.5.2/scripts/get_bank_registry_hr.py
+-rwxr-xr-x   0        0        0     1213 2020-02-02 00:00:00.000000 schwifty-2024.5.2/scripts/get_bank_registry_hu.py
+-rw-r--r--   0        0        0     8112 2020-02-02 00:00:00.000000 schwifty-2024.5.2/scripts/get_bank_registry_it.py
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 schwifty-2024.5.2/scripts/get_bank_registry_lt.py
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 schwifty-2024.5.2/scripts/get_bank_registry_lv.py
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 schwifty-2024.5.2/scripts/get_bank_registry_nl.py
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 schwifty-2024.5.2/scripts/get_bank_registry_no.py
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 schwifty-2024.5.2/scripts/get_bank_registry_pl.py
+-rwxr-xr-x   0        0        0     1110 2020-02-02 00:00:00.000000 schwifty-2024.5.2/scripts/get_bank_registry_ro.py
+-rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 schwifty-2024.5.2/scripts/get_bank_registry_se.py
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 schwifty-2024.5.2/scripts/get_bank_registry_si.py
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 schwifty-2024.5.2/scripts/get_bank_registry_sk.py
+-rw-r--r--   0        0        0     2483 2020-02-02 00:00:00.000000 schwifty-2024.5.2/scripts/get_bank_registry_ua.py
+-rwxr-xr-x   0        0        0     3190 2020-02-02 00:00:00.000000 schwifty-2024.5.2/scripts/get_iban_registry.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 schwifty-2024.5.2/scripts/requirements.txt
+-rwxr-xr-x   0        0        0      322 2020-02-02 00:00:00.000000 schwifty-2024.5.2/scripts/update-all.sh
+-rw-r--r--   0        0        0     7669 2020-02-02 00:00:00.000000 schwifty-2024.5.2/tests/test_bic.py
+-rw-r--r--   0        0        0     3480 2020-02-02 00:00:00.000000 schwifty-2024.5.2/tests/test_checksum.py
+-rw-r--r--   0        0        0    15450 2020-02-02 00:00:00.000000 schwifty-2024.5.2/tests/test_iban.py
+-rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 schwifty-2024.5.2/tests/test_registry.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 schwifty-2024.5.2/.gitignore
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 schwifty-2024.5.2/LICENSE
+-rw-r--r--   0        0        0     3528 2020-02-02 00:00:00.000000 schwifty-2024.5.2/README.rst
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 schwifty-2024.5.2/hatch.toml
+-rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 schwifty-2024.5.2/pyproject.toml
+-rw-r--r--   0        0        0     4776 2020-02-02 00:00:00.000000 schwifty-2024.5.2/PKG-INFO
```

### Comparing `schwifty-2024.5.1/CHANGELOG.rst` & `schwifty-2024.5.2/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 .. _changelog:
 
 Changelog
 =========
 
 Versions follow `CalVer <http://www.calver.org/>`_ with the scheme ``YY.0M.Micro``.
 
+`2024.05.2`_ - 2024/05/09
+-------------------------
+Fixed
+~~~~~
+* Add `typing-extensions` as explicit dependency for Python < 3.11 to support the `Self` type.
+
 `2024.05.1`_ - 2024/05/09
 -------------------------
 Changed
 ~~~~~~~
 * Remove custom collection logic of the bank registry for ``pyinstaller``. The changes introduced in
   `#92 <https://github.com/mdomke/schwifty/pull/92>`_ were wrong and have been reverted. Usage
   example
@@ -589,17 +595,18 @@
 -------------------------
 
 Added
 ~~~~~
 * Added :attr:`.BIC.country` and :attr:`.IBAN.country`.
 
 
+.. _2024.05.2: https://github.com/mdomke/schwifty/compare/2024.05.1...2024.05.2
 .. _2024.05.1: https://github.com/mdomke/schwifty/compare/2024.05.0...2024.05.1
 .. _2024.05.0: https://github.com/mdomke/schwifty/compare/2024.04.0...2024.05.0
-.. _2024.04.0: https://github.com/mdomke/schwifty/compare/2023.01.1...2024.04.0
+.. _2024.04.0: https://github.com/mdomke/schwifty/compare/2024.01.1...2024.04.0
 .. _2024.01.1: https://github.com/mdomke/schwifty/compare/2023.11.2...2024.01.1
 .. _2023.11.2: https://github.com/mdomke/schwifty/compare/2023.11.1...2023.11.2
 .. _2023.11.1: https://github.com/mdomke/schwifty/compare/2023.11.0...2023.11.1
 .. _2023.11.0: https://github.com/mdomke/schwifty/compare/2023.10.0...2023.11.0
 .. _2023.10.0: https://github.com/mdomke/schwifty/compare/2023.09.0...2023.10.0
 .. _2023.09.0: https://github.com/mdomke/schwifty/compare/2023.06.0...2023.09.0
 .. _2023.06.0: https://github.com/mdomke/schwifty/compare/2023.03.0...2023.06.0
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_g1o6r5q6_/tmpbe5p7xhn_TarContainer/0/3.rst", line 642, column 0: CDATA terminal not found*

```diff
@@ -1,6 +1,8 @@
 .. _changelog: Changelog ========= Versions follow `CalVer
-www.calver.org/>`_ with the scheme ``YY.0M.Micro``. `2024.05.1`_ - 2024/05/09 -
------------------------- Changed ~~~~~~~ * Remove custom collection logic of
-the bank registry for ``pyinstaller``. The changes introduced in `#92
+www.calver.org/>`_ with the scheme ``YY.0M.Micro``. `2024.05.2`_ - 2024/05/09 -
+------------------------ Fixed ~~~~~ * Add `typing-extensions` as explicit
+dependency for Python < 3.11 to support the `Self` type. `2024.05.1`_ - 2024/
+05/09 ------------------------- Changed ~~~~~~~ * Remove custom collection
+logic of the bank registry for ``pyinstaller``. The changes introduced in `#92
 github.com/mdomke/schwifty/pull/92>`_ were wrong and have been reverted. Usage
 example .. code-block:: bash $ pyinstaller
```

### Comparing `schwifty-2024.5.1/devbox.lock` & `schwifty-2024.5.2/devbox.lock`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/.github/workflows/lint-and-test.yml` & `schwifty-2024.5.2/.github/workflows/lint-and-test.yml`

 * *Files 3% similar despite different names*

```diff
@@ -56,9 +56,11 @@
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
           allow-prereleases: true
       - name: Install dependencies
         run: pip install hatch
+      - name: Smoke test installation
+        run: pip install .
       - name: Test
         run: hatch run cov-test
```

### Comparing `schwifty-2024.5.1/.github/workflows/publish.yml` & `schwifty-2024.5.2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/docs/Makefile` & `schwifty-2024.5.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/docs/source/api.rst` & `schwifty-2024.5.2/docs/source/api.rst`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/docs/source/conf.py` & `schwifty-2024.5.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/docs/source/examples.rst` & `schwifty-2024.5.2/docs/source/examples.rst`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/docs/source/ilikewhatugot.png` & `schwifty-2024.5.2/docs/source/ilikewhatugot.png`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/docs/source/index.rst` & `schwifty-2024.5.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/docs/source/troubleshooting.rst` & `schwifty-2024.5.2/docs/source/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/schwifty/bban.py` & `schwifty-2024.5.2/schwifty/bban.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/schwifty/bic.py` & `schwifty-2024.5.2/schwifty/bic.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/schwifty/common.py` & `schwifty-2024.5.2/schwifty/common.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/schwifty/exceptions.py` & `schwifty-2024.5.2/schwifty/exceptions.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/schwifty/iban.py` & `schwifty-2024.5.2/schwifty/iban.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/schwifty/registry.py` & `schwifty-2024.5.2/schwifty/registry.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/schwifty/bank_registry/README.md` & `schwifty-2024.5.2/schwifty/bank_registry/README.md`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/schwifty/bank_registry/generated_at.json` & `schwifty-2024.5.2/schwifty/bank_registry/generated_at.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/schwifty/bank_registry/generated_ba.json` & `schwifty-2024.5.2/schwifty/bank_registry/generated_ba.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/schwifty/bank_registry/generated_be.json` & `schwifty-2024.5.2/schwifty/bank_registry/generated_be.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/schwifty/bank_registry/generated_ch.json` & `schwifty-2024.5.2/schwifty/bank_registry/generated_ch.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/schwifty/bank_registry/generated_cz.json` & `schwifty-2024.5.2/schwifty/bank_registry/generated_cz.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/schwifty/bank_registry/generated_de.json` & `schwifty-2024.5.2/schwifty/bank_registry/generated_de.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/schwifty/bank_registry/generated_ee.json` & `schwifty-2024.5.2/schwifty/bank_registry/generated_ee.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/schwifty/bank_registry/generated_es.json` & `schwifty-2024.5.2/schwifty/bank_registry/generated_es.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/schwifty/bank_registry/generated_fi.json` & `schwifty-2024.5.2/schwifty/bank_registry/generated_fi.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/schwifty/bank_registry/generated_ge.json` & `schwifty-2024.5.2/schwifty/bank_registry/generated_ge.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/schwifty/bank_registry/generated_hr.json` & `schwifty-2024.5.2/schwifty/bank_registry/generated_hr.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/schwifty/bank_registry/generated_hu.json` & `schwifty-2024.5.2/schwifty/bank_registry/generated_hu.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/schwifty/bank_registry/generated_it.json` & `schwifty-2024.5.2/schwifty/bank_registry/generated_it.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/schwifty/bank_registry/generated_kz.json` & `schwifty-2024.5.2/schwifty/bank_registry/generated_kz.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/schwifty/bank_registry/generated_lt.json` & `schwifty-2024.5.2/schwifty/bank_registry/generated_lt.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/schwifty/bank_registry/generated_lv.json` & `schwifty-2024.5.2/schwifty/bank_registry/generated_lv.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/schwifty/bank_registry/generated_md.json` & `schwifty-2024.5.2/schwifty/bank_registry/generated_md.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/schwifty/bank_registry/generated_nl.json` & `schwifty-2024.5.2/schwifty/bank_registry/generated_nl.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/schwifty/bank_registry/generated_no.json` & `schwifty-2024.5.2/schwifty/bank_registry/generated_no.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/schwifty/bank_registry/generated_pl.json` & `schwifty-2024.5.2/schwifty/bank_registry/generated_pl.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/schwifty/bank_registry/generated_ro.json` & `schwifty-2024.5.2/schwifty/bank_registry/generated_ro.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/schwifty/bank_registry/generated_rs.json` & `schwifty-2024.5.2/schwifty/bank_registry/generated_rs.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/schwifty/bank_registry/generated_se.json` & `schwifty-2024.5.2/schwifty/bank_registry/generated_se.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/schwifty/bank_registry/generated_si.json` & `schwifty-2024.5.2/schwifty/bank_registry/generated_si.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/schwifty/bank_registry/generated_sk.json` & `schwifty-2024.5.2/schwifty/bank_registry/generated_sk.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/schwifty/bank_registry/generated_ua.json` & `schwifty-2024.5.2/schwifty/bank_registry/generated_ua.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/schwifty/bank_registry/manual_ad.json` & `schwifty-2024.5.2/schwifty/bank_registry/manual_ad.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/schwifty/bank_registry/manual_ae.json` & `schwifty-2024.5.2/schwifty/bank_registry/manual_ae.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/schwifty/bank_registry/manual_bg.json` & `schwifty-2024.5.2/schwifty/bank_registry/manual_bg.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/schwifty/bank_registry/manual_cr.json` & `schwifty-2024.5.2/schwifty/bank_registry/manual_cr.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/schwifty/bank_registry/manual_cy.json` & `schwifty-2024.5.2/schwifty/bank_registry/manual_cy.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/schwifty/bank_registry/manual_es.json` & `schwifty-2024.5.2/schwifty/bank_registry/manual_es.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/schwifty/bank_registry/manual_fr.json` & `schwifty-2024.5.2/schwifty/bank_registry/manual_fr.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/schwifty/bank_registry/manual_gb.json` & `schwifty-2024.5.2/schwifty/bank_registry/manual_gb.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/schwifty/bank_registry/manual_gr.json` & `schwifty-2024.5.2/schwifty/bank_registry/manual_gr.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/schwifty/bank_registry/manual_ie.json` & `schwifty-2024.5.2/schwifty/bank_registry/manual_ie.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/schwifty/bank_registry/manual_is.json` & `schwifty-2024.5.2/schwifty/bank_registry/manual_is.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/schwifty/bank_registry/manual_it.json` & `schwifty-2024.5.2/schwifty/bank_registry/manual_it.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/schwifty/bank_registry/manual_lu.json` & `schwifty-2024.5.2/schwifty/bank_registry/manual_lu.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/schwifty/bank_registry/manual_me.json` & `schwifty-2024.5.2/schwifty/bank_registry/manual_me.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/schwifty/bank_registry/manual_pt.json` & `schwifty-2024.5.2/schwifty/bank_registry/manual_pt.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/schwifty/bank_registry/manual_sa.json` & `schwifty-2024.5.2/schwifty/bank_registry/manual_sa.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/schwifty/bank_registry/manual_tr.json` & `schwifty-2024.5.2/schwifty/bank_registry/manual_tr.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/schwifty/checksum/__init__.py` & `schwifty-2024.5.2/schwifty/checksum/__init__.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/schwifty/checksum/czech_republic.py` & `schwifty-2024.5.2/schwifty/checksum/czech_republic.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/schwifty/checksum/estonia.py` & `schwifty-2024.5.2/schwifty/checksum/estonia.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/schwifty/checksum/france.py` & `schwifty-2024.5.2/schwifty/checksum/france.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/schwifty/checksum/germany.py` & `schwifty-2024.5.2/schwifty/checksum/germany.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/schwifty/checksum/iceland.py` & `schwifty-2024.5.2/schwifty/checksum/iceland.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/schwifty/checksum/italy.py` & `schwifty-2024.5.2/schwifty/checksum/italy.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/schwifty/checksum/netherlands.py` & `schwifty-2024.5.2/schwifty/checksum/netherlands.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/schwifty/checksum/norway.py` & `schwifty-2024.5.2/schwifty/checksum/norway.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/schwifty/checksum/poland.py` & `schwifty-2024.5.2/schwifty/checksum/poland.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/schwifty/checksum/spain.py` & `schwifty-2024.5.2/schwifty/checksum/spain.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/schwifty/iban_registry/README.md` & `schwifty-2024.5.2/schwifty/iban_registry/README.md`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/schwifty/iban_registry/generated.json` & `schwifty-2024.5.2/schwifty/iban_registry/generated.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/schwifty/iban_registry/overwrite.json` & `schwifty-2024.5.2/schwifty/iban_registry/overwrite.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/scripts/get_bank_registry_at.py` & `schwifty-2024.5.2/scripts/get_bank_registry_at.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/scripts/get_bank_registry_be.py` & `schwifty-2024.5.2/scripts/get_bank_registry_be.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/scripts/get_bank_registry_ch.py` & `schwifty-2024.5.2/scripts/get_bank_registry_ch.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/scripts/get_bank_registry_cz.py` & `schwifty-2024.5.2/scripts/get_bank_registry_cz.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/scripts/get_bank_registry_de.py` & `schwifty-2024.5.2/scripts/get_bank_registry_de.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/scripts/get_bank_registry_es.py` & `schwifty-2024.5.2/scripts/get_bank_registry_es.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/scripts/get_bank_registry_fi.py` & `schwifty-2024.5.2/scripts/get_bank_registry_fi.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/scripts/get_bank_registry_hr.py` & `schwifty-2024.5.2/scripts/get_bank_registry_hr.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/scripts/get_bank_registry_hu.py` & `schwifty-2024.5.2/scripts/get_bank_registry_hu.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/scripts/get_bank_registry_it.py` & `schwifty-2024.5.2/scripts/get_bank_registry_it.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/scripts/get_bank_registry_lt.py` & `schwifty-2024.5.2/scripts/get_bank_registry_lt.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/scripts/get_bank_registry_lv.py` & `schwifty-2024.5.2/scripts/get_bank_registry_lv.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/scripts/get_bank_registry_nl.py` & `schwifty-2024.5.2/scripts/get_bank_registry_nl.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/scripts/get_bank_registry_no.py` & `schwifty-2024.5.2/scripts/get_bank_registry_no.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/scripts/get_bank_registry_pl.py` & `schwifty-2024.5.2/scripts/get_bank_registry_pl.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/scripts/get_bank_registry_ro.py` & `schwifty-2024.5.2/scripts/get_bank_registry_ro.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/scripts/get_bank_registry_se.py` & `schwifty-2024.5.2/scripts/get_bank_registry_se.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/scripts/get_bank_registry_si.py` & `schwifty-2024.5.2/scripts/get_bank_registry_si.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/scripts/get_bank_registry_sk.py` & `schwifty-2024.5.2/scripts/get_bank_registry_sk.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/scripts/get_bank_registry_ua.py` & `schwifty-2024.5.2/scripts/get_bank_registry_ua.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/scripts/get_iban_registry.py` & `schwifty-2024.5.2/scripts/get_iban_registry.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/tests/test_bic.py` & `schwifty-2024.5.2/tests/test_bic.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/tests/test_checksum.py` & `schwifty-2024.5.2/tests/test_checksum.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/tests/test_iban.py` & `schwifty-2024.5.2/tests/test_iban.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/tests/test_registry.py` & `schwifty-2024.5.2/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/LICENSE` & `schwifty-2024.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/README.rst` & `schwifty-2024.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/hatch.toml` & `schwifty-2024.5.2/hatch.toml`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.1/pyproject.toml` & `schwifty-2024.5.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 ]
 requires-python = ">=3.8"
 authors = [
     { name = "Martin Domke", email = "mail@martindomke.net" },
 ]
 dependencies = [
     "importlib_resources>=5.10; python_version <= '3.11'",
+    "typing-extensions>=4.0.1; python_version <= '3.10'",
     "pycountry",
 ]
 
 [project.optional-dependencies]
 pydantic = [
     "pydantic>=2.0"
 ]
```

### Comparing `schwifty-2024.5.1/PKG-INFO` & `schwifty-2024.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: schwifty
-Version: 2024.5.1
+Version: 2024.5.2
 Project-URL: Changelog, https://github.com/mdomke/schwifty/blob/main/CHANGELOG.rst
 Project-URL: Documentation, https://schwifty.readthedocs.io/en/latest/
 Project-URL: Homepage, http://github.com/mdomke/schwifty
 Author-email: Martin Domke <mail@martindomke.net>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,14 +18,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Office/Business :: Financial
 Requires-Python: >=3.8
 Requires-Dist: importlib-resources>=5.10; python_version <= '3.11'
 Requires-Dist: pycountry
+Requires-Dist: typing-extensions>=4.0.1; python_version <= '3.10'
 Provides-Extra: pydantic
 Requires-Dist: pydantic>=2.0; extra == 'pydantic'
 Description-Content-Type: text/x-rst
 
 .. image:: https://img.shields.io/pypi/v/schwifty.svg?style=flat-square
     :target: https://pypi.python.org/pypi/schwifty
 .. image:: https://img.shields.io/github/actions/workflow/status/mdomke/schwifty/lint-and-test.yml?branch=main&style=flat-square
```

