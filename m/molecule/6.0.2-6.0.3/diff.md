# Comparing `tmp/molecule-6.0.2.tar.gz` & `tmp/molecule-6.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molecule-6.0.2.tar", last modified: Wed Aug 30 10:22:05 2023, max compression
+gzip compressed data, was "molecule-6.0.3.tar", last modified: Wed Dec 13 13:38:15 2023, max compression
```

## Comparing `molecule-6.0.2.tar` & `molecule-6.0.3.tar`

### file list

```diff
@@ -1,469 +1,472 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.407365 molecule-6.0.2/
--rw-r--r--   0 runner    (1001) docker     (999)       99 2023-08-30 10:21:49.000000 molecule-6.0.2/.ansible.cfg
--rw-r--r--   0 runner    (1001) docker     (999)       35 2023-08-30 10:21:49.000000 molecule-6.0.2/.codespellrc
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.371365 molecule-6.0.2/.config/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.371365 molecule-6.0.2/.config/molecule/
--rw-r--r--   0 runner    (1001) docker     (999)       41 2023-08-30 10:21:49.000000 molecule-6.0.2/.config/molecule/config.yml
--rw-r--r--   0 runner    (1001) docker     (999)     2199 2023-08-30 10:21:49.000000 molecule-6.0.2/.config/molecule.spec
--rw-r--r--   0 runner    (1001) docker     (999)       58 2023-08-30 10:21:49.000000 molecule-6.0.2/.config/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (999)      416 2023-08-30 10:21:49.000000 molecule-6.0.2/.config/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (999)       24 2023-08-30 10:21:49.000000 molecule-6.0.2/.config/requirements-testinfra.txt
--rw-r--r--   0 runner    (1001) docker     (999)      226 2023-08-30 10:21:49.000000 molecule-6.0.2/.config/requirements.in
--rw-r--r--   0 runner    (1001) docker     (999)       23 2023-08-30 10:21:49.000000 molecule-6.0.2/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (999)     3277 2023-08-30 10:21:49.000000 molecule-6.0.2/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.375365 molecule-6.0.2/.github/
--rw-r--r--   0 runner    (1001) docker     (999)       64 2023-08-30 10:21:49.000000 molecule-6.0.2/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (999)      162 2023-08-30 10:21:49.000000 molecule-6.0.2/.github/CODE_OF_CONDUCT.md
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.375365 molecule-6.0.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (999)     1042 2023-08-30 10:21:49.000000 molecule-6.0.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (999)     2050 2023-08-30 10:21:49.000000 molecule-6.0.2/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (999)      325 2023-08-30 10:21:49.000000 molecule-6.0.2/.github/ISSUE_TEMPLATE/security_bug_report.md
--rw-r--r--   0 runner    (1001) docker     (999)      363 2023-08-30 10:21:49.000000 molecule-6.0.2/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (999)      112 2023-08-30 10:21:49.000000 molecule-6.0.2/.github/patchback.yml
--rw-r--r--   0 runner    (1001) docker     (999)       69 2023-08-30 10:21:49.000000 molecule-6.0.2/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.375365 molecule-6.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (999)      244 2023-08-30 10:21:49.000000 molecule-6.0.2/.github/workflows/ack.yml
--rw-r--r--   0 runner    (1001) docker     (999)      248 2023-08-30 10:21:49.000000 molecule-6.0.2/.github/workflows/push.yml
--rw-r--r--   0 runner    (1001) docker     (999)      745 2023-08-30 10:21:49.000000 molecule-6.0.2/.github/workflows/redirects.yml
--rw-r--r--   0 runner    (1001) docker     (999)      969 2023-08-30 10:21:49.000000 molecule-6.0.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (999)     4569 2023-08-30 10:21:49.000000 molecule-6.0.2/.github/workflows/tox.yml
--rw-r--r--   0 runner    (1001) docker     (999)      416 2023-08-30 10:21:49.000000 molecule-6.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (999)       11 2023-08-30 10:21:49.000000 molecule-6.0.2/.npmrc
--rw-r--r--   0 runner    (1001) docker     (999)     1211 2023-08-30 10:21:49.000000 molecule-6.0.2/.packit.yaml
--rw-r--r--   0 runner    (1001) docker     (999)     2538 2023-08-30 10:21:49.000000 molecule-6.0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (999)      217 2023-08-30 10:21:49.000000 molecule-6.0.2/.readthedocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.375365 molecule-6.0.2/.vscode/
--rw-r--r--   0 runner    (1001) docker     (999)      458 2023-08-30 10:21:49.000000 molecule-6.0.2/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (999)     1345 2023-08-30 10:21:49.000000 molecule-6.0.2/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (999)      597 2023-08-30 10:21:49.000000 molecule-6.0.2/.yamllint
--rw-r--r--   0 runner    (1001) docker     (999)     1618 2023-08-30 10:21:49.000000 molecule-6.0.2/DCO_1_1.md
--rw-r--r--   0 runner    (1001) docker     (999)     1118 2023-08-30 10:21:49.000000 molecule-6.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (999)       12 2023-08-30 10:21:49.000000 molecule-6.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (999)     4674 2023-08-30 10:22:05.407365 molecule-6.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     3080 2023-08-30 10:21:49.000000 molecule-6.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (999)      517 2023-08-30 10:21:49.000000 molecule-6.0.2/bindep.txt
--rw-r--r--   0 runner    (1001) docker     (999)      140 2023-08-30 10:21:49.000000 molecule-6.0.2/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (999)      590 2023-08-30 10:21:49.000000 molecule-6.0.2/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.375365 molecule-6.0.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.359365 molecule-6.0.2/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.375365 molecule-6.0.2/docs/_static/images/
--rw-r--r--   0 runner    (1001) docker     (999)    15406 2023-08-30 10:21:49.000000 molecule-6.0.2/docs/_static/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (999)    33945 2023-08-30 10:21:49.000000 molecule-6.0.2/docs/_static/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (999)   143898 2023-08-30 10:21:49.000000 molecule-6.0.2/docs/_static/images/logo_big.png
--rw-r--r--   0 runner    (1001) docker     (999)    10447 2023-08-30 10:21:49.000000 molecule-6.0.2/docs/ci.md
--rw-r--r--   0 runner    (1001) docker     (999)     7985 2023-08-30 10:21:49.000000 molecule-6.0.2/docs/configuration.md
--rw-r--r--   0 runner    (1001) docker     (999)     3722 2023-08-30 10:21:49.000000 molecule-6.0.2/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (999)      917 2023-08-30 10:21:49.000000 molecule-6.0.2/docs/docker.md
--rw-r--r--   0 runner    (1001) docker     (999)    12915 2023-08-30 10:21:49.000000 molecule-6.0.2/docs/examples.md
--rw-r--r--   0 runner    (1001) docker     (999)     3999 2023-08-30 10:21:49.000000 molecule-6.0.2/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (999)     7544 2023-08-30 10:21:49.000000 molecule-6.0.2/docs/getting-started.md
--rw-r--r--   0 runner    (1001) docker     (999)       54 2023-08-30 10:21:49.000000 molecule-6.0.2/docs/google04e29a42ae6e6cbc.html
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.375365 molecule-6.0.2/docs/images/
--rw-r--r--   0 runner    (1001) docker     (999)   187162 2023-08-30 10:21:49.000000 molecule-6.0.2/docs/images/collection_structure_and_ansible_cfg.png
--rw-r--r--   0 runner    (1001) docker     (999)    15406 2023-08-30 10:21:49.000000 molecule-6.0.2/docs/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (999)    33945 2023-08-30 10:21:49.000000 molecule-6.0.2/docs/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (999)     1047 2023-08-30 10:21:49.000000 molecule-6.0.2/docs/images/logo.svg
--rw-r--r--   0 runner    (1001) docker     (999)     1347 2023-08-30 10:21:49.000000 molecule-6.0.2/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (999)     4597 2023-08-30 10:21:49.000000 molecule-6.0.2/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (999)     4516 2023-08-30 10:21:49.000000 molecule-6.0.2/docs/kubevirt.md
--rw-r--r--   0 runner    (1001) docker     (999)     1484 2023-08-30 10:21:49.000000 molecule-6.0.2/docs/next.md
--rw-r--r--   0 runner    (1001) docker     (999)      917 2023-08-30 10:21:49.000000 molecule-6.0.2/docs/podman.md
--rw-r--r--   0 runner    (1001) docker     (999)      344 2023-08-30 10:21:49.000000 molecule-6.0.2/docs/redirects.yml
--rw-r--r--   0 runner    (1001) docker     (999)     2171 2023-08-30 10:21:49.000000 molecule-6.0.2/docs/usage.md
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.363365 molecule-6.0.2/docs/working/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.379365 molecule-6.0.2/docs/working/contributor_guide/
--rw-r--r--   0 runner    (1001) docker     (999)       18 2023-08-30 10:21:49.000000 molecule-6.0.2/docs/working/contributor_guide/code_of_conduct.md
--rw-r--r--   0 runner    (1001) docker     (999)       27 2023-08-30 10:21:49.000000 molecule-6.0.2/docs/working/contributor_guide/contribution_requirements.md
--rw-r--r--   0 runner    (1001) docker     (999)       21 2023-08-30 10:21:49.000000 molecule-6.0.2/docs/working/contributor_guide/developer_contact.md
--rw-r--r--   0 runner    (1001) docker     (999)       39 2023-08-30 10:21:49.000000 molecule-6.0.2/docs/working/contributor_guide/environment_setup.md
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.379365 molecule-6.0.2/docs/working/examples/
--rw-r--r--   0 runner    (1001) docker     (999)       12 2023-08-30 10:21:49.000000 molecule-6.0.2/docs/working/examples/example_1.md
--rw-r--r--   0 runner    (1001) docker     (999)       12 2023-08-30 10:21:49.000000 molecule-6.0.2/docs/working/examples/example_2.md
--rw-r--r--   0 runner    (1001) docker     (999)       12 2023-08-30 10:21:49.000000 molecule-6.0.2/docs/working/examples/example_3.md
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.379365 molecule-6.0.2/docs/working/faq/
--rw-r--r--   0 runner    (1001) docker     (999)       29 2023-08-30 10:21:49.000000 molecule-6.0.2/docs/working/faq/faq.md
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.379365 molecule-6.0.2/docs/working/getting_started/
--rw-r--r--   0 runner    (1001) docker     (999)       18 2023-08-30 10:21:49.000000 molecule-6.0.2/docs/working/getting_started/getting_started.md
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.379365 molecule-6.0.2/docs/working/installation/
--rw-r--r--   0 runner    (1001) docker     (999)       20 2023-08-30 10:21:49.000000 molecule-6.0.2/docs/working/installation/install.md
--rw-r--r--   0 runner    (1001) docker     (999)       12 2023-08-30 10:21:49.000000 molecule-6.0.2/docs/working/installation/upgrade.md
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.379365 molecule-6.0.2/docs/working/introduction/
--rw-r--r--   0 runner    (1001) docker     (999)       15 2023-08-30 10:21:49.000000 molecule-6.0.2/docs/working/introduction/introduction.md
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.379365 molecule-6.0.2/docs/working/references/
--rw-r--r--   0 runner    (1001) docker     (999)       25 2023-08-30 10:21:49.000000 molecule-6.0.2/docs/working/references/cli.md
--rw-r--r--   0 runner    (1001) docker     (999)       16 2023-08-30 10:21:49.000000 molecule-6.0.2/docs/working/references/configuration.md
--rw-r--r--   0 runner    (1001) docker     (999)       26 2023-08-30 10:21:49.000000 molecule-6.0.2/docs/working/references/porting_change_log.md
--rw-r--r--   0 runner    (1001) docker     (999)       11 2023-08-30 10:21:49.000000 molecule-6.0.2/docs/working/references/road_map.md
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.379365 molecule-6.0.2/docs/working/user_guide/
--rw-r--r--   0 runner    (1001) docker     (999)       23 2023-08-30 10:21:49.000000 molecule-6.0.2/docs/working/user_guide/ci_integration.md
--rw-r--r--   0 runner    (1001) docker     (999)       36 2023-08-30 10:21:49.000000 molecule-6.0.2/docs/working/user_guide/creating_testing_collection.md
--rw-r--r--   0 runner    (1001) docker     (999)       33 2023-08-30 10:21:49.000000 molecule-6.0.2/docs/working/user_guide/testing_existing_collection.md
--rw-r--r--   0 runner    (1001) docker     (999)       25 2023-08-30 10:21:49.000000 molecule-6.0.2/docs/working/user_guide/testing_existing_roles.md
--rw-r--r--   0 runner    (1001) docker     (999)       25 2023-08-30 10:21:49.000000 molecule-6.0.2/docs/working/user_guide/understanding.md
--rw-r--r--   0 runner    (1001) docker     (999)       20 2023-08-30 10:21:49.000000 molecule-6.0.2/docs/working/user_guide/using_tox-ansible.md
--rw-r--r--   0 runner    (1001) docker     (999)       95 2023-08-30 10:21:49.000000 molecule-6.0.2/linkcheckerrc
--rw-r--r--   0 runner    (1001) docker     (999)     4493 2023-08-30 10:21:49.000000 molecule-6.0.2/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.363365 molecule-6.0.2/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.379365 molecule-6.0.2/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (999)      203 2023-08-30 10:21:49.000000 molecule-6.0.2/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (999)     1217 2023-08-30 10:21:49.000000 molecule-6.0.2/molecule/default/create.yml
--rw-r--r--   0 runner    (1001) docker     (999)      617 2023-08-30 10:21:49.000000 molecule-6.0.2/molecule/default/destroy.yml
--rw-r--r--   0 runner    (1001) docker     (999)      182 2023-08-30 10:21:49.000000 molecule-6.0.2/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.379365 molecule-6.0.2/molecule/docker/
--rw-r--r--   0 runner    (1001) docker     (999)      944 2023-08-30 10:21:49.000000 molecule-6.0.2/molecule/docker/converge.yml
--rw-r--r--   0 runner    (1001) docker     (999)     2302 2023-08-30 10:21:49.000000 molecule-6.0.2/molecule/docker/create.yml
--rw-r--r--   0 runner    (1001) docker     (999)      551 2023-08-30 10:21:49.000000 molecule-6.0.2/molecule/docker/destroy.yml
--rw-r--r--   0 runner    (1001) docker     (999)      139 2023-08-30 10:21:49.000000 molecule-6.0.2/molecule/docker/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (999)       34 2023-08-30 10:21:49.000000 molecule-6.0.2/molecule/docker/requirements.yml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.379365 molecule-6.0.2/molecule/docker/tasks/
--rw-r--r--   0 runner    (1001) docker     (999)      293 2023-08-30 10:21:49.000000 molecule-6.0.2/molecule/docker/tasks/create-fail.yml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.379365 molecule-6.0.2/molecule/kubevirt/
--rw-r--r--   0 runner    (1001) docker     (999)      944 2023-08-30 10:21:49.000000 molecule-6.0.2/molecule/kubevirt/converge.yml
--rw-r--r--   0 runner    (1001) docker     (999)     4346 2023-08-30 10:21:49.000000 molecule-6.0.2/molecule/kubevirt/create.yml
--rw-r--r--   0 runner    (1001) docker     (999)      634 2023-08-30 10:21:49.000000 molecule-6.0.2/molecule/kubevirt/destroy.yml
--rw-r--r--   0 runner    (1001) docker     (999)      995 2023-08-30 10:21:49.000000 molecule-6.0.2/molecule/kubevirt/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (999)       70 2023-08-30 10:21:49.000000 molecule-6.0.2/molecule/kubevirt/requirements.yml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.383365 molecule-6.0.2/molecule/kubevirt/tasks/
--rw-r--r--   0 runner    (1001) docker     (999)     2821 2023-08-30 10:21:49.000000 molecule-6.0.2/molecule/kubevirt/tasks/create_vm.yml
--rw-r--r--   0 runner    (1001) docker     (999)     1199 2023-08-30 10:21:49.000000 molecule-6.0.2/molecule/kubevirt/tasks/create_vm_dictionary.yml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.383365 molecule-6.0.2/molecule/podman/
--rw-r--r--   0 runner    (1001) docker     (999)      944 2023-08-30 10:21:49.000000 molecule-6.0.2/molecule/podman/converge.yml
--rw-r--r--   0 runner    (1001) docker     (999)     2357 2023-08-30 10:21:49.000000 molecule-6.0.2/molecule/podman/create.yml
--rw-r--r--   0 runner    (1001) docker     (999)      745 2023-08-30 10:21:49.000000 molecule-6.0.2/molecule/podman/destroy.yml
--rw-r--r--   0 runner    (1001) docker     (999)      139 2023-08-30 10:21:49.000000 molecule-6.0.2/molecule/podman/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (999)       35 2023-08-30 10:21:49.000000 molecule-6.0.2/molecule/podman/requirements.yml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.383365 molecule-6.0.2/molecule/podman/tasks/
--rw-r--r--   0 runner    (1001) docker     (999)      356 2023-08-30 10:21:49.000000 molecule-6.0.2/molecule/podman/tasks/create-fail.yml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.383365 molecule-6.0.2/molecule/smoke/
--rw-r--r--   0 runner    (1001) docker     (999)      369 2023-08-30 10:21:49.000000 molecule-6.0.2/molecule/smoke/converge.yml
--rw-r--r--   0 runner    (1001) docker     (999)       31 2023-08-30 10:21:49.000000 molecule-6.0.2/molecule/smoke/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.383365 molecule-6.0.2/playbooks/
--rw-r--r--   0 runner    (1001) docker     (999)      849 2023-08-30 10:21:49.000000 molecule-6.0.2/playbooks/snap-pre-run.yaml
--rw-r--r--   0 runner    (1001) docker     (999)     6618 2023-08-30 10:21:49.000000 molecule-6.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (999)       78 2023-08-30 10:21:49.000000 molecule-6.0.2/runtime.txt
--rw-r--r--   0 runner    (1001) docker     (999)       38 2023-08-30 10:22:05.407365 molecule-6.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.383365 molecule-6.0.2/snap/
--rw-r--r--   0 runner    (1001) docker     (999)      546 2023-08-30 10:21:49.000000 molecule-6.0.2/snap/snapcraft.yaml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.363365 molecule-6.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.383365 molecule-6.0.2/src/molecule/
--rw-r--r--   0 runner    (1001) docker     (999)     1392 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     1217 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/__main__.py
--rw-r--r--   0 runner    (1001) docker     (999)      160 2023-08-30 10:22:05.000000 molecule-6.0.2/src/molecule/_version.py
--rw-r--r--   0 runner    (1001) docker     (999)     2425 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/api.py
--rw-r--r--   0 runner    (1001) docker     (999)      272 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/app.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.387365 molecule-6.0.2/src/molecule/command/
--rw-r--r--   0 runner    (1001) docker     (999)     2151 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)    10206 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/command/base.py
--rw-r--r--   0 runner    (1001) docker     (999)     2460 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/command/check.py
--rw-r--r--   0 runner    (1001) docker     (999)     2293 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/command/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (999)     2326 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/command/converge.py
--rw-r--r--   0 runner    (1001) docker     (999)     2466 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/command/create.py
--rw-r--r--   0 runner    (1001) docker     (999)     2067 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/command/dependency.py
--rw-r--r--   0 runner    (1001) docker     (999)     3101 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/command/destroy.py
--rw-r--r--   0 runner    (1001) docker     (999)     2360 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/command/drivers.py
--rw-r--r--   0 runner    (1001) docker     (999)     4522 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/command/idempotence.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.387365 molecule-6.0.2/src/molecule/command/init/
--rw-r--r--   0 runner    (1001) docker     (999)        7 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/command/init/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     1616 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/command/init/base.py
--rw-r--r--   0 runner    (1001) docker     (999)     1435 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/command/init/init.py
--rw-r--r--   0 runner    (1001) docker     (999)     5388 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/command/init/scenario.py
--rw-r--r--   0 runner    (1001) docker     (999)     3696 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/command/list.py
--rw-r--r--   0 runner    (1001) docker     (999)     4896 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/command/login.py
--rw-r--r--   0 runner    (1001) docker     (999)     2772 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/command/matrix.py
--rw-r--r--   0 runner    (1001) docker     (999)     4301 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/command/prepare.py
--rw-r--r--   0 runner    (1001) docker     (999)     1853 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/command/reset.py
--rw-r--r--   0 runner    (1001) docker     (999)     2392 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/command/side_effect.py
--rw-r--r--   0 runner    (1001) docker     (999)     2061 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/command/syntax.py
--rw-r--r--   0 runner    (1001) docker     (999)     3541 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/command/test.py
--rw-r--r--   0 runner    (1001) docker     (999)     2073 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/command/verify.py
--rw-r--r--   0 runner    (1001) docker     (999)    17530 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/config.py
--rw-r--r--   0 runner    (1001) docker     (999)     2749 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/console.py
--rw-r--r--   0 runner    (1001) docker     (999)      264 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.387365 molecule-6.0.2/src/molecule/data/
--rw-r--r--   0 runner    (1001) docker     (999)       45 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     2554 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/data/driver.json
--rw-r--r--   0 runner    (1001) docker     (999)     1123 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/data/init-scenario.yml
--rw-r--r--   0 runner    (1001) docker     (999)    14472 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/data/molecule.json
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.363365 molecule-6.0.2/src/molecule/data/templates/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.387365 molecule-6.0.2/src/molecule/data/templates/scenario/
--rw-r--r--   0 runner    (1001) docker     (999)      203 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/data/templates/scenario/converge.yml.j2
--rw-r--r--   0 runner    (1001) docker     (999)     1206 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/data/templates/scenario/create.yml.j2
--rw-r--r--   0 runner    (1001) docker     (999)      645 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/data/templates/scenario/destroy.yml.j2
--rw-r--r--   0 runner    (1001) docker     (999)      182 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/data/templates/scenario/molecule.yml.j2
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.387365 molecule-6.0.2/src/molecule/dependency/
--rw-r--r--   0 runner    (1001) docker     (999)        7 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/dependency/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.391365 molecule-6.0.2/src/molecule/dependency/ansible_galaxy/
--rw-r--r--   0 runner    (1001) docker     (999)     4055 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/dependency/ansible_galaxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     4060 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/dependency/ansible_galaxy/base.py
--rw-r--r--   0 runner    (1001) docker     (999)      960 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/dependency/ansible_galaxy/collections.py
--rw-r--r--   0 runner    (1001) docker     (999)      844 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/dependency/ansible_galaxy/roles.py
--rw-r--r--   0 runner    (1001) docker     (999)     4217 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/dependency/base.py
--rw-r--r--   0 runner    (1001) docker     (999)     3229 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/dependency/shell.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.391365 molecule-6.0.2/src/molecule/driver/
--rw-r--r--   0 runner    (1001) docker     (999)        7 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/driver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     8872 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/driver/base.py
--rw-r--r--   0 runner    (1001) docker     (999)     8923 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/driver/delegated.py
--rw-r--r--   0 runner    (1001) docker     (999)     4470 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/interpolation.py
--rw-r--r--   0 runner    (1001) docker     (999)     6713 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.391365 molecule-6.0.2/src/molecule/model/
--rw-r--r--   0 runner    (1001) docker     (999)        7 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     2896 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/model/schema_v3.py
--rw-r--r--   0 runner    (1001) docker     (999)     2944 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/platforms.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.391365 molecule-6.0.2/src/molecule/provisioner/
--rw-r--r--   0 runner    (1001) docker     (999)        7 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/provisioner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)    33606 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/provisioner/ansible.py
--rw-r--r--   0 runner    (1001) docker     (999)     5681 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/provisioner/ansible_playbook.py
--rw-r--r--   0 runner    (1001) docker     (999)     5036 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/provisioner/ansible_playbooks.py
--rw-r--r--   0 runner    (1001) docker     (999)     2023 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/provisioner/base.py
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/py.typed
--rw-r--r--   0 runner    (1001) docker     (999)     7686 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/scenario.py
--rw-r--r--   0 runner    (1001) docker     (999)     4754 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/scenarios.py
--rw-r--r--   0 runner    (1001) docker     (999)     5843 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/shell.py
--rw-r--r--   0 runner    (1001) docker     (999)     4681 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/state.py
--rw-r--r--   0 runner    (1001) docker     (999)     1368 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/status.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.391365 molecule-6.0.2/src/molecule/test/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.391365 molecule-6.0.2/src/molecule/test/a_unit/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/a_unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.395365 molecule-6.0.2/src/molecule/test/a_unit/command/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/a_unit/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     1749 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/a_unit/command/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.395365 molecule-6.0.2/src/molecule/test/a_unit/command/init/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/a_unit/command/init/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     2270 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/a_unit/command/init/test_scenario.py
--rw-r--r--   0 runner    (1001) docker     (999)    10366 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/a_unit/command/test_base.py
--rw-r--r--   0 runner    (1001) docker     (999)     1839 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/a_unit/command/test_check.py
--rw-r--r--   0 runner    (1001) docker     (999)     2612 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/a_unit/command/test_cleanup.py
--rw-r--r--   0 runner    (1001) docker     (999)     2694 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/a_unit/command/test_converge.py
--rw-r--r--   0 runner    (1001) docker     (999)     2517 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/a_unit/command/test_create.py
--rw-r--r--   0 runner    (1001) docker     (999)     1773 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/a_unit/command/test_dependency.py
--rw-r--r--   0 runner    (1001) docker     (999)     2715 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/a_unit/command/test_destroy.py
--rw-r--r--   0 runner    (1001) docker     (999)     5074 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/a_unit/command/test_idempotence.py
--rw-r--r--   0 runner    (1001) docker     (999)     1843 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/a_unit/command/test_list.py
--rw-r--r--   0 runner    (1001) docker     (999)     4664 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/a_unit/command/test_login.py
--rw-r--r--   0 runner    (1001) docker     (999)     1155 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/a_unit/command/test_matrix.py
--rw-r--r--   0 runner    (1001) docker     (999)     3283 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/a_unit/command/test_prepare.py
--rw-r--r--   0 runner    (1001) docker     (999)     2772 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/a_unit/command/test_side_effect.py
--rw-r--r--   0 runner    (1001) docker     (999)     1901 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/a_unit/command/test_syntax.py
--rw-r--r--   0 runner    (1001) docker     (999)     1153 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/a_unit/command/test_test.py
--rw-r--r--   0 runner    (1001) docker     (999)     1705 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/a_unit/command/test_verify.py
--rw-r--r--   0 runner    (1001) docker     (999)     6428 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/a_unit/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.395365 molecule-6.0.2/src/molecule/test/a_unit/cookiecutter/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/a_unit/cookiecutter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     1912 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/a_unit/cookiecutter/test_molecule.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.395365 molecule-6.0.2/src/molecule/test/a_unit/dependency/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/a_unit/dependency/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.395365 molecule-6.0.2/src/molecule/test/a_unit/dependency/ansible_galaxy/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/a_unit/dependency/ansible_galaxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     5956 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/a_unit/dependency/ansible_galaxy/test_collections.py
--rw-r--r--   0 runner    (1001) docker     (999)     5853 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/a_unit/dependency/ansible_galaxy/test_roles.py
--rw-r--r--   0 runner    (1001) docker     (999)     4466 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/a_unit/dependency/test_shell.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.395365 molecule-6.0.2/src/molecule/test/a_unit/driver/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/a_unit/driver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     9841 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/a_unit/driver/test_delegated.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.395365 molecule-6.0.2/src/molecule/test/a_unit/lint/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/a_unit/lint/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.395365 molecule-6.0.2/src/molecule/test/a_unit/model/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/a_unit/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.395365 molecule-6.0.2/src/molecule/test/a_unit/model/v2/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/a_unit/model/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     1980 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/a_unit/model/v2/conftest.py
--rw-r--r--   0 runner    (1001) docker     (999)     2850 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/a_unit/model/v2/test_dependency_section.py
--rw-r--r--   0 runner    (1001) docker     (999)     4082 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/a_unit/model/v2/test_driver_section.py
--rw-r--r--   0 runner    (1001) docker     (999)     1367 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/a_unit/model/v2/test_platforms_section.py
--rw-r--r--   0 runner    (1001) docker     (999)     2942 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/a_unit/model/v2/test_provisioner_section.py
--rw-r--r--   0 runner    (1001) docker     (999)     2011 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/a_unit/model/v2/test_scenario_section.py
--rw-r--r--   0 runner    (1001) docker     (999)     1814 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/a_unit/model/v2/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (999)     2591 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/a_unit/model/v2/test_verifier_section.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.395365 molecule-6.0.2/src/molecule/test/a_unit/provisioner/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/a_unit/provisioner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)    23871 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/a_unit/provisioner/test_ansible.py
--rw-r--r--   0 runner    (1001) docker     (999)     7105 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/a_unit/provisioner/test_ansible_playbook.py
--rw-r--r--   0 runner    (1001) docker     (999)     4527 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/a_unit/provisioner/test_ansible_playbooks.py
--rw-r--r--   0 runner    (1001) docker     (999)     1625 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/a_unit/test_api.py
--rw-r--r--   0 runner    (1001) docker     (999)    11459 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/a_unit/test_config.py
--rw-r--r--   0 runner    (1001) docker     (999)     3647 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/a_unit/test_interpolation.py
--rw-r--r--   0 runner    (1001) docker     (999)     4156 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/a_unit/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (999)     2281 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/a_unit/test_platforms.py
--rw-r--r--   0 runner    (1001) docker     (999)     6784 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/a_unit/test_scenario.py
--rw-r--r--   0 runner    (1001) docker     (999)     6229 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/a_unit/test_scenarios.py
--rw-r--r--   0 runner    (1001) docker     (999)     2279 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/a_unit/test_scenarios_ordered.py
--rw-r--r--   0 runner    (1001) docker     (999)     1247 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/a_unit/test_shell.py
--rw-r--r--   0 runner    (1001) docker     (999)     3245 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/a_unit/test_state.py
--rw-r--r--   0 runner    (1001) docker     (999)     1960 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/a_unit/test_status.py
--rw-r--r--   0 runner    (1001) docker     (999)      824 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/a_unit/test_text.py
--rw-r--r--   0 runner    (1001) docker     (999)     9362 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/a_unit/test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.399365 molecule-6.0.2/src/molecule/test/a_unit/verifier/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/a_unit/verifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     2776 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/a_unit/verifier/test_ansible.py
--rw-r--r--   0 runner    (1001) docker     (999)     8714 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/a_unit/verifier/test_testinfra.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.399365 molecule-6.0.2/src/molecule/test/b_functional/
--rw-r--r--   0 runner    (1001) docker     (999)      398 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/b_functional/.ansible-lint
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/b_functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     8286 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/b_functional/conftest.py
--rw-r--r--   0 runner    (1001) docker     (999)    11617 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/b_functional/test_command.py
--rw-r--r--   0 runner    (1001) docker     (999)     4697 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.399365 molecule-6.0.2/src/molecule/test/resources/
--rw-r--r--   0 runner    (1001) docker     (999)      172 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/resources/.yamllint
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.399365 molecule-6.0.2/src/molecule/test/resources/invalid_role_template/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.399365 molecule-6.0.2/src/molecule/test/resources/invalid_role_template/bad_format/
--rw-r--r--   0 runner    (1001) docker     (999)      205 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/resources/invalid_role_template/bad_format/README.md
--rw-r--r--   0 runner    (1001) docker     (999)       65 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/resources/invalid_role_template/cookiecutter.json
--rw-r--r--   0 runner    (1001) docker     (999)      157 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/resources/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.363365 molecule-6.0.2/src/molecule/test/resources/playbooks/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.399365 molecule-6.0.2/src/molecule/test/resources/playbooks/delegated/
--rw-r--r--   0 runner    (1001) docker     (999)      138 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/resources/playbooks/delegated/create.yml
--rw-r--r--   0 runner    (1001) docker     (999)      140 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/resources/playbooks/delegated/destroy.yml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.363365 molecule-6.0.2/src/molecule/test/resources/playbooks/delegated/inventory/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.363365 molecule-6.0.2/src/molecule/test/resources/playbooks/delegated/inventory/group_vars/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.399365 molecule-6.0.2/src/molecule/test/resources/playbooks/delegated/inventory/group_vars/all/
--rw-r--r--   0 runner    (1001) docker     (999)       19 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/resources/playbooks/delegated/inventory/group_vars/all/all.yml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.363365 molecule-6.0.2/src/molecule/test/resources/roles/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.363365 molecule-6.0.2/src/molecule/test/resources/roles/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.399365 molecule-6.0.2/src/molecule/test/resources/roles/molecule/meta/
--rw-r--r--   0 runner    (1001) docker     (999)      234 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/resources/roles/molecule/meta/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.399365 molecule-6.0.2/src/molecule/test/resources/roles/molecule/tasks/
--rw-r--r--   0 runner    (1001) docker     (999)      330 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/resources/roles/molecule/tasks/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.399365 molecule-6.0.2/src/molecule/test/resources/sample-collection/
--rw-r--r--   0 runner    (1001) docker     (999)      488 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/resources/sample-collection/galaxy.yml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.363365 molecule-6.0.2/src/molecule/test/resources/sample-collection/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.399365 molecule-6.0.2/src/molecule/test/resources/sample-collection/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (999)      179 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/resources/sample-collection/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (999)      140 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/resources/sample-collection/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.367365 molecule-6.0.2/src/molecule/test/resources/sample-collection/roles/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.367365 molecule-6.0.2/src/molecule/test/resources/sample-collection/roles/get_rich/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.399365 molecule-6.0.2/src/molecule/test/resources/sample-collection/roles/get_rich/tasks/
--rw-r--r--   0 runner    (1001) docker     (999)       95 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/resources/sample-collection/roles/get_rich/tasks/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.367365 molecule-6.0.2/src/molecule/test/resources/schema_instance_files/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.399365 molecule-6.0.2/src/molecule/test/resources/schema_instance_files/invalid/
--rw-r--r--   0 runner    (1001) docker     (999)      100 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/resources/schema_instance_files/invalid/molecule_delegated.yml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.399365 molecule-6.0.2/src/molecule/test/resources/schema_instance_files/valid/
--rw-r--r--   0 runner    (1001) docker     (999)     1226 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/resources/schema_instance_files/valid/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.399365 molecule-6.0.2/src/molecule/test/scenarios/
--rw-r--r--   0 runner    (1001) docker     (999)      378 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/scenarios/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.367365 molecule-6.0.2/src/molecule/test/scenarios/cleanup/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.367365 molecule-6.0.2/src/molecule/test/scenarios/cleanup/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.399365 molecule-6.0.2/src/molecule/test/scenarios/cleanup/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (999)      156 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/scenarios/cleanup/molecule/default/cleanup.yml
--rw-r--r--   0 runner    (1001) docker     (999)      182 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/scenarios/cleanup/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (999)      253 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/scenarios/cleanup/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.399365 molecule-6.0.2/src/molecule/test/scenarios/cleanup/molecule/default/tests/
--rw-r--r--   0 runner    (1001) docker     (999)      369 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/scenarios/cleanup/molecule/default/tests/test_cleanup.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.367365 molecule-6.0.2/src/molecule/test/scenarios/dependency/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.367365 molecule-6.0.2/src/molecule/test/scenarios/dependency/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.399365 molecule-6.0.2/src/molecule/test/scenarios/dependency/molecule/ansible-galaxy/
--rw-r--r--   0 runner    (1001) docker     (999)      463 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/scenarios/dependency/molecule/ansible-galaxy/converge.yml
--rw-r--r--   0 runner    (1001) docker     (999)      334 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/scenarios/dependency/molecule/ansible-galaxy/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (999)      218 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/scenarios/dependency/molecule/ansible-galaxy/requirements.yml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.399365 molecule-6.0.2/src/molecule/test/scenarios/dependency/molecule/shell/
--rw-r--r--   0 runner    (1001) docker     (999)      463 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/scenarios/dependency/molecule/shell/converge.yml
--rw-r--r--   0 runner    (1001) docker     (999)      443 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/scenarios/dependency/molecule/shell/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.367365 molecule-6.0.2/src/molecule/test/scenarios/driver/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.367365 molecule-6.0.2/src/molecule/test/scenarios/driver/delegated/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.399365 molecule-6.0.2/src/molecule/test/scenarios/driver/delegated/meta/
--rw-r--r--   0 runner    (1001) docker     (999)      178 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/scenarios/driver/delegated/meta/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.367365 molecule-6.0.2/src/molecule/test/scenarios/driver/delegated/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.399365 molecule-6.0.2/src/molecule/test/scenarios/driver/delegated/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (999)       72 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/scenarios/driver/delegated/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (999)       54 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/scenarios/driver/delegated/molecule/default/create.yml
--rw-r--r--   0 runner    (1001) docker     (999)       55 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/scenarios/driver/delegated/molecule/default/destroy.yml
--rw-r--r--   0 runner    (1001) docker     (999)      325 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/scenarios/driver/delegated/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.367365 molecule-6.0.2/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.403365 molecule-6.0.2/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/meta/
--rw-r--r--   0 runner    (1001) docker     (999)      178 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/meta/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.367365 molecule-6.0.2/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.403365 molecule-6.0.2/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (999)       72 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (999)       54 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/molecule/default/create.yml
--rw-r--r--   0 runner    (1001) docker     (999)       55 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/molecule/default/destroy.yml
--rw-r--r--   0 runner    (1001) docker     (999)      344 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.403365 molecule-6.0.2/src/molecule/test/scenarios/host_group_vars/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.367365 molecule-6.0.2/src/molecule/test/scenarios/host_group_vars/group_vars/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.403365 molecule-6.0.2/src/molecule/test/scenarios/host_group_vars/group_vars/example/
--rw-r--r--   0 runner    (1001) docker     (999)       44 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/scenarios/host_group_vars/group_vars/example/all.yml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.403365 molecule-6.0.2/src/molecule/test/scenarios/host_group_vars/host_vars/
--rw-r--r--   0 runner    (1001) docker     (999)       44 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/scenarios/host_group_vars/host_vars/extra-host
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.403365 molecule-6.0.2/src/molecule/test/scenarios/host_group_vars/host_vars/instance/
--rw-r--r--   0 runner    (1001) docker     (999)       43 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/scenarios/host_group_vars/host_vars/instance/all.yml
--rw-r--r--   0 runner    (1001) docker     (999)       11 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/scenarios/host_group_vars/hosts
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.367365 molecule-6.0.2/src/molecule/test/scenarios/host_group_vars/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.403365 molecule-6.0.2/src/molecule/test/scenarios/host_group_vars/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (999)     1336 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/scenarios/host_group_vars/molecule/default/converge.yml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.367365 molecule-6.0.2/src/molecule/test/scenarios/host_group_vars/molecule/default/group_vars/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.403365 molecule-6.0.2/src/molecule/test/scenarios/host_group_vars/molecule/default/group_vars/example/
--rw-r--r--   0 runner    (1001) docker     (999)       41 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/scenarios/host_group_vars/molecule/default/group_vars/example/all.yml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.367365 molecule-6.0.2/src/molecule/test/scenarios/host_group_vars/molecule/default/host_vars/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.403365 molecule-6.0.2/src/molecule/test/scenarios/host_group_vars/molecule/default/host_vars/instance/
--rw-r--r--   0 runner    (1001) docker     (999)       40 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/scenarios/host_group_vars/molecule/default/host_vars/instance/all.yml
--rw-r--r--   0 runner    (1001) docker     (999)      674 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/scenarios/host_group_vars/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.403365 molecule-6.0.2/src/molecule/test/scenarios/host_group_vars/molecule/links/
--rw-r--r--   0 runner    (1001) docker     (999)      442 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/scenarios/host_group_vars/molecule/links/converge.yml
--rw-r--r--   0 runner    (1001) docker     (999)      373 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/scenarios/host_group_vars/molecule/links/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.367365 molecule-6.0.2/src/molecule/test/scenarios/idempotence/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.367365 molecule-6.0.2/src/molecule/test/scenarios/idempotence/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.403365 molecule-6.0.2/src/molecule/test/scenarios/idempotence/molecule/raises/
--rw-r--r--   0 runner    (1001) docker     (999)       98 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/scenarios/idempotence/molecule/raises/converge.yml
--rw-r--r--   0 runner    (1001) docker     (999)      291 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/scenarios/idempotence/molecule/raises/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.403365 molecule-6.0.2/src/molecule/test/scenarios/idempotence/tasks/
--rw-r--r--   0 runner    (1001) docker     (999)      388 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/scenarios/idempotence/tasks/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.367365 molecule-6.0.2/src/molecule/test/scenarios/interpolation/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.367365 molecule-6.0.2/src/molecule/test/scenarios/interpolation/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.403365 molecule-6.0.2/src/molecule/test/scenarios/interpolation/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (999)      155 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/scenarios/interpolation/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (999)      183 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/scenarios/interpolation/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.367365 molecule-6.0.2/src/molecule/test/scenarios/overrride_driver/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.367365 molecule-6.0.2/src/molecule/test/scenarios/overrride_driver/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.403365 molecule-6.0.2/src/molecule/test/scenarios/overrride_driver/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (999)      155 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/scenarios/overrride_driver/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (999)      170 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/scenarios/overrride_driver/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.367365 molecule-6.0.2/src/molecule/test/scenarios/side_effect/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.367365 molecule-6.0.2/src/molecule/test/scenarios/side_effect/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.403365 molecule-6.0.2/src/molecule/test/scenarios/side_effect/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (999)      328 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/scenarios/side_effect/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (999)      261 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/scenarios/side_effect/molecule/default/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (999)      238 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/scenarios/side_effect/molecule/default/side_effect.yml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.403365 molecule-6.0.2/src/molecule/test/scenarios/side_effect/molecule/default/tests/
--rw-r--r--   0 runner    (1001) docker     (999)      334 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/scenarios/side_effect/molecule/default/tests/test_side_effect.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.367365 molecule-6.0.2/src/molecule/test/scenarios/test_destroy_strategy/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.367365 molecule-6.0.2/src/molecule/test/scenarios/test_destroy_strategy/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.403365 molecule-6.0.2/src/molecule/test/scenarios/test_destroy_strategy/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (999)      159 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/scenarios/test_destroy_strategy/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (999)      170 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/scenarios/test_destroy_strategy/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.403365 molecule-6.0.2/src/molecule/test/scenarios/test_destroy_strategy/molecule/default/tests/
--rw-r--r--   0 runner    (1001) docker     (999)      786 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/scenarios/test_destroy_strategy/molecule/default/tests/test_destroy_strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.403365 molecule-6.0.2/src/molecule/test/scenarios/verifier/
--rw-r--r--   0 runner    (1001) docker     (999)      181 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/scenarios/verifier/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.371365 molecule-6.0.2/src/molecule/test/scenarios/verifier/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.403365 molecule-6.0.2/src/molecule/test/scenarios/verifier/molecule/testinfra/
--rw-r--r--   0 runner    (1001) docker     (999)       80 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/scenarios/verifier/molecule/testinfra/converge.yml
--rw-r--r--   0 runner    (1001) docker     (999)      339 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/scenarios/verifier/molecule/testinfra/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.403365 molecule-6.0.2/src/molecule/test/scenarios/verifier/molecule/testinfra/shared/
--rw-r--r--   0 runner    (1001) docker     (999)      335 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/scenarios/verifier/molecule/testinfra/shared/test_shared.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.407365 molecule-6.0.2/src/molecule/test/scenarios/verifier/molecule/testinfra/tests/
--rw-r--r--   0 runner    (1001) docker     (999)      335 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/scenarios/verifier/molecule/testinfra/tests/test_testinfra.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.403365 molecule-6.0.2/src/molecule/test/scenarios/verifier/molecule/testinfra-pre-commit/
--rw-r--r--   0 runner    (1001) docker     (999)      455 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/scenarios/verifier/molecule/testinfra-pre-commit/converge.yml
--rw-r--r--   0 runner    (1001) docker     (999)      290 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/scenarios/verifier/molecule/testinfra-pre-commit/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.403365 molecule-6.0.2/src/molecule/test/scenarios/verifier/molecule/testinfra-pre-commit/tests/
--rw-r--r--   0 runner    (1001) docker     (999)      157 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/test/scenarios/verifier/molecule/testinfra-pre-commit/tests/test_testinfra_pre_commit.py
--rw-r--r--   0 runner    (1001) docker     (999)     1446 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/text.py
--rw-r--r--   0 runner    (1001) docker     (999)    11940 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/util.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.407365 molecule-6.0.2/src/molecule/verifier/
--rw-r--r--   0 runner    (1001) docker     (999)        7 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/verifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     2677 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/verifier/ansible.py
--rw-r--r--   0 runner    (1001) docker     (999)     3556 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/verifier/base.py
--rw-r--r--   0 runner    (1001) docker     (999)     6724 2023-08-30 10:21:49.000000 molecule-6.0.2/src/molecule/verifier/testinfra.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.383365 molecule-6.0.2/src/molecule.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)     4674 2023-08-30 10:22:05.000000 molecule-6.0.2/src/molecule.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)    14037 2023-08-30 10:22:05.000000 molecule-6.0.2/src/molecule.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-30 10:22:05.000000 molecule-6.0.2/src/molecule.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)      232 2023-08-30 10:22:05.000000 molecule-6.0.2/src/molecule.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (999)      485 2023-08-30 10:22:05.000000 molecule-6.0.2/src/molecule.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (999)        9 2023-08-30 10:22:05.000000 molecule-6.0.2/src/molecule.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 10:22:05.407365 molecule-6.0.2/tools/
--rwxr-xr-x   0 runner    (1001) docker     (999)      248 2023-08-30 10:21:49.000000 molecule-6.0.2/tools/get-version.sh
--rw-r--r--   0 runner    (1001) docker     (999)        7 2023-08-30 10:21:49.000000 molecule-6.0.2/tools/opts.txt
--rwxr-xr-x   0 runner    (1001) docker     (999)      235 2023-08-30 10:21:49.000000 molecule-6.0.2/tools/smoketest.sh
--rwxr-xr-x   0 runner    (1001) docker     (999)      688 2023-08-30 10:21:49.000000 molecule-6.0.2/tools/test-setup.sh
--rwxr-xr-x   0 runner    (1001) docker     (999)      214 2023-08-30 10:21:49.000000 molecule-6.0.2/tools/update-version.sh
--rw-r--r--   0 runner    (1001) docker     (999)     4334 2023-08-30 10:21:49.000000 molecule-6.0.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.587156 molecule-6.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2023-12-13 13:38:02.000000 molecule-6.0.3/.ansible-lint
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2023-12-13 13:38:02.000000 molecule-6.0.3/.ansible-lint-ignore
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2023-12-13 13:38:02.000000 molecule-6.0.3/.ansible.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2023-12-13 13:38:02.000000 molecule-6.0.3/.codespellrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.527156 molecule-6.0.3/.config/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.527156 molecule-6.0.3/.config/molecule/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2023-12-13 13:38:02.000000 molecule-6.0.3/.config/molecule/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2023-12-13 13:38:02.000000 molecule-6.0.3/.config/molecule.spec
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2023-12-13 13:38:02.000000 molecule-6.0.3/.config/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2023-12-13 13:38:02.000000 molecule-6.0.3/.config/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2023-12-13 13:38:02.000000 molecule-6.0.3/.config/requirements-testinfra.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2023-12-13 13:38:02.000000 molecule-6.0.3/.config/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2023-12-13 13:38:02.000000 molecule-6.0.3/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3269 2023-12-13 13:38:02.000000 molecule-6.0.3/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.527156 molecule-6.0.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2023-12-13 13:38:02.000000 molecule-6.0.3/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2023-12-13 13:38:02.000000 molecule-6.0.3/.github/CODE_OF_CONDUCT.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.527156 molecule-6.0.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     2781 2023-12-13 13:38:02.000000 molecule-6.0.3/.github/ISSUE_TEMPLATE/bug.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2023-12-13 13:38:02.000000 molecule-6.0.3/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2023-12-13 13:38:02.000000 molecule-6.0.3/.github/ISSUE_TEMPLATE/security_bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2023-12-13 13:38:02.000000 molecule-6.0.3/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2023-12-13 13:38:02.000000 molecule-6.0.3/.github/patchback.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2023-12-13 13:38:02.000000 molecule-6.0.3/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.531156 molecule-6.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2023-12-13 13:38:02.000000 molecule-6.0.3/.github/workflows/ack.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2023-12-13 13:38:02.000000 molecule-6.0.3/.github/workflows/push.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2023-12-13 13:38:02.000000 molecule-6.0.3/.github/workflows/redirects.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2023-12-13 13:38:02.000000 molecule-6.0.3/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4569 2023-12-13 13:38:02.000000 molecule-6.0.3/.github/workflows/tox.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2023-12-13 13:38:02.000000 molecule-6.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2023-12-13 13:38:02.000000 molecule-6.0.3/.npmrc
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2023-12-13 13:38:02.000000 molecule-6.0.3/.packit.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2023-12-13 13:38:02.000000 molecule-6.0.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2023-12-13 13:38:02.000000 molecule-6.0.3/.readthedocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.531156 molecule-6.0.3/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2023-12-13 13:38:02.000000 molecule-6.0.3/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2023-12-13 13:38:02.000000 molecule-6.0.3/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2023-12-13 13:38:02.000000 molecule-6.0.3/.yamllint
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2023-12-13 13:38:02.000000 molecule-6.0.3/DCO_1_1.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2023-12-13 13:38:02.000000 molecule-6.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2023-12-13 13:38:02.000000 molecule-6.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5822 2023-12-13 13:38:15.587156 molecule-6.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3080 2023-12-13 13:38:02.000000 molecule-6.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2023-12-13 13:38:02.000000 molecule-6.0.3/bindep.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2023-12-13 13:38:02.000000 molecule-6.0.3/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2023-12-13 13:38:02.000000 molecule-6.0.3/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.531156 molecule-6.0.3/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.507156 molecule-6.0.3/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.535156 molecule-6.0.3/docs/_static/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2023-12-13 13:38:02.000000 molecule-6.0.3/docs/_static/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    33945 2023-12-13 13:38:02.000000 molecule-6.0.3/docs/_static/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)   143898 2023-12-13 13:38:02.000000 molecule-6.0.3/docs/_static/images/logo_big.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10447 2023-12-13 13:38:02.000000 molecule-6.0.3/docs/ci.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7985 2023-12-13 13:38:02.000000 molecule-6.0.3/docs/configuration.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3722 2023-12-13 13:38:02.000000 molecule-6.0.3/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2023-12-13 13:38:02.000000 molecule-6.0.3/docs/docker.md
+-rw-r--r--   0 runner    (1001) docker     (127)    12907 2023-12-13 13:38:02.000000 molecule-6.0.3/docs/examples.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3999 2023-12-13 13:38:02.000000 molecule-6.0.3/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7667 2023-12-13 13:38:02.000000 molecule-6.0.3/docs/getting-started.md
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2023-12-13 13:38:02.000000 molecule-6.0.3/docs/google04e29a42ae6e6cbc.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.535156 molecule-6.0.3/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    41215 2023-12-13 13:38:02.000000 molecule-6.0.3/docs/images/collection_structure.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2023-12-13 13:38:02.000000 molecule-6.0.3/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4597 2023-12-13 13:38:02.000000 molecule-6.0.3/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4516 2023-12-13 13:38:02.000000 molecule-6.0.3/docs/kubevirt.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2023-12-13 13:38:02.000000 molecule-6.0.3/docs/next.md
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2023-12-13 13:38:02.000000 molecule-6.0.3/docs/podman.md
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2023-12-13 13:38:02.000000 molecule-6.0.3/docs/redirects.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2171 2023-12-13 13:38:02.000000 molecule-6.0.3/docs/usage.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.507156 molecule-6.0.3/docs/working/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.535156 molecule-6.0.3/docs/working/contributor_guide/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2023-12-13 13:38:02.000000 molecule-6.0.3/docs/working/contributor_guide/code_of_conduct.md
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2023-12-13 13:38:02.000000 molecule-6.0.3/docs/working/contributor_guide/contribution_requirements.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2023-12-13 13:38:02.000000 molecule-6.0.3/docs/working/contributor_guide/developer_contact.md
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2023-12-13 13:38:02.000000 molecule-6.0.3/docs/working/contributor_guide/environment_setup.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.535156 molecule-6.0.3/docs/working/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2023-12-13 13:38:02.000000 molecule-6.0.3/docs/working/examples/example_1.md
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2023-12-13 13:38:02.000000 molecule-6.0.3/docs/working/examples/example_2.md
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2023-12-13 13:38:02.000000 molecule-6.0.3/docs/working/examples/example_3.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.535156 molecule-6.0.3/docs/working/faq/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2023-12-13 13:38:02.000000 molecule-6.0.3/docs/working/faq/faq.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.535156 molecule-6.0.3/docs/working/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2023-12-13 13:38:02.000000 molecule-6.0.3/docs/working/getting_started/getting_started.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.535156 molecule-6.0.3/docs/working/installation/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2023-12-13 13:38:02.000000 molecule-6.0.3/docs/working/installation/install.md
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2023-12-13 13:38:02.000000 molecule-6.0.3/docs/working/installation/upgrade.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.535156 molecule-6.0.3/docs/working/introduction/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2023-12-13 13:38:02.000000 molecule-6.0.3/docs/working/introduction/introduction.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.535156 molecule-6.0.3/docs/working/references/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2023-12-13 13:38:02.000000 molecule-6.0.3/docs/working/references/cli.md
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2023-12-13 13:38:02.000000 molecule-6.0.3/docs/working/references/configuration.md
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2023-12-13 13:38:02.000000 molecule-6.0.3/docs/working/references/porting_change_log.md
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2023-12-13 13:38:02.000000 molecule-6.0.3/docs/working/references/road_map.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.539156 molecule-6.0.3/docs/working/user_guide/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2023-12-13 13:38:02.000000 molecule-6.0.3/docs/working/user_guide/ci_integration.md
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2023-12-13 13:38:02.000000 molecule-6.0.3/docs/working/user_guide/creating_testing_collection.md
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-13 13:38:02.000000 molecule-6.0.3/docs/working/user_guide/testing_existing_collection.md
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2023-12-13 13:38:02.000000 molecule-6.0.3/docs/working/user_guide/testing_existing_roles.md
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2023-12-13 13:38:02.000000 molecule-6.0.3/docs/working/user_guide/understanding.md
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2023-12-13 13:38:02.000000 molecule-6.0.3/docs/working/user_guide/using_tox-ansible.md
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2023-12-13 13:38:02.000000 molecule-6.0.3/linkcheckerrc
+-rw-r--r--   0 runner    (1001) docker     (127)     4056 2023-12-13 13:38:02.000000 molecule-6.0.3/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.507156 molecule-6.0.3/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.539156 molecule-6.0.3/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2023-12-13 13:38:02.000000 molecule-6.0.3/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2023-12-13 13:38:02.000000 molecule-6.0.3/molecule/default/create.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2023-12-13 13:38:02.000000 molecule-6.0.3/molecule/default/destroy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2023-12-13 13:38:02.000000 molecule-6.0.3/molecule/default/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.539156 molecule-6.0.3/molecule/docker/
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2023-12-13 13:38:02.000000 molecule-6.0.3/molecule/docker/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2023-12-13 13:38:02.000000 molecule-6.0.3/molecule/docker/create.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2023-12-13 13:38:02.000000 molecule-6.0.3/molecule/docker/destroy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2023-12-13 13:38:02.000000 molecule-6.0.3/molecule/docker/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2023-12-13 13:38:02.000000 molecule-6.0.3/molecule/docker/requirements.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.539156 molecule-6.0.3/molecule/docker/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2023-12-13 13:38:02.000000 molecule-6.0.3/molecule/docker/tasks/create-fail.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.539156 molecule-6.0.3/molecule/kubevirt/
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2023-12-13 13:38:02.000000 molecule-6.0.3/molecule/kubevirt/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4364 2023-12-13 13:38:02.000000 molecule-6.0.3/molecule/kubevirt/create.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2023-12-13 13:38:02.000000 molecule-6.0.3/molecule/kubevirt/destroy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2023-12-13 13:38:02.000000 molecule-6.0.3/molecule/kubevirt/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2023-12-13 13:38:02.000000 molecule-6.0.3/molecule/kubevirt/requirements.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.539156 molecule-6.0.3/molecule/kubevirt/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)     2821 2023-12-13 13:38:02.000000 molecule-6.0.3/molecule/kubevirt/tasks/create_vm.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2023-12-13 13:38:02.000000 molecule-6.0.3/molecule/kubevirt/tasks/create_vm_dictionary.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.543156 molecule-6.0.3/molecule/podman/
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2023-12-13 13:38:02.000000 molecule-6.0.3/molecule/podman/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2023-12-13 13:38:02.000000 molecule-6.0.3/molecule/podman/create.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2023-12-13 13:38:02.000000 molecule-6.0.3/molecule/podman/destroy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2023-12-13 13:38:02.000000 molecule-6.0.3/molecule/podman/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2023-12-13 13:38:02.000000 molecule-6.0.3/molecule/podman/requirements.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.543156 molecule-6.0.3/molecule/podman/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2023-12-13 13:38:02.000000 molecule-6.0.3/molecule/podman/tasks/create-fail.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.543156 molecule-6.0.3/molecule/smoke/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2023-12-13 13:38:02.000000 molecule-6.0.3/molecule/smoke/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2023-12-13 13:38:02.000000 molecule-6.0.3/molecule/smoke/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.543156 molecule-6.0.3/playbooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2023-12-13 13:38:02.000000 molecule-6.0.3/playbooks/snap-pre-run.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6610 2023-12-13 13:38:02.000000 molecule-6.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2023-12-13 13:38:02.000000 molecule-6.0.3/requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2023-12-13 13:38:02.000000 molecule-6.0.3/runtime.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 13:38:15.587156 molecule-6.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.543156 molecule-6.0.3/snap/
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2023-12-13 13:38:02.000000 molecule-6.0.3/snap/snapcraft.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.507156 molecule-6.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.547156 molecule-6.0.3/src/molecule/
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2023-12-13 13:38:02.000000 molecule-6.0.3/src/molecule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2023-12-13 13:38:02.000000 molecule-6.0.3/src/molecule/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2023-12-13 13:38:15.000000 molecule-6.0.3/src/molecule/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2425 2023-12-13 13:38:02.000000 molecule-6.0.3/src/molecule/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2023-12-13 13:38:02.000000 molecule-6.0.3/src/molecule/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.551156 molecule-6.0.3/src/molecule/command/
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2023-12-13 13:38:02.000000 molecule-6.0.3/src/molecule/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10206 2023-12-13 13:38:02.000000 molecule-6.0.3/src/molecule/command/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2460 2023-12-13 13:38:02.000000 molecule-6.0.3/src/molecule/command/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2023-12-13 13:38:02.000000 molecule-6.0.3/src/molecule/command/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 2023-12-13 13:38:02.000000 molecule-6.0.3/src/molecule/command/converge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2023-12-13 13:38:02.000000 molecule-6.0.3/src/molecule/command/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2023-12-13 13:38:02.000000 molecule-6.0.3/src/molecule/command/dependency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3101 2023-12-13 13:38:02.000000 molecule-6.0.3/src/molecule/command/destroy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2023-12-13 13:38:02.000000 molecule-6.0.3/src/molecule/command/drivers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4522 2023-12-13 13:38:02.000000 molecule-6.0.3/src/molecule/command/idempotence.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.551156 molecule-6.0.3/src/molecule/command/init/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2023-12-13 13:38:02.000000 molecule-6.0.3/src/molecule/command/init/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2023-12-13 13:38:02.000000 molecule-6.0.3/src/molecule/command/init/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2023-12-13 13:38:02.000000 molecule-6.0.3/src/molecule/command/init/init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5388 2023-12-13 13:38:02.000000 molecule-6.0.3/src/molecule/command/init/scenario.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3696 2023-12-13 13:38:02.000000 molecule-6.0.3/src/molecule/command/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4896 2023-12-13 13:38:02.000000 molecule-6.0.3/src/molecule/command/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2772 2023-12-13 13:38:02.000000 molecule-6.0.3/src/molecule/command/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4301 2023-12-13 13:38:02.000000 molecule-6.0.3/src/molecule/command/prepare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2023-12-13 13:38:02.000000 molecule-6.0.3/src/molecule/command/reset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2392 2023-12-13 13:38:02.000000 molecule-6.0.3/src/molecule/command/side_effect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2023-12-13 13:38:02.000000 molecule-6.0.3/src/molecule/command/syntax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3541 2023-12-13 13:38:02.000000 molecule-6.0.3/src/molecule/command/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2023-12-13 13:38:02.000000 molecule-6.0.3/src/molecule/command/verify.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17530 2023-12-13 13:38:02.000000 molecule-6.0.3/src/molecule/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2749 2023-12-13 13:38:02.000000 molecule-6.0.3/src/molecule/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2023-12-13 13:38:02.000000 molecule-6.0.3/src/molecule/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.551156 molecule-6.0.3/src/molecule/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2023-12-13 13:38:02.000000 molecule-6.0.3/src/molecule/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2554 2023-12-13 13:38:02.000000 molecule-6.0.3/src/molecule/data/driver.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2023-12-13 13:38:02.000000 molecule-6.0.3/src/molecule/data/init-scenario.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    14472 2023-12-13 13:38:02.000000 molecule-6.0.3/src/molecule/data/molecule.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.511156 molecule-6.0.3/src/molecule/data/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.555156 molecule-6.0.3/src/molecule/data/templates/scenario/
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2023-12-13 13:38:02.000000 molecule-6.0.3/src/molecule/data/templates/scenario/converge.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2023-12-13 13:38:02.000000 molecule-6.0.3/src/molecule/data/templates/scenario/create.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2023-12-13 13:38:02.000000 molecule-6.0.3/src/molecule/data/templates/scenario/destroy.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2023-12-13 13:38:02.000000 molecule-6.0.3/src/molecule/data/templates/scenario/molecule.yml.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.555156 molecule-6.0.3/src/molecule/dependency/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2023-12-13 13:38:02.000000 molecule-6.0.3/src/molecule/dependency/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.555156 molecule-6.0.3/src/molecule/dependency/ansible_galaxy/
+-rw-r--r--   0 runner    (1001) docker     (127)     4055 2023-12-13 13:38:02.000000 molecule-6.0.3/src/molecule/dependency/ansible_galaxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4060 2023-12-13 13:38:02.000000 molecule-6.0.3/src/molecule/dependency/ansible_galaxy/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2023-12-13 13:38:02.000000 molecule-6.0.3/src/molecule/dependency/ansible_galaxy/collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2023-12-13 13:38:02.000000 molecule-6.0.3/src/molecule/dependency/ansible_galaxy/roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4217 2023-12-13 13:38:02.000000 molecule-6.0.3/src/molecule/dependency/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3229 2023-12-13 13:38:02.000000 molecule-6.0.3/src/molecule/dependency/shell.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.555156 molecule-6.0.3/src/molecule/driver/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2023-12-13 13:38:02.000000 molecule-6.0.3/src/molecule/driver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8872 2023-12-13 13:38:02.000000 molecule-6.0.3/src/molecule/driver/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8917 2023-12-13 13:38:02.000000 molecule-6.0.3/src/molecule/driver/delegated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4471 2023-12-13 13:38:02.000000 molecule-6.0.3/src/molecule/interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6713 2023-12-13 13:38:02.000000 molecule-6.0.3/src/molecule/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.555156 molecule-6.0.3/src/molecule/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2023-12-13 13:38:02.000000 molecule-6.0.3/src/molecule/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2023-12-13 13:38:02.000000 molecule-6.0.3/src/molecule/model/schema_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2944 2023-12-13 13:38:02.000000 molecule-6.0.3/src/molecule/platforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.555156 molecule-6.0.3/src/molecule/provisioner/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2023-12-13 13:38:02.000000 molecule-6.0.3/src/molecule/provisioner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33606 2023-12-13 13:38:02.000000 molecule-6.0.3/src/molecule/provisioner/ansible.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5681 2023-12-13 13:38:02.000000 molecule-6.0.3/src/molecule/provisioner/ansible_playbook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5036 2023-12-13 13:38:02.000000 molecule-6.0.3/src/molecule/provisioner/ansible_playbooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2023-12-13 13:38:02.000000 molecule-6.0.3/src/molecule/provisioner/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:02.000000 molecule-6.0.3/src/molecule/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     7686 2023-12-13 13:38:02.000000 molecule-6.0.3/src/molecule/scenario.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4754 2023-12-13 13:38:02.000000 molecule-6.0.3/src/molecule/scenarios.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5843 2023-12-13 13:38:02.000000 molecule-6.0.3/src/molecule/shell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4681 2023-12-13 13:38:02.000000 molecule-6.0.3/src/molecule/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2023-12-13 13:38:02.000000 molecule-6.0.3/src/molecule/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2023-12-13 13:38:02.000000 molecule-6.0.3/src/molecule/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11937 2023-12-13 13:38:02.000000 molecule-6.0.3/src/molecule/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.559156 molecule-6.0.3/src/molecule/verifier/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2023-12-13 13:38:02.000000 molecule-6.0.3/src/molecule/verifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2023-12-13 13:38:02.000000 molecule-6.0.3/src/molecule/verifier/ansible.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3556 2023-12-13 13:38:02.000000 molecule-6.0.3/src/molecule/verifier/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6724 2023-12-13 13:38:02.000000 molecule-6.0.3/src/molecule/verifier/testinfra.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.583156 molecule-6.0.3/src/molecule.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5822 2023-12-13 13:38:15.000000 molecule-6.0.3/src/molecule.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12342 2023-12-13 13:38:15.000000 molecule-6.0.3/src/molecule.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 13:38:15.000000 molecule-6.0.3/src/molecule.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2023-12-13 13:38:15.000000 molecule-6.0.3/src/molecule.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2023-12-13 13:38:15.000000 molecule-6.0.3/src/molecule.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-13 13:38:15.000000 molecule-6.0.3/src/molecule.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.559156 molecule-6.0.3/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:02.000000 molecule-6.0.3/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.559156 molecule-6.0.3/test/a_unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:02.000000 molecule-6.0.3/test/a_unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.563156 molecule-6.0.3/test/a_unit/command/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:02.000000 molecule-6.0.3/test/a_unit/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2023-12-13 13:38:02.000000 molecule-6.0.3/test/a_unit/command/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.563156 molecule-6.0.3/test/a_unit/command/init/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:02.000000 molecule-6.0.3/test/a_unit/command/init/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2279 2023-12-13 13:38:02.000000 molecule-6.0.3/test/a_unit/command/init/test_scenario.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10062 2023-12-13 13:38:02.000000 molecule-6.0.3/test/a_unit/command/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2023-12-13 13:38:02.000000 molecule-6.0.3/test/a_unit/command/test_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2628 2023-12-13 13:38:02.000000 molecule-6.0.3/test/a_unit/command/test_cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2703 2023-12-13 13:38:02.000000 molecule-6.0.3/test/a_unit/command/test_converge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2023-12-13 13:38:02.000000 molecule-6.0.3/test/a_unit/command/test_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2023-12-13 13:38:02.000000 molecule-6.0.3/test/a_unit/command/test_dependency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2023-12-13 13:38:02.000000 molecule-6.0.3/test/a_unit/command/test_destroy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5086 2023-12-13 13:38:02.000000 molecule-6.0.3/test/a_unit/command/test_idempotence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2023-12-13 13:38:02.000000 molecule-6.0.3/test/a_unit/command/test_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4670 2023-12-13 13:38:02.000000 molecule-6.0.3/test/a_unit/command/test_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2023-12-13 13:38:02.000000 molecule-6.0.3/test/a_unit/command/test_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3299 2023-12-13 13:38:02.000000 molecule-6.0.3/test/a_unit/command/test_prepare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2796 2023-12-13 13:38:02.000000 molecule-6.0.3/test/a_unit/command/test_side_effect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2023-12-13 13:38:02.000000 molecule-6.0.3/test/a_unit/command/test_syntax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2023-12-13 13:38:02.000000 molecule-6.0.3/test/a_unit/command/test_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1712 2023-12-13 13:38:02.000000 molecule-6.0.3/test/a_unit/command/test_verify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6419 2023-12-13 13:38:02.000000 molecule-6.0.3/test/a_unit/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.563156 molecule-6.0.3/test/a_unit/cookiecutter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:02.000000 molecule-6.0.3/test/a_unit/cookiecutter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2023-12-13 13:38:02.000000 molecule-6.0.3/test/a_unit/cookiecutter/test_molecule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.563156 molecule-6.0.3/test/a_unit/dependency/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:02.000000 molecule-6.0.3/test/a_unit/dependency/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.567156 molecule-6.0.3/test/a_unit/dependency/ansible_galaxy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:02.000000 molecule-6.0.3/test/a_unit/dependency/ansible_galaxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6136 2023-12-13 13:38:02.000000 molecule-6.0.3/test/a_unit/dependency/ansible_galaxy/test_collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5925 2023-12-13 13:38:02.000000 molecule-6.0.3/test/a_unit/dependency/ansible_galaxy/test_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4552 2023-12-13 13:38:02.000000 molecule-6.0.3/test/a_unit/dependency/test_shell.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.567156 molecule-6.0.3/test/a_unit/driver/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:02.000000 molecule-6.0.3/test/a_unit/driver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9883 2023-12-13 13:38:02.000000 molecule-6.0.3/test/a_unit/driver/test_delegated.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.567156 molecule-6.0.3/test/a_unit/lint/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:02.000000 molecule-6.0.3/test/a_unit/lint/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.567156 molecule-6.0.3/test/a_unit/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:02.000000 molecule-6.0.3/test/a_unit/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.567156 molecule-6.0.3/test/a_unit/model/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:02.000000 molecule-6.0.3/test/a_unit/model/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2023-12-13 13:38:02.000000 molecule-6.0.3/test/a_unit/model/v2/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2850 2023-12-13 13:38:02.000000 molecule-6.0.3/test/a_unit/model/v2/test_dependency_section.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4082 2023-12-13 13:38:02.000000 molecule-6.0.3/test/a_unit/model/v2/test_driver_section.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2023-12-13 13:38:02.000000 molecule-6.0.3/test/a_unit/model/v2/test_platforms_section.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2942 2023-12-13 13:38:02.000000 molecule-6.0.3/test/a_unit/model/v2/test_provisioner_section.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2023-12-13 13:38:02.000000 molecule-6.0.3/test/a_unit/model/v2/test_scenario_section.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2023-12-13 13:38:02.000000 molecule-6.0.3/test/a_unit/model/v2/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2591 2023-12-13 13:38:02.000000 molecule-6.0.3/test/a_unit/model/v2/test_verifier_section.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.567156 molecule-6.0.3/test/a_unit/provisioner/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:02.000000 molecule-6.0.3/test/a_unit/provisioner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23974 2023-12-13 13:38:02.000000 molecule-6.0.3/test/a_unit/provisioner/test_ansible.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7113 2023-12-13 13:38:02.000000 molecule-6.0.3/test/a_unit/provisioner/test_ansible_playbook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4518 2023-12-13 13:38:02.000000 molecule-6.0.3/test/a_unit/provisioner/test_ansible_playbooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2023-12-13 13:38:02.000000 molecule-6.0.3/test/a_unit/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11459 2023-12-13 13:38:02.000000 molecule-6.0.3/test/a_unit/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3647 2023-12-13 13:38:02.000000 molecule-6.0.3/test/a_unit/test_interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4156 2023-12-13 13:38:02.000000 molecule-6.0.3/test/a_unit/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2023-12-13 13:38:02.000000 molecule-6.0.3/test/a_unit/test_platforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6820 2023-12-13 13:38:02.000000 molecule-6.0.3/test/a_unit/test_scenario.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6229 2023-12-13 13:38:02.000000 molecule-6.0.3/test/a_unit/test_scenarios.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2279 2023-12-13 13:38:02.000000 molecule-6.0.3/test/a_unit/test_scenarios_ordered.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2023-12-13 13:38:02.000000 molecule-6.0.3/test/a_unit/test_shell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3251 2023-12-13 13:38:02.000000 molecule-6.0.3/test/a_unit/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2023-12-13 13:38:02.000000 molecule-6.0.3/test/a_unit/test_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2023-12-13 13:38:02.000000 molecule-6.0.3/test/a_unit/test_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9353 2023-12-13 13:38:02.000000 molecule-6.0.3/test/a_unit/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.571156 molecule-6.0.3/test/a_unit/verifier/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:02.000000 molecule-6.0.3/test/a_unit/verifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2023-12-13 13:38:02.000000 molecule-6.0.3/test/a_unit/verifier/test_ansible.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8858 2023-12-13 13:38:02.000000 molecule-6.0.3/test/a_unit/verifier/test_testinfra.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.571156 molecule-6.0.3/test/b_functional/
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2023-12-13 13:38:02.000000 molecule-6.0.3/test/b_functional/.ansible-lint
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:02.000000 molecule-6.0.3/test/b_functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8277 2023-12-13 13:38:02.000000 molecule-6.0.3/test/b_functional/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11899 2023-12-13 13:38:02.000000 molecule-6.0.3/test/b_functional/test_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4697 2023-12-13 13:38:02.000000 molecule-6.0.3/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.571156 molecule-6.0.3/test/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2023-12-13 13:38:02.000000 molecule-6.0.3/test/resources/.yamllint
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.571156 molecule-6.0.3/test/resources/invalid_role_template/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.571156 molecule-6.0.3/test/resources/invalid_role_template/bad_format/
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2023-12-13 13:38:02.000000 molecule-6.0.3/test/resources/invalid_role_template/bad_format/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2023-12-13 13:38:02.000000 molecule-6.0.3/test/resources/invalid_role_template/cookiecutter.json
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2023-12-13 13:38:02.000000 molecule-6.0.3/test/resources/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.511156 molecule-6.0.3/test/resources/playbooks/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.571156 molecule-6.0.3/test/resources/playbooks/delegated/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2023-12-13 13:38:02.000000 molecule-6.0.3/test/resources/playbooks/delegated/create.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2023-12-13 13:38:02.000000 molecule-6.0.3/test/resources/playbooks/delegated/destroy.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.511156 molecule-6.0.3/test/resources/playbooks/delegated/inventory/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.511156 molecule-6.0.3/test/resources/playbooks/delegated/inventory/group_vars/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.571156 molecule-6.0.3/test/resources/playbooks/delegated/inventory/group_vars/all/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2023-12-13 13:38:02.000000 molecule-6.0.3/test/resources/playbooks/delegated/inventory/group_vars/all/all.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.511156 molecule-6.0.3/test/resources/roles/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.515156 molecule-6.0.3/test/resources/roles/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.571156 molecule-6.0.3/test/resources/roles/molecule/meta/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2023-12-13 13:38:02.000000 molecule-6.0.3/test/resources/roles/molecule/meta/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.571156 molecule-6.0.3/test/resources/roles/molecule/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2023-12-13 13:38:02.000000 molecule-6.0.3/test/resources/roles/molecule/tasks/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.571156 molecule-6.0.3/test/resources/sample-collection/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2023-12-13 13:38:02.000000 molecule-6.0.3/test/resources/sample-collection/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2023-12-13 13:38:02.000000 molecule-6.0.3/test/resources/sample-collection/galaxy.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.571156 molecule-6.0.3/test/resources/sample-collection/meta/
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2023-12-13 13:38:02.000000 molecule-6.0.3/test/resources/sample-collection/meta/runtime.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.515156 molecule-6.0.3/test/resources/sample-collection/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.571156 molecule-6.0.3/test/resources/sample-collection/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2023-12-13 13:38:02.000000 molecule-6.0.3/test/resources/sample-collection/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2023-12-13 13:38:02.000000 molecule-6.0.3/test/resources/sample-collection/molecule/default/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.515156 molecule-6.0.3/test/resources/sample-collection/roles/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.515156 molecule-6.0.3/test/resources/sample-collection/roles/get_rich/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.575156 molecule-6.0.3/test/resources/sample-collection/roles/get_rich/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2023-12-13 13:38:02.000000 molecule-6.0.3/test/resources/sample-collection/roles/get_rich/tasks/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.515156 molecule-6.0.3/test/resources/schema_instance_files/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.575156 molecule-6.0.3/test/resources/schema_instance_files/invalid/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2023-12-13 13:38:02.000000 molecule-6.0.3/test/resources/schema_instance_files/invalid/molecule_delegated.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.575156 molecule-6.0.3/test/resources/schema_instance_files/valid/
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2023-12-13 13:38:02.000000 molecule-6.0.3/test/resources/schema_instance_files/valid/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.575156 molecule-6.0.3/test/scenarios/
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2023-12-13 13:38:02.000000 molecule-6.0.3/test/scenarios/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.515156 molecule-6.0.3/test/scenarios/cleanup/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.515156 molecule-6.0.3/test/scenarios/cleanup/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.575156 molecule-6.0.3/test/scenarios/cleanup/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2023-12-13 13:38:02.000000 molecule-6.0.3/test/scenarios/cleanup/molecule/default/cleanup.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2023-12-13 13:38:02.000000 molecule-6.0.3/test/scenarios/cleanup/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2023-12-13 13:38:02.000000 molecule-6.0.3/test/scenarios/cleanup/molecule/default/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.575156 molecule-6.0.3/test/scenarios/cleanup/molecule/default/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2023-12-13 13:38:02.000000 molecule-6.0.3/test/scenarios/cleanup/molecule/default/tests/test_cleanup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.515156 molecule-6.0.3/test/scenarios/dependency/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.515156 molecule-6.0.3/test/scenarios/dependency/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.575156 molecule-6.0.3/test/scenarios/dependency/molecule/ansible-galaxy/
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2023-12-13 13:38:02.000000 molecule-6.0.3/test/scenarios/dependency/molecule/ansible-galaxy/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2023-12-13 13:38:02.000000 molecule-6.0.3/test/scenarios/dependency/molecule/ansible-galaxy/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2023-12-13 13:38:02.000000 molecule-6.0.3/test/scenarios/dependency/molecule/ansible-galaxy/requirements.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.575156 molecule-6.0.3/test/scenarios/dependency/molecule/shell/
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2023-12-13 13:38:02.000000 molecule-6.0.3/test/scenarios/dependency/molecule/shell/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2023-12-13 13:38:02.000000 molecule-6.0.3/test/scenarios/dependency/molecule/shell/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.515156 molecule-6.0.3/test/scenarios/driver/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.515156 molecule-6.0.3/test/scenarios/driver/delegated/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.575156 molecule-6.0.3/test/scenarios/driver/delegated/meta/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2023-12-13 13:38:02.000000 molecule-6.0.3/test/scenarios/driver/delegated/meta/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.515156 molecule-6.0.3/test/scenarios/driver/delegated/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.575156 molecule-6.0.3/test/scenarios/driver/delegated/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2023-12-13 13:38:02.000000 molecule-6.0.3/test/scenarios/driver/delegated/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2023-12-13 13:38:02.000000 molecule-6.0.3/test/scenarios/driver/delegated/molecule/default/create.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2023-12-13 13:38:02.000000 molecule-6.0.3/test/scenarios/driver/delegated/molecule/default/destroy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2023-12-13 13:38:02.000000 molecule-6.0.3/test/scenarios/driver/delegated/molecule/default/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.515156 molecule-6.0.3/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.575156 molecule-6.0.3/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/meta/
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2023-12-13 13:38:02.000000 molecule-6.0.3/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/meta/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.515156 molecule-6.0.3/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.579156 molecule-6.0.3/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2023-12-13 13:38:02.000000 molecule-6.0.3/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2023-12-13 13:38:02.000000 molecule-6.0.3/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/molecule/default/create.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2023-12-13 13:38:02.000000 molecule-6.0.3/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/molecule/default/destroy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2023-12-13 13:38:02.000000 molecule-6.0.3/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/molecule/default/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.579156 molecule-6.0.3/test/scenarios/host_group_vars/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.515156 molecule-6.0.3/test/scenarios/host_group_vars/group_vars/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.579156 molecule-6.0.3/test/scenarios/host_group_vars/group_vars/example/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2023-12-13 13:38:02.000000 molecule-6.0.3/test/scenarios/host_group_vars/group_vars/example/all.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.579156 molecule-6.0.3/test/scenarios/host_group_vars/host_vars/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2023-12-13 13:38:02.000000 molecule-6.0.3/test/scenarios/host_group_vars/host_vars/extra-host
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.579156 molecule-6.0.3/test/scenarios/host_group_vars/host_vars/instance/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2023-12-13 13:38:02.000000 molecule-6.0.3/test/scenarios/host_group_vars/host_vars/instance/all.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2023-12-13 13:38:02.000000 molecule-6.0.3/test/scenarios/host_group_vars/hosts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.519156 molecule-6.0.3/test/scenarios/host_group_vars/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.579156 molecule-6.0.3/test/scenarios/host_group_vars/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2023-12-13 13:38:02.000000 molecule-6.0.3/test/scenarios/host_group_vars/molecule/default/converge.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.519156 molecule-6.0.3/test/scenarios/host_group_vars/molecule/default/group_vars/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.579156 molecule-6.0.3/test/scenarios/host_group_vars/molecule/default/group_vars/example/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2023-12-13 13:38:02.000000 molecule-6.0.3/test/scenarios/host_group_vars/molecule/default/group_vars/example/all.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.519156 molecule-6.0.3/test/scenarios/host_group_vars/molecule/default/host_vars/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.579156 molecule-6.0.3/test/scenarios/host_group_vars/molecule/default/host_vars/instance/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2023-12-13 13:38:02.000000 molecule-6.0.3/test/scenarios/host_group_vars/molecule/default/host_vars/instance/all.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2023-12-13 13:38:02.000000 molecule-6.0.3/test/scenarios/host_group_vars/molecule/default/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.579156 molecule-6.0.3/test/scenarios/host_group_vars/molecule/links/
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2023-12-13 13:38:02.000000 molecule-6.0.3/test/scenarios/host_group_vars/molecule/links/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2023-12-13 13:38:02.000000 molecule-6.0.3/test/scenarios/host_group_vars/molecule/links/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.519156 molecule-6.0.3/test/scenarios/idempotence/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.519156 molecule-6.0.3/test/scenarios/idempotence/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.579156 molecule-6.0.3/test/scenarios/idempotence/molecule/raises/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2023-12-13 13:38:02.000000 molecule-6.0.3/test/scenarios/idempotence/molecule/raises/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2023-12-13 13:38:02.000000 molecule-6.0.3/test/scenarios/idempotence/molecule/raises/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.579156 molecule-6.0.3/test/scenarios/idempotence/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2023-12-13 13:38:02.000000 molecule-6.0.3/test/scenarios/idempotence/tasks/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.519156 molecule-6.0.3/test/scenarios/interpolation/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.519156 molecule-6.0.3/test/scenarios/interpolation/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.579156 molecule-6.0.3/test/scenarios/interpolation/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2023-12-13 13:38:02.000000 molecule-6.0.3/test/scenarios/interpolation/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2023-12-13 13:38:02.000000 molecule-6.0.3/test/scenarios/interpolation/molecule/default/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.519156 molecule-6.0.3/test/scenarios/overrride_driver/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.519156 molecule-6.0.3/test/scenarios/overrride_driver/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.579156 molecule-6.0.3/test/scenarios/overrride_driver/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2023-12-13 13:38:02.000000 molecule-6.0.3/test/scenarios/overrride_driver/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2023-12-13 13:38:02.000000 molecule-6.0.3/test/scenarios/overrride_driver/molecule/default/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.519156 molecule-6.0.3/test/scenarios/side_effect/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.519156 molecule-6.0.3/test/scenarios/side_effect/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.579156 molecule-6.0.3/test/scenarios/side_effect/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2023-12-13 13:38:02.000000 molecule-6.0.3/test/scenarios/side_effect/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2023-12-13 13:38:02.000000 molecule-6.0.3/test/scenarios/side_effect/molecule/default/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2023-12-13 13:38:02.000000 molecule-6.0.3/test/scenarios/side_effect/molecule/default/side_effect.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.579156 molecule-6.0.3/test/scenarios/side_effect/molecule/default/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2023-12-13 13:38:02.000000 molecule-6.0.3/test/scenarios/side_effect/molecule/default/tests/test_side_effect.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.519156 molecule-6.0.3/test/scenarios/test_destroy_strategy/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.519156 molecule-6.0.3/test/scenarios/test_destroy_strategy/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.583156 molecule-6.0.3/test/scenarios/test_destroy_strategy/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2023-12-13 13:38:02.000000 molecule-6.0.3/test/scenarios/test_destroy_strategy/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2023-12-13 13:38:02.000000 molecule-6.0.3/test/scenarios/test_destroy_strategy/molecule/default/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.583156 molecule-6.0.3/test/scenarios/test_destroy_strategy/molecule/default/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2023-12-13 13:38:02.000000 molecule-6.0.3/test/scenarios/test_destroy_strategy/molecule/default/tests/test_destroy_strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.583156 molecule-6.0.3/test/scenarios/verifier/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2023-12-13 13:38:02.000000 molecule-6.0.3/test/scenarios/verifier/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.519156 molecule-6.0.3/test/scenarios/verifier/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.583156 molecule-6.0.3/test/scenarios/verifier/molecule/testinfra/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2023-12-13 13:38:02.000000 molecule-6.0.3/test/scenarios/verifier/molecule/testinfra/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2023-12-13 13:38:02.000000 molecule-6.0.3/test/scenarios/verifier/molecule/testinfra/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.583156 molecule-6.0.3/test/scenarios/verifier/molecule/testinfra/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2023-12-13 13:38:02.000000 molecule-6.0.3/test/scenarios/verifier/molecule/testinfra/shared/test_shared.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.583156 molecule-6.0.3/test/scenarios/verifier/molecule/testinfra/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2023-12-13 13:38:02.000000 molecule-6.0.3/test/scenarios/verifier/molecule/testinfra/tests/test_testinfra.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.583156 molecule-6.0.3/test/scenarios/verifier/molecule/testinfra-pre-commit/
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2023-12-13 13:38:02.000000 molecule-6.0.3/test/scenarios/verifier/molecule/testinfra-pre-commit/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2023-12-13 13:38:02.000000 molecule-6.0.3/test/scenarios/verifier/molecule/testinfra-pre-commit/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.583156 molecule-6.0.3/test/scenarios/verifier/molecule/testinfra-pre-commit/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2023-12-13 13:38:02.000000 molecule-6.0.3/test/scenarios/verifier/molecule/testinfra-pre-commit/tests/test_testinfra_pre_commit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 13:38:15.583156 molecule-6.0.3/tools/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      248 2023-12-13 13:38:02.000000 molecule-6.0.3/tools/get-version.sh
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2023-12-13 13:38:02.000000 molecule-6.0.3/tools/opts.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      235 2023-12-13 13:38:02.000000 molecule-6.0.3/tools/smoketest.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      688 2023-12-13 13:38:02.000000 molecule-6.0.3/tools/test-setup.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      214 2023-12-13 13:38:02.000000 molecule-6.0.3/tools/update-version.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     4334 2023-12-13 13:38:02.000000 molecule-6.0.3/tox.ini
```

### Comparing `molecule-6.0.2/.config/molecule.spec` & `molecule-6.0.3/.config/molecule.spec`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/.gitattributes` & `molecule-6.0.3/.gitattributes`

 * *Files 2% similar despite different names*

