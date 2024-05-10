# Comparing `tmp/molecule-qemu-0.5.8.tar.gz` & `tmp/molecule-qemu-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molecule-qemu-0.5.8.tar", last modified: Wed Feb 21 09:26:45 2024, max compression
+gzip compressed data, was "molecule-qemu-0.5.9.tar", last modified: Sun Mar  3 10:46:10 2024, max compression
```

## Comparing `molecule-qemu-0.5.8.tar` & `molecule-qemu-0.5.9.tar`

### file list

```diff
@@ -1,114 +1,112 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 09:26:45.787474 molecule-qemu-0.5.8/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/.ansible-lint
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 09:26:45.767474 molecule-qemu-0.5.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 09:26:45.771474 molecule-qemu-0.5.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/.github/workflows/ansible-lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/.github/workflows/ansible-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/.github/workflows/python-lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/.github/workflows/python-release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 09:26:45.771474 molecule-qemu-0.5.8/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/.yamllint
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     8616 2024-02-21 09:26:45.787474 molecule-qemu-0.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8304 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 09:26:45.771474 molecule-qemu-0.5.8/molecule_qemu/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/molecule_qemu/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 09:26:45.771474 molecule-qemu-0.5.8/molecule_qemu/cookiecutter/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/molecule_qemu/cookiecutter/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 09:26:45.767474 molecule-qemu-0.5.8/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 09:26:45.771474 molecule-qemu-0.5.8/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/collections.yml
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/prepare.yml
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/requirements.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/molecule_qemu/driver.json
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/molecule_qemu/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 09:26:45.779474 molecule-qemu-0.5.8/molecule_qemu/playbooks/
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/molecule_qemu/playbooks/cleanup.yml
--rw-r--r--   0 runner    (1001) docker     (127)    15420 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/molecule_qemu/playbooks/create.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/molecule_qemu/playbooks/destroy.yml
--rw-r--r--   0 runner    (1001) docker     (127)  2097152 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/molecule_qemu/playbooks/edk2-aarch64.fd
--rw-r--r--   0 runner    (1001) docker     (127)  2097152 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/molecule_qemu/playbooks/edk2-x86_64.fd
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/molecule_qemu/playbooks/side_effect.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 09:26:45.779474 molecule-qemu-0.5.8/molecule_qemu/playbooks/templates/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/molecule_qemu/playbooks/templates/meta-data.j2
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/molecule_qemu/playbooks/templates/user-data.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 09:26:45.787474 molecule-qemu-0.5.8/molecule_qemu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8616 2024-02-21 09:26:45.000000 molecule-qemu-0.5.8/molecule_qemu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-02-21 09:26:45.000000 molecule-qemu-0.5.8/molecule_qemu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-21 09:26:45.000000 molecule-qemu-0.5.8/molecule_qemu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-21 09:26:45.000000 molecule-qemu-0.5.8/molecule_qemu.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-21 09:26:45.000000 molecule-qemu-0.5.8/molecule_qemu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-21 09:26:45.000000 molecule-qemu-0.5.8/molecule_qemu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/requirements.yml
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-02-21 09:26:45.787474 molecule-qemu-0.5.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 09:26:45.779474 molecule-qemu-0.5.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/tests/.yamllint
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 09:26:45.767474 molecule-qemu-0.5.8/tests/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 09:26:45.779474 molecule-qemu-0.5.8/tests/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/tests/molecule/default/collections.yml
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/tests/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/tests/molecule/default/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/tests/molecule/default/prepare.yml
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/tests/molecule/default/requirements.yml
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/tests/molecule/default/verify.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 09:26:45.779474 molecule-qemu-0.5.8/tests/molecule/network-shared/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/tests/molecule/network-shared/collections.yml
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/tests/molecule/network-shared/converge.yml
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/tests/molecule/network-shared/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/tests/molecule/network-shared/prepare.yml
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/tests/molecule/network-shared/requirements.yml
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/tests/molecule/network-shared/verify.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 09:26:45.783474 molecule-qemu-0.5.8/tests/molecule/network-user/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/tests/molecule/network-user/collections.yml
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/tests/molecule/network-user/converge.yml
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/tests/molecule/network-user/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/tests/molecule/network-user/prepare.yml
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/tests/molecule/network-user/requirements.yml
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/tests/molecule/network-user/verify.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 09:26:45.783474 molecule-qemu-0.5.8/tests/molecule/os-debian-bookworm/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/tests/molecule/os-debian-bookworm/collections.yml
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/tests/molecule/os-debian-bookworm/converge.yml
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/tests/molecule/os-debian-bookworm/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/tests/molecule/os-debian-bookworm/prepare.yml
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/tests/molecule/os-debian-bookworm/requirements.yml
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/tests/molecule/os-debian-bookworm/verify.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 09:26:45.783474 molecule-qemu-0.5.8/tests/molecule/os-debian-bullseye/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/tests/molecule/os-debian-bullseye/collections.yml
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/tests/molecule/os-debian-bullseye/converge.yml
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/tests/molecule/os-debian-bullseye/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/tests/molecule/os-debian-bullseye/prepare.yml
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/tests/molecule/os-debian-bullseye/requirements.yml
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/tests/molecule/os-debian-bullseye/verify.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 09:26:45.783474 molecule-qemu-0.5.8/tests/molecule/os-ubuntu-focal/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/tests/molecule/os-ubuntu-focal/collections.yml
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/tests/molecule/os-ubuntu-focal/converge.yml
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/tests/molecule/os-ubuntu-focal/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/tests/molecule/os-ubuntu-focal/prepare.yml
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/tests/molecule/os-ubuntu-focal/requirements.yml
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/tests/molecule/os-ubuntu-focal/verify.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 09:26:45.787474 molecule-qemu-0.5.8/tests/molecule/os-ubuntu-jammy/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/tests/molecule/os-ubuntu-jammy/collections.yml
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/tests/molecule/os-ubuntu-jammy/converge.yml
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/tests/molecule/os-ubuntu-jammy/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/tests/molecule/os-ubuntu-jammy/prepare.yml
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/tests/molecule/os-ubuntu-jammy/requirements.yml
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/tests/molecule/os-ubuntu-jammy/verify.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 09:26:45.787474 molecule-qemu-0.5.8/tests/molecule/platform-amd64/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/tests/molecule/platform-amd64/collections.yml
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/tests/molecule/platform-amd64/converge.yml
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/tests/molecule/platform-amd64/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/tests/molecule/platform-amd64/prepare.yml
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/tests/molecule/platform-amd64/requirements.yml
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/tests/molecule/platform-amd64/verify.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 09:26:45.787474 molecule-qemu-0.5.8/tests/molecule/platform-arm64/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/tests/molecule/platform-arm64/collections.yml
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/tests/molecule/platform-arm64/converge.yml
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/tests/molecule/platform-arm64/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/tests/molecule/platform-arm64/prepare.yml
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/tests/molecule/platform-arm64/requirements.yml
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-02-21 09:26:38.000000 molecule-qemu-0.5.8/tests/molecule/platform-arm64/verify.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 10:46:10.092475 molecule-qemu-0.5.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/.ansible-lint
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 10:46:10.072475 molecule-qemu-0.5.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 10:46:10.076475 molecule-qemu-0.5.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/.github/workflows/ansible-lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/.github/workflows/ansible-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/.github/workflows/python-lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/.github/workflows/python-release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/.yamllint
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     8974 2024-03-03 10:46:10.092475 molecule-qemu-0.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8662 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 10:46:10.076475 molecule-qemu-0.5.9/molecule_qemu/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/molecule_qemu/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 10:46:10.076475 molecule-qemu-0.5.9/molecule_qemu/cookiecutter/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/molecule_qemu/cookiecutter/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 10:46:10.072475 molecule-qemu-0.5.9/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 10:46:10.076475 molecule-qemu-0.5.9/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/collections.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/prepare.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/molecule_qemu/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2661 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/molecule_qemu/driver.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/molecule_qemu/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 10:46:10.084474 molecule-qemu-0.5.9/molecule_qemu/playbooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/molecule_qemu/playbooks/cleanup.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    16058 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/molecule_qemu/playbooks/create.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/molecule_qemu/playbooks/destroy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)  2097152 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/molecule_qemu/playbooks/edk2-aarch64.fd
+-rw-r--r--   0 runner    (1001) docker     (127)  2097152 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/molecule_qemu/playbooks/edk2-x86_64.fd
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/molecule_qemu/playbooks/side_effect.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 10:46:10.084474 molecule-qemu-0.5.9/molecule_qemu/playbooks/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/molecule_qemu/playbooks/templates/meta-data.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/molecule_qemu/playbooks/templates/user-data.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 10:46:10.092475 molecule-qemu-0.5.9/molecule_qemu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8974 2024-03-03 10:46:10.000000 molecule-qemu-0.5.9/molecule_qemu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3723 2024-03-03 10:46:10.000000 molecule-qemu-0.5.9/molecule_qemu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-03 10:46:10.000000 molecule-qemu-0.5.9/molecule_qemu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-03 10:46:10.000000 molecule-qemu-0.5.9/molecule_qemu.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-03 10:46:10.000000 molecule-qemu-0.5.9/molecule_qemu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-03 10:46:10.000000 molecule-qemu-0.5.9/molecule_qemu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-03 10:46:10.096475 molecule-qemu-0.5.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 10:46:10.084474 molecule-qemu-0.5.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/tests/.yamllint
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 10:46:10.072475 molecule-qemu-0.5.9/tests/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 10:46:10.084474 molecule-qemu-0.5.9/tests/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/tests/molecule/default/collections.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/tests/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/tests/molecule/default/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/tests/molecule/default/prepare.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/tests/molecule/default/requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/tests/molecule/default/verify.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 10:46:10.088475 molecule-qemu-0.5.9/tests/molecule/network-shared/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/tests/molecule/network-shared/collections.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/tests/molecule/network-shared/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/tests/molecule/network-shared/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/tests/molecule/network-shared/prepare.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/tests/molecule/network-shared/requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/tests/molecule/network-shared/verify.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 10:46:10.088475 molecule-qemu-0.5.9/tests/molecule/network-user/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/tests/molecule/network-user/collections.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/tests/molecule/network-user/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/tests/molecule/network-user/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/tests/molecule/network-user/prepare.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/tests/molecule/network-user/requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/tests/molecule/network-user/verify.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 10:46:10.088475 molecule-qemu-0.5.9/tests/molecule/os-debian-bookworm/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/tests/molecule/os-debian-bookworm/collections.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/tests/molecule/os-debian-bookworm/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/tests/molecule/os-debian-bookworm/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/tests/molecule/os-debian-bookworm/prepare.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/tests/molecule/os-debian-bookworm/requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/tests/molecule/os-debian-bookworm/verify.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 10:46:10.088475 molecule-qemu-0.5.9/tests/molecule/os-debian-bullseye/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/tests/molecule/os-debian-bullseye/collections.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/tests/molecule/os-debian-bullseye/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/tests/molecule/os-debian-bullseye/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/tests/molecule/os-debian-bullseye/prepare.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/tests/molecule/os-debian-bullseye/requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/tests/molecule/os-debian-bullseye/verify.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 10:46:10.092475 molecule-qemu-0.5.9/tests/molecule/os-ubuntu-focal/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/tests/molecule/os-ubuntu-focal/collections.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/tests/molecule/os-ubuntu-focal/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/tests/molecule/os-ubuntu-focal/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/tests/molecule/os-ubuntu-focal/prepare.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/tests/molecule/os-ubuntu-focal/requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/tests/molecule/os-ubuntu-focal/verify.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 10:46:10.092475 molecule-qemu-0.5.9/tests/molecule/os-ubuntu-jammy/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/tests/molecule/os-ubuntu-jammy/collections.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/tests/molecule/os-ubuntu-jammy/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/tests/molecule/os-ubuntu-jammy/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/tests/molecule/os-ubuntu-jammy/prepare.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/tests/molecule/os-ubuntu-jammy/requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/tests/molecule/os-ubuntu-jammy/verify.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 10:46:10.092475 molecule-qemu-0.5.9/tests/molecule/platform-amd64/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/tests/molecule/platform-amd64/collections.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/tests/molecule/platform-amd64/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/tests/molecule/platform-amd64/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/tests/molecule/platform-amd64/prepare.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/tests/molecule/platform-amd64/requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/tests/molecule/platform-amd64/verify.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-03 10:46:10.092475 molecule-qemu-0.5.9/tests/molecule/platform-arm64/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/tests/molecule/platform-arm64/collections.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/tests/molecule/platform-arm64/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/tests/molecule/platform-arm64/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/tests/molecule/platform-arm64/prepare.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/tests/molecule/platform-arm64/requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-03-03 10:46:05.000000 molecule-qemu-0.5.9/tests/molecule/platform-arm64/verify.yml
```

### Comparing `molecule-qemu-0.5.8/.github/workflows/ansible-test.yml` & `molecule-qemu-0.5.9/.github/workflows/ansible-test.yml`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.5.8/.github/workflows/python-release.yml` & `molecule-qemu-0.5.9/.github/workflows/python-release.yml`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.5.8/.gitignore` & `molecule-qemu-0.5.9/.gitignore`

 * *Files 8% similar despite different names*

```diff
@@ -124,7 +124,9 @@
 .mypy_cache/
 .dmypy.json
 dmypy.json
 
 # Pyre type checker
 .pyre/
 src/molecule_plugins/_version.py
