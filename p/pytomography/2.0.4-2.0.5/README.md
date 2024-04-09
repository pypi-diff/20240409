# Comparing `tmp/pytomography-2.0.4.tar.gz` & `tmp/pytomography-2.0.5.tar.gz`

## Comparing `pytomography-2.0.4.tar` & `pytomography-2.0.5.tar`

### file list

```diff
@@ -1,129 +1,129 @@
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 pytomography-2.0.4/.readthedocs.yaml
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 pytomography-2.0.4/.github/workflows/publish-to-test-pypi.yml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 pytomography-2.0.4/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 pytomography-2.0.4/docs/make.bat
--rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 pytomography-2.0.4/docs/source/conf.py
--rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 pytomography-2.0.4/docs/source/developers_guide.md
--rw-r--r--   0        0        0     8291 2020-02-02 00:00:00.000000 pytomography-2.0.4/docs/source/external_data.md
--rw-r--r--   0        0        0     4473 2020-02-02 00:00:00.000000 pytomography-2.0.4/docs/source/index.md
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 pytomography-2.0.4/docs/source/usage.md
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 pytomography-2.0.4/docs/source/_templates/autoapi/index.rst
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 pytomography-2.0.4/docs/source/_templates/autoapi/python/attribute.rst
--rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 pytomography-2.0.4/docs/source/_templates/autoapi/python/class.rst
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 pytomography-2.0.4/docs/source/_templates/autoapi/python/data.rst
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 pytomography-2.0.4/docs/source/_templates/autoapi/python/exception.rst
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 pytomography-2.0.4/docs/source/_templates/autoapi/python/function.rst
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 pytomography-2.0.4/docs/source/_templates/autoapi/python/method.rst
--rw-r--r--   0        0        0     2424 2020-02-02 00:00:00.000000 pytomography-2.0.4/docs/source/_templates/autoapi/python/module.rst
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 pytomography-2.0.4/docs/source/_templates/autoapi/python/package.rst
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 pytomography-2.0.4/docs/source/_templates/autoapi/python/property.rst
--rw-r--r--   0        0        0   489349 2020-02-02 00:00:00.000000 pytomography-2.0.4/docs/source/images/PT1.png
--rw-r--r--   0        0        0   275608 2020-02-02 00:00:00.000000 pytomography-2.0.4/docs/source/images/coordinate_conventions.png
--rw-r--r--   0        0        0    37985 2020-02-02 00:00:00.000000 pytomography-2.0.4/docs/source/images/emission.png
--rw-r--r--   0        0        0   347262 2020-02-02 00:00:00.000000 pytomography-2.0.4/docs/source/images/figure4.jpg
--rw-r--r--   0        0        0  1799116 2020-02-02 00:00:00.000000 pytomography-2.0.4/docs/source/images/figure5.jpg
--rw-r--r--   0        0        0    44334 2020-02-02 00:00:00.000000 pytomography-2.0.4/docs/source/images/psf.png
--rw-r--r--   0        0        0    79798 2020-02-02 00:00:00.000000 pytomography-2.0.4/docs/source/images/psf2.png
--rw-r--r--   0        0        0    95998 2020-02-02 00:00:00.000000 pytomography-2.0.4/docs/source/images/pytomo_front_title.png
--rw-r--r--   0        0        0   115913 2020-02-02 00:00:00.000000 pytomography-2.0.4/docs/source/images/sample_MIP.png
--rw-r--r--   0        0        0   115388 2020-02-02 00:00:00.000000 pytomography-2.0.4/docs/source/images/sample_MIPa.png
--rw-r--r--   0        0        0    17745 2020-02-02 00:00:00.000000 pytomography-2.0.4/docs/source/notebooks/conventions.ipynb
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 pytomography-2.0.4/docs/source/notebooks/script_to_generate_eta_for_petsird.py
--rw-r--r--   0        0        0   104099 2020-02-02 00:00:00.000000 pytomography-2.0.4/docs/source/notebooks/t_PETGATE.ipynb
--rw-r--r--   0        0        0    51834 2020-02-02 00:00:00.000000 pytomography-2.0.4/docs/source/notebooks/t_PETSIRD.ipynb
--rw-r--r--   0        0        0    97562 2020-02-02 00:00:00.000000 pytomography-2.0.4/docs/source/notebooks/t_dicomdata.ipynb
--rw-r--r--   0        0        0   218952 2020-02-02 00:00:00.000000 pytomography-2.0.4/docs/source/notebooks/t_dicommultibed.ipynb
--rw-r--r--   0        0        0   146023 2020-02-02 00:00:00.000000 pytomography-2.0.4/docs/source/notebooks/t_fbp.ipynb
--rw-r--r--   0        0        0   199250 2020-02-02 00:00:00.000000 pytomography-2.0.4/docs/source/notebooks/t_quantitative.ipynb
--rw-r--r--   0        0        0   987989 2020-02-02 00:00:00.000000 pytomography-2.0.4/docs/source/notebooks/t_siminddata.ipynb
--rw-r--r--   0        0        0    86315 2020-02-02 00:00:00.000000 pytomography-2.0.4/docs/source/notebooks/t_uncertainty_spect.ipynb
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/__init__.py
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/algorithms/__init__.py
--rw-r--r--   0        0        0     4424 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/algorithms/dip_recon.py
--rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/algorithms/fbp.py
--rw-r--r--   0        0        0    32430 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/algorithms/preconditioned_gradient_ascent.py
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/callbacks/__init__.py
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/callbacks/callback.py
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/callbacks/data_saving.py
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/callbacks/likelihood.py
--rw-r--r--   0        0        0    15700 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/data/collim.col
--rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/data/NIST_attenuation_data/adipose.csv
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/data/NIST_attenuation_data/air.csv
--rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/data/NIST_attenuation_data/aluminum.csv
--rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/data/NIST_attenuation_data/bonecortical.csv
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/data/NIST_attenuation_data/boneequivplastic.csv
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/data/NIST_attenuation_data/breast.csv
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/data/NIST_attenuation_data/lead.csv
--rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/data/NIST_attenuation_data/lungtissue.csv
--rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/data/NIST_attenuation_data/muscle.csv
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/data/NIST_attenuation_data/tissueequivplastic.csv
--rw-r--r--   0        0        0     2252 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/data/NIST_attenuation_data/tungsten.csv
--rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/data/NIST_attenuation_data/water.csv
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/io/__init__.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/io/CT/__init__.py
--rw-r--r--   0        0        0     6746 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/io/CT/attenuation_map.py
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/io/PET/__init__.py
--rw-r--r--   0        0        0    20320 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/io/PET/gate.py
--rw-r--r--   0        0        0     4951 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/io/PET/petsird.py
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/io/PET/prd/__init__.py
--rw-r--r--   0        0        0    46593 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/io/PET/prd/_binary.py
--rw-r--r--   0        0        0     3352 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/io/PET/prd/_dtypes.py
--rw-r--r--   0        0        0    39753 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/io/PET/prd/_ndjson.py
--rw-r--r--   0        0        0    11577 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/io/PET/prd/binary.py
--rw-r--r--   0        0        0    29567 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/io/PET/prd/ndjson.py
--rw-r--r--   0        0        0     7190 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/io/PET/prd/protocols.py
--rw-r--r--   0        0        0    15398 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/io/PET/prd/types.py
--rw-r--r--   0        0        0     9563 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/io/PET/prd/yardl_types.py
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/io/SPECT/__init__.py
--rw-r--r--   0        0        0    27509 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/io/SPECT/dicom.py
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/io/SPECT/shared.py
--rw-r--r--   0        0        0    11979 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/io/SPECT/simind.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/io/shared/__init__.py
--rw-r--r--   0        0        0     4157 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/io/shared/dicom.py
--rw-r--r--   0        0        0     5555 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/io/shared/dicom_creation.py
--rw-r--r--   0        0        0     2791 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/io/shared/interfile.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/likelihoods/__init__.py
--rw-r--r--   0        0        0     3712 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/likelihoods/likelihood.py
--rw-r--r--   0        0        0     4011 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/likelihoods/mse_objective.py
--rw-r--r--   0        0        0     6290 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/likelihoods/poisson_log_likelihood.py
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/metadata/__init__.py
--rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/metadata/metadata.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/metadata/PET/__init__.py
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/metadata/PET/pet_tof_metadata.py
--rw-r--r--   0        0        0     3308 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/metadata/PET/petlm_metadata.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/metadata/SPECT/__init__.py
--rw-r--r--   0        0        0     4678 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/metadata/SPECT/spect_metadata.py
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/priors/__init__.py
--rw-r--r--   0        0        0    16142 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/priors/nearest_neighbour.py
--rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/priors/prior.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/projectors/__init__.py
--rw-r--r--   0        0        0    10401 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/projectors/system_matrix.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/projectors/PET/__init__.py
--rw-r--r--   0        0        0    16250 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/projectors/PET/petlm_system_matrix.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/projectors/SPECT/__init__.py
--rw-r--r--   0        0        0    19516 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/projectors/SPECT/spect_system_matrix.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/projectors/shared/__init__.py
--rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/projectors/shared/kem_system_matrix.py
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/projectors/shared/motion_correction_system_matrix.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/transforms/__init__.py
--rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/transforms/transform.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/transforms/SPECT/__init__.py
--rw-r--r--   0        0        0     6411 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/transforms/SPECT/attenuation.py
--rw-r--r--   0        0        0     2940 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/transforms/SPECT/cutoff.py
--rw-r--r--   0        0        0    14373 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/transforms/SPECT/psf.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/transforms/shared/__init__.py
--rw-r--r--   0        0        0     2976 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/transforms/shared/filters.py
--rw-r--r--   0        0        0     7245 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/transforms/shared/kem.py
--rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/transforms/shared/motion.py
--rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/transforms/shared/spatial.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/utils/__init__.py
--rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/utils/fourier_filters.py
--rw-r--r--   0        0        0     3928 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/utils/misc.py
--rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/utils/nist_data.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/utils/scatter.py
--rw-r--r--   0        0        0     5891 2020-02-02 00:00:00.000000 pytomography-2.0.4/src/pytomography/utils/spatial.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 pytomography-2.0.4/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 pytomography-2.0.4/LICENSE
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 pytomography-2.0.4/README.md
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 pytomography-2.0.4/pyproject.toml
--rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 pytomography-2.0.4/PKG-INFO
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 pytomography-2.0.5/.readthedocs.yaml
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 pytomography-2.0.5/.github/workflows/publish-to-test-pypi.yml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 pytomography-2.0.5/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 pytomography-2.0.5/docs/make.bat
+-rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 pytomography-2.0.5/docs/source/conf.py
+-rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 pytomography-2.0.5/docs/source/developers_guide.md
+-rw-r--r--   0        0        0     8291 2020-02-02 00:00:00.000000 pytomography-2.0.5/docs/source/external_data.md
+-rw-r--r--   0        0        0     4473 2020-02-02 00:00:00.000000 pytomography-2.0.5/docs/source/index.md
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 pytomography-2.0.5/docs/source/usage.md
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 pytomography-2.0.5/docs/source/_templates/autoapi/index.rst
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 pytomography-2.0.5/docs/source/_templates/autoapi/python/attribute.rst
+-rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 pytomography-2.0.5/docs/source/_templates/autoapi/python/class.rst
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 pytomography-2.0.5/docs/source/_templates/autoapi/python/data.rst
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 pytomography-2.0.5/docs/source/_templates/autoapi/python/exception.rst
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 pytomography-2.0.5/docs/source/_templates/autoapi/python/function.rst
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 pytomography-2.0.5/docs/source/_templates/autoapi/python/method.rst
+-rw-r--r--   0        0        0     2424 2020-02-02 00:00:00.000000 pytomography-2.0.5/docs/source/_templates/autoapi/python/module.rst
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 pytomography-2.0.5/docs/source/_templates/autoapi/python/package.rst
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 pytomography-2.0.5/docs/source/_templates/autoapi/python/property.rst
+-rw-r--r--   0        0        0   489349 2020-02-02 00:00:00.000000 pytomography-2.0.5/docs/source/images/PT1.png
+-rw-r--r--   0        0        0   275608 2020-02-02 00:00:00.000000 pytomography-2.0.5/docs/source/images/coordinate_conventions.png
+-rw-r--r--   0        0        0    37985 2020-02-02 00:00:00.000000 pytomography-2.0.5/docs/source/images/emission.png
+-rw-r--r--   0        0        0   347262 2020-02-02 00:00:00.000000 pytomography-2.0.5/docs/source/images/figure4.jpg
+-rw-r--r--   0        0        0  1799116 2020-02-02 00:00:00.000000 pytomography-2.0.5/docs/source/images/figure5.jpg
+-rw-r--r--   0        0        0    44334 2020-02-02 00:00:00.000000 pytomography-2.0.5/docs/source/images/psf.png
+-rw-r--r--   0        0        0    79798 2020-02-02 00:00:00.000000 pytomography-2.0.5/docs/source/images/psf2.png
+-rw-r--r--   0        0        0    95998 2020-02-02 00:00:00.000000 pytomography-2.0.5/docs/source/images/pytomo_front_title.png
+-rw-r--r--   0        0        0   115913 2020-02-02 00:00:00.000000 pytomography-2.0.5/docs/source/images/sample_MIP.png
+-rw-r--r--   0        0        0   115388 2020-02-02 00:00:00.000000 pytomography-2.0.5/docs/source/images/sample_MIPa.png
+-rw-r--r--   0        0        0    17745 2020-02-02 00:00:00.000000 pytomography-2.0.5/docs/source/notebooks/conventions.ipynb
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 pytomography-2.0.5/docs/source/notebooks/script_to_generate_eta_for_petsird.py
+-rw-r--r--   0        0        0   104099 2020-02-02 00:00:00.000000 pytomography-2.0.5/docs/source/notebooks/t_PETGATE.ipynb
+-rw-r--r--   0        0        0    51834 2020-02-02 00:00:00.000000 pytomography-2.0.5/docs/source/notebooks/t_PETSIRD.ipynb
+-rw-r--r--   0        0        0    97562 2020-02-02 00:00:00.000000 pytomography-2.0.5/docs/source/notebooks/t_dicomdata.ipynb
+-rw-r--r--   0        0        0   218952 2020-02-02 00:00:00.000000 pytomography-2.0.5/docs/source/notebooks/t_dicommultibed.ipynb
+-rw-r--r--   0        0        0   146023 2020-02-02 00:00:00.000000 pytomography-2.0.5/docs/source/notebooks/t_fbp.ipynb
+-rw-r--r--   0        0        0   199250 2020-02-02 00:00:00.000000 pytomography-2.0.5/docs/source/notebooks/t_quantitative.ipynb
+-rw-r--r--   0        0        0   987989 2020-02-02 00:00:00.000000 pytomography-2.0.5/docs/source/notebooks/t_siminddata.ipynb
+-rw-r--r--   0        0        0    86315 2020-02-02 00:00:00.000000 pytomography-2.0.5/docs/source/notebooks/t_uncertainty_spect.ipynb
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/__init__.py
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/algorithms/__init__.py
+-rw-r--r--   0        0        0     4424 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/algorithms/dip_recon.py
+-rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/algorithms/fbp.py
+-rw-r--r--   0        0        0    32430 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/algorithms/preconditioned_gradient_ascent.py
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/callbacks/__init__.py
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/callbacks/callback.py
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/callbacks/data_saving.py
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/callbacks/likelihood.py
+-rw-r--r--   0        0        0    15700 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/data/collim.col
+-rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/data/NIST_attenuation_data/adipose.csv
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/data/NIST_attenuation_data/air.csv
+-rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/data/NIST_attenuation_data/aluminum.csv
+-rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/data/NIST_attenuation_data/bonecortical.csv
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/data/NIST_attenuation_data/boneequivplastic.csv
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/data/NIST_attenuation_data/breast.csv
+-rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/data/NIST_attenuation_data/lead.csv
+-rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/data/NIST_attenuation_data/lungtissue.csv
+-rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/data/NIST_attenuation_data/muscle.csv
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/data/NIST_attenuation_data/tissueequivplastic.csv
+-rw-r--r--   0        0        0     2252 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/data/NIST_attenuation_data/tungsten.csv
+-rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/data/NIST_attenuation_data/water.csv
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/io/__init__.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/io/CT/__init__.py
+-rw-r--r--   0        0        0     6746 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/io/CT/attenuation_map.py
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/io/PET/__init__.py
+-rw-r--r--   0        0        0    20320 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/io/PET/gate.py
+-rw-r--r--   0        0        0     4951 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/io/PET/petsird.py
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/io/PET/prd/__init__.py
+-rw-r--r--   0        0        0    46593 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/io/PET/prd/_binary.py
+-rw-r--r--   0        0        0     3352 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/io/PET/prd/_dtypes.py
+-rw-r--r--   0        0        0    39753 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/io/PET/prd/_ndjson.py
+-rw-r--r--   0        0        0    11577 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/io/PET/prd/binary.py
+-rw-r--r--   0        0        0    29567 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/io/PET/prd/ndjson.py
+-rw-r--r--   0        0        0     7190 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/io/PET/prd/protocols.py
+-rw-r--r--   0        0        0    15398 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/io/PET/prd/types.py
+-rw-r--r--   0        0        0     9563 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/io/PET/prd/yardl_types.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/io/SPECT/__init__.py
+-rw-r--r--   0        0        0    27516 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/io/SPECT/dicom.py
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/io/SPECT/shared.py
+-rw-r--r--   0        0        0    11979 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/io/SPECT/simind.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/io/shared/__init__.py
+-rw-r--r--   0        0        0     4157 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/io/shared/dicom.py
+-rw-r--r--   0        0        0     5555 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/io/shared/dicom_creation.py
+-rw-r--r--   0        0        0     2791 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/io/shared/interfile.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/likelihoods/__init__.py
+-rw-r--r--   0        0        0     3712 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/likelihoods/likelihood.py
+-rw-r--r--   0        0        0     4011 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/likelihoods/mse_objective.py
+-rw-r--r--   0        0        0     6290 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/likelihoods/poisson_log_likelihood.py
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/metadata/__init__.py
+-rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/metadata/metadata.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/metadata/PET/__init__.py
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/metadata/PET/pet_tof_metadata.py
+-rw-r--r--   0        0        0     3308 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/metadata/PET/petlm_metadata.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/metadata/SPECT/__init__.py
+-rw-r--r--   0        0        0     4678 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/metadata/SPECT/spect_metadata.py
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/priors/__init__.py
+-rw-r--r--   0        0        0    16142 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/priors/nearest_neighbour.py
+-rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/priors/prior.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/projectors/__init__.py
+-rw-r--r--   0        0        0    10401 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/projectors/system_matrix.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/projectors/PET/__init__.py
+-rw-r--r--   0        0        0    16250 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/projectors/PET/petlm_system_matrix.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/projectors/SPECT/__init__.py
+-rw-r--r--   0        0        0    19516 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/projectors/SPECT/spect_system_matrix.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/projectors/shared/__init__.py
+-rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/projectors/shared/kem_system_matrix.py
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/projectors/shared/motion_correction_system_matrix.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/transforms/__init__.py
+-rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/transforms/transform.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/transforms/SPECT/__init__.py
+-rw-r--r--   0        0        0     6411 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/transforms/SPECT/attenuation.py
+-rw-r--r--   0        0        0     2940 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/transforms/SPECT/cutoff.py
+-rw-r--r--   0        0        0    14373 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/transforms/SPECT/psf.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/transforms/shared/__init__.py
+-rw-r--r--   0        0        0     2976 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/transforms/shared/filters.py
+-rw-r--r--   0        0        0     7245 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/transforms/shared/kem.py
+-rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/transforms/shared/motion.py
+-rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/transforms/shared/spatial.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/utils/__init__.py
+-rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/utils/fourier_filters.py
+-rw-r--r--   0        0        0     3928 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/utils/misc.py
+-rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/utils/nist_data.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/utils/scatter.py
+-rw-r--r--   0        0        0     5891 2020-02-02 00:00:00.000000 pytomography-2.0.5/src/pytomography/utils/spatial.py
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 pytomography-2.0.5/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 pytomography-2.0.5/LICENSE
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 pytomography-2.0.5/README.md
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 pytomography-2.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 pytomography-2.0.5/PKG-INFO
```