```diff
@@ -194,9 +194,9 @@
 *.pyo binary
 
 # Note: .db, .p, and .pkl files are associated
 # with the python modules ``pickle``, ``dbm.*``,
 # ``shelve``, ``marshal``, ``anydbm``, & ``bsddb``
 # (among others).
 
-# Needed for setuptools-scm-git-archive:
+# Needed for setuptools-scm>=7.0
 .git_archival.txt  export-subst
```

### Comparing `molecule-6.0.2/.github/workflows/redirects.yml` & `molecule-6.0.3/.github/workflows/redirects.yml`

 * *Files 24% similar despite different names*

```diff
@@ -14,16 +14,16 @@
   workflow_dispatch:
 
 jobs:
   docs:
     environment: release
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v3
-      - uses: actions/setup-python@v4
+      - uses: actions/checkout@v4
+      - uses: actions/setup-python@v5
 
       - name: Upgrade Python toolchain
         run: python3 -m pip install --upgrade pip setuptools wheel
 
       - name: Install readthedocs-cli
         run: python3 -m pip install readthedocs-cli
```

### Comparing `molecule-6.0.2/.github/workflows/release.yml` & `molecule-6.0.3/.github/workflows/release.yml`

 * *Files 1% similar despite different names*

```diff
@@ -15,23 +15,23 @@
     env:
       FORCE_COLOR: 1
       PY_COLORS: 1
       TOXENV: pkg
 
     steps:
       - name: Switch to using Python 3.9 by default
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: 3.9
 
       - name: Install tox
         run: python3 -m pip install --user "tox>=4.0.0"
 
       - name: Check out src from Git
-        uses: actions/checkout@v3
+        uses: actions/checkout@v4
         with:
           fetch-depth: 0 # needed by setuptools-scm
           submodules: true
 
       - name: Build dists
         run: python -m tox
```