+
+.vscode/
```

### Comparing `molecule-qemu-0.5.8/.yamllint` & `molecule-qemu-0.5.9/.yamllint`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.5.8/LICENSE` & `molecule-qemu-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.5.8/Makefile` & `molecule-qemu-0.5.9/Makefile`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.5.8/PKG-INFO` & `molecule-qemu-0.5.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molecule-qemu
-Version: 0.5.8
+Version: 0.5.9
 Summary: Molecule QEMU
 Author-email: Andrey Gubarev <andrey@andreygubarev.com>
 License: MIT
 Project-URL: Homepage, https://github.com/andreygubarev/molecule-qemu/
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: molecule>=5.0
@@ -28,14 +28,25 @@
 Support of other platforms and guest OS is possible, but not tested. Please, open an issue if you want to add support for other platforms.
 
 Supported network modes:
 
 - `user` - QEMU's user networking mode
 - `vmnet-shared` - QEMU's `vmnet-shared` networking mode (MacOS only)
 
+
+Supported disk types:
+
+- `virtio` - QEMU's virtio disk type
+- `virtio-scsi` - QEMU's virtio-scsi disk type
+
+Supported BIOS types:
+
+- `uefi` - QEMU's uefi used for image with uefi configured
+- `bios` - QEMU's bios used for image with bios configured
+
 ## Quick start
 
 Install `molecule-qemu` python package:
 
 ```bash
 pip install molecule-qemu
 ```
