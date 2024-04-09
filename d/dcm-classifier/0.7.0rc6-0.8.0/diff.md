# Comparing `tmp/dcm_classifier-0.7.0rc6.tar.gz` & `tmp/dcm_classifier-0.8.0.tar.gz`

## Comparing `dcm_classifier-0.7.0rc6.tar` & `dcm_classifier-0.8.0.tar`

### file list

```diff
@@ -1,83 +1,58 @@
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/.pre-commit-config.yaml
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/push_pip.sh
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/requirements.txt
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/requirements_dev.txt
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/.github/ISSUE_TEMPLATE/chore-template.md
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/.github/ISSUE_TEMPLATE/documentation_improvement.md
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/.github/workflows/push_to_main.yml
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/min_req_venv/pyvenv.cfg
--rw-r--r--   0        0        0     9033 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/min_req_venv/bin/Activate.ps1
--rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/min_req_venv/bin/activate
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/min_req_venv/bin/activate.csh
--rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/min_req_venv/bin/activate.fish
--rwxr-xr-x   0        0        0      261 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/min_req_venv/bin/coloredlogs
--rwxr-xr-x   0        0        0      263 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/min_req_venv/bin/f2py
--rwxr-xr-x   0        0        0      317 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/min_req_venv/bin/gdcmanon
--rwxr-xr-x   0        0        0      317 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/min_req_venv/bin/gdcmconv
--rwxr-xr-x   0        0        0      317 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/min_req_venv/bin/gdcmdiff
--rwxr-xr-x   0        0        0      317 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/min_req_venv/bin/gdcmdump
--rwxr-xr-x   0        0        0      317 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/min_req_venv/bin/gdcmgendir
--rwxr-xr-x   0        0        0      317 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/min_req_venv/bin/gdcmimg
--rwxr-xr-x   0        0        0      317 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/min_req_venv/bin/gdcminfo
--rwxr-xr-x   0        0        0      317 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/min_req_venv/bin/gdcmpap3
--rwxr-xr-x   0        0        0      317 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/min_req_venv/bin/gdcmraw
--rwxr-xr-x   0        0        0      317 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/min_req_venv/bin/gdcmscanner
--rwxr-xr-x   0        0        0      317 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/min_req_venv/bin/gdcmscu
--rwxr-xr-x   0        0        0      317 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/min_req_venv/bin/gdcmtar
--rwxr-xr-x   0        0        0      317 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/min_req_venv/bin/gdcmxml
--rwxr-xr-x   0        0        0      263 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/min_req_venv/bin/humanfriendly
--rwxr-xr-x   0        0        0      252 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/min_req_venv/bin/isympy
--rwxr-xr-x   0        0        0      280 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/min_req_venv/bin/onnxruntime_test
--rwxr-xr-x   0        0        0      268 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/min_req_venv/bin/pip
--rwxr-xr-x   0        0        0      268 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/min_req_venv/bin/pip3
--rwxr-xr-x   0        0        0      262 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/min_req_venv/bin/pydicom
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/min_req_venv/bin/python -> python3
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/min_req_venv/bin/python3 -> /usr/bin/python3
--rwxr-xr-x   0        0        0      256 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/min_req_venv/bin/tabulate
--rw-r--r--   0        0        0   312427 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/models/ova_rf_classifier.onnx
--rw-r--r--   0        0        0   197260 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/models/rf_classifier.onnx
--rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/scripts/anonymize_dicom_directory.py
--rw-r--r--   0        0        0     5185 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/scripts/classify_study.py
--rw-r--r--   0        0        0     7627 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/scripts/create_dicom_fields_sheet.py
--rw-r--r--   0        0        0     5519 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/scripts/create_training_sheet.py
--rw-r--r--   0        0        0    17402 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/scripts/dcm-classifier-training-tutorial.ipynb
--rw-r--r--   0        0        0    22366 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/scripts/modality_classifier_training.py
--rw-r--r--   0        0        0     3037 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/scripts/organize_dicom_to_bids.py
--rw-r--r--   0        0        0    11468 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/scripts/orientation_model_training.py
--rwxr-xr-x   0        0        0      934 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/scripts/run_all_dicom_data_sheets.sh
--rw-r--r--   0        0        0    11770 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/scripts/running_classifier.ipynb
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/scripts/todo_list
--rw-r--r--   0        0        0    11826 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/scripts/training_config.py
--rw-r--r--   0        0        0     7348 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/scripts/utilities.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/src/dcm_classifier/README.md
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/src/dcm_classifier/__init__.py
--rw-r--r--   0        0        0     2990 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/src/dcm_classifier/dicom_config.py
--rw-r--r--   0        0        0    11127 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/src/dcm_classifier/dicom_series.py
--rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/src/dcm_classifier/dicom_validator.py
--rw-r--r--   0        0        0    18769 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/src/dcm_classifier/dicom_volume.py
--rw-r--r--   0        0        0    22684 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/src/dcm_classifier/example_image_processing.py
--rw-r--r--   0        0        0    18162 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/src/dcm_classifier/image_type_inference.py
--rw-r--r--   0        0        0    16845 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/src/dcm_classifier/study_processing.py
--rw-r--r--   0        0        0    32251 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/src/dcm_classifier/utility_functions.py
--rw-r--r--   0        0        0   312427 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/src/dcm_classifier/models/ova_rf_classifier.onnx
--rw-r--r--   0        0        0     8871 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/tests/conftest.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/tests/testing_data/.gitignore
--rw-r--r--   0        0        0  2200109 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/tests/testing_data/anonymized_testing_data.tar.gz
--rw-r--r--   0        0        0   190042 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/tests/testing_data/mock_data.txt
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/tests/testing_data/test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/tests/testing_data/dummy_directory/dir_with_one_file/00.file
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/tests/testing_data/dummy_directory/dir_with_two_files/100.file
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/tests/testing_data/dummy_directory/dir_with_two_files/200.file
--rw-r--r--   0        0        0     6901 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/tests/unit_testing/test_dicom_series.py
--rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/tests/unit_testing/test_dicom_validator.py
--rw-r--r--   0        0        0     9894 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/tests/unit_testing/test_dicom_volume.py
--rw-r--r--   0        0        0     4276 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/tests/unit_testing/test_study_processing.py
--rw-r--r--   0        0        0    11309 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/tests/unit_testing/test_utility_functions.py
--rw-r--r--   0        0        0     6694 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/.gitignore
--rw-r--r--   0        0        0    11362 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/LICENSE
--rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/README.md
--rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/pyproject.toml
--rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc6/PKG-INFO
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/.git
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/push_pip.sh
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/requirements.txt
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/requirements_dev.txt
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/.github/ISSUE_TEMPLATE/chore-template.md
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/.github/ISSUE_TEMPLATE/documentation_improvement.md
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/.github/workflows/push_to_main.yml
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/citations/EndNote_citation.enw
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/citations/RIS_citation.ris
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/citations/bib_citation.bib
+-rw-r--r--   0        0        0   312427 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/models/ova_rf_classifier.onnx
+-rw-r--r--   0        0        0   197260 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/models/rf_classifier.onnx
+-rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/scripts/anonymize_dicom_directory.py
+-rw-r--r--   0        0        0     5833 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/scripts/classify_study.py
+-rw-r--r--   0        0        0     7627 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/scripts/create_dicom_fields_sheet.py
+-rw-r--r--   0        0        0     5519 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/scripts/create_training_sheet.py
+-rw-r--r--   0        0        0    17402 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/scripts/dcm-classifier-training-tutorial.ipynb
+-rw-r--r--   0        0        0    22366 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/scripts/modality_classifier_training.py
+-rw-r--r--   0        0        0     3037 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/scripts/organize_dicom_to_bids.py
+-rw-r--r--   0        0        0    11468 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/scripts/orientation_model_training.py
+-rwxr-xr-x   0        0        0      934 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/scripts/run_all_dicom_data_sheets.sh
+-rw-r--r--   0        0        0    21094 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/scripts/running_classifier.ipynb
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/scripts/todo_list
+-rw-r--r--   0        0        0    11826 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/scripts/training_config.py
+-rw-r--r--   0        0        0     7348 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/scripts/utilities.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/src/dcm_classifier/README.md
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/src/dcm_classifier/__init__.py
+-rw-r--r--   0        0        0     2990 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/src/dcm_classifier/dicom_config.py
+-rw-r--r--   0        0        0    11127 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/src/dcm_classifier/dicom_series.py
+-rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/src/dcm_classifier/dicom_validator.py
+-rw-r--r--   0        0        0    18769 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/src/dcm_classifier/dicom_volume.py
+-rw-r--r--   0        0        0    22684 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/src/dcm_classifier/example_image_processing.py
+-rw-r--r--   0        0        0    18085 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/src/dcm_classifier/image_type_inference.py
+-rw-r--r--   0        0        0    16845 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/src/dcm_classifier/study_processing.py
+-rw-r--r--   0        0        0    32251 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/src/dcm_classifier/utility_functions.py
+-rw-r--r--   0        0        0   312427 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/src/dcm_classifier/models/ova_rf_classifier.onnx
+-rw-r--r--   0        0        0     8871 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/tests/conftest.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/tests/testing_data/.gitignore
+-rw-r--r--   0        0        0  2200109 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/tests/testing_data/anonymized_testing_data.tar.gz
+-rw-r--r--   0        0        0   190042 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/tests/testing_data/mock_data.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/tests/testing_data/dummy_directory/dir_with_one_file/00.file
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/tests/testing_data/dummy_directory/dir_with_two_files/100.file
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/tests/testing_data/dummy_directory/dir_with_two_files/200.file
+-rw-r--r--   0        0        0     6901 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/tests/unit_testing/test_dicom_series.py
+-rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/tests/unit_testing/test_dicom_validator.py
+-rw-r--r--   0        0        0     9894 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/tests/unit_testing/test_dicom_volume.py
+-rw-r--r--   0        0        0     4276 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/tests/unit_testing/test_study_processing.py
+-rw-r--r--   0        0        0    11309 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/tests/unit_testing/test_utility_functions.py
+-rw-r--r--   0        0        0     6694 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/.gitignore
+-rw-r--r--   0        0        0    11362 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/LICENSE
+-rw-r--r--   0        0        0     5373 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/README.md
+-rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     6185 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/PKG-INFO
```