### Comparing `molecule-6.0.2/.github/workflows/tox.yml` & `molecule-6.0.3/.github/workflows/tox.yml`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
       matrix: ${{ steps.generate_matrix.outputs.matrix }}
     steps:
       - name: Determine matrix
         id: generate_matrix
         uses: coactions/dynamic-matrix@v1
         with:
           min_python: "3.9"
-          max_python: "3.11"
+          max_python: "3.12"
           other_names: |
             lint
             docs
             pkg
             eco
             py311-devel
 
@@ -49,15 +49,15 @@
     strategy:
       fail-fast: false
       matrix: ${{ fromJson(needs.pre.outputs.matrix) }}
 
     env:
       PYTEST_REQPASS: 450
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           fetch-depth: 0 # needed by setuptools-scm
           submodules: true
 
       - name: Set pre-commit cache
         uses: actions/cache@v3
         if: ${{ matrix.passed_name == 'lint' }}
@@ -79,15 +79,15 @@
         run: |
           ansible --version \
           && virtualenv foo \
           && source foo/bin/activate \
           && ansible --version
       - name: Set up Python ${{ matrix.python_version || '3.9' }}
         if: "!contains(matrix.shell, 'wsl')"
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           cache: pip
           python-version: ${{ matrix.python_version || '3.9' }}
 
       - name: Install tox
         run: |
           python3 -m pip install --upgrade pip