@@ -85,14 +96,18 @@
     network_ssh_port: 2222 # optional, default is 22
     network_ssh_user: ansible # optional, default is ansible
 
     vm_cpus: 1 # optional, default is 1
     vm_memory: 512 # optional, default is 512
     vm_disk: 8G # optional, default is 8G
     vm_extra_args: "" # optional, additional arguments to be passed to QEMU, default is empty
+
+    disk_type: virtio-scsi # optional, default is virtio
+
+    bios_type: bios # optional, default is uefi
 ```
 
 ### Dependencies
 
 Driver depends on:
 
 - QEMU (tested with 8.0.2, 8.0.4, 8.1.0)
```

### Comparing `molecule-qemu-0.5.8/README.md` & `molecule-qemu-0.5.9/molecule_qemu.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: molecule-qemu
+Version: 0.5.9
+Summary: Molecule QEMU
+Author-email: Andrey Gubarev <andrey@andreygubarev.com>
+License: MIT
+Project-URL: Homepage, https://github.com/andreygubarev/molecule-qemu/
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: molecule>=5.0
+
 # `molecule-qemu`
 
 Molecule QEMU driver for testing Ansible roles.
 
 Supported platforms:
 
 - MacOS 13.x (arm64)
@@ -17,14 +28,25 @@
 Support of other platforms and guest OS is possible, but not tested. Please, open an issue if you want to add support for other platforms.
 
 Supported network modes:
 
 - `user` - QEMU's user networking mode
 - `vmnet-shared` - QEMU's `vmnet-shared` networking mode (MacOS only)
 