### Comparing `dcm_classifier-0.7.0rc6/.pre-commit-config.yaml` & `dcm_classifier-0.8.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc6/.github/PULL_REQUEST_TEMPLATE.md` & `dcm_classifier-0.8.0/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc6/.github/ISSUE_TEMPLATE/bug_report.md` & `dcm_classifier-0.8.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc6/.github/ISSUE_TEMPLATE/documentation_improvement.md` & `dcm_classifier-0.8.0/.github/ISSUE_TEMPLATE/documentation_improvement.md`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc6/.github/ISSUE_TEMPLATE/feature_request.md` & `dcm_classifier-0.8.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc6/.github/workflows/push_to_main.yml` & `dcm_classifier-0.8.0/.github/workflows/push_to_main.yml`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc6/models/ova_rf_classifier.onnx` & `dcm_classifier-0.8.0/models/ova_rf_classifier.onnx`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc6/models/rf_classifier.onnx` & `dcm_classifier-0.8.0/models/rf_classifier.onnx`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc6/scripts/anonymize_dicom_directory.py` & `dcm_classifier-0.8.0/scripts/anonymize_dicom_directory.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc6/scripts/classify_study.py` & `dcm_classifier-0.8.0/scripts/classify_study.py`

 * *Files 7% similar despite different names*