```

### Comparing `molecule-6.0.2/.packit.yaml` & `molecule-6.0.3/.packit.yaml`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/.pre-commit-config.yaml` & `molecule-6.0.3/.pre-commit-config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,64 +1,67 @@
 ---
+ci:
+  skip:
+    - ansible-lint
 default_language_version:
   python: python3.9
 repos:
   - repo: https://github.com/pre-commit/mirrors-prettier
     # keep it before yamllint
-    rev: "v3.0.1"
+    rev: "v4.0.0-alpha.4"
     hooks:
       - id: prettier
         # Temporary excludes so we can gradually normalize the formatting
         exclude: >
           (?x)^(
-            src/molecule/test/resources/templates/.*|
+            test/resources/templates/.*|
           )$
         additional_dependencies:
           - prettier
           - prettier-plugin-toml
   - repo: https://github.com/codespell-project/codespell
-    rev: v2.2.5
+    rev: v2.2.6
     hooks:
       - id: codespell
   - repo: https://github.com/psf/black
-    rev: 23.7.0
+    rev: 23.11.0
     hooks:
       - id: black
         language_version: python3
   - repo: https://github.com/pre-commit/pre-commit-hooks.git
-    rev: v4.4.0
+    rev: v4.5.0
     hooks:
       - id: end-of-file-fixer
       - id: trailing-whitespace
       - id: mixed-line-ending
       - id: check-byte-order-marker
       - id: check-executables-have-shebangs
       - id: check-merge-conflict
       - id: debug-statements
         language_version: python3
 
   - repo: https://github.com/adrienverge/yamllint.git
-    rev: v1.32.0
+    rev: v1.33.0
     hooks:
       - id: yamllint
         files: \.(yaml|yml)$
         types: [file, yaml]
         entry: yamllint --strict
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: "v0.0.284"
+    rev: "v0.1.7"
     hooks:
       - id: ruff
         args: [--fix, --exit-non-zero-on-fix]
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.5.0
+    rev: v1.7.1
     hooks:
       - id: mypy
         # empty args needed in order to match mypy cli behavior
         args: []
-        entry: mypy src/
+        entry: mypy src/ test/
         pass_filenames: false
         additional_dependencies:
           - ansible-compat>=4.1.8
           - click>=8.0.1,<8.1.4 # https://github.com/pallets/click/issues/2558
           - enrich>=1.2.7
           - importlib-metadata>=4.6.1
           - jinja2
@@ -70,15 +73,15 @@
           - types-PyYAML
           - types-dataclasses
           - types-filelock
           - types-jsonschema
           - types-setuptools
           - wcmatch
   - repo: https://github.com/pycqa/pylint
-    rev: v3.0.0a6
+    rev: v3.0.1
     hooks:
       - id: pylint
         args:
           - --output-format=colorized
         additional_dependencies:
           - ansible-compat>=4.1.8
           - click
@@ -86,7 +89,11 @@
           - enrich>=1.2.7
           - filelock
           - jsonschema
           - pexpect
           - pytest-mock
           - pytest-testinfra
           - wcmatch
+  - repo: https://github.com/ansible/ansible-lint
+    rev: v6.22.1
+    hooks:
+      - id: ansible-lint
```

### Comparing `molecule-6.0.2/.vscode/settings.json` & `molecule-6.0.3/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/.yamllint` & `molecule-6.0.3/.yamllint`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/DCO_1_1.md` & `molecule-6.0.3/DCO_1_1.md`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/LICENSE` & `molecule-6.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/PKG-INFO` & `molecule-6.0.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molecule
-Version: 6.0.2
+Version: 6.0.3
 Summary: Molecule aids in the development and testing of Ansible roles
 Author-email: Ansible by Red Hat <info@ansible.com>
 Maintainer-email: Ansible by Red Hat <info@ansible.com>
 License: MIT
 Project-URL: homepage, https://github.com/ansible-community/molecule
 Project-URL: documentation, https://molecule.readthedocs.io/
 Project-URL: repository, https://github.com/ansible-community/molecule
@@ -18,26 +18,53 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Software Development :: Bug Tracking
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Utilities
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: ansible-compat>=4.1.8
+Requires-Dist: ansible-core>=2.12.10
+Requires-Dist: click<9,>=8.0
+Requires-Dist: click-help-colors>=0.9
+Requires-Dist: enrich>=1.2.7
+Requires-Dist: jsonschema>=4.9.1
+Requires-Dist: Jinja2>=2.11.3
+Requires-Dist: packaging
+Requires-Dist: pluggy<2.0,>=0.7.1
+Requires-Dist: PyYAML>=5.1
+Requires-Dist: rich>=9.5.1
+Requires-Dist: wcmatch>=8.1.2
 Provides-Extra: docs
+Requires-Dist: mkdocs-ansible[lock]>=0.2.0; extra == "docs"
+Requires-Dist: pipdeptree>=2.4.0; extra == "docs"
+Requires-Dist: linkchecker==10.2.1; extra == "docs"
 Provides-Extra: test
+Requires-Dist: ansible-lint>=6.12.1; extra == "test"
+Requires-Dist: ansi2html>=1.8.0; extra == "test"
+Requires-Dist: coverage>=7.0.3; extra == "test"
+Requires-Dist: filelock>=3.9.0; extra == "test"
+Requires-Dist: pexpect<5,>=4.8.0; extra == "test"
+Requires-Dist: pytest-mock>=3.10.0; extra == "test"
+Requires-Dist: pytest-plus>=0.4.0; extra == "test"
+Requires-Dist: pytest-xdist>=3.1.0; extra == "test"
+Requires-Dist: pytest>=7.2.0; extra == "test"
+Requires-Dist: check-jsonschema; extra == "test"
 Provides-Extra: testinfra