+
+Supported disk types:
+
+- `virtio` - QEMU's virtio disk type
+- `virtio-scsi` - QEMU's virtio-scsi disk type
+
+Supported BIOS types:
+
+- `uefi` - QEMU's uefi used for image with uefi configured
+- `bios` - QEMU's bios used for image with bios configured
+
 ## Quick start
 
 Install `molecule-qemu` python package:
 
 ```bash
 pip install molecule-qemu
 ```
@@ -74,14 +96,18 @@
     network_ssh_port: 2222 # optional, default is 22
     network_ssh_user: ansible # optional, default is ansible
 
     vm_cpus: 1 # optional, default is 1
     vm_memory: 512 # optional, default is 512
     vm_disk: 8G # optional, default is 8G
     vm_extra_args: "" # optional, additional arguments to be passed to QEMU, default is empty
+
+    disk_type: virtio-scsi # optional, default is virtio
+
+    bios_type: bios # optional, default is uefi
 ```
 
 ### Dependencies
 
 Driver depends on:
 
 - QEMU (tested with 8.0.2, 8.0.4, 8.1.0)
```

### Comparing `molecule-qemu-0.5.8/molecule_qemu/driver.json` & `molecule-qemu-0.5.9/molecule_qemu/driver.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997569444444444%*

 * *Differences: {"'$defs'": "{'MoleculePlatformModel': {'properties': {'image_format': {'enum': {insert: [(1, "*

 * *            "'raw')]}}, 'disk_type': OrderedDict([('title', 'Disk Type'), ('type', 'string'), "*

 * *            "('enum', ['virtio', 'virtio-scsi'])]), 'bios_type': OrderedDict([('title', 'Bios "*

 * *            "Type'), ('type', 'string'), ('enum', ['uefi', 'bios'])])}}}"}*