```diff
@@ -77,21 +77,40 @@
     list_of_probabilities: list[pd.DataFrame] = []
     list_of_dictionaries: list[dict[str, str]] = []
 
     for series_number, series in study.series_dictionary.items():
         for index, volume in enumerate(series.get_volume_list()):
             current_dict: dict[str, str] = ordered_dict()
             current_dict["Series#"] = str(series_number)
-            current_dict["Vol.#"] = str(volume.get_volume_index())
-            current_dict["Volume Modality"] = str(volume.get_volume_modality())
-            current_dict["Series Modality"] = str(series.get_series_modality())
-            current_dict["Acq.Plane"] = str(volume.get_acquisition_plane())
-            current_dict["Isotropic"] = str(volume.get_is_isotropic())
+            try:
+                current_dict["Vol.#"] = str(volume.get_volume_index())
+            except AttributeError:
+                current_dict["Vol.#"] = "None"
+            try:
+                current_dict["Volume Modality"] = str(volume.get_volume_modality())
+            except AttributeError:
+                current_dict["Volume Modality"] = "None"
+            try:
+                current_dict["Series Modality"] = str(series.get_series_modality())
+            except AttributeError:
+                current_dict["Series Modality"] = "None"
+            try:
+                current_dict["Acq.Plane"] = str(volume.get_acquisition_plane())
+            except AttributeError:
+                current_dict["Acq.Plane"] = "None"
+            try:
+                current_dict["Isotropic"] = str(volume.get_is_isotropic())
+            except AttributeError:
+                current_dict["Isotropic"] = "None"
+
             print(volume.get_modality_probabilities().to_string(index=False))
-            current_dict["Bvalue"] = str(volume.get_volume_bvalue())
+            try:
+                current_dict["Bvalue"] = str(volume.get_volume_bvalue())
+            except AttributeError:
+                current_dict["Bvalue"] = "None"
             try:
                 current_dict["SeriesDesc"] = volume.get_volume_series_description()
             except AttributeError:
                 current_dict["SeriesDesc"] = "None"
             inputs_df: dict[str, Any] = volume.get_volume_dictionary()
             current_dict["ImageType"] = str(inputs_df.get("ImageType", "Unknown"))
             for unwanted in [
```