-License-File: LICENSE
+Requires-Dist: pytest-testinfra>=8.1.0; extra == "testinfra"
 
 # About Ansible Molecule
 
 [![PyPI Package](https://img.shields.io/pypi/v/molecule)](https://pypi.org/project/molecule/)
 [![Documentation Status](https://readthedocs.org/projects/molecule/badge/?version=latest)](https://ansible.readthedocs.io/projects/molecule)
 [![image](https://github.com/ansible-community/molecule/workflows/tox/badge.svg)](https://github.com/ansible-community/molecule/actions)
 [![Python Black Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
```

### Comparing `molecule-6.0.2/README.md` & `molecule-6.0.3/README.md`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/bindep.txt` & `molecule-6.0.3/bindep.txt`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/conftest.py` & `molecule-6.0.3/conftest.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/docs/_static/images/favicon.ico` & `molecule-6.0.3/docs/_static/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/docs/_static/images/logo.png` & `molecule-6.0.3/docs/_static/images/logo.png`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/docs/_static/images/logo_big.png` & `molecule-6.0.3/docs/_static/images/logo_big.png`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/docs/ci.md` & `molecule-6.0.3/docs/ci.md`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/docs/configuration.md` & `molecule-6.0.3/docs/configuration.md`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/docs/contributing.md` & `molecule-6.0.3/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/docs/docker.md` & `molecule-6.0.3/docs/docker.md`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/docs/examples.md` & `molecule-6.0.3/docs/examples.md`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 to the Docker image used in the scenario.
 
 Note: `platforms[*].pre_build_image` defaults to `true` in each
 scenario's generated `molecule.yml` file.
 
 ## Docker With Non-Privileged User
 
-The default Molecule Docker driver executes Ansible playbooks as the
+The Molecule Docker driver executes Ansible playbooks as the
 root user. If your workflow requires adding support for running as a
 non-privileged user, then adapt `molecule.yml` and `Dockerfile.j2` as
 follows.
 
 Note: The `Dockerfile` templating and image building processes are only
 done for scenarios with `pre_build_image = False`, which is not the
 default setting in generated `molecule.yml` files.
```

### Comparing `molecule-6.0.2/docs/faq.md` & `molecule-6.0.3/docs/faq.md`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/docs/getting-started.md` & `molecule-6.0.3/docs/getting-started.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 The following guide will step through an example of developing and
 testing a new Ansible collection. After reading this guide, you should be
 familiar with the basics of how to use Molecule and what it can offer.
 
 1.  Create a collection
 
-    One of the recommended ways to create a collection is to place it under the `collections/ansible_collections` directory.
+    One of the recommended ways to create a collection is to place it under a `collections/ansible_collections` directory. If you don't put your collection into a directory named `ansible_collections`, _molecule won't be able to find your role_.
 
     ```bash
       ansible-galaxy collection init foo.bar
     ```
 
 - cd to the `roles` directory in your new collection.
 
@@ -37,29 +37,29 @@
       ---
       - name: Test new role from within this playbook
         hosts: localhost
         gather_facts: false
         tasks:
           - name: Testing role
             ansible.builtin.include_role:
-            name: foo.bar.my_role
-            tasks_from: main.yml
+              name: foo.bar.my_role
+              tasks_from: main.yml
       ```
 
 - Adding Molecule to the Collection
 
       1. Create a new directory in your collection called `extensions`.
 
       2. cd to the `extensions` directory and initialize a new default molecule scenario.
 
           ```bash
              molecule init scenario
           ```
 
-![Collection Structure and ansible config file collections path](images/collection_structure_and_ansible_cfg.png)
+![Collection Structure and ansible config file collections path](images/collection_structure.png)
 
 Before moving to test the playbooks or roles, the sections below provide information related to Scenarios.
 
 ## Molecule Scenarios
 
 Scenarios are the starting point for a lot of powerful functionality that Molecule offers.
 For now, we can think of a scenario as a test suite for roles or playbooks within a collection.
@@ -97,15 +97,15 @@
 
     ``` yaml
     - name: Verify
         hosts: all
         become: true
         tasks:
         - name: Initialize role without actually running it
-            ansible.builtin.include_role:
+          ansible.builtin.include_role:
             name: my_role
             tasks_from: init
 
     # Start testing: can use role library now
     ```
 
 ## Inspecting the `molecule.yml`
@@ -114,16 +114,16 @@
 [YAML](https://yaml.org/) file whose keys represent the high-level
 components that Molecule provides. These are:
 
 - The [dependency](configuration.md#dependency) manager. Molecule
   uses [galaxy development guide]
   by default to resolve your role dependencies.
 - The [driver](configuration.md#driver) provider. Molecule uses
-  [Docker](https://docs.docker.com/) by default. Molecule uses the
-  driver to delegate the task of creating instances.
+  the [Delegated](configuration.md#delegated) driver by default.
+  Molecule uses the driver to delegate the task of creating instances.
 - The [platforms](configuration.md#platforms) definitions. Molecule
   relies on this to know which instances to create, name and to which
   group each instance belongs. If you need to test your role against
   multiple popular distributions (CentOS, Fedora, Debian), you can
   specify that in this section.
 - The [provisioner](configuration.md#provisioner). Molecule only
   provides an Ansible provisioner. Ansible manages the life cycle of
```

### Comparing `molecule-6.0.2/docs/index.md` & `molecule-6.0.3/docs/index.md`

 * *Files 0% similar despite different names*

```diff
@@ -30,11 +30,11 @@
 - [Ansible Collections: Role Tests with
   Molecule](https://ericsysmin.com/2020/04/30/ansible-collections-role-tests-with-molecule/)
   @ericsysmin
 - [Molecule v3 Slides](https://sbarnea.com/slides/molecule/#/)
   @ssbarnea.
 - [Testing your Ansible roles with
   Molecule](https://www.jeffgeerling.com/blog/2018/testing-your-ansible-roles-molecule)
-  @geerlinguy
+  @geerlingguy
 - [How to test Ansible and don't go
   nuts](https://www.goncharov.xyz/it/ansible-testing-en.html)
   @ultral
```

### Comparing `molecule-6.0.2/docs/installation.md` & `molecule-6.0.3/docs/installation.md`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/docs/kubevirt.md` & `molecule-6.0.3/docs/kubevirt.md`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/docs/next.md` & `molecule-6.0.3/docs/next.md`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/docs/podman.md` & `molecule-6.0.3/docs/podman.md`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/docs/usage.md` & `molecule-6.0.3/docs/usage.md`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/mkdocs.yml` & `molecule-6.0.3/mkdocs.yml`

 * *Files 7% similar despite different names*

```diff
@@ -3,41 +3,24 @@
 site_url: https://ansible.readthedocs.io/projects/molecule/
 repo_url: https://github.com/ansible-community/molecule
 edit_uri: blob/main/docs/
 copyright: Copyright © 2023 Red Hat, Inc.
 strict: true
 
 theme:
-  name: "material"
-  logo: images/logo.svg
-  favicon: images/favicon.ico
+  name: ansible
   features:
     - content.code.copy
     - content.action.edit
     - navigation.expand
     - navigation.sections
     - navigation.instant
     - navigation.indexes
     - navigation.tracking
     - toc.integrate
-  palette:
-    - media: "(prefers-color-scheme: light)"
-      primary: teal
-      accent: blue
-      scheme: default
-      toggle:
-        icon: material/brightness-7
-        name: Switch to dark mode
-    - media: "(prefers-color-scheme: dark)"
-      scheme: slate
-      primary: teal
-      accent: blue
-      toggle:
-        icon: material/brightness-4
-        name: Switch to light mode
 extra:
   social:
     - icon: fontawesome/brands/python
       link: https://pypi.org/project/molecule/
       name: PyPI
     - icon: fontawesome/solid/scroll
       link: https://github.com/ansible-community/molecule/releases
@@ -95,15 +78,15 @@
           - working/contributor_guide/developer_contact.md
           - working/contributor_guide/environment_setup.md
           - working/contributor_guide/contribution_requirements.md
 
 plugins:
   - autorefs
   - search
-  - social
+  - material/social
 
   - mkdocstrings:
       enable_inventory: true
       default_handler: python
       handlers:
         python:
           paths: [src]
```

### Comparing `molecule-6.0.2/molecule/default/create.yml` & `molecule-6.0.3/molecule/default/create.yml`

 * *Files 1% similar despite different names*

```diff
@@ -30,8 +30,8 @@
         - name: Dump instance config
           ansible.builtin.copy:
             content: |
               # Molecule managed
 
               {{ instance_conf | to_json | from_json | to_yaml }}
             dest: "{{ molecule_instance_config }}"
-            mode: 0600
+            mode: "0600"
```

### Comparing `molecule-6.0.2/molecule/default/destroy.yml` & `molecule-6.0.3/molecule/default/destroy.yml`

 * *Files 3% similar despite different names*

```diff
@@ -16,9 +16,9 @@
     - name: Dump instance config
       ansible.builtin.copy:
         content: |
           # Molecule managed
 
           {{ instance_conf | to_json | from_json | to_yaml }}
         dest: "{{ molecule_instance_config }}"
-        mode: 0600
+        mode: "0600"
       when: server.changed | default(false) | bool # noqa no-handler
```

### Comparing `molecule-6.0.2/molecule/docker/converge.yml` & `molecule-6.0.3/molecule/docker/converge.yml`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/molecule/docker/create.yml` & `molecule-6.0.3/molecule/docker/create.yml`

 * *Files 4% similar despite different names*

```diff
@@ -38,25 +38,25 @@
             children:
               molecule:
                 hosts:
                   "{{ item.name }}":
                     ansible_connection: community.docker.docker
       ansible.builtin.set_fact:
         molecule_inventory: >
-          {{ molecule_inventory | combine(inventory_partial_yaml | from_yaml) }}
+          {{ molecule_inventory | combine(inventory_partial_yaml | from_yaml, recursive=true) }}
       loop: "{{ molecule_yml.platforms }}"
       loop_control:
         label: "{{ item.name }}"
 
     - name: Dump molecule_inventory
       ansible.builtin.copy:
         content: |
           {{ molecule_inventory | to_yaml }}
         dest: "{{ molecule_ephemeral_directory }}/inventory/molecule_inventory.yml"
-        mode: 0600
+        mode: "0600"
 
     - name: Force inventory refresh
       ansible.builtin.meta: refresh_inventory
 
     - name: Fail if molecule group is missing
       ansible.builtin.assert:
         that: "'molecule' in groups"
```

### Comparing `molecule-6.0.2/molecule/docker/destroy.yml` & `molecule-6.0.3/molecule/docker/destroy.yml`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/molecule/kubevirt/converge.yml` & `molecule-6.0.3/molecule/kubevirt/converge.yml`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/molecule/kubevirt/create.yml` & `molecule-6.0.3/molecule/kubevirt/create.yml`

 * *Files 6% similar despite different names*

```diff
@@ -2,34 +2,35 @@
   hosts: localhost
   connection: local
   gather_facts: false
   vars:
     temporary_ssh_key_size: 2048 # Variable for the size of the SSH key
   tasks:
     - name: Set default SSH key path # Sets the path of the SSH key
-      set_fact:
-        tempoary_ssh_key_path: "{{ molecule_ephemeral_directory }}/identity_file"
+      ansible.builtin.set_fact:
+        temporary_ssh_key_path: "{{ molecule_ephemeral_directory }}/identity_file"
 
     - name: Generate SSH key pair # Generates a new SSH key pair
       community.crypto.openssh_keypair:
-        path: "{{ tempoary_ssh_key_path }}"
+        path: "{{ temporary_ssh_key_path }}"
         size: "{{ temporary_ssh_key_size }}"
       register: temporary_ssh_keypair # Stores the output of this task in a variable
 
     - name: Set SSH public key # Sets the SSH public key from the key pair
-      set_fact:
+      ansible.builtin.set_fact:
         temporary_ssh_public_key: "{{ temporary_ssh_keypair.public_key }}"
 
     - name: Create VM in KubeVirt # Calls another file to create the VM in KubeVirt
-      include_tasks: tasks/create_vm.yml
+      ansible.builtin.include_tasks: tasks/create_vm.yml
       loop: "{{ molecule_yml.platforms }}" # Loops over all platforms defined in molecule_yml
       loop_control:
         loop_var: vm # Sets the variable for the current item in the loop
 
     - name: Create Nodeport service if ssh_type is set to NodePort # Conditional block, executes if vm.ssh_service.type is NodePort
+      when: "vm.ssh_service.type == 'NodePort'" # The block is executed when this condition is met
       block:
         - name: Create ssh NodePort Kubernetes Services # Creates a new NodePort service in Kubernetes
           kubernetes.core.k8s:
             state: present
             definition:
               apiVersion: v1
               kind: Service
@@ -54,42 +55,41 @@
             kind: Service
             name: "{{ vm.name }}"
             namespace: "{{ vm.namespace }}"
           loop: "{{ molecule_yml.platforms }}" # Loops over all platforms defined in molecule_yml
           loop_control:
             loop_var: vm # Sets the variable for the current item in the loop
           register: node_port_services # Stores the output of this task in a variable
-      when: "vm.ssh_service.type == 'NodePort'" # The block is executed when this condition is met
 
     - name: Create VM dictionary # Calls another file to create a dictionary with information about the VM
-      include_tasks: tasks/create_vm_dictionary.yml
+      ansible.builtin.include_tasks: tasks/create_vm_dictionary.yml
       loop: "{{ molecule_yml.platforms }}" # Loops over all platforms defined in molecule_yml
       loop_control:
         loop_var: vm # Sets the variable for the current item in the loop
 
     - name: Create ansible inventory from dictionary # Creates an Ansible inventory file from the dictionary
       vars:
         molecule_inventory:
           all:
             children:
               molecule:
                 hosts: "{{ molecule_systems }}"
       ansible.builtin.copy:
         content: "{{ molecule_inventory | to_nice_yaml }}"
         dest: "{{ molecule_ephemeral_directory }}/inventory/molecule_inventory.yml"
-        mode: 0600 # Sets the permissions of the file to -rw-------
+        mode: "0600" # Sets the permissions of the file to -rw-------
 
     - name: Refresh inventory # Refreshes the inventory
       ansible.builtin.meta: refresh_inventory
 
     - name: Assert molecule group exists # Checks if the 'molecule' group exists in the inventory
       ansible.builtin.assert:
         that: "'molecule' in groups"
         fail_msg: "Molecule group was not found in inventory groups: {{ groups }}"
-      run_once: true # Ensures this task is only run once, not on every host in 'hosts'
+      run_once: true # noqa: run-once
 
 - name: Validate that inventory was refreshed # New playbook to validate the inventory
   hosts: molecule # Runs on hosts in the 'molecule' group
   gather_facts: false # Disables fact gathering
   tasks:
     - name: Wait for the host to be reachable # Waits for the host to become reachable
       ansible.builtin.wait_for_connection:
```

### Comparing `molecule-6.0.2/molecule/kubevirt/destroy.yml` & `molecule-6.0.3/molecule/kubevirt/destroy.yml`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/molecule/kubevirt/molecule.yml` & `molecule-6.0.3/molecule/kubevirt/molecule.yml`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/molecule/kubevirt/tasks/create_vm.yml` & `molecule-6.0.3/molecule/kubevirt/tasks/create_vm.yml`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/molecule/kubevirt/tasks/create_vm_dictionary.yml` & `molecule-6.0.3/molecule/kubevirt/tasks/create_vm_dictionary.yml`

 * *Files 10% similar despite different names*

```diff
@@ -3,17 +3,17 @@
   vars:
     # This variable block is setting the `ssh_service_address` variable.
     # It first checks if the service type of the SSH service is 'NodePort'.
     # If it is, it retrieves the 'nodePort' from the services results.
     ssh_service_address: >-
       {%- set svc_type = vm.ssh_service.type | default(None) -%}
       {%- if svc_type == 'NodePort' -%}
-        {{(node_port_services.results | selectattr('vm.name','==',vm.name) | first)['resources'][0]['spec']['ports'][0]['nodePort']  }}
+        {{ (node_port_services.results | selectattr('vm.name', '==', vm.name) | first)['resources'][0]['spec']['ports'][0]['nodePort'] }}
       {%- endif -%}
-  set_fact:
+  ansible.builtin.set_fact:
     # Here, the task is updating the `molecule_systems` dictionary with new VM information.
     # If `molecule_systems` doesn't exist, it is created as an empty dictionary.
     # Then it is combined with a new dictionary for the current VM, containing ansible connection details.
     molecule_systems: >-
       {{
         molecule_systems | default({}) | combine({
           vm.name: {
```

### Comparing `molecule-6.0.2/molecule/podman/converge.yml` & `molecule-6.0.3/molecule/podman/converge.yml`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/molecule/podman/create.yml` & `molecule-6.0.3/molecule/podman/create.yml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 - name: Create
   hosts: localhost
   gather_facts: false
   vars:
     molecule_inventory:
       all:
         hosts: {}
-        molecule: {}
+        children:
+          molecule:
+            hosts: {}
+
   tasks:
     - name: Create a container
       containers.podman.podman_container:
         name: "{{ item.name }}"
         image: "{{ item.image }}"
         state: started
         command: sleep 1d
@@ -39,25 +42,25 @@
             children:
               molecule:
                 hosts:
                   "{{ item.name }}":
                     ansible_connection: containers.podman.podman
       ansible.builtin.set_fact:
         molecule_inventory: >
-          {{ molecule_inventory | combine(inventory_partial_yaml | from_yaml) }}
+          {{ molecule_inventory | combine(inventory_partial_yaml | from_yaml, recursive=true) }}
       loop: "{{ molecule_yml.platforms }}"
       loop_control:
         label: "{{ item.name }}"
 
     - name: Dump molecule_inventory
       ansible.builtin.copy:
         content: |
           {{ molecule_inventory | to_yaml }}
         dest: "{{ molecule_ephemeral_directory }}/inventory/molecule_inventory.yml"
-        mode: 0600
+        mode: "0600"
 
     - name: Force inventory refresh
       ansible.builtin.meta: refresh_inventory
 
     - name: Fail if molecule group is missing
       ansible.builtin.assert:
         that: "'molecule' in groups"
```

### Comparing `molecule-6.0.2/molecule/podman/destroy.yml` & `molecule-6.0.3/molecule/podman/destroy.yml`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/playbooks/snap-pre-run.yaml` & `molecule-6.0.3/playbooks/snap-pre-run.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,39 @@
-- hosts: all
+- name: Snap-pre-run
+  hosts: all
   become: true
   tasks:
     - name: Install snapd
       ansible.builtin.package:
         name: snapd
         state: present
 
     - name: Enable snapd service
       ansible.builtin.service:
         name: snapd.socket
         state: started
 
-    - when: ansible_os_family == 'Debian'
-      name: Install snapcraft (debian)
+    - name: Install snapcraft (debian)
+      when: ansible_os_family == 'Debian'
       ansible.builtin.package:
         name: snapcraft
         state: present
 
-    - when: ansible_os_family == 'RedHat'
+    - name: Install snapcraft (RedHat)
+      when: ansible_os_family == 'RedHat'
       block:
         - name: Activate snapd
           ansible.builtin.shell: |
             ln -s /var/lib/snapd/snap /snap
+          changed_when: true
 
         - name: Install snapcraft (redhat)
           ansible.builtin.shell: |
             type snapcraft || snap install --classic snapcraft
+          changed_when: true
 
     - name: Validate snapd install
       ansible.builtin.shell: |
         set -e
         snap version
         snapcraft version
+      changed_when: false
```

### Comparing `molecule-6.0.2/pyproject.toml` & `molecule-6.0.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -25,14 +25,15 @@
   "License :: OSI Approved :: MIT License",
   "Operating System :: MacOS",
   "Operating System :: POSIX",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
   "Programming Language :: Python",
   "Topic :: System :: Systems Administration",
   "Topic :: Software Development :: Bug Tracking",
   "Topic :: Software Development :: Quality Assurance",
   "Topic :: Software Development :: Testing",
   "Topic :: Utilities",
 ]
@@ -153,21 +154,21 @@
 ]
 norecursedirs = [
   ".eggs",
   ".tox",
   "build",
   "dist",
   "doc",
-  "src/molecule/test/resources",
-  "src/molecule/test/scenarios",
+  "test/resources",
+  "test/scenarios",
 ]
 addopts = "--doctest-modules --durations 10 --color=yes"
 doctest_optionflags = ["ALLOW_UNICODE", "ELLIPSIS"]
 junit_suite_name = "molecule_test_suite"
-testpaths = "src/molecule/test/"
+testpaths = "test/"
 filterwarnings = [
   # treat warnings as errors unless we add them below
   "error",
   # https://github.com/certifi/python-certifi/pull/193
   "ignore:path is deprecated.*:DeprecationWarning",
   # https://github.com/pytest-dev/pytest-cov/issues/557
   "ignore:The --rsyncdir command line argument and rsyncdirs config variable are deprecated.:DeprecationWarning",
@@ -212,15 +213,15 @@
 [tool.ruff.flake8-pytest-style]
 parametrize-values-type = "tuple"
 
 [tool.ruff.isort]
 known-first-party = ["molecule"]
 
 [tool.ruff.per-file-ignores]
-"src/molecule/test/**.py" = ["S"]
+"test/**.py" = ["S"]
 "src/molecule/*/\\{\\{*/**.py" = ["S"]
 
 [tool.setuptools.dynamic]
 optional-dependencies.docs = { file = [".config/requirements-docs.txt"] }
 optional-dependencies.test = { file = [".config/requirements-test.txt"] }
 optional-dependencies.testinfra = { file = [
   ".config/requirements-testinfra.txt",
```

### Comparing `molecule-6.0.2/src/molecule/__init__.py` & `molecule-6.0.3/src/molecule/__init__.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/src/molecule/__main__.py` & `molecule-6.0.3/src/molecule/__main__.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/src/molecule/api.py` & `molecule-6.0.3/src/molecule/api.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/src/molecule/command/__init__.py` & `molecule-6.0.3/src/molecule/command/__init__.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/src/molecule/command/base.py` & `molecule-6.0.3/src/molecule/command/base.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/src/molecule/command/check.py` & `molecule-6.0.3/src/molecule/command/check.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/src/molecule/command/cleanup.py` & `molecule-6.0.3/src/molecule/command/cleanup.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/src/molecule/command/converge.py` & `molecule-6.0.3/src/molecule/command/converge.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/src/molecule/command/create.py` & `molecule-6.0.3/src/molecule/command/create.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,14 +37,19 @@
         """Execute the actions necessary to perform a `molecule create` and \
         returns None.
 
         :return: None
         """
         self._config.state.change_state("driver", self._config.driver.name)
 
+        if self._config.state.created:
+            msg = "Skipping, instances already created."
+            LOG.warning(msg)
+            return
+
         self._config.provisioner.create()
 
         self._config.state.change_state("created", True)
 
 
 @base.click_command_ex()
 @click.pass_context
```

### Comparing `molecule-6.0.2/src/molecule/command/dependency.py` & `molecule-6.0.3/src/molecule/command/dependency.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/src/molecule/command/destroy.py` & `molecule-6.0.3/src/molecule/command/destroy.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/src/molecule/command/drivers.py` & `molecule-6.0.3/src/molecule/command/drivers.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/src/molecule/command/idempotence.py` & `molecule-6.0.3/src/molecule/command/idempotence.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/src/molecule/command/init/base.py` & `molecule-6.0.3/src/molecule/command/init/base.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/src/molecule/command/init/init.py` & `molecule-6.0.3/src/molecule/command/init/init.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/src/molecule/command/init/scenario.py` & `molecule-6.0.3/src/molecule/command/init/scenario.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/src/molecule/command/list.py` & `molecule-6.0.3/src/molecule/command/list.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/src/molecule/command/login.py` & `molecule-6.0.3/src/molecule/command/login.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/src/molecule/command/matrix.py` & `molecule-6.0.3/src/molecule/command/matrix.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from molecule import scenarios
 from molecule.command import base
 
 LOG = logging.getLogger(__name__)
 
 
 class Matrix(base.Base):
-    """Matric Command Class.
+    """Matrix Command Class.
 
     .. program:: molecule matrix subcommand
 
     .. option:: molecule matrix subcommand
 
         Target the default scenario.
```

### Comparing `molecule-6.0.2/src/molecule/command/prepare.py` & `molecule-6.0.3/src/molecule/command/prepare.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/src/molecule/command/reset.py` & `molecule-6.0.3/src/molecule/command/reset.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/src/molecule/command/side_effect.py` & `molecule-6.0.3/src/molecule/command/side_effect.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/src/molecule/command/syntax.py` & `molecule-6.0.3/src/molecule/command/syntax.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/src/molecule/command/test.py` & `molecule-6.0.3/src/molecule/command/test.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/src/molecule/command/verify.py` & `molecule-6.0.3/src/molecule/command/verify.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/src/molecule/config.py` & `molecule-6.0.3/src/molecule/config.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/src/molecule/console.py` & `molecule-6.0.3/src/molecule/console.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/src/molecule/data/driver.json` & `molecule-6.0.3/src/molecule/data/driver.json`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/src/molecule/data/init-scenario.yml` & `molecule-6.0.3/src/molecule/data/init-scenario.yml`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/src/molecule/data/molecule.json` & `molecule-6.0.3/src/molecule/data/molecule.json`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/src/molecule/data/templates/scenario/create.yml.j2` & `molecule-6.0.3/src/molecule/data/templates/scenario/create.yml.j2`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 {% raw -%}
 - name: Create
   hosts: localhost
   connection: local
   gather_facts: false
   # no_log: "{{ molecule_no_log }}"
   tasks:
-
     # TODO: Developer must implement and populate 'server' variable
 
     - name: Create instance config
       when: server.changed | default(false) | bool  # noqa no-handler
       block:
         - name: Populate instance config dict  # noqa jinja
           ansible.builtin.set_fact:
@@ -30,9 +29,9 @@
         - name: Dump instance config
           ansible.builtin.copy:
             content: |
               # Molecule managed
 
               {{ instance_conf | to_json | from_json | to_yaml }}
             dest: "{{ molecule_instance_config }}"
-            mode: 0600
+            mode: "0600"
 {%- endraw %}
```

### Comparing `molecule-6.0.2/src/molecule/data/templates/scenario/destroy.yml.j2` & `molecule-6.0.3/src/molecule/data/templates/scenario/destroy.yml.j2`

 * *Files 3% similar despite different names*

```diff
@@ -17,10 +17,10 @@
     - name: Dump instance config
       ansible.builtin.copy:
         content: |
           # Molecule managed
 
           {{ instance_conf | to_json | from_json | to_yaml }}
         dest: "{{ molecule_instance_config }}"
-        mode: 0600
+        mode: "0600"
       when: server.changed | default(false) | bool  # noqa no-handler
 {%- endraw %}
```

### Comparing `molecule-6.0.2/src/molecule/dependency/ansible_galaxy/__init__.py` & `molecule-6.0.3/src/molecule/dependency/ansible_galaxy/__init__.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/src/molecule/dependency/ansible_galaxy/base.py` & `molecule-6.0.3/src/molecule/dependency/ansible_galaxy/base.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/src/molecule/dependency/ansible_galaxy/collections.py` & `molecule-6.0.3/src/molecule/dependency/ansible_galaxy/collections.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/src/molecule/dependency/ansible_galaxy/roles.py` & `molecule-6.0.3/src/molecule/dependency/ansible_galaxy/roles.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/src/molecule/dependency/base.py` & `molecule-6.0.3/src/molecule/dependency/base.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/src/molecule/dependency/shell.py` & `molecule-6.0.3/src/molecule/dependency/shell.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/src/molecule/driver/base.py` & `molecule-6.0.3/src/molecule/driver/base.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/src/molecule/driver/delegated.py` & `molecule-6.0.3/src/molecule/driver/delegated.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 LOG = logging.getLogger(__name__)
 
 
 class Delegated(Driver):
     r"""The class responsible for managing default instances.
 
-    Delegated is `not` the default driver used in Molecule.
+    Delegated is the default driver used in Molecule.
 
     Under this driver, it is the developers responsibility to implement the
     create and destroy playbooks.  ``Managed`` is the default behaviour of all
     drivers.
 
     ``` yaml
         driver:
```

### Comparing `molecule-6.0.2/src/molecule/interpolation.py` & `molecule-6.0.3/src/molecule/interpolation.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
 # Taken from Docker Compose:
 # https://github.com/docker/compose/blob/master/compose/config/interpolation.py
-"""Iterpolation Module."""
+"""Interpolation Module."""
 
 import string
 from collections.abc import MutableMapping
 
 
 class InvalidInterpolation(Exception):
     """InvalidInterpolation Exception."""
```

### Comparing `molecule-6.0.2/src/molecule/logger.py` & `molecule-6.0.3/src/molecule/logger.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/src/molecule/model/schema_v3.py` & `molecule-6.0.3/src/molecule/model/schema_v3.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/src/molecule/platforms.py` & `molecule-6.0.3/src/molecule/platforms.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/src/molecule/provisioner/ansible.py` & `molecule-6.0.3/src/molecule/provisioner/ansible.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/src/molecule/provisioner/ansible_playbook.py` & `molecule-6.0.3/src/molecule/provisioner/ansible_playbook.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/src/molecule/provisioner/ansible_playbooks.py` & `molecule-6.0.3/src/molecule/provisioner/ansible_playbooks.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/src/molecule/provisioner/base.py` & `molecule-6.0.3/src/molecule/provisioner/base.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/src/molecule/scenario.py` & `molecule-6.0.3/src/molecule/scenario.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/src/molecule/scenarios.py` & `molecule-6.0.3/src/molecule/scenarios.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/src/molecule/shell.py` & `molecule-6.0.3/src/molecule/shell.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/src/molecule/state.py` & `molecule-6.0.3/src/molecule/state.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/src/molecule/status.py` & `molecule-6.0.3/src/molecule/status.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/src/molecule/test/a_unit/command/conftest.py` & `molecule-6.0.3/test/a_unit/command/conftest.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/src/molecule/test/a_unit/command/init/test_scenario.py` & `molecule-6.0.3/test/a_unit/command/init/test_scenario.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 
 @pytest.fixture()
 def _instance(_command_args):
     return scenario.Scenario(_command_args)
 
 
-def test_execute(temp_dir, _instance, patched_logger_info):
+def test_scenario_execute(temp_dir, _instance, patched_logger_info):
     _instance.execute()
 
     msg = "Initializing new scenario test-scenario..."
     patched_logger_info.assert_any_call(msg)
 
     assert os.path.isdir("./molecule/test-scenario")
```

### Comparing `molecule-6.0.2/src/molecule/test/a_unit/command/test_base.py` & `molecule-6.0.3/test/a_unit/command/test_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 @pytest.fixture()
 def _instance(_base_class, config_instance: config.Config):
     return _base_class(config_instance)
 
 
 @pytest.fixture()
 def _patched_base_setup(mocker):
-    return mocker.patch("molecule.test.a_unit.command.test_base.ExtendedBase._setup")
+    return mocker.patch("test.a_unit.command.test_base.ExtendedBase._setup")
 
 
 @pytest.fixture()
 def _patched_write_config(mocker):
     return mocker.patch("molecule.provisioner.ansible.Ansible.write_config")
 
 
@@ -69,37 +69,32 @@
 
 @pytest.fixture()
 def _patched_execute_scenario(mocker):
     return mocker.patch("molecule.command.base.execute_scenario")
 
 
 @pytest.fixture()
-def _patched_print_matrix(mocker):
-    return mocker.patch("molecule.scenarios.Scenarios.print_matrix")
-
-
-@pytest.fixture()
 def _patched_prune(mocker):
     return mocker.patch("molecule.scenario.Scenario.prune")
 
 
 @pytest.fixture()
 def _patched_sysexit(mocker):
     return mocker.patch("molecule.util.sysexit")
 
 
-def test_config_private_member(_instance):
+def test_command_config_private_member(_instance):
     assert isinstance(_instance._config, config.Config)
 
 
 def test_init_calls_setup(_patched_base_setup, _instance):
     _patched_base_setup.assert_called_once_with()
 
 
-def test_setup(
+def test_command_setup(
     mocker: MockerFixture,
     patched_add_or_update_vars,
     _patched_write_config,
     _patched_manage_inventory,
     _instance,
 ):
     assert os.path.isdir(os.path.dirname(_instance._config.provisioner.inventory_file))
@@ -107,28 +102,24 @@
 
     _patched_manage_inventory.assert_called_once_with()
     _patched_write_config.assert_called_once_with()
 
 
 def test_execute_cmdline_scenarios(
     config_instance: config.Config,
-    _patched_print_matrix,
     _patched_execute_scenario,
 ):
     # Ensure execute_cmdline_scenarios runs normally:
-    # - scenarios.print_matrix is called, which also indicates Scenarios
-    #   was instantiated correctly
     # - execute_scenario is called once, indicating the function correctly
     #   loops over Scenarios.
     scenario_name = None
     args: dict[str, str] = {}
     command_args = {"destroy": "always", "subcommand": "test"}
     base.execute_cmdline_scenarios(scenario_name, args, command_args)
 
-    assert _patched_print_matrix.called_once_with()
     assert _patched_execute_scenario.call_count == 1
 
 
 def test_execute_cmdline_scenarios_prune(
     config_instance: config.Config,
     _patched_prune,
     _patched_execute_subcommand,
```

### Comparing `molecule-6.0.2/src/molecule/test/a_unit/command/test_check.py` & `molecule-6.0.3/test/a_unit/command/test_check.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 def _patched_ansible_check(mocker):
     return mocker.patch("molecule.provisioner.ansible.Ansible.check")
 
 
 # NOTE(retr0h): The use of the `patched_config_validate` fixture, disables
 # config.Config._validate from executing.  Thus preventing odd side-effects
 # throughout patched.assert_called unit tests.
-def test_execute(
+def test_check_execute(
     mocker: MockerFixture,
     caplog,
     _patched_ansible_check,
     patched_config_validate,
     config_instance: config.Config,
 ):
     c = check.Check(config_instance)
```

### Comparing `molecule-6.0.2/src/molecule/test/a_unit/command/test_cleanup.py` & `molecule-6.0.3/test/a_unit/command/test_cleanup.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 # config.Config._validate from executing.  Thus preventing odd side-effects
 # throughout patched.assert_called unit tests.
 @pytest.mark.parametrize(
     "config_instance",
     ["_command_provisioner_section_with_cleanup_data"],
     indirect=True,
 )
-def test_execute(
+def test_cleanup_execute(
     mocker: MockerFixture,
     _patched_ansible_cleanup,
     caplog,
     patched_config_validate,
     config_instance: config.Config,
 ):
     pb = os.path.join(config_instance.scenario.directory, "cleanup.yml")
@@ -59,15 +59,15 @@
     cu.execute()
 
     assert "cleanup" in caplog.text
 
     _patched_ansible_cleanup.assert_called_once_with()
 
 
-def test_execute_skips_when_playbook_not_configured(
+def test_cleanup_execute_skips_when_playbook_not_configured(
     caplog,
     _patched_ansible_cleanup,
     config_instance: config.Config,
 ):
     cu = cleanup.Cleanup(config_instance)
     cu.execute()
```

### Comparing `molecule-6.0.2/src/molecule/test/a_unit/command/test_converge.py` & `molecule-6.0.3/test/a_unit/command/test_converge.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 from molecule.command import converge
 from molecule.shell import main
 
 
 # NOTE(retr0h): The use of the `patched_config_validate` fixture, disables
 # config.Config._validate from executing.  Thus preventing odd side-effects
 # throughout patched.assert_called unit tests.
-def test_execute(
+def test_converge_execute(
     mocker: MockerFixture,
     caplog: LogCaptureFixture,
     patched_ansible_converge: Mock,
     patched_config_validate: Any,
     config_instance: config.Config,
 ) -> None:
     c = converge.Converge(config_instance)
```

### Comparing `molecule-6.0.2/src/molecule/test/a_unit/command/test_create.py` & `molecule-6.0.3/test/a_unit/command/test_create.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     return mocker.patch("molecule.command.create.Create._setup")
 
 
 # NOTE(retr0h): The use of the `patched_config_validate` fixture, disables
 # config.Config._validate from executing.  Thus preventing odd side-effects
 # throughout patched.assert_called unit tests.
 @pytest.mark.skip(reason="create not running for delegated")
-def test_execute(
+def test_create_execute(
     mocker: MockerFixture,
     caplog,
     command_patched_ansible_create,
     patched_config_validate,
     config_instance: config.Config,
 ):
     c = create.Create(config_instance)
```

### Comparing `molecule-6.0.2/src/molecule/test/a_unit/command/test_dependency.py` & `molecule-6.0.3/test/a_unit/command/test_dependency.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from molecule import config
 from molecule.command import dependency
 
 
 # NOTE(retr0h): The use of the `patched_config_validate` fixture, disables
 # config.Config._validate from executing.  Thus preventing odd side-effects
 # throughout patched.assert_called unit tests.
-def test_execute(
+def test_dependency_execute(
     mocker: MockerFixture,
     caplog,
     patched_ansible_galaxy,
     patched_config_validate,
     config_instance: config.Config,
 ):
     d = dependency.Dependency(config_instance)
```

### Comparing `molecule-6.0.2/src/molecule/test/a_unit/command/test_destroy.py` & `molecule-6.0.3/test/a_unit/command/test_destroy.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     return mocker.patch("molecule.command.destroy.Destroy._setup")
 
 
 # NOTE(retr0h): The use of the `patched_config_validate` fixture, disables
 # config.Config._validate from executing.  Thus preventing odd side-effects
 # throughout patched.assert_called unit tests.
 @pytest.mark.skip(reason="destroy not running for delegated")
-def test_execute(
+def test_destroy_execute(
     mocker: MockerFixture,
     caplog,
     patched_config_validate,
     _patched_ansible_destroy,
     config_instance: config.Config,
 ):
     d = destroy.Destroy(config_instance)
```

### Comparing `molecule-6.0.2/src/molecule/test/a_unit/command/test_idempotence.py` & `molecule-6.0.3/test/a_unit/command/test_idempotence.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 @pytest.fixture()
 def _instance(patched_config_validate, config_instance: config.Config):
     config_instance.state.change_state("converged", True)
 
     return idempotence.Idempotence(config_instance)
 
 
-def test_execute(
+def test_idempotence_execute(
     mocker: MockerFixture,
     caplog: pytest.LogCaptureFixture,
     patched_ansible_converge,
     _patched_is_idempotent: Mock,
     _instance,
 ):
     _instance.execute()
```

### Comparing `molecule-6.0.2/src/molecule/test/a_unit/command/test_list.py` & `molecule-6.0.3/test/a_unit/command/test_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 #  DEALINGS IN THE SOFTWARE.
 
 from molecule import config
 from molecule.command import list
 from molecule.driver import base
 
 
-def test_execute(capsys, config_instance: config.Config):
+def test_list_execute(capsys, config_instance: config.Config):
     l = list.List(config_instance)
     x = [
         base.Status(
             instance_name="instance-1",
             driver_name="default",
             provisioner_name="ansible",
             scenario_name="default",
```

### Comparing `molecule-6.0.2/src/molecule/test/a_unit/command/test_login.py` & `molecule-6.0.3/test/a_unit/command/test_login.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 @pytest.fixture()
 def _instance(config_instance: config.Config):
     config_instance.state.change_state("created", True)
 
     return login.Login(config_instance)
 
 
-def test_execute(mocker: MockerFixture, _instance):
+def test_login_execute(mocker: MockerFixture, _instance):
     _instance._config.command_args = {"host": "instance-1"}
     m = mocker.patch("molecule.command.login.Login._get_login")
     _instance.execute()
 
     m.assert_called_once_with("instance-1")
```

### Comparing `molecule-6.0.2/src/molecule/test/a_unit/command/test_matrix.py` & `molecule-6.0.3/test/a_unit/command/test_matrix.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/src/molecule/test/a_unit/command/test_prepare.py` & `molecule-6.0.3/test/a_unit/command/test_prepare.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 def _patched_ansible_prepare(mocker):
     return mocker.patch("molecule.provisioner.ansible.Ansible.prepare")
 
 
 # NOTE(retr0h): The use of the `patched_config_validate` fixture, disables
 # config.Config._validate from executing.  Thus preventing odd side-effects
 # throughout patched.assert_called unit tests.
-def test_execute(
+def test_prepare_execute(
     mocker: MockerFixture,
     caplog,
     _patched_ansible_prepare,
     patched_config_validate,
     config_instance: config.Config,
 ):
     pb = os.path.join(config_instance.scenario.directory, "prepare.yml")
@@ -67,15 +67,15 @@
 
     msg = "Skipping, instances already prepared."
     assert msg in caplog.text
 
     assert not _patched_ansible_prepare.called
 
 
-def test_execute_skips_when_playbook_not_configured(
+def test_prepare_execute_skips_when_playbook_not_configured(
     caplog,
     _patched_ansible_prepare,
     config_instance: config.Config,
 ):
     p = prepare.Prepare(config_instance)
     p.execute()
```

### Comparing `molecule-6.0.2/src/molecule/test/a_unit/command/test_side_effect.py` & `molecule-6.0.3/test/a_unit/command/test_side_effect.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 # config.Config._validate from executing.  Thus preventing odd side-effects
 # throughout patched.assert_called unit tests.
 @pytest.mark.parametrize(
     "config_instance",
     ["_command_provisioner_section_with_side_effect_data"],
     indirect=True,
 )
-def test_execute(
+def test_side_effect_execute(
     mocker: MockerFixture,
     _patched_ansible_side_effect,
     caplog,
     patched_config_validate,
     config_instance: config.Config,
 ):
     pb = os.path.join(config_instance.scenario.directory, "side_effect.yml")
@@ -65,15 +65,15 @@
 
     assert "default" in caplog.text
     assert "side_effect" in caplog.text
 
     _patched_ansible_side_effect.assert_called_once_with(None)
 
 
-def test_execute_skips_when_playbook_not_configured(
+def test_side_effect_execute_skips_when_playbook_not_configured(
     caplog,
     _patched_ansible_side_effect,
     config_instance: config.Config,
 ):
     se = side_effect.SideEffect(config_instance)
     se.execute()
```

### Comparing `molecule-6.0.2/src/molecule/test/a_unit/command/test_syntax.py` & `molecule-6.0.3/test/a_unit/command/test_syntax.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 def _patched_ansible_syntax(mocker):
     return mocker.patch("molecule.provisioner.ansible.Ansible.syntax")
 
 
 # NOTE(retr0h): The use of the `patched_config_validate` fixture, disables
 # config.Config._validate from executing.  Thus preventing odd side-effects
 # throughout patched.assert_called unit tests.
-def test_execute(
+def test_syntax_execute(
     mocker: MockerFixture,
     caplog,
     _patched_ansible_syntax,
     patched_config_validate,
     config_instance: config.Config,
 ):
     s = syntax.Syntax(config_instance)
```

### Comparing `molecule-6.0.2/src/molecule/test/a_unit/command/test_test.py` & `molecule-6.0.3/test/a_unit/command/test_test.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/src/molecule/test/a_unit/command/test_verify.py` & `molecule-6.0.3/test/a_unit/command/test_verify.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from molecule import config
 from molecule.command import verify
 
 
 # NOTE(retr0h): The use of the `patched_config_validate` fixture, disables
 # config.Config._validate from executing.  Thus preventing odd side-effects
 # throughout patched.assert_called unit tests.
-def test_execute(
+def test_verify_execute(
     mocker: MockerFixture,
     caplog,
     patched_default_verifier,
     patched_config_validate,
     config_instance: config.Config,
 ):
     v = verify.Verify(config_instance)
```

### Comparing `molecule-6.0.2/src/molecule/test/a_unit/conftest.py` & `molecule-6.0.3/test/a_unit/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,28 +20,28 @@
 
 import copy
 import os
 import shutil
 from collections.abc import Generator
 from pathlib import Path
 from subprocess import CompletedProcess
+from test.conftest import (
+    molecule_directory,
+    molecule_ephemeral_directory,
+    molecule_file,
+    molecule_scenario_directory,
+)
 from typing import Any
 from unittest.mock import Mock
 from uuid import uuid4
 
 import pytest
 from pytest_mock import MockerFixture
 
 from molecule import config, util
-from molecule.test.conftest import (
-    molecule_directory,
-    molecule_ephemeral_directory,
-    molecule_file,
-    molecule_scenario_directory,
-)
 
 
 def write_molecule_file(filename: str, data: Any) -> None:
     util.write_file(filename, util.safe_dump(data))
 
 
 def os_split(s: str) -> tuple[str, ...]:
```

### Comparing `molecule-6.0.2/src/molecule/test/a_unit/cookiecutter/test_molecule.py` & `molecule-6.0.3/test/a_unit/cookiecutter/test_molecule.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/src/molecule/test/a_unit/dependency/ansible_galaxy/test_collections.py` & `molecule-6.0.3/test/a_unit/dependency/ansible_galaxy/test_collections.py`

 * *Files 8% similar despite different names*

```diff
@@ -61,68 +61,68 @@
 
 
 @pytest.fixture()
 def role_file(_instance):
     return os.path.join(_instance._config.scenario.directory, "collections.yml")
 
 
-def test_config_private_member(_instance):
+def test_collections_config_private_member(_instance):
     assert isinstance(_instance._config, config.Config)
 
 
-def test_default_options_property(_instance, role_file):
+def test_collections_default_options_property(_instance, role_file):
     x = {"requirements-file": role_file, "force": False}
 
     assert x == _instance.default_options
 
 
-def test_default_env_property(_instance):
+def test_collections_default_env_property(_instance):
     env = _instance.default_env
 
     assert "MOLECULE_FILE" in env
     assert "MOLECULE_INVENTORY_FILE" in env
     assert "MOLECULE_SCENARIO_DIRECTORY" in env
     assert "MOLECULE_INSTANCE_CONFIG" in env
 
 
-def test_name_property(_instance):
+def test_collections_name_property(_instance):
     assert _instance.name == "galaxy"
 
 
-def test_enabled_property(_instance):
+def test_collections_enabled_property(_instance):
     assert _instance.enabled
 
 
 @pytest.mark.parametrize("config_instance", ["_dependency_section_data"], indirect=True)
-def test_options_property(_instance, role_file):
+def test_collections_options_property(_instance, role_file):
     x = {
         "force": False,
         "requirements-file": role_file,
         "foo": "bar",
         "v": True,
     }
 
     assert x == _instance.options
 
 
 @pytest.mark.parametrize("config_instance", ["_dependency_section_data"], indirect=True)
-def test_options_property_handles_cli_args(role_file, _instance):
+def test_collections_options_property_handles_cli_args(role_file, _instance):
     _instance._config.args = {"debug": True}
     x = {
         "force": False,
         "requirements-file": role_file,
         "foo": "bar",
         "vvv": True,
     }
 
     assert x == _instance.options
 
 
 @pytest.mark.parametrize("config_instance", ["_dependency_section_data"], indirect=True)
-def test_env_property(_instance):
+def test_collections_env_property(_instance):
     assert _instance.env["FOO"] == "bar"
 
 
 @pytest.mark.parametrize("config_instance", ["_dependency_section_data"], indirect=True)
 def test_collections_bake(_instance, role_file):
     _instance.bake()
     args = [
@@ -134,15 +134,15 @@
         "--requirements-file",
         role_file,
         "-v",
     ]
     assert _instance._sh_command == args
 
 
-def test_execute(
+def test_collections_execute(
     patched_run_command,
     _patched_ansible_galaxy_has_requirements_file,
     caplog,
     _instance,
 ):
     _instance._sh_command = "patched-command"
     _instance.execute()
@@ -153,44 +153,44 @@
         check=True,
     )
 
     msg = "Dependency completed successfully."
     assert msg in caplog.text
 
 
-def test_execute_does_not_execute_when_disabled(
+def test_collections_execute_does_not_execute_when_disabled(
     patched_run_command,
     caplog,
     _instance,
 ):
     _instance._config.config["dependency"]["enabled"] = False
     _instance.execute()
 
     assert not patched_run_command.called
 
     msg = "Skipping, dependency is disabled."
     assert msg in caplog.text
 
 
-def test_execute_does_not_execute_when_no_requirements_file(
+def test_collections_execute_does_not_execute_when_no_requirements_file(
     patched_run_command,
     _patched_ansible_galaxy_has_requirements_file,
     caplog,
     _instance,
 ):
     _patched_ansible_galaxy_has_requirements_file.return_value = False
     _instance.execute()
 
     assert not patched_run_command.called
 
     msg = "Skipping, missing the requirements file."
     assert msg in caplog.text
 
 
-def test_execute_bakes(
+def test_collections_execute_bakes(
     patched_run_command,
     _instance,
     role_file,
     _patched_ansible_galaxy_has_requirements_file,
 ):
     _instance.execute()
 
@@ -205,17 +205,17 @@
     patched_run_command.side_effect = SystemExit(1)
     with pytest.raises(SystemExit) as e:
         _instance.execute()
 
     assert e.value.code == 1
 
 
-def test_setup(_instance):
+def test_collections_setup(_instance):
     _instance._setup()
 
 
-def test_role_file(role_file, _instance):
+def test_collections_role_file(role_file, _instance):
     assert role_file == _instance.requirements_file
 
 
-def test_has_requirements_file(_instance):
+def test_collections_has_requirements_file(_instance):
     assert not _instance._has_requirements_file()
```

### Comparing `molecule-6.0.2/src/molecule/test/a_unit/dependency/ansible_galaxy/test_roles.py` & `molecule-6.0.3/test/a_unit/dependency/ansible_galaxy/test_roles.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,68 +60,68 @@
 
 
 @pytest.fixture()
 def role_file(_instance):
     return os.path.join(_instance._config.scenario.directory, "requirements.yml")
 
 
-def test_config_private_member(_instance):
+def test_roles_config_private_member(_instance):
     assert isinstance(_instance._config, config.Config)
 
 
-def test_default_options_property(_instance, role_file):
+def test_roles_default_options_property(_instance, role_file):
     x = {"role-file": role_file, "force": False}
 
     assert x == _instance.default_options
 
 
-def test_default_env_property(_instance):
+def test_roles_default_env_property(_instance):
     env = _instance.default_env
 
     assert "MOLECULE_FILE" in env
     assert "MOLECULE_INVENTORY_FILE" in env
     assert "MOLECULE_SCENARIO_DIRECTORY" in env
     assert "MOLECULE_INSTANCE_CONFIG" in env
 
 
-def test_name_property(_instance):
+def test_roles_name_property(_instance):
     assert _instance.name == "galaxy"
 
 
-def test_enabled_property(_instance):
+def test_roles_enabled_property(_instance):
     assert _instance.enabled
 
 
 @pytest.mark.parametrize("config_instance", ["_dependency_section_data"], indirect=True)
-def test_options_property(_instance, role_file):
+def test_roles_options_property(_instance, role_file):
     x = {
         "force": False,
         "role-file": role_file,
         "foo": "bar",
         "v": True,
     }
 
     assert x == _instance.options
 
 
 @pytest.mark.parametrize("config_instance", ["_dependency_section_data"], indirect=True)
-def test_options_property_handles_cli_args(role_file, _instance):
+def test_roles_options_property_handles_cli_args(role_file, _instance):
     _instance._config.args = {"debug": True}
     x = {
         "force": False,
         "role-file": role_file,
         "foo": "bar",
         "vvv": True,
     }
 
     assert x == _instance.options
 
 
 @pytest.mark.parametrize("config_instance", ["_dependency_section_data"], indirect=True)
-def test_env_property(_instance):
+def test_roles_env_property(_instance):
     assert _instance.env["FOO"] == "bar"
 
 
 @pytest.mark.parametrize("config_instance", ["_dependency_section_data"], indirect=True)
 def test_galaxy_bake(_instance, role_file):
     _instance.bake()
     args = [
@@ -151,44 +151,44 @@
         check=True,
     )
 
     msg = "Dependency completed successfully."
     assert msg in caplog.text
 
 
-def test_execute_does_not_execute_when_disabled(
+def test_roles_execute_does_not_execute_when_disabled(
     patched_run_command,
     caplog,
     _instance,
 ):
     _instance._config.config["dependency"]["enabled"] = False
     _instance.execute()
 
     assert not patched_run_command.called
 
     msg = "Skipping, dependency is disabled."
     assert msg in caplog.text
 
 
-def test_execute_does_not_execute_when_no_requirements_file(
+def test_roles_execute_does_not_execute_when_no_requirements_file(
     patched_run_command,
     _patched_ansible_galaxy_has_requirements_file,
     caplog,
     _instance,
 ):
     _patched_ansible_galaxy_has_requirements_file.return_value = False
     _instance.execute()
 
     assert not patched_run_command.called
 
     msg = "Skipping, missing the requirements file."
     assert msg in caplog.text
 
 
-def test_execute_bakes(
+def test_roles_execute_bakes(
     patched_run_command,
     _instance,
     role_file,
     _patched_ansible_galaxy_has_requirements_file,
 ):
     _instance.execute()
     assert _instance._sh_command is not None
@@ -208,9 +208,9 @@
     assert e.value.code == 1
 
 
 def test_role_file(role_file, _instance):
     assert role_file == _instance.requirements_file
 
 
-def test_has_requirements_file(_instance):
+def test_roles_has_requirements_file(_instance):
     assert not _instance._has_requirements_file()
```

### Comparing `molecule-6.0.2/src/molecule/test/a_unit/dependency/test_shell.py` & `molecule-6.0.3/test/a_unit/dependency/test_shell.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,90 +45,94 @@
     _dependency_section_data,
     patched_config_validate,
     config_instance: config.Config,
 ):
     return shell.Shell(config_instance)
 
 
-def test_config_private_member(_instance):
+def test_shell_config_private_member(_instance):
     assert isinstance(_instance._config, config.Config)
 
 
-def test_default_options_property(_instance):
+def test_shell_default_options_property(_instance):
     x = {}
 
     assert x == _instance.default_options
 
 
-def test_default_env_property(_instance):
+def test_shell_default_env_property(_instance):
     assert "MOLECULE_FILE" in _instance.default_env
     assert "MOLECULE_INVENTORY_FILE" in _instance.default_env
     assert "MOLECULE_SCENARIO_DIRECTORY" in _instance.default_env
     assert "MOLECULE_INSTANCE_CONFIG" in _instance.default_env
 
 
 @pytest.mark.parametrize("config_instance", ["_dependency_section_data"], indirect=True)
-def test_name_property(_instance):
+def test_shell_name_property(_instance):
     assert _instance.name == "shell"
 
 
-def test_enabled_property(_instance):
+def test_shell_enabled_property(_instance):
     assert _instance.enabled
 
 
 @pytest.mark.parametrize("config_instance", ["_dependency_section_data"], indirect=True)
-def test_options_property(_instance):
+def test_shell_options_property(_instance):
     x = {"foo": "bar"}
 
     assert x == _instance.options
 
 
 @pytest.mark.parametrize("config_instance", ["_dependency_section_data"], indirect=True)
-def test_options_property_handles_cli_args(_instance):
+def test_shell_options_property_handles_cli_args(_instance):
     _instance._config.args = {}
     x = {"foo": "bar"}
 
     assert x == _instance.options
 
 
 @pytest.mark.parametrize("config_instance", ["_dependency_section_data"], indirect=True)
-def test_env_property(_instance):
+def test_shell_env_property(_instance):
     assert _instance.env["FOO"] == "bar"
 
 
-def test_execute(patched_run_command, caplog: pytest.LogCaptureFixture, _instance):
+def test_shell_execute(
+    patched_run_command,
+    caplog: pytest.LogCaptureFixture,
+    _instance,
+):
     _instance._sh_command = "patched-command"
     _instance.execute()
 
     patched_run_command.assert_called_once_with(
         "patched-command",
         debug=False,
         check=True,
     )
 
     msg = "Dependency completed successfully."
     assert msg in caplog.text
 
 
-def test_execute_does_not_execute_when_disabled(
+def test_shell_execute_does_not_execute_when_disabled(
     patched_run_command,
     caplog: pytest.LogCaptureFixture,
     _instance,
 ):
     _instance._config.config["dependency"]["enabled"] = False
     _instance.execute()
 
     assert not patched_run_command.called
 
     msg = "Skipping, dependency is disabled."
     assert msg in caplog.text
 
 
 @pytest.mark.parametrize("config_instance", ["_dependency_section_data"], indirect=True)
-def test_execute_bakes(patched_run_command, _instance):
+def test_dependency_execute_bakes(patched_run_command, _instance):
     _instance.execute()
     assert patched_run_command.call_count == 1
 
 
 @pytest.mark.parametrize("config_instance", ["_dependency_section_data"], indirect=True)
 def test_dep_executes_catches_and_exits_return_code(patched_run_command, _instance):
     patched_run_command.side_effect = SystemExit(1)
```

### Comparing `molecule-6.0.2/src/molecule/test/a_unit/driver/test_delegated.py` & `molecule-6.0.3/test/a_unit/driver/test_delegated.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,21 +15,21 @@
 #  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 #  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 #  DEALINGS IN THE SOFTWARE.
 
 import os
+from test.conftest import is_subset
 
 import pytest
 from pytest_mock import MockerFixture
 
 from molecule import config
 from molecule.driver import delegated
-from molecule.test.conftest import is_subset
 
 
 @pytest.fixture()
 def _driver_managed_section_data():
     return {
         "driver": {
             "name": "default",
@@ -53,48 +53,48 @@
 
 
 @pytest.fixture()
 def _instance(config_instance: config.Config):
     return delegated.Delegated(config_instance)
 
 
-def test_config_private_member(_instance):
+def test_delegated_config_private_member(_instance):
     assert isinstance(_instance._config, config.Config)
 
 
-def test_testinfra_options_property(_instance):
+def test_delegated_options_property2(_instance):
     assert {
         "connection": "ansible",
         "ansible-inventory": _instance._config.provisioner.inventory_directory,
     } == _instance.testinfra_options
 
 
-def test_name_property(_instance):
+def test_delegated_name_property(_instance):
     assert _instance.name == "default"
 
 
 @pytest.mark.parametrize(
     "config_instance",
     ["_driver_unmanaged_section_data"],
     indirect=True,
 )
-def test_options_property(_instance):
+def test_delegated_options_property(_instance):
     x = {
         "managed": False,
     }
 
     assert x == _instance.options
 
 
 @pytest.mark.parametrize(
     "config_instance",
     ["_driver_managed_section_data"],
     indirect=True,
 )
-def test_options_property_when_managed(_instance):
+def test_delegated_options_property_when_managed(_instance):
     x = {"managed": True}
 
     assert x == _instance.options
 
 
 @pytest.mark.parametrize(
     "config_instance",
@@ -327,15 +327,15 @@
     assert result[1].driver_name == "default"
     assert result[1].provisioner_name == "ansible"
     assert result[1].scenario_name == "default"
     assert result[1].created == "false"
     assert result[1].converged == "false"
 
 
-def test_created(_instance):
+def test_delegated_created(_instance):
     assert _instance._created() == "false"
 
 
 @pytest.fixture()
 def _driver_options_managed_section_data():
     return {"driver": {"options": {"managed": False}}}
```

### Comparing `molecule-6.0.2/src/molecule/test/a_unit/model/v2/conftest.py` & `molecule-6.0.3/test/a_unit/model/v2/conftest.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/src/molecule/test/a_unit/model/v2/test_dependency_section.py` & `molecule-6.0.3/test/a_unit/model/v2/test_dependency_section.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/src/molecule/test/a_unit/model/v2/test_driver_section.py` & `molecule-6.0.3/test/a_unit/model/v2/test_driver_section.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/src/molecule/test/a_unit/model/v2/test_platforms_section.py` & `molecule-6.0.3/test/a_unit/model/v2/test_platforms_section.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/src/molecule/test/a_unit/model/v2/test_provisioner_section.py` & `molecule-6.0.3/test/a_unit/model/v2/test_provisioner_section.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/src/molecule/test/a_unit/model/v2/test_scenario_section.py` & `molecule-6.0.3/test/a_unit/model/v2/test_scenario_section.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/src/molecule/test/a_unit/model/v2/test_schema.py` & `molecule-6.0.3/test/a_unit/model/v2/test_schema.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,19 +28,19 @@
 
 def test_molecule_schema():
     cmd = [
         "check-jsonschema",
         "-v",
         "--schemafile",
         "src/molecule/data/molecule.json",
-        "src/molecule/test/resources/schema_instance_files/valid/molecule.yml",
+        "test/resources/schema_instance_files/valid/molecule.yml",
     ]
     assert run_command(cmd).returncode == 0
 
     cmd = [
         "check-jsonschema",
         "-v",
         "--schemafile",
         "src/molecule/data/driver.json",
-        "src/molecule/test/resources/schema_instance_files/invalid/molecule_delegated.yml",
+        "test/resources/schema_instance_files/invalid/molecule_delegated.yml",
     ]
     assert run_command(cmd).returncode != 0
```

### Comparing `molecule-6.0.2/src/molecule/test/a_unit/model/v2/test_verifier_section.py` & `molecule-6.0.3/test/a_unit/model/v2/test_verifier_section.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/src/molecule/test/a_unit/provisioner/test_ansible.py` & `molecule-6.0.3/test/a_unit/provisioner/test_ansible.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,21 +17,21 @@
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 #  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 #  DEALINGS IN THE SOFTWARE.
 
 import collections
 import os
 import re
+from test.a_unit.conftest import os_split
 
 import pytest
 from pytest_mock import MockerFixture
 
 from molecule import config, util
 from molecule.provisioner import ansible, ansible_playbooks
-from molecule.test.a_unit.conftest import os_split
 
 
 @pytest.fixture()
 def _patched_ansible_playbook(mocker):
     m = mocker.patch("molecule.provisioner.ansible_playbook.AnsiblePlaybook")
     m.return_value.execute.return_value = b"patched-ansible-playbook-stdout"
 
@@ -88,15 +88,15 @@
 
 
 @pytest.fixture()
 def _instance(_provisioner_section_data, config_instance: config.Config):
     return ansible.Ansible(config_instance)
 
 
-def test_config_private_member(_instance):
+def test_profisioner_config_private_member(_instance):
     assert isinstance(_instance._config, config.Config)
 
 
 def test_default_config_options_property(_instance):
     x = {
         "defaults": {
             "ansible_managed": "Ansible managed: Do NOT edit this file manually!",
@@ -113,33 +113,33 @@
             "scp_if_ssh": True,
         },
     }
 
     assert x == _instance.default_config_options
 
 
-def test_default_options_property(_instance):
+def test_provisioner_default_options_property(_instance):
     assert {"skip-tags": "molecule-notest,notest"} == _instance.default_options
 
 
-def test_default_env_property(_instance):
+def test_ansible_default_env_property(_instance):
     x = _instance._config.provisioner.config_file
 
     assert x == _instance.default_env["ANSIBLE_CONFIG"]
     assert "MOLECULE_FILE" in _instance.default_env
     assert "MOLECULE_INVENTORY_FILE" in _instance.default_env
     assert "MOLECULE_SCENARIO_DIRECTORY" in _instance.default_env
     assert "MOLECULE_INSTANCE_CONFIG" in _instance.default_env
     assert "ANSIBLE_CONFIG" in _instance.env
     assert "ANSIBLE_ROLES_PATH" in _instance.env
     assert "ANSIBLE_LIBRARY" in _instance.env
     assert "ANSIBLE_FILTER_PLUGINS" in _instance.env
 
 
-def test_name_property(_instance):
+def test_provisioner_name_property(_instance):
     assert _instance.name == "ansible"
 
 
 @pytest.mark.parametrize(
     "config_instance",
     ["_provisioner_section_data"],
     indirect=True,
@@ -166,28 +166,28 @@
 
 
 @pytest.mark.parametrize(
     "config_instance",
     ["_provisioner_section_data"],
     indirect=True,
 )
-def test_options_property(_instance):
+def test_ansible_options_property(_instance):
     x = {"become": True, "foo": "bar", "v": True, "skip-tags": "molecule-notest,notest"}
 
     assert x == _instance.options
 
 
-def test_options_property_does_not_merge(_instance):
+def test_ansible_options_property_does_not_merge(_instance):
     for action in ["create", "destroy"]:
         _instance._config.action = action
 
         assert {"skip-tags": "molecule-notest,notest"} == _instance.options
 
 
-def test_options_property_handles_cli_args(_instance):
+def test_provisioner_ansible_options_property_handles_cli_args(_instance):
     _instance._config.args = {"debug": True}
     x = {
         "vvv": True,
         "become": True,
         "diff": True,
         "skip-tags": "molecule-notest,notest",
     }
@@ -196,15 +196,15 @@
 
 
 @pytest.mark.parametrize(
     "config_instance",
     ["_provisioner_section_data"],
     indirect=True,
 )
-def test_env_property(_instance):
+def test_provisioner_env_property(_instance):
     x = _instance._config.provisioner.config_file
 
     assert x == _instance.env["ANSIBLE_CONFIG"]
     assert _instance.env["FOO"] == "bar"
 
 
 @pytest.mark.parametrize(
@@ -302,15 +302,15 @@
     assert x == _instance.config_file
 
 
 def test_playbooks_property(_instance):
     assert isinstance(_instance.playbooks, ansible_playbooks.AnsiblePlaybooks)
 
 
-def test_directory_property(_instance):
+def test_provisioner_directory_property(_instance):
     result = _instance.directory
     parts = os_split(result)
 
     assert parts[-3:] == ("molecule", "provisioner", "ansible")
 
 
 def test_playbooks_cleaned_property_is_optional(_instance):
@@ -453,15 +453,15 @@
         _patched_ansible_playbook.assert_called_once_with(
             _instance._config.provisioner.playbooks.verify,
             _instance._config,
         )
         _patched_ansible_playbook.return_value.execute.assert_called_once_with()
 
 
-def test_write_config(temp_dir, _instance):
+def test_ansible_write_config(temp_dir, _instance):
     _instance.write_config()
 
     assert os.path.isfile(_instance.config_file)
 
 
 def test_manage_inventory(
     _instance,
```

### Comparing `molecule-6.0.2/src/molecule/test/a_unit/provisioner/test_ansible_playbook.py` & `molecule-6.0.3/test/a_unit/provisioner/test_ansible_playbook.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,15 +190,15 @@
 
 def test_execute_playbook(patched_run_command, _instance):
     _instance._ansible_command = "patched-command"
     result = _instance.execute()
     assert result == "patched-run-command-stdout"
 
 
-def test_execute_bakes(_inventory_directory, patched_run_command, _instance):
+def test_ansible_execute_bakes(_inventory_directory, patched_run_command, _instance):
     _instance.execute()
 
     assert _instance._ansible_command is not None
 
     args = [
         "ansible-playbook",
         "--inventory",
```

### Comparing `molecule-6.0.2/src/molecule/test/a_unit/provisioner/test_ansible_playbooks.py` & `molecule-6.0.3/test/a_unit/provisioner/test_ansible_playbooks.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,20 +15,20 @@
 #  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 #  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 #  DEALINGS IN THE SOFTWARE.
 
 import os
+from test.a_unit.conftest import os_split
 
 import pytest
 
 from molecule import config, util
 from molecule.provisioner import ansible_playbooks
-from molecule.test.a_unit.conftest import os_split
 
 
 @pytest.fixture()
 def _provisioner_section_data():
     return {"provisioner": {"name": "ansible", "options": {}, "config_options": {}}}
```

### Comparing `molecule-6.0.2/src/molecule/test/a_unit/test_api.py` & `molecule-6.0.3/test/a_unit/test_api.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/src/molecule/test/a_unit/test_config.py` & `molecule-6.0.3/test/a_unit/test_config.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/src/molecule/test/a_unit/test_interpolation.py` & `molecule-6.0.3/test/a_unit/test_interpolation.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/src/molecule/test/a_unit/test_logger.py` & `molecule-6.0.3/test/a_unit/test_logger.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/src/molecule/test/a_unit/test_platforms.py` & `molecule-6.0.3/test/a_unit/test_platforms.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/src/molecule/test/a_unit/test_scenario.py` & `molecule-6.0.3/test/a_unit/test_scenario.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,31 +75,31 @@
         assert not os.path.isdir(os.path.join(e_dir, pruned_dir))
 
 
 def test_config_member(_instance):
     assert isinstance(_instance.config, config.Config)
 
 
-def test_init_calls_setup(patched_scenario_setup, _instance):
+def test_scenario_init_calls_setup(patched_scenario_setup, _instance):
     patched_scenario_setup.assert_called_once_with()
 
 
-def test_name_property(_instance):
+def test_scenario_name_property(_instance):
     assert _instance.name == "default"
 
 
-def test_directory_property(molecule_scenario_directory_fixture, _instance):
+def test_scenario_directory_property(molecule_scenario_directory_fixture, _instance):
     assert molecule_scenario_directory_fixture == _instance.directory
 
 
 def test_ephemeral_directory_property(_instance):
     assert os.access(_instance.ephemeral_directory, os.W_OK)
 
 
-def test_inventory_directory_property(_instance):
+def test_scenario_inventory_directory_property(_instance):
     ephemeral_directory = _instance.config.scenario.ephemeral_directory
     e_dir = os.path.join(ephemeral_directory, "inventory")
 
     assert e_dir == _instance.inventory_directory
 
 
 def test_check_sequence_property(_instance):
```

### Comparing `molecule-6.0.2/src/molecule/test/a_unit/test_scenarios.py` & `molecule-6.0.3/test/a_unit/test_scenarios.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/src/molecule/test/a_unit/test_scenarios_ordered.py` & `molecule-6.0.3/test/a_unit/test_scenarios_ordered.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/src/molecule/test/a_unit/test_shell.py` & `molecule-6.0.3/test/a_unit/test_shell.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/src/molecule/test/a_unit/test_state.py` & `molecule-6.0.3/test/a_unit/test_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     assert not _instance.converged
 
 
 def test_created(_instance):
     assert not _instance.created
 
 
-def test_driver(_instance):
+def test_state_driver(_instance):
     assert not _instance.driver
 
 
 def test_prepared(_instance):
     assert not _instance.prepared
```

### Comparing `molecule-6.0.2/src/molecule/test/a_unit/test_status.py` & `molecule-6.0.3/test/a_unit/test_status.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/src/molecule/test/a_unit/test_text.py` & `molecule-6.0.3/test/a_unit/test_text.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/src/molecule/test/a_unit/test_util.py` & `molecule-6.0.3/test/a_unit/test_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,24 +19,24 @@
 #  DEALINGS IN THE SOFTWARE.
 
 
 import binascii
 import os
 import warnings
 from pathlib import Path
+from test.conftest import get_molecule_file, molecule_directory
 from typing import Any
 
 import pytest
 from pytest_mock import MockerFixture
 
 from molecule import util
 from molecule.api import IncompatibleMoleculeRuntimeWarning, MoleculeRuntimeWarning
 from molecule.console import console
 from molecule.constants import MOLECULE_HEADER
-from molecule.test.conftest import get_molecule_file, molecule_directory
 from molecule.text import strip_ansi_escape
 
 
 def test_print_debug():
     expected = "DEBUG: test_title:\ntest_data\n"
     with console.capture() as capture:
         util.print_debug("test_title", "test_data")
```

### Comparing `molecule-6.0.2/src/molecule/test/a_unit/verifier/test_ansible.py` & `molecule-6.0.3/test/a_unit/verifier/test_ansible.py`

 * *Files 13% similar despite different names*

```diff
@@ -27,64 +27,64 @@
     _verifier_section_data,
     patched_config_validate,
     config_instance: config.Config,
 ):
     return ansible.Ansible(config_instance)
 
 
-def test_config_private_member(_instance):
+def test_verifier_config_private_member(_instance):
     assert isinstance(_instance._config, config.Config)
 
 
-def test_default_options_property(_instance):
+def test_verifier_default_options_property(_instance):
     assert {} == _instance.default_options
 
 
-def test_default_env_property(_instance):
+def test_verifier_ansible_default_env_property(_instance):
     assert "MOLECULE_FILE" in _instance.default_env
     assert "MOLECULE_INVENTORY_FILE" in _instance.default_env
     assert "MOLECULE_SCENARIO_DIRECTORY" in _instance.default_env
     assert "MOLECULE_INSTANCE_CONFIG" in _instance.default_env
 
 
 @pytest.mark.parametrize("config_instance", ["_verifier_section_data"], indirect=True)
-def test_env_property(_instance):
+def test_verifier_env_property(_instance):
     assert _instance.env["FOO"] == "bar"
 
 
-def test_name_property(_instance):
+def test_verifier_name_property(_instance):
     assert _instance.name == "ansible"
 
 
-def test_enabled_property(_instance):
+def test_ansible_enabled_property(_instance):
     assert _instance.enabled
 
 
-def test_directory_property(_instance):
+def test_verifier_directory_property(_instance):
     parts = _instance.directory.split(os.path.sep)
     # Unused by Ansible verifier
     assert ["molecule", "default", "tests"] == parts[-3:]
 
 
 @pytest.mark.parametrize("config_instance", ["_verifier_section_data"], indirect=True)
-def test_options_property(_instance):
+def test_verifier_ansible_options_property(_instance):
     x = {}
 
     assert x == _instance.options
 
 
 @pytest.mark.parametrize("config_instance", ["_verifier_section_data"], indirect=True)
-def test_options_property_handles_cli_args(_instance):
+def test_verifier_ansible_options_property_handles_cli_args(_instance):
     _instance._config.args = {"debug": True}
     x = {}
 
     assert x == _instance.options
 
 
-def test_execute(caplog, _patched_ansible_verify, _instance):
+def test_ansible_execute(caplog, _patched_ansible_verify, _instance):
     _instance.execute()
 
     _patched_ansible_verify.assert_called_once_with(None)
 
     msg = "Running Ansible Verifier"
     assert msg in caplog.text
```

### Comparing `molecule-6.0.2/src/molecule/test/a_unit/verifier/test_testinfra.py` & `molecule-6.0.3/test/a_unit/verifier/test_testinfra.py`

 * *Files 10% similar despite different names*

```diff
@@ -60,19 +60,19 @@
 
 
 @pytest.fixture()
 def inventory_directory(_instance):
     return _instance._config.provisioner.inventory_directory
 
 
-def test_config_private_member(_instance):
+def test_testinfra_config_private_member(_instance):
     assert isinstance(_instance._config, config.Config)
 
 
-def test_default_options_property(inventory_directory, _instance):
+def test_testinfra_default_options_property(inventory_directory, _instance):
     x = {
         "connection": "ansible",
         "ansible-inventory": inventory_directory,
         "p": "no:cacheprovider",
     }
 
     assert x == _instance.default_options
@@ -103,15 +103,15 @@
         "sudo": True,
         "p": "no:cacheprovider",
     }
 
     assert x == _instance.default_options
 
 
-def test_default_env_property(_instance):
+def test_testinfra_default_env_property(_instance):
     assert "MOLECULE_FILE" in _instance.default_env
     assert "MOLECULE_INVENTORY_FILE" in _instance.default_env
     assert "MOLECULE_SCENARIO_DIRECTORY" in _instance.default_env
     assert "MOLECULE_INSTANCE_CONFIG" in _instance.default_env
 
 
 @pytest.mark.parametrize("config_instance", ["_verifier_section_data"], indirect=True)
@@ -130,31 +130,31 @@
         util.write_file(f, "")
 
     x = [file1_file, file2_file, match1_file, match2_file, test_subdir_file]
     assert sorted(x) == sorted(_instance.additional_files_or_dirs)
 
 
 @pytest.mark.parametrize("config_instance", ["_verifier_section_data"], indirect=True)
-def test_env_property(_instance):
+def test_testinfra_env_property(_instance):
     assert _instance.env["FOO"] == "bar"
     assert "ANSIBLE_CONFIG" in _instance.env
     assert "ANSIBLE_ROLES_PATH" in _instance.env
     assert "ANSIBLE_LIBRARY" in _instance.env
     assert "ANSIBLE_FILTER_PLUGINS" in _instance.env
 
 
-def test_name_property(_instance):
+def test_testinfra_name_property(_instance):
     assert _instance.name == "testinfra"
 
 
-def test_enabled_property(_instance):
+def test_testinfra_enabled_property(_instance):
     assert _instance.enabled
 
 
-def test_directory_property(_instance):
+def test_testinfra_directory_property(_instance):
     parts = _instance.directory.split(os.path.sep)
 
     assert ["molecule", "default", "tests"] == parts[-3:]
 
 
 @pytest.fixture()
 def _verifier_testinfra_directory_section_data():
@@ -167,29 +167,29 @@
     indirect=True,
 )
 def test_directory_property_overridden(_instance):
     assert _instance.directory == "/tmp/foo/bar"
 
 
 @pytest.mark.parametrize("config_instance", ["_verifier_section_data"], indirect=True)
-def test_options_property(inventory_directory, _instance):
+def test_testinfra_options_property(inventory_directory, _instance):
     x = {
         "connection": "ansible",
         "ansible-inventory": inventory_directory,
         "foo": "bar",
         "v": True,
         "verbose": True,
         "p": "no:cacheprovider",
     }
 
     assert x == _instance.options
 
 
 @pytest.mark.parametrize("config_instance", ["_verifier_section_data"], indirect=True)
-def test_options_property_handles_cli_args(inventory_directory, _instance):
+def test_tesinfra_options_property_handles_cli_args(inventory_directory, _instance):
     _instance._config.args = {"debug": True}
     x = {
         "connection": "ansible",
         "ansible-inventory": inventory_directory,
         "foo": "bar",
         "debug": True,
         "vvv": True,
@@ -197,15 +197,15 @@
         "p": "no:cacheprovider",
     }
 
     assert x == _instance.options
 
 
 @pytest.mark.parametrize("config_instance", ["_verifier_section_data"], indirect=True)
-def test_bake(_patched_testinfra_get_tests, inventory_directory, _instance):
+def test_testinfra_bake(_patched_testinfra_get_tests, inventory_directory, _instance):
     _instance._tests = ["foo.py", "bar.py"]
     _instance.bake()
     args = [
         "pytest",
         "--ansible-inventory",
         inventory_directory,
         "--connection",
@@ -218,15 +218,15 @@
         "bar.py",
         "-v",
     ]
 
     assert _instance._testinfra_command == args
 
 
-def test_execute(
+def test_testinfra_execute(
     caplog,
     patched_run_command,
     _patched_testinfra_get_tests,
     _instance,
 ):
     _instance.execute()
 
@@ -235,15 +235,15 @@
     msg = f"Executing Testinfra tests found in {_instance.directory}/..."
     msg2 = "Verifier completed successfully."
     assert msg in caplog.text
     assert msg2 in caplog.text
     assert "pytest" == patched_run_command.call_args[0][0][0]
 
 
-def test_execute_does_not_execute(
+def test_testinfra_execute_does_not_execute(
     patched_run_command,
     caplog,
     _instance,
 ):
     _instance._config.config["verifier"]["enabled"] = False
     _instance.execute()
 
@@ -262,15 +262,19 @@
 
     assert not patched_run_command.called
 
     msg = "Skipping, no tests found."
     assert msg in caplog.text
 
 
-def test_execute_bakes(patched_run_command, _patched_testinfra_get_tests, _instance):
+def test_testinfra_execute_bakes(
+    patched_run_command,
+    _patched_testinfra_get_tests,
+    _instance,
+):
     _instance.execute()
 
     assert _instance._testinfra_command is not None
 
     assert patched_run_command.call_count == 1
```

### Comparing `molecule-6.0.2/src/molecule/test/b_functional/conftest.py` & `molecule-6.0.3/test/b_functional/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,24 +20,24 @@
 #  DEALINGS IN THE SOFTWARE.
 from __future__ import annotations
 
 import os
 import shutil
 import subprocess
 from subprocess import PIPE
+from test.conftest import change_dir_to, molecule_directory
 
 import pexpect
 import pytest
 from ansible_compat.ports import cache
 from packaging.version import Version
 
 import molecule
 from molecule import logger, util
 from molecule.app import app
-from molecule.test.conftest import change_dir_to, molecule_directory
 from molecule.text import strip_ansi_color
 from molecule.util import run_command
 
 LOG = logger.get_logger(__name__)
 
 IS_TRAVIS = os.getenv("TRAVIS") and os.getenv("CI")
 # requires >=1.5.1 due to missing cp command, we tested with 1.4.2-stable3 and
```

### Comparing `molecule-6.0.2/src/molecule/test/b_functional/test_command.py` & `molecule-6.0.3/test/b_functional/test_command.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,26 +17,26 @@
 #  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 #  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 #  DEALINGS IN THE SOFTWARE.
 from __future__ import annotations
 
 import os
 import pathlib
-
-import pytest
-from pytest import FixtureRequest
-
-from molecule.command import base
-from molecule.test.b_functional.conftest import (
+from test.b_functional.conftest import (
     idempotence,
     init_scenario,
     list_with_format_plain,
     run_test,
     verify,
 )
+
+import pytest
+from pytest import FixtureRequest
+
+from molecule.command import base
 from molecule.util import run_command
 
 
 @pytest.fixture()
 def scenario_to_test(request):
     return request.param
 
@@ -66,56 +66,56 @@
         return None
 
 
 @pytest.mark.extensive()
 @pytest.mark.parametrize(
     ("scenario_to_test", "driver_name", "scenario_name"),
     [
-        ("driver/delegated", "default", "default"),
+        pytest.param("driver/delegated", "default", "default", id="0"),
     ],
     indirect=["scenario_to_test", "driver_name", "scenario_name"],
 )
 def test_command_check(scenario_to_test, with_scenario, scenario_name):
     cmd = ["molecule", "check", "--scenario-name", scenario_name]
     assert run_command(cmd).returncode == 0
 
 
 @pytest.mark.extensive()
 @pytest.mark.parametrize(
     ("scenario_to_test", "driver_name", "scenario_name"),
     [
-        ("driver/delegated", "default", "default"),
+        pytest.param("driver/delegated", "default", "default", id="0"),
     ],
     indirect=["scenario_to_test", "driver_name", "scenario_name"],
 )
 @pytest.mark.serial()
 def test_command_cleanup(scenario_to_test, with_scenario, scenario_name):
     cmd = ["molecule", "cleanup", "--scenario-name", scenario_name]
     assert run_command(cmd).returncode == 0
 
 
 @pytest.mark.extensive()
 @pytest.mark.parametrize(
     ("scenario_to_test", "driver_name", "scenario_name"),
     [
-        ("driver/delegated", "default", "default"),
+        pytest.param("driver/delegated", "default", "default", id="0"),
     ],
     indirect=["scenario_to_test", "driver_name", "scenario_name"],
 )
 @pytest.mark.serial()
 def test_command_converge(scenario_to_test, with_scenario, scenario_name):
     cmd = ["molecule", "converge", "--scenario-name", scenario_name]
     assert run_command(cmd).returncode == 0
 
 
 @pytest.mark.extensive()
 @pytest.mark.parametrize(
     ("scenario_to_test", "driver_name", "scenario_name"),
     [
-        ("driver/delegated", "default", "default"),
+        pytest.param("driver/delegated", "default", "default", id="0"),
     ],
     indirect=["scenario_to_test", "driver_name", "scenario_name"],
 )
 @pytest.mark.serial()
 def test_command_create(scenario_to_test, with_scenario, scenario_name, tmp_path):
     cmd = ["molecule", "create", "--scenario-name", scenario_name]
     assert run_command(cmd, env=os.environ).returncode == 0
@@ -148,28 +148,28 @@
     assert run_command(cmd, echo=True).returncode == 0
 
 
 @pytest.mark.serial()
 @pytest.mark.extensive()
 @pytest.mark.parametrize(
     ("scenario_to_test", "driver_name", "scenario_name"),
-    [("driver/delegated", "default", "default")],
+    [pytest.param("driver/delegated", "default", "default", id="0")],
     indirect=["scenario_to_test", "driver_name", "scenario_name"],
 )
 def test_command_destroy(scenario_to_test, with_scenario, scenario_name):
     cmd = ["molecule", "destroy", "--scenario-name", scenario_name]
     assert run_command(cmd).returncode == 0
 
 
 @pytest.mark.serial()
 @pytest.mark.extensive()
 @pytest.mark.parametrize(
     ("scenario_to_test", "driver_name", "scenario_name"),
     [
-        ("driver/delegated", "default", "default"),
+        pytest.param("driver/delegated", "default", "default", id="0"),
     ],
     indirect=["scenario_to_test", "driver_name", "scenario_name"],
 )
 def test_command_idempotence(scenario_to_test, with_scenario, scenario_name):
     idempotence(scenario_name)
 
 
@@ -178,32 +178,33 @@
     init_scenario(temp_dir, "default")
 
 
 @pytest.mark.serial()
 @pytest.mark.parametrize(
     ("scenario_to_test", "driver_name", "expected"),
     [
-        (
+        pytest.param(
             "driver/delegated",
             "default",
             "instance        default ansible default",
+            id="0",
         ),
     ],
     indirect=["scenario_to_test", "driver_name"],
 )
 def test_command_list_with_format_plain(scenario_to_test, with_scenario, expected):
     list_with_format_plain(expected)
 
 
 @pytest.mark.serial()
 @pytest.mark.extensive()
 @pytest.mark.parametrize(
     ("scenario_to_test", "driver_name", "scenario_name"),
     [
-        ("driver/delegated", "default", "default"),
+        pytest.param("driver/delegated", "default", "default", id="0"),
     ],
     indirect=["scenario_to_test", "driver_name", "scenario_name"],
 )
 def test_command_prepare(scenario_to_test, with_scenario, scenario_name):
     cmd = ["molecule", "create", "--scenario-name", scenario_name]
     assert run_command(cmd).returncode == 0
 
@@ -212,42 +213,42 @@
 
 
 @pytest.mark.serial()
 @pytest.mark.extensive()
 @pytest.mark.parametrize(
     ("scenario_to_test", "driver_name", "scenario_name"),
     [
-        ("driver/delegated", "default", "default"),
+        pytest.param("driver/delegated", "default", "default", id="0"),
     ],
     indirect=["scenario_to_test", "driver_name", "scenario_name"],
 )
 def test_command_side_effect(scenario_to_test, with_scenario, scenario_name):
     cmd = ["molecule", "side-effect", "--scenario-name", scenario_name]
     assert run_command(cmd).returncode == 0
 
 
 @pytest.mark.serial()
 @pytest.mark.extensive()
 @pytest.mark.parametrize(
     ("scenario_to_test", "driver_name", "scenario_name"),
     [
-        ("driver/delegated", "default", "default"),
+        pytest.param("driver/delegated", "default", "default", id="0"),
     ],
     indirect=["scenario_to_test", "driver_name", "scenario_name"],
 )
 def test_command_syntax(scenario_to_test, with_scenario, scenario_name):
     cmd = ["molecule", "syntax", "--scenario-name", scenario_name]
     assert run_command(cmd).returncode == 0
 
 
 @pytest.mark.serial()
 @pytest.mark.parametrize(
     ("scenario_to_test", "driver_name", "scenario_name"),
     [
-        ("driver/delegated", "default", "default"),
+        pytest.param("driver/delegated", "default", "default", id="0"),
     ],
     indirect=["scenario_to_test", "driver_name", "scenario_name"],
 )
 def test_command_test(scenario_to_test, with_scenario, scenario_name, driver_name):
     run_test(driver_name, scenario_name)
 
 
@@ -276,15 +277,15 @@
     assert run_command(cmd).returncode == 0
 
 
 @pytest.mark.serial()
 @pytest.mark.parametrize(
     ("scenario_to_test", "driver_name", "scenario_name", "platform_name"),
     [
-        ("driver/delegated", "default", "default", "instance"),
+        pytest.param("driver/delegated", "default", "default", "instance", id="0"),
     ],
     indirect=["scenario_to_test", "driver_name", "scenario_name", "platform_name"],
 )
 def test_command_test_with_platform_name(
     scenario_to_test,
     with_scenario,
     scenario_name,
@@ -294,18 +295,19 @@
     run_test_with_platform_name(driver_name, platform_name, scenario_name)
 
 
 @pytest.mark.serial()
 @pytest.mark.parametrize(
     ("scenario_to_test", "driver_name", "scenario_name"),
     [
-        (
+        pytest.param(
             "driver/delegated_invalid_role_name_with_role_name_check_equals_to_1",
             "default",
             "default",
+            id="0",
         ),
     ],
     indirect=["scenario_to_test", "driver_name", "scenario_name"],
 )
 def test_command_test_with_role_name_check_equals_to_1(
     scenario_to_test,
     with_scenario,
@@ -316,27 +318,27 @@
 
 
 @pytest.mark.serial()
 @pytest.mark.extensive()
 @pytest.mark.parametrize(
     ("scenario_to_test", "driver_name", "scenario_name"),
     [
-        ("driver/delegated", "default", "default"),
+        pytest.param("driver/delegated", "default", "default", id="0"),
     ],
     indirect=["scenario_to_test", "driver_name", "scenario_name"],
 )
 def test_command_verify(scenario_to_test, with_scenario, scenario_name):
     verify(scenario_name)
 
 
 def test_sample_collection() -> None:
     assert (
         run_command(
             ["molecule", "test"],
-            cwd="src/molecule/test/resources/sample-collection",
+            cwd="test/resources/sample-collection",
         ).returncode
         == 0
     )
 
 
 @pytest.mark.parametrize(
     ("scenario_name"),
```

### Comparing `molecule-6.0.2/src/molecule/test/conftest.py` & `molecule-6.0.3/test/conftest.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/src/molecule/test/resources/schema_instance_files/valid/molecule.yml` & `molecule-6.0.3/test/resources/schema_instance_files/valid/molecule.yml`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/src/molecule/test/scenarios/host_group_vars/molecule/default/converge.yml` & `molecule-6.0.3/test/scenarios/host_group_vars/molecule/default/converge.yml`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 ---
-- hosts: instance
+- name: Molecule test fixture
+  hosts: instance
   gather_facts: false
   tasks:
     - name: Host vars host_var for host host-group-vars from molecule.yml
       ansible.builtin.debug:
         var: host_group_vars_host_molecule_yml
 
     - name: Host vars from host_vars existing directory
@@ -24,20 +25,22 @@
       ansible.builtin.debug:
         var: host_group_vars_example_1_child_group_molecule_yml
 
     - name: Variable from extra_host from molecule.yml
       ansible.builtin.debug:
         var: hostvars['extra_host']['host_group_vars_extra_host_molecule_yml']
 
-- hosts: example
+- name: Molecule test fixture
+  hosts: example
   gather_facts: false
   tasks:
     - name: Dummy converge of example group
       ansible.builtin.debug:
         var: ansible_host
 
-- hosts: example_1
+- name: Molecule test fixture
+  hosts: example_1
   gather_facts: false
   tasks:
     - name: Dummy converge of child example_1 group
       ansible.builtin.debug:
         var: ansible_host
```

### Comparing `molecule-6.0.2/src/molecule/test/scenarios/host_group_vars/molecule/default/molecule.yml` & `molecule-6.0.3/test/scenarios/host_group_vars/molecule/default/molecule.yml`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/src/molecule/test/scenarios/test_destroy_strategy/molecule/default/tests/test_destroy_strategy.py` & `molecule-6.0.3/test/scenarios/test_destroy_strategy/molecule/default/tests/test_destroy_strategy.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/src/molecule/text.py` & `molecule-6.0.3/src/molecule/text.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/src/molecule/util.py` & `molecule-6.0.3/src/molecule/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -251,15 +251,15 @@
     return f"{instance_name}-{scenario_name}"
 
 
 def verbose_flag(options):
     """Return computed verbosity flag."""
     verbose = "v"
     verbose_flag = []
-    for _i in range(0, 3):
+    for _i in range(3):
         if options.get(verbose):
             verbose_flag = [f"-{verbose}"]
             del options[verbose]
             if options.get("verbose"):
                 del options["verbose"]
             break
         verbose = verbose + "v"
```

### Comparing `molecule-6.0.2/src/molecule/verifier/ansible.py` & `molecule-6.0.3/src/molecule/verifier/ansible.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/src/molecule/verifier/base.py` & `molecule-6.0.3/src/molecule/verifier/base.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/src/molecule/verifier/testinfra.py` & `molecule-6.0.3/src/molecule/verifier/testinfra.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/src/molecule.egg-info/PKG-INFO` & `molecule-6.0.3/src/molecule.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molecule
-Version: 6.0.2
+Version: 6.0.3
 Summary: Molecule aids in the development and testing of Ansible roles
 Author-email: Ansible by Red Hat <info@ansible.com>
 Maintainer-email: Ansible by Red Hat <info@ansible.com>
 License: MIT
 Project-URL: homepage, https://github.com/ansible-community/molecule
 Project-URL: documentation, https://molecule.readthedocs.io/
 Project-URL: repository, https://github.com/ansible-community/molecule
@@ -18,26 +18,53 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Software Development :: Bug Tracking
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Utilities
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: ansible-compat>=4.1.8
+Requires-Dist: ansible-core>=2.12.10
+Requires-Dist: click<9,>=8.0
+Requires-Dist: click-help-colors>=0.9
+Requires-Dist: enrich>=1.2.7
+Requires-Dist: jsonschema>=4.9.1
+Requires-Dist: Jinja2>=2.11.3
+Requires-Dist: packaging
+Requires-Dist: pluggy<2.0,>=0.7.1
+Requires-Dist: PyYAML>=5.1
+Requires-Dist: rich>=9.5.1
+Requires-Dist: wcmatch>=8.1.2
 Provides-Extra: docs
+Requires-Dist: mkdocs-ansible[lock]>=0.2.0; extra == "docs"
+Requires-Dist: pipdeptree>=2.4.0; extra == "docs"
+Requires-Dist: linkchecker==10.2.1; extra == "docs"
 Provides-Extra: test
+Requires-Dist: ansible-lint>=6.12.1; extra == "test"
+Requires-Dist: ansi2html>=1.8.0; extra == "test"
+Requires-Dist: coverage>=7.0.3; extra == "test"
+Requires-Dist: filelock>=3.9.0; extra == "test"
+Requires-Dist: pexpect<5,>=4.8.0; extra == "test"
+Requires-Dist: pytest-mock>=3.10.0; extra == "test"
+Requires-Dist: pytest-plus>=0.4.0; extra == "test"
+Requires-Dist: pytest-xdist>=3.1.0; extra == "test"
+Requires-Dist: pytest>=7.2.0; extra == "test"
+Requires-Dist: check-jsonschema; extra == "test"
 Provides-Extra: testinfra
-License-File: LICENSE
+Requires-Dist: pytest-testinfra>=8.1.0; extra == "testinfra"
 
 # About Ansible Molecule
 
 [![PyPI Package](https://img.shields.io/pypi/v/molecule)](https://pypi.org/project/molecule/)
 [![Documentation Status](https://readthedocs.org/projects/molecule/badge/?version=latest)](https://ansible.readthedocs.io/projects/molecule)
 [![image](https://github.com/ansible-community/molecule/workflows/tox/badge.svg)](https://github.com/ansible-community/molecule/actions)
 [![Python Black Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
```

### Comparing `molecule-6.0.2/tools/test-setup.sh` & `molecule-6.0.3/tools/test-setup.sh`

 * *Files identical despite different names*

### Comparing `molecule-6.0.2/tox.ini` & `molecule-6.0.3/tox.ini`

 * *Files 0% similar despite different names*

```diff
@@ -82,16 +82,16 @@
 usedevelop = false
 
 [testenv:docs]
 description = Build documentation
 passenv = *
 usedevelop = true
 commands =
+    linkchecker -f linkcheckerrc docs
     mkdocs build --strict
-    linkchecker -f linkcheckerrc site
 extras =
     docs
 
 [testenv:pkg]
 description =
     Do packaging/distribution. If tag is not present or PEP440 compliant upload to
     PYPI could fail
```