### Comparing `pytomography-2.0.4/.github/workflows/publish-to-test-pypi.yml` & `pytomography-2.0.5/.github/workflows/publish-to-test-pypi.yml`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/docs/Makefile` & `pytomography-2.0.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/docs/make.bat` & `pytomography-2.0.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/docs/source/conf.py` & `pytomography-2.0.5/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/docs/source/developers_guide.md` & `pytomography-2.0.5/docs/source/developers_guide.md`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/docs/source/external_data.md` & `pytomography-2.0.5/docs/source/external_data.md`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/docs/source/index.md` & `pytomography-2.0.5/docs/source/index.md`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/docs/source/usage.md` & `pytomography-2.0.5/docs/source/usage.md`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/docs/source/_templates/autoapi/python/class.rst` & `pytomography-2.0.5/docs/source/_templates/autoapi/python/class.rst`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/docs/source/_templates/autoapi/python/data.rst` & `pytomography-2.0.5/docs/source/_templates/autoapi/python/data.rst`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/docs/source/_templates/autoapi/python/function.rst` & `pytomography-2.0.5/docs/source/_templates/autoapi/python/function.rst`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/docs/source/_templates/autoapi/python/method.rst` & `pytomography-2.0.5/docs/source/_templates/autoapi/python/method.rst`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/docs/source/_templates/autoapi/python/module.rst` & `pytomography-2.0.5/docs/source/_templates/autoapi/python/module.rst`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/docs/source/images/PT1.png` & `pytomography-2.0.5/docs/source/images/PT1.png`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/docs/source/images/coordinate_conventions.png` & `pytomography-2.0.5/docs/source/images/coordinate_conventions.png`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/docs/source/images/emission.png` & `pytomography-2.0.5/docs/source/images/emission.png`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/docs/source/images/figure4.jpg` & `pytomography-2.0.5/docs/source/images/figure4.jpg`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/docs/source/images/figure5.jpg` & `pytomography-2.0.5/docs/source/images/figure5.jpg`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/docs/source/images/psf.png` & `pytomography-2.0.5/docs/source/images/psf.png`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/docs/source/images/psf2.png` & `pytomography-2.0.5/docs/source/images/psf2.png`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/docs/source/images/pytomo_front_title.png` & `pytomography-2.0.5/docs/source/images/pytomo_front_title.png`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/docs/source/images/sample_MIP.png` & `pytomography-2.0.5/docs/source/images/sample_MIP.png`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/docs/source/images/sample_MIPa.png` & `pytomography-2.0.5/docs/source/images/sample_MIPa.png`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/docs/source/notebooks/conventions.ipynb` & `pytomography-2.0.5/docs/source/notebooks/conventions.ipynb`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/docs/source/notebooks/t_PETGATE.ipynb` & `pytomography-2.0.5/docs/source/notebooks/t_PETGATE.ipynb`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/docs/source/notebooks/t_PETSIRD.ipynb` & `pytomography-2.0.5/docs/source/notebooks/t_PETSIRD.ipynb`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/docs/source/notebooks/t_dicomdata.ipynb` & `pytomography-2.0.5/docs/source/notebooks/t_dicomdata.ipynb`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/docs/source/notebooks/t_dicommultibed.ipynb` & `pytomography-2.0.5/docs/source/notebooks/t_dicommultibed.ipynb`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/docs/source/notebooks/t_fbp.ipynb` & `pytomography-2.0.5/docs/source/notebooks/t_fbp.ipynb`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/docs/source/notebooks/t_quantitative.ipynb` & `pytomography-2.0.5/docs/source/notebooks/t_quantitative.ipynb`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/docs/source/notebooks/t_siminddata.ipynb` & `pytomography-2.0.5/docs/source/notebooks/t_siminddata.ipynb`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/docs/source/notebooks/t_uncertainty_spect.ipynb` & `pytomography-2.0.5/docs/source/notebooks/t_uncertainty_spect.ipynb`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/src/pytomography/__init__.py` & `pytomography-2.0.5/src/pytomography/__init__.py`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/src/pytomography/algorithms/dip_recon.py` & `pytomography-2.0.5/src/pytomography/algorithms/dip_recon.py`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/src/pytomography/algorithms/fbp.py` & `pytomography-2.0.5/src/pytomography/algorithms/fbp.py`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/src/pytomography/algorithms/preconditioned_gradient_ascent.py` & `pytomography-2.0.5/src/pytomography/algorithms/preconditioned_gradient_ascent.py`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/src/pytomography/callbacks/__init__.py` & `pytomography-2.0.5/src/pytomography/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/src/pytomography/callbacks/callback.py` & `pytomography-2.0.5/src/pytomography/callbacks/callback.py`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/src/pytomography/callbacks/data_saving.py` & `pytomography-2.0.5/src/pytomography/callbacks/data_saving.py`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/src/pytomography/callbacks/likelihood.py` & `pytomography-2.0.5/src/pytomography/callbacks/likelihood.py`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/src/pytomography/data/collim.col` & `pytomography-2.0.5/src/pytomography/data/collim.col`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/src/pytomography/data/NIST_attenuation_data/adipose.csv` & `pytomography-2.0.5/src/pytomography/data/NIST_attenuation_data/adipose.csv`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/src/pytomography/data/NIST_attenuation_data/air.csv` & `pytomography-2.0.5/src/pytomography/data/NIST_attenuation_data/air.csv`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/src/pytomography/data/NIST_attenuation_data/aluminum.csv` & `pytomography-2.0.5/src/pytomography/data/NIST_attenuation_data/aluminum.csv`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/src/pytomography/data/NIST_attenuation_data/bonecortical.csv` & `pytomography-2.0.5/src/pytomography/data/NIST_attenuation_data/bonecortical.csv`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/src/pytomography/data/NIST_attenuation_data/boneequivplastic.csv` & `pytomography-2.0.5/src/pytomography/data/NIST_attenuation_data/boneequivplastic.csv`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/src/pytomography/data/NIST_attenuation_data/breast.csv` & `pytomography-2.0.5/src/pytomography/data/NIST_attenuation_data/breast.csv`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/src/pytomography/data/NIST_attenuation_data/lead.csv` & `pytomography-2.0.5/src/pytomography/data/NIST_attenuation_data/lead.csv`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/src/pytomography/data/NIST_attenuation_data/lungtissue.csv` & `pytomography-2.0.5/src/pytomography/data/NIST_attenuation_data/lungtissue.csv`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/src/pytomography/data/NIST_attenuation_data/muscle.csv` & `pytomography-2.0.5/src/pytomography/data/NIST_attenuation_data/muscle.csv`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/src/pytomography/data/NIST_attenuation_data/tissueequivplastic.csv` & `pytomography-2.0.5/src/pytomography/data/NIST_attenuation_data/tissueequivplastic.csv`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/src/pytomography/data/NIST_attenuation_data/tungsten.csv` & `pytomography-2.0.5/src/pytomography/data/NIST_attenuation_data/tungsten.csv`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/src/pytomography/data/NIST_attenuation_data/water.csv` & `pytomography-2.0.5/src/pytomography/data/NIST_attenuation_data/water.csv`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/src/pytomography/io/CT/attenuation_map.py` & `pytomography-2.0.5/src/pytomography/io/CT/attenuation_map.py`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/src/pytomography/io/PET/__init__.py` & `pytomography-2.0.5/src/pytomography/io/PET/__init__.py`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/src/pytomography/io/PET/gate.py` & `pytomography-2.0.5/src/pytomography/io/PET/gate.py`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/src/pytomography/io/PET/petsird.py` & `pytomography-2.0.5/src/pytomography/io/PET/petsird.py`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/src/pytomography/io/PET/prd/__init__.py` & `pytomography-2.0.5/src/pytomography/io/PET/prd/__init__.py`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/src/pytomography/io/PET/prd/_binary.py` & `pytomography-2.0.5/src/pytomography/io/PET/prd/_binary.py`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/src/pytomography/io/PET/prd/_dtypes.py` & `pytomography-2.0.5/src/pytomography/io/PET/prd/_dtypes.py`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/src/pytomography/io/PET/prd/_ndjson.py` & `pytomography-2.0.5/src/pytomography/io/PET/prd/_ndjson.py`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/src/pytomography/io/PET/prd/binary.py` & `pytomography-2.0.5/src/pytomography/io/PET/prd/binary.py`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/src/pytomography/io/PET/prd/ndjson.py` & `pytomography-2.0.5/src/pytomography/io/PET/prd/ndjson.py`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/src/pytomography/io/PET/prd/protocols.py` & `pytomography-2.0.5/src/pytomography/io/PET/prd/protocols.py`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/src/pytomography/io/PET/prd/types.py` & `pytomography-2.0.5/src/pytomography/io/PET/prd/types.py`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/src/pytomography/io/PET/prd/yardl_types.py` & `pytomography-2.0.5/src/pytomography/io/PET/prd/yardl_types.py`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/src/pytomography/io/SPECT/dicom.py` & `pytomography-2.0.5/src/pytomography/io/SPECT/dicom.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 import warnings
+import copy
 import os
 import collections.abc
 from collections.abc import Sequence
 from pathlib import Path
 from typing import Sequence
 import numpy as np
 import numpy.linalg as npl