### Comparing `dcm_classifier-0.7.0rc6/scripts/create_dicom_fields_sheet.py` & `dcm_classifier-0.8.0/scripts/create_dicom_fields_sheet.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc6/scripts/create_training_sheet.py` & `dcm_classifier-0.8.0/scripts/create_training_sheet.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc6/scripts/dcm-classifier-training-tutorial.ipynb` & `dcm_classifier-0.8.0/scripts/dcm-classifier-training-tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc6/scripts/modality_classifier_training.py` & `dcm_classifier-0.8.0/scripts/modality_classifier_training.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc6/scripts/organize_dicom_to_bids.py` & `dcm_classifier-0.8.0/scripts/organize_dicom_to_bids.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc6/scripts/orientation_model_training.py` & `dcm_classifier-0.8.0/scripts/orientation_model_training.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc6/scripts/run_all_dicom_data_sheets.sh` & `dcm_classifier-0.8.0/scripts/run_all_dicom_data_sheets.sh`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc6/scripts/todo_list` & `dcm_classifier-0.8.0/scripts/todo_list`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc6/scripts/training_config.py` & `dcm_classifier-0.8.0/scripts/training_config.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc6/scripts/utilities.py` & `dcm_classifier-0.8.0/scripts/utilities.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc6/src/dcm_classifier/dicom_config.py` & `dcm_classifier-0.8.0/src/dcm_classifier/dicom_config.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc6/src/dcm_classifier/dicom_series.py` & `dcm_classifier-0.8.0/src/dcm_classifier/dicom_series.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc6/src/dcm_classifier/dicom_validator.py` & `dcm_classifier-0.8.0/src/dcm_classifier/dicom_validator.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc6/src/dcm_classifier/dicom_volume.py` & `dcm_classifier-0.8.0/src/dcm_classifier/dicom_volume.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc6/src/dcm_classifier/example_image_processing.py` & `dcm_classifier-0.8.0/src/dcm_classifier/example_image_processing.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc6/src/dcm_classifier/image_type_inference.py` & `dcm_classifier-0.8.0/src/dcm_classifier/image_type_inference.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,15 @@
         Args:
             classification_model_filename (Union[str, Path]): Path to the classification model file (base implementation requires ONNX file).
             classification_feature_list (List[str]): List of features used for classification.
             image_type_map (Dict[str, str]): Mapping between class name and model integer output.
             mode (str): "series" or "volume" to run inference on series or volume level (a series could have multiple subvolumes).
             min_probability_threshold (float): Minimum probability threshold for classification, defaults to 0.4. If maximum class probability is below this threshold, the image type is set to "unknown".
         """
-        print("classification_model_filename", classification_model_filename)
+
         self.classification_model_filename: str | Path = Path(
             classification_model_filename
         )
         self.classification_feature_list: list[str] = classification_feature_list
         self.imagetype_to_int_map: dict[str, int] = image_type_map
         self.int_to_imagetype_map: dict[int, str] = self.get_int_to_type_map()
         self.min_probability_threshold: float = min_probability_threshold
```

### Comparing `dcm_classifier-0.7.0rc6/src/dcm_classifier/study_processing.py` & `dcm_classifier-0.8.0/src/dcm_classifier/study_processing.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc6/src/dcm_classifier/utility_functions.py` & `dcm_classifier-0.8.0/src/dcm_classifier/utility_functions.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc6/src/dcm_classifier/models/ova_rf_classifier.onnx` & `dcm_classifier-0.8.0/src/dcm_classifier/models/ova_rf_classifier.onnx`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc6/tests/conftest.py` & `dcm_classifier-0.8.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc6/tests/testing_data/anonymized_testing_data.tar.gz` & `dcm_classifier-0.8.0/tests/testing_data/anonymized_testing_data.tar.gz`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc6/tests/testing_data/mock_data.txt` & `dcm_classifier-0.8.0/tests/testing_data/mock_data.txt`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc6/tests/unit_testing/test_dicom_series.py` & `dcm_classifier-0.8.0/tests/unit_testing/test_dicom_series.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc6/tests/unit_testing/test_dicom_validator.py` & `dcm_classifier-0.8.0/tests/unit_testing/test_dicom_validator.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc6/tests/unit_testing/test_dicom_volume.py` & `dcm_classifier-0.8.0/tests/unit_testing/test_dicom_volume.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc6/tests/unit_testing/test_study_processing.py` & `dcm_classifier-0.8.0/tests/unit_testing/test_study_processing.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc6/tests/unit_testing/test_utility_functions.py` & `dcm_classifier-0.8.0/tests/unit_testing/test_utility_functions.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc6/.gitignore` & `dcm_classifier-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc6/LICENSE` & `dcm_classifier-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc6/pyproject.toml` & `dcm_classifier-0.8.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "dcm_classifier"
-version = '0.7.0.rc6'
+version = '0.8.0'
 authors = [
   { name="Michal Brzus", email="michal-brzus@uiowa.edu" },
   { name="Hans Johnson", email="hans-johnson@uiowa.edu" },
+  { name="Cavan Riley", email="cavan-riley@uiowa.edu" },
 ]
 description = "This is a consolidation of work from NAMIC efforts primarily at the University of Iowa."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
```