```diff
@@ -12,29 +12,46 @@
             },
             "title": "MoleculeDriverModel",
             "type": "object"
         },
         "MoleculePlatformModel": {
             "additionalProperties": true,
             "properties": {
+                "bios_type": {
+                    "enum": [
+                        "uefi",
+                        "bios"
+                    ],
+                    "title": "Bios Type",
+                    "type": "string"
+                },
+                "disk_type": {
+                    "enum": [
+                        "virtio",
+                        "virtio-scsi"
+                    ],
+                    "title": "Disk Type",
+                    "type": "string"
+                },
                 "image_arch": {
                     "enum": [
                         "x86_64",
                         "aarch64"
                     ],
                     "title": "Image Architecture",
                     "type": "string"
                 },
                 "image_checksum": {
                     "title": "Image Checksum",
                     "type": "string"
                 },
                 "image_format": {
                     "enum": [
-                        "qcow2"
+                        "qcow2",
+                        "raw"
                     ],
                     "title": "Image Format",
                     "type": "string"
                 },
                 "image_url": {
                     "title": "Image URL",
                     "type": "string"
```

### Comparing `molecule-qemu-0.5.8/molecule_qemu/driver.py` & `molecule-qemu-0.5.9/molecule_qemu/driver.py`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.5.8/molecule_qemu/playbooks/create.yml` & `molecule-qemu-0.5.9/molecule_qemu/playbooks/create.yml`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,16 @@
     qemu_image_arch: "x86_64"
     qemu_image_format: "qcow2"
     qemu_vm_memory: "512"
     qemu_vm_cpus: "1"
     qemu_vm_disk: "8G"
     qemu_network_extra_args: ""
     qemu_network_mode: "user"
+    qemu_bios_type: "uefi"
+    qemu_disk_type: "virtio"
     qemu_timeout_arp: 120
     qemu_timeout_ssh: 600
 
   environment:
     http_proxy: "{{ lookup('ansible.builtin.env', 'http_proxy') | default(omit) }}"
     https_proxy: "{{ lookup('ansible.builtin.env', 'https_proxy') | default(omit) }}"
 