@@ -570,20 +571,21 @@
     Args:
         object (torch.Tensor): Reconstructed object of shape [1,Lx,Ly,Lz].
         save_path (str): Location of folder where to save the DICOM output files.
         file_NM (str): File path of the projection data corresponding to the reconstruction.
         recon_name (str): Type of reconstruction performed. Obtained from the `recon_method_str` attribute of a reconstruction algorithm class.
         return_ds (bool): If true, returns the DICOM dataset objects instead of saving to file. Defaults to False.
     """
-    try:
-        Path(save_path).resolve().mkdir(parents=True, exist_ok=False)
-    except:
-        raise Exception(
-            f"Folder {save_path} already exists; new folder name is required."
-        )
+    if not return_ds:
+        try:
+            Path(save_path).resolve().mkdir(parents=True, exist_ok=False)
+        except:
+            raise Exception(
+                f"Folder {save_path} already exists; new folder name is required."
+            )
     # Convert tensor image to numpy array
     pixel_data = torch.permute(object.squeeze(),(2,1,0)).cpu().numpy()    
     scale_factor = (2**16 - 1) / pixel_data.max()
     pixel_data *= scale_factor #maximum dynamic range
     pixel_data = pixel_data.astype(np.uint16)
     # Get affine information
     ds_NM = pydicom.dcmread(file_NM)
@@ -616,23 +618,22 @@
     ds.PhotometricInterpretation = "MONOCHROME2"
     ds.PixelRepresentation = 0
     ds.ReconstructionMethod = recon_name
     # Create all slices
     dss = []
     for i in range(pixel_data.shape[0]):
         # Load existing DICOM file
-        ds_i = ds.copy()
+        ds_i = copy.deepcopy(ds)
         ds_i.InstanceNumber = i + 1
         ds_i.ImagePositionPatient = [Sx, Sy, Sz + i * dz]
         # Create SOP Instance UID unique to slice
-        SOP_instance_UID_slice = f"{ds_i.SOPInstanceUID[:-3]}{i+1:03d}"
-        ds_i.SOPInstanceUID = SOP_instance_UID_slice
-        ds_i.file_meta.MediaStorageSOPInstanceUID = SOP_instance_UID_slice
+        ds_i.SOPInstanceUID = f"{ds.SOPInstanceUID[:-3]}{i+1:03d}"
+        ds_i.file_meta.MediaStorageSOPInstanceUID = ds_i.SOPInstanceUID
         # Set the pixel data
         ds_i.PixelData = pixel_data[i].tobytes()
         dss.append(ds_i)
     if return_ds:
         return dss
     else:
         for ds_i in dss:
-            ds_i.save_as(os.path.join(save_path, f'{ds.SOPInstanceUID}.dcm'))
+            ds_i.save_as(os.path.join(save_path, f'{ds_i.SOPInstanceUID}.dcm'))
```

### Comparing `pytomography-2.0.4/src/pytomography/io/SPECT/shared.py` & `pytomography-2.0.5/src/pytomography/io/SPECT/shared.py`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/src/pytomography/io/SPECT/simind.py` & `pytomography-2.0.5/src/pytomography/io/SPECT/simind.py`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/src/pytomography/io/shared/dicom.py` & `pytomography-2.0.5/src/pytomography/io/shared/dicom.py`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/src/pytomography/io/shared/dicom_creation.py` & `pytomography-2.0.5/src/pytomography/io/shared/dicom_creation.py`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/src/pytomography/io/shared/interfile.py` & `pytomography-2.0.5/src/pytomography/io/shared/interfile.py`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/src/pytomography/likelihoods/likelihood.py` & `pytomography-2.0.5/src/pytomography/likelihoods/likelihood.py`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/src/pytomography/likelihoods/mse_objective.py` & `pytomography-2.0.5/src/pytomography/likelihoods/mse_objective.py`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/src/pytomography/likelihoods/poisson_log_likelihood.py` & `pytomography-2.0.5/src/pytomography/likelihoods/poisson_log_likelihood.py`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/src/pytomography/metadata/metadata.py` & `pytomography-2.0.5/src/pytomography/metadata/metadata.py`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/src/pytomography/metadata/PET/pet_tof_metadata.py` & `pytomography-2.0.5/src/pytomography/metadata/PET/pet_tof_metadata.py`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/src/pytomography/metadata/PET/petlm_metadata.py` & `pytomography-2.0.5/src/pytomography/metadata/PET/petlm_metadata.py`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/src/pytomography/metadata/SPECT/spect_metadata.py` & `pytomography-2.0.5/src/pytomography/metadata/SPECT/spect_metadata.py`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/src/pytomography/priors/__init__.py` & `pytomography-2.0.5/src/pytomography/priors/__init__.py`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/src/pytomography/priors/nearest_neighbour.py` & `pytomography-2.0.5/src/pytomography/priors/nearest_neighbour.py`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/src/pytomography/priors/prior.py` & `pytomography-2.0.5/src/pytomography/priors/prior.py`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/src/pytomography/projectors/system_matrix.py` & `pytomography-2.0.5/src/pytomography/projectors/system_matrix.py`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/src/pytomography/projectors/PET/petlm_system_matrix.py` & `pytomography-2.0.5/src/pytomography/projectors/PET/petlm_system_matrix.py`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/src/pytomography/projectors/SPECT/spect_system_matrix.py` & `pytomography-2.0.5/src/pytomography/projectors/SPECT/spect_system_matrix.py`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/src/pytomography/projectors/shared/kem_system_matrix.py` & `pytomography-2.0.5/src/pytomography/projectors/shared/kem_system_matrix.py`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/src/pytomography/projectors/shared/motion_correction_system_matrix.py` & `pytomography-2.0.5/src/pytomography/projectors/shared/motion_correction_system_matrix.py`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/src/pytomography/transforms/transform.py` & `pytomography-2.0.5/src/pytomography/transforms/transform.py`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/src/pytomography/transforms/SPECT/attenuation.py` & `pytomography-2.0.5/src/pytomography/transforms/SPECT/attenuation.py`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/src/pytomography/transforms/SPECT/cutoff.py` & `pytomography-2.0.5/src/pytomography/transforms/SPECT/cutoff.py`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/src/pytomography/transforms/SPECT/psf.py` & `pytomography-2.0.5/src/pytomography/transforms/SPECT/psf.py`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/src/pytomography/transforms/shared/filters.py` & `pytomography-2.0.5/src/pytomography/transforms/shared/filters.py`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/src/pytomography/transforms/shared/kem.py` & `pytomography-2.0.5/src/pytomography/transforms/shared/kem.py`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/src/pytomography/transforms/shared/motion.py` & `pytomography-2.0.5/src/pytomography/transforms/shared/motion.py`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/src/pytomography/transforms/shared/spatial.py` & `pytomography-2.0.5/src/pytomography/transforms/shared/spatial.py`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/src/pytomography/utils/__init__.py` & `pytomography-2.0.5/src/pytomography/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/src/pytomography/utils/fourier_filters.py` & `pytomography-2.0.5/src/pytomography/utils/fourier_filters.py`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/src/pytomography/utils/misc.py` & `pytomography-2.0.5/src/pytomography/utils/misc.py`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/src/pytomography/utils/nist_data.py` & `pytomography-2.0.5/src/pytomography/utils/nist_data.py`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/src/pytomography/utils/scatter.py` & `pytomography-2.0.5/src/pytomography/utils/scatter.py`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/src/pytomography/utils/spatial.py` & `pytomography-2.0.5/src/pytomography/utils/spatial.py`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/LICENSE` & `pytomography-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/README.md` & `pytomography-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pytomography-2.0.4/pyproject.toml` & `pytomography-2.0.5/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "toml"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pytomography"
-version = "2.0.4"
+version = "2.0.5"
 
 authors = [
   { name="Luke Polson", email="lukepolson@outlook.com" },
 ]
 description = "Package to perform tomographic image reconstruction"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `pytomography-2.0.4/PKG-INFO` & `pytomography-2.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pytomography
-Version: 2.0.4
+Version: 2.0.5
 Summary: Package to perform tomographic image reconstruction
 Project-URL: Homepage, https://github.com/qurit/PyTomography
 Project-URL: Bug Tracker, https://github.com/qurit/PyTomography/issues
 Author-email: Luke Polson <lukepolson@outlook.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