@@ -56,14 +58,18 @@
             "network_ssh_port": "{{ item.network_ssh_port | default(22) }}",
             "network_ssh_user": "{{ item.network_ssh_user | default('ansible') }}",
 
             "vm_extra_args": "{{ item.vm_extra_args | default(qemu_extra_args) }}",
             "vm_cpus": "{{ item.vm_cpus | default(qemu_vm_cpus) }}",
             "vm_memory": "{{ item.vm_memory | default(qemu_vm_memory) }}",
             "vm_disk": "{{ item.vm_disk | default(qemu_vm_disk) }}",
+            
+            "disk_type": "{{ item.disk_type | default(qemu_disk_type) }}",
+
+            "bios_type": "{{ item.bios_type | default(qemu_bios_type) }}",
 
             "path_disk": "{{ molecule_ephemeral_directory }}/run/{{ item.name }}.qcow2",
             "path_pid": "{{ molecule_ephemeral_directory }}/run/{{ item.name }}.pid",
           }
       loop: "{{ molecule_yml.platforms }}"
       loop_control:
         label: "{{ item.name }}"
@@ -85,14 +91,16 @@
         success_msg: "Molecule instances are properly defined"
 
     - name: Assert supported VMs configuration
       ansible.builtin.assert:
         that:
           - item.image_arch in ['x86_64', 'aarch64']
           - item.network_mode in ['user', 'vmnet-shared']
+          - item.disk_type in ['virtio', 'virtio-scsi']
+          - item.bios_type in ['uefi', 'bios']
         fail_msg: "Molecule instance {{ item.name }} configuration is not supported"
         success_msg: "Molecule instance {{ item.name }} configuration is supported"
       loop: "{{ molecule_instances }}"
       loop_control:
         label: "{{ item.name }}"
 
     - name: Assert VMs network configuration
@@ -289,29 +297,37 @@
 
         -display none
         -m {{ item.vm_memory }}
         -smp {{ item.vm_cpus }}
 
         -boot d
         -cdrom {{ molecule_ephemeral_directory }}/run/cloud-init/{{ item.name }}.iso
-        -drive if=virtio,file={{ item.path_disk }}
+        {% if item.disk_type == 'virtio' %}
+          -drive if=virtio,file={{ item.path_disk }}
+        {% elif item.disk_type == 'virtio-scsi' %}
+          -drive if=none,id=hd,file={{ item.path_disk }}
+          -device virtio-scsi-pci,id=scsi
+          -device scsi-hd,drive=hd
+        {% endif %}
 
         {% if item.network_mode == 'vmnet-shared' %}
           -nic vmnet-shared,model=virtio-net-pci,mac={{ item.network_mac }}
         {% endif %}
 
         {% if item.network_mode == 'user' %}
           {% if item.network_extra_args == '' %}
             -nic user,model=virtio-net-pci,hostfwd=tcp::{{ item.network_ssh_port }}-:22
           {% else %}
             -nic user,model=virtio-net-pci,hostfwd=tcp::{{ item.network_ssh_port }}-:22,{{ item.network_extra_args }}
           {% endif %}
         {% endif %}
 
-        -bios {{ molecule_driver_directory }}/edk2-{{ item.image_arch }}.fd
+        {% if item.bios_type == 'uefi' %}
+          -bios {{ molecule_driver_directory }}/edk2-{{ item.image_arch }}.fd
+        {% endif %}
 
         {% if item.image_arch == 'aarch64' %}
           -machine virt
           {% if item.image_arch == qemu_machine and qemu_cap_hvf %}
             -cpu host
             -accel hvf
           {% else %}
```

### Comparing `molecule-qemu-0.5.8/molecule_qemu/playbooks/destroy.yml` & `molecule-qemu-0.5.9/molecule_qemu/playbooks/destroy.yml`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.5.8/molecule_qemu/playbooks/edk2-aarch64.fd` & `molecule-qemu-0.5.9/molecule_qemu/playbooks/edk2-aarch64.fd`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.5.8/molecule_qemu/playbooks/edk2-x86_64.fd` & `molecule-qemu-0.5.9/molecule_qemu/playbooks/edk2-x86_64.fd`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.5.8/molecule_qemu.egg-info/PKG-INFO` & `molecule-qemu-0.5.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: molecule-qemu
-Version: 0.5.8
-Summary: Molecule QEMU
-Author-email: Andrey Gubarev <andrey@andreygubarev.com>
-License: MIT
-Project-URL: Homepage, https://github.com/andreygubarev/molecule-qemu/
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: molecule>=5.0
-
 # `molecule-qemu`
 
 Molecule QEMU driver for testing Ansible roles.
 
 Supported platforms:
 
 - MacOS 13.x (arm64)
@@ -28,14 +17,25 @@
 Support of other platforms and guest OS is possible, but not tested. Please, open an issue if you want to add support for other platforms.
 
 Supported network modes:
 
 - `user` - QEMU's user networking mode
 - `vmnet-shared` - QEMU's `vmnet-shared` networking mode (MacOS only)
 
+
+Supported disk types:
+
+- `virtio` - QEMU's virtio disk type
+- `virtio-scsi` - QEMU's virtio-scsi disk type
+
+Supported BIOS types:
+
+- `uefi` - QEMU's uefi used for image with uefi configured
+- `bios` - QEMU's bios used for image with bios configured
+
 ## Quick start
 
 Install `molecule-qemu` python package:
 
 ```bash
 pip install molecule-qemu
 ```
@@ -85,14 +85,18 @@
     network_ssh_port: 2222 # optional, default is 22
     network_ssh_user: ansible # optional, default is ansible
 
     vm_cpus: 1 # optional, default is 1
     vm_memory: 512 # optional, default is 512
     vm_disk: 8G # optional, default is 8G
     vm_extra_args: "" # optional, additional arguments to be passed to QEMU, default is empty
+
+    disk_type: virtio-scsi # optional, default is virtio
+
+    bios_type: bios # optional, default is uefi
 ```
 
 ### Dependencies
 
 Driver depends on:
 
 - QEMU (tested with 8.0.2, 8.0.4, 8.1.0)
```

### Comparing `molecule-qemu-0.5.8/molecule_qemu.egg-info/SOURCES.txt` & `molecule-qemu-0.5.9/molecule_qemu.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 pyproject.toml
 requirements.yml
 setup.cfg
 .github/workflows/ansible-lint.yml
 .github/workflows/ansible-test.yml
 .github/workflows/python-lint.yml
 .github/workflows/python-release.yml
-.vscode/settings.json
 molecule_qemu/__init__.py
 molecule_qemu/driver.json
 molecule_qemu/driver.py
 molecule_qemu.egg-info/PKG-INFO
 molecule_qemu.egg-info/SOURCES.txt
 molecule_qemu.egg-info/dependency_links.txt
 molecule_qemu.egg-info/entry_points.txt
```

### Comparing `molecule-qemu-0.5.8/pyproject.toml` & `molecule-qemu-0.5.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.5.8/tests/.yamllint` & `molecule-qemu-0.5.9/tests/.yamllint`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.5.8/tests/molecule/network-shared/molecule.yml` & `molecule-qemu-0.5.9/tests/molecule/network-shared/molecule.yml`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.5.8/tests/molecule/network-user/molecule.yml` & `molecule-qemu-0.5.9/tests/molecule/network-user/molecule.yml`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.5.8/tests/molecule/os-debian-bookworm/molecule.yml` & `molecule-qemu-0.5.9/tests/molecule/os-debian-bookworm/molecule.yml`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.5.8/tests/molecule/os-debian-bullseye/molecule.yml` & `molecule-qemu-0.5.9/tests/molecule/os-debian-bullseye/molecule.yml`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.5.8/tests/molecule/os-ubuntu-focal/molecule.yml` & `molecule-qemu-0.5.9/tests/molecule/os-ubuntu-focal/molecule.yml`

 * *Files identical despite different names*

### Comparing `molecule-qemu-0.5.8/tests/molecule/os-ubuntu-jammy/molecule.yml` & `molecule-qemu-0.5.9/tests/molecule/os-ubuntu-jammy/molecule.yml`

 * *Files identical despite different names*

