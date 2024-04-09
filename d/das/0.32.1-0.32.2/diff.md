# Comparing `tmp/das-0.32.1.tar.gz` & `tmp/das-0.32.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "das-0.32.1.tar", last modified: Fri Mar  8 10:54:16 2024, max compression
+gzip compressed data, was "das-0.32.2.tar", last modified: Thu Mar 14 15:07:47 2024, max compression
```

## Comparing `das-0.32.1.tar` & `das-0.32.2.tar`

### file list

```diff
@@ -1,203 +1,203 @@
--rw-r--r--   0        0        0     1583 2024-02-03 13:48:02.400024 das-0.32.1/.github/workflows/publish.yml
--rw-r--r--   0        0        0     2320 2023-03-05 11:53:05.046670 das-0.32.1/.github/workflows/test.yml
--rwxr-xr-x   0        0        0     1764 2022-12-28 08:32:12.045976 das-0.32.1/.gitignore
--rw-r--r--   0        0        0     3706 2024-02-08 09:02:14.000000 das-0.32.1/README.md
--rw-r--r--   0        0        0      177 2022-09-24 07:20:14.000000 das-0.32.1/build_env.yml
--rw-r--r--   0        0        0   267514 2021-09-25 13:47:07.000000 das-0.32.1/colab/colab.ipynb
--rwxr-xr-x   0        0        0      573 2024-01-01 20:55:43.964062 das-0.32.1/conda/das-osxarm/build.sh
--rwxr-xr-x   0        0        0       33 2024-01-13 12:36:02.000000 das-0.32.1/conda/das-osxarm/conda_build_config.yaml
--rwxr-xr-x   0        0        0     1123 2024-01-13 18:51:23.000000 das-0.32.1/conda/das-osxarm/meta.yaml
--rwxr-xr-x   0        0        0      373 2024-01-13 21:23:04.027270 das-0.32.1/conda/das-test/build_osxarm64.sh
--rwxr-xr-x   0        0        0      284 2023-10-10 14:22:06.000000 das-0.32.1/conda/das-test/build_unix.sh
--rwxr-xr-x   0        0        0      307 2023-10-10 14:21:58.000000 das-0.32.1/conda/das-test/build_win.bat
--rwxr-xr-x   0        0        0       33 2024-01-13 18:16:30.851370 das-0.32.1/conda/das-test/conda_build_config.yaml
--rwxr-xr-x   0        0        0     1879 2024-02-03 13:48:02.400264 das-0.32.1/conda/das-test/meta.yaml
--rwxr-xr-x   0        0        0      307 2023-10-10 14:21:58.000000 das-0.32.1/conda/das/bld.bat
--rwxr-xr-x   0        0        0      284 2023-10-10 14:22:06.000000 das-0.32.1/conda/das/build.sh
--rwxr-xr-x   0        0        0       40 2021-10-12 09:05:12.000000 das-0.32.1/conda/das/conda_build_config.yaml
--rwxr-xr-x   0        0        0     1618 2024-02-03 13:08:38.609792 das-0.32.1/conda/das/meta.yaml
--rw-r--r--   0        0        0       51 2022-09-24 07:20:14.867621 das-0.32.1/condarc.yml
--rw-r--r--   0        0        0      774 2021-08-23 12:53:04.000000 das-0.32.1/docs/Makefile
--rw-r--r--   0        0        0      656 2023-04-18 07:18:53.000000 das-0.32.1/docs/README.md
--rw-r--r--   0        0        0      850 2024-02-23 19:42:19.359221 das-0.32.1/docs/api.rst
--rw-r--r--   0        0        0       62 2021-08-15 14:38:11.000000 das-0.32.1/docs/api/das.annot.rst
--rw-r--r--   0        0        0       83 2021-12-05 14:12:32.604858 das-0.32.1/docs/api/das.augmentation.rst
--rw-r--r--   0        0        0       89 2022-03-04 10:09:15.000000 das-0.32.1/docs/api/das.block_stratify.rst
--rw-r--r--   0        0        0       56 2021-08-15 14:38:12.000000 das-0.32.1/docs/api/das.cli.rst
--rw-r--r--   0        0        0       59 2021-08-15 14:38:12.000000 das-0.32.1/docs/api/das.data.rst
--rw-r--r--   0        0        0       74 2021-08-15 14:38:12.000000 das-0.32.1/docs/api/das.data_hash.rst
--rw-r--r--   0        0        0       71 2021-08-15 14:38:12.000000 das-0.32.1/docs/api/das.evaluate.rst
--rw-r--r--   0        0        0       80 2021-08-15 14:38:12.000000 das-0.32.1/docs/api/das.event_utils.rst
--rw-r--r--   0        0        0       53 2021-08-15 14:38:12.000000 das-0.32.1/docs/api/das.io.rst
--rw-r--r--   0        0        0      101 2021-08-15 14:38:12.000000 das-0.32.1/docs/api/das.kapre.augmentation.rst
--rw-r--r--   0        0        0       86 2021-08-15 14:38:12.000000 das-0.32.1/docs/api/das.kapre.backend.rst
--rw-r--r--   0        0        0      104 2021-08-15 14:38:12.000000 das-0.32.1/docs/api/das.kapre.backend_keras.rst
--rw-r--r--   0        0        0       95 2021-08-15 14:38:12.000000 das-0.32.1/docs/api/das.kapre.filterbank.rst
--rw-r--r--   0        0        0      107 2021-08-15 14:38:12.000000 das-0.32.1/docs/api/das.kapre.time_frequency.rst
--rw-r--r--   0        0        0       80 2021-08-15 14:38:12.000000 das-0.32.1/docs/api/das.kapre.utils.rst
--rw-r--r--   0        0        0       83 2021-08-15 14:38:12.000000 das-0.32.1/docs/api/das.make_dataset.rst
--rw-r--r--   0        0        0       74 2021-09-23 16:25:49.000000 das-0.32.1/docs/api/das.menagerie.rst
--rw-r--r--   0        0        0       65 2021-08-15 14:38:12.000000 das-0.32.1/docs/api/das.models.rst
--rw-r--r--   0        0        0       86 2021-12-05 14:12:32.714910 das-0.32.1/docs/api/das.models_legacy.rst
--rw-r--r--   0        0        0      119 2023-12-20 18:46:31.000000 das-0.32.1/docs/api/das.morpholayers.constraints.rst
--rw-r--r--   0        0        0      122 2023-12-20 18:46:31.000000 das-0.32.1/docs/api/das.morpholayers.initializers.rst
--rw-r--r--   0        0        0      104 2023-12-20 18:46:31.000000 das-0.32.1/docs/api/das.morpholayers.layers.rst
--rw-r--r--   0        0        0      122 2023-12-20 18:46:31.000000 das-0.32.1/docs/api/das.morpholayers.regularizers.rst
--rw-r--r--   0        0        0       68 2021-08-15 14:38:12.000000 das-0.32.1/docs/api/das.neptune.rst
--rw-r--r--   0        0        0       68 2021-08-15 14:38:12.000000 das-0.32.1/docs/api/das.npy_dir.rst
--rw-r--r--   0        0        0       89 2022-03-04 10:09:15.000000 das-0.32.1/docs/api/das.postprocessing.rst
--rw-r--r--   0        0        0       68 2021-08-15 14:38:12.000000 das-0.32.1/docs/api/das.predict.rst
--rw-r--r--   0        0        0       80 2022-07-22 08:59:26.000000 das-0.32.1/docs/api/das.predict_oom.rst
--rw-r--r--   0        0        0       80 2021-08-15 14:38:12.000000 das-0.32.1/docs/api/das.pulse_utils.rst
--rw-r--r--   0        0        0       86 2021-08-15 14:38:12.000000 das-0.32.1/docs/api/das.segment_utils.rst
--rw-r--r--   0        0        0       77 2022-05-04 14:42:30.000000 das-0.32.1/docs/api/das.spec_utils.rst
--rw-r--r--   0        0        0       68 2021-08-15 14:38:12.000000 das-0.32.1/docs/api/das.tcn.tcn.rst
--rw-r--r--   0        0        0       80 2021-08-15 14:38:12.000000 das-0.32.1/docs/api/das.tcn.tcn_new.rst
--rw-r--r--   0        0        0       71 2021-12-15 19:50:49.620244 das-0.32.1/docs/api/das.tracking.rst
--rw-r--r--   0        0        0       62 2021-08-15 14:38:12.000000 das-0.32.1/docs/api/das.train.rst
--rw-r--r--   0        0        0       89 2021-08-15 14:38:12.000000 das-0.32.1/docs/api/das.train_transfer.rst
--rw-r--r--   0        0        0       77 2021-12-05 14:12:32.833215 das-0.32.1/docs/api/das.train_tune.rst
--rw-r--r--   0        0        0       62 2021-08-15 14:38:12.000000 das-0.32.1/docs/api/das.utils.rst
--rw-r--r--   0        0        0       77 2021-08-15 14:38:13.000000 das-0.32.1/docs/api/das.utils_plot.rst
--rw-r--r--   0        0        0     3499 2022-11-09 19:08:12.080481 das-0.32.1/docs/conf.py
--rw-r--r--   0        0        0     2649 2023-01-08 09:40:58.000000 das-0.32.1/docs/index.rst
--rw-r--r--   0        0        0     2985 2024-02-23 19:43:10.905056 das-0.32.1/docs/installation.md
--rw-r--r--   0        0        0   109962 2023-12-20 18:56:02.269848 das-0.32.1/docs/jupyter_execute/00b86cf553e61db9b1d9039084ecb3de176c5128f74e1d9cbf226df4fd4b098c.jpg
--rw-r--r--   0        0        0    12227 2023-12-20 18:56:01.767453 das-0.32.1/docs/jupyter_execute/05bb23a35be292dacca29115895aa30b477b3702733812dc88eedec9108561fd.png
--rw-r--r--   0        0        0    38383 2023-12-20 18:56:01.991624 das-0.32.1/docs/jupyter_execute/0f4e455010d95626191b2c7cf3b5bb49f9aeaa9a4b91c3d3a77728209e542b28.jpg
--rw-r--r--   0        0        0    82121 2023-12-20 18:56:02.225344 das-0.32.1/docs/jupyter_execute/0f87b4789d1dea68deb5dbd5c8169c3307774631e0c4720e8230b5bf13ceb4ab.jpg
--rw-r--r--   0        0        0    90389 2023-12-20 18:56:02.273171 das-0.32.1/docs/jupyter_execute/1003c63cf4d33f7a19fa2966dbb8efaebbb8cded2d1f307be357976833342305.jpg
--rw-r--r--   0        0        0    74891 2023-12-20 18:56:02.019932 das-0.32.1/docs/jupyter_execute/15961ee4ef682feb0773b21475bcaf9571ce3cbffdcdb03e80c24b12e8c1433d.jpg
--rw-r--r--   0        0        0    10638 2023-12-20 18:56:01.992446 das-0.32.1/docs/jupyter_execute/18f69ae6eccfcaef9677e0db0e0223dcf2011fdc33c3c65f17dcf5b56f154725.jpg
--rw-r--r--   0        0        0    51018 2023-12-20 18:56:02.273661 das-0.32.1/docs/jupyter_execute/1f70d964adae8f5937528754bfbf018926b44f563247167c283ba3d6ec6912af.jpg
--rw-r--r--   0        0        0    94656 2023-12-20 18:56:02.071496 das-0.32.1/docs/jupyter_execute/2d19a4031347cfcde5655f0dcfceefec27aaf73fcc741ab1ab0195ccd943b251.png
--rw-r--r--   0        0        0    30828 2023-12-20 18:56:01.993128 das-0.32.1/docs/jupyter_execute/30eacca7324ff8d5eb2b8a221da4d1e31e83a9da73b5f02656c038110f164fc5.jpg
--rw-r--r--   0        0        0    32606 2023-12-20 18:56:02.091522 das-0.32.1/docs/jupyter_execute/31f31c028cd32511865d9b4377790afc32485c5d30387adc29f6007cdf70df7f.jpg
--rw-r--r--   0        0        0    64881 2023-12-20 18:56:01.993676 das-0.32.1/docs/jupyter_execute/3594e0999cf561fa210f5aa128dc8c1bdf1cd54cfc522303870b7ac0996d6d81.jpg
--rw-r--r--   0        0        0    69902 2023-12-20 18:56:02.233145 das-0.32.1/docs/jupyter_execute/36e975676dc3c37f488f6a644a09d8b0f059858482001b8b13a7a2a830677a7a.jpg
--rw-r--r--   0        0        0    36118 2023-12-20 18:56:01.991146 das-0.32.1/docs/jupyter_execute/411ad01b915cabb08f441d57ed6c1395642c93fdba43c5ab6a3664995bb157ab.jpg
--rw-r--r--   0        0        0   133684 2023-12-20 18:56:01.810418 das-0.32.1/docs/jupyter_execute/42e6d26af2159c983a442fa87ce71bc8d4af03073a37f56384a0f6aa07bccd4b.jpg
--rw-r--r--   0        0        0    74310 2023-12-20 18:56:02.250444 das-0.32.1/docs/jupyter_execute/51ad2dee4a168546bfaf845facb661b5f4436899bd96e179ff9ea85aca33ae9c.png
--rw-r--r--   0        0        0    15662 2023-12-20 18:56:01.811015 das-0.32.1/docs/jupyter_execute/5334ee66c97affed7823118c36b355c37407fbaaa038895e0872fe8090ce816a.jpg
--rw-r--r--   0        0        0    87812 2023-12-20 18:56:01.772999 das-0.32.1/docs/jupyter_execute/59e6ffa2a5eeba3ca1f8907236c54231658e8f1b0a9a792d95781be7d5b8c1fd.png
--rw-r--r--   0        0        0    16787 2023-12-20 18:56:01.994381 das-0.32.1/docs/jupyter_execute/6f8b4b2ebfcd0679a3727b0192658ca56d59490c9c0362db4d3cea0224fd2429.jpg
--rw-r--r--   0        0        0    25664 2023-12-20 18:56:02.233669 das-0.32.1/docs/jupyter_execute/7270f0505dfe5c4c4083e0aa090c5ddf270ca488482cda44c8b6c315075f226f.jpg
--rw-r--r--   0        0        0   131884 2023-12-20 18:56:02.271023 das-0.32.1/docs/jupyter_execute/72cd6540b8d8c6b5fd1039cfe919928abc36b30a1f5e220e687cd807fe104fcc.jpg
--rw-r--r--   0        0        0   103999 2023-12-20 18:56:02.020485 das-0.32.1/docs/jupyter_execute/7876649fe14736f36ea3121f36405b25aa875478aa7bfdd42fa94e78abe45ceb.jpg
--rw-r--r--   0        0        0    21164 2023-12-20 18:56:01.994070 das-0.32.1/docs/jupyter_execute/7962da1c27c61360e1c35f7f230b67c31fe8dfe3fefeb90e1e63d25c2865a2ce.jpg
--rw-r--r--   0        0        0    11245 2023-12-20 18:56:01.992119 das-0.32.1/docs/jupyter_execute/8866e0d0472b30efbee828d80f76edc46540e0bb8ac2fb22e0e38319c5287c3c.jpg
--rw-r--r--   0        0        0    29388 2023-12-20 18:56:02.091017 das-0.32.1/docs/jupyter_execute/8aa7e22a172f489f402d455824660ee508d1837b7b4e209d2e2374fd0443f39a.jpg
--rw-r--r--   0        0        0    79037 2023-12-20 18:56:02.234192 das-0.32.1/docs/jupyter_execute/9a879c388a68d6b65ccfd5b822a225ff9453cf3c1647ae1c3e5e6813ef9b5a83.jpg
--rw-r--r--   0        0        0   146245 2023-12-20 18:56:02.272143 das-0.32.1/docs/jupyter_execute/a0597b24513779a6876e1003b3c0aee8bb6693276d5901190b86a2efa59e42de.jpg
--rw-r--r--   0        0        0    12151 2023-12-20 18:56:01.811355 das-0.32.1/docs/jupyter_execute/a6f5b756241918250a1f5e8a45f2cc509c003233ff7eaaf5870f0c5ca62b7473.jpg
--rw-r--r--   0        0        0   190352 2023-12-20 18:56:02.226838 das-0.32.1/docs/jupyter_execute/b5b6635b8c13e3b79594f06a6bd2c4fca4781f6810494c4286fc7b2aca32f2d1.jpg
--rw-r--r--   0        0        0    14654 2023-12-20 18:56:02.091918 das-0.32.1/docs/jupyter_execute/b919c302a83f2ef38e79ccbb5c939bb0f5336a657168bc9b2e010da4cd1d56cd.jpg
--rw-r--r--   0        0        0    25292 2023-12-20 18:56:01.992776 das-0.32.1/docs/jupyter_execute/bd4feef74fd6786267ce2fc20695be861a5c06f7e4b973ee72c6ba79292d6f5d.jpg
--rw-r--r--   0        0        0    33580 2023-12-20 18:56:02.049371 das-0.32.1/docs/jupyter_execute/c3b46f8cc6ce88b46b7b54dec7c7182ca88ccb66249098a0101904dab6e2ee05.png
--rw-r--r--   0        0        0    69718 2023-12-20 18:56:02.251245 das-0.32.1/docs/jupyter_execute/d9ecc34617ef75d86ce90957aca0103c23f426fdcf89347c7780d7528c30a00a.png
--rw-r--r--   0        0        0    86769 2023-12-20 18:56:02.019325 das-0.32.1/docs/jupyter_execute/e3eb93d28f5c2028549805bd3181ff21fea996bb882fe6a99c80a2506f68339f.jpg
--rw-r--r--   0        0        0    59110 2023-12-20 18:56:02.090531 das-0.32.1/docs/jupyter_execute/eb4201de71c8575059afc78398a57c865d785ca997ac7f55fb269ab8d605e524.jpg
--rw-r--r--   0        0        0    52009 2023-12-20 18:56:01.773625 das-0.32.1/docs/jupyter_execute/fe1262a9629ae4f353920933ba7773c9101afee6ae8ab2c3e6f14199ca7be0b6.png
--rw-r--r--   0        0        0    37136 2023-12-20 18:56:01.691532 das-0.32.1/docs/jupyter_execute/technical/cli.ipynb
--rw-r--r--   0        0        0   267513 2023-12-20 18:56:01.776740 das-0.32.1/docs/jupyter_execute/tutorials/colab.ipynb
--rw-r--r--   0        0        0     5129 2023-12-20 18:56:01.796427 das-0.32.1/docs/jupyter_execute/tutorials/continue_training.ipynb
--rw-r--r--   0        0        0   246982 2023-12-20 18:56:01.814829 das-0.32.1/docs/jupyter_execute/tutorials/evaluate_bird.ipynb
--rw-r--r--   0        0        0   373096 2023-12-20 18:56:01.997248 das-0.32.1/docs/jupyter_execute/tutorials/evaluate_fly.ipynb
--rw-r--r--   0        0        0   360089 2023-12-20 18:56:02.022333 das-0.32.1/docs/jupyter_execute/tutorials/inspect_dataset.ipynb
--rw-r--r--   0        0        0    70067 2023-12-20 18:56:02.051644 das-0.32.1/docs/jupyter_execute/tutorials/make_ds_notebook.ipynb
--rw-r--r--   0        0        0   140002 2023-12-20 18:56:02.072969 das-0.32.1/docs/jupyter_execute/tutorials/predict.ipynb
--rw-r--r--   0        0        0   193820 2023-12-20 18:56:02.093763 das-0.32.1/docs/jupyter_execute/tutorials/realtime.ipynb
--rw-r--r--   0        0        0    56475 2023-12-20 18:56:02.122290 das-0.32.1/docs/jupyter_execute/tutorials/train.ipynb
--rw-r--r--   0        0        0      981 2023-12-20 18:56:02.131310 das-0.32.1/docs/jupyter_execute/tutorials/tuning.ipynb
--rw-r--r--   0        0        0   617950 2023-12-20 18:56:02.238535 das-0.32.1/docs/jupyter_execute/unsupervised/birds.ipynb
--rw-r--r--   0        0        0   200095 2023-12-20 18:56:02.252757 das-0.32.1/docs/jupyter_execute/unsupervised/flies.ipynb
--rw-r--r--   0        0        0   719003 2023-12-20 18:56:02.277401 das-0.32.1/docs/jupyter_execute/unsupervised/mice.ipynb
--rw-r--r--   0        0        0      795 2021-08-12 19:27:18.000000 das-0.32.1/docs/make.bat
--rw-r--r--   0        0        0     1068 2021-08-15 15:00:19.000000 das-0.32.1/docs/make_api_doctree.py
--rw-r--r--   0        0        0     9775 2023-01-08 09:32:51.000000 das-0.32.1/docs/quickstart_bird.md
--rw-r--r--   0        0        0    11856 2023-01-08 09:28:27.000000 das-0.32.1/docs/quickstart_fly.md
--rw-r--r--   0        0        0    37137 2022-09-18 16:59:07.938194 das-0.32.1/docs/technical/cli.ipynb
--rw-r--r--   0        0        0     7137 2022-02-18 11:19:41.000000 das-0.32.1/docs/technical/data_formats.md
--rw-r--r--   0        0        0      840 2021-11-11 20:17:52.000000 das-0.32.1/docs/technical/installation_apple-arm.md
--rw-r--r--   0        0        0      254 2021-08-23 13:21:25.000000 das-0.32.1/docs/technical/technical.rst
--rw-r--r--   0        0        0      144 2022-01-14 14:23:10.000000 das-0.32.1/docs/tracking/fixing_identities.md
--rw-r--r--   0        0        0     3153 2022-09-19 13:10:08.000000 das-0.32.1/docs/tutorials/architecture_tuning.md
--rw-r--r--   0        0        0   267514 2021-09-25 13:47:07.000000 das-0.32.1/docs/tutorials/colab.ipynb
--rw-r--r--   0        0        0     5152 2022-06-09 10:37:23.000000 das-0.32.1/docs/tutorials/continue_training.ipynb
--rw-r--r--   0        0        0     5929 2022-02-18 11:14:07.000000 das-0.32.1/docs/tutorials/convert.md
--rw-r--r--   0        0        0   246983 2021-09-25 13:50:30.000000 das-0.32.1/docs/tutorials/evaluate_bird.ipynb
--rw-r--r--   0        0        0   373097 2022-09-25 17:24:36.592635 das-0.32.1/docs/tutorials/evaluate_fly.ipynb
--rw-r--r--   0        0        0     1131 2022-09-18 17:21:36.193272 das-0.32.1/docs/tutorials/experiment_tracking.md
--rwxr-xr-x   0        0        0   360090 2021-09-25 12:38:04.000000 das-0.32.1/docs/tutorials/inspect_dataset.ipynb
--rw-r--r--   0        0        0      127 2020-12-07 15:26:25.000000 das-0.32.1/docs/tutorials/label_segments.md
--rw-r--r--   0        0        0    70068 2021-09-25 12:36:01.000000 das-0.32.1/docs/tutorials/make_ds_notebook.ipynb
--rwxr-xr-x   0        0        0      982 2020-03-18 12:54:18.000000 das-0.32.1/docs/tutorials/ncb.mplstyle
--rw-r--r--   0        0        0   140003 2022-07-25 11:04:46.000000 das-0.32.1/docs/tutorials/predict.ipynb
--rwxr-xr-x   0        0        0   193821 2022-09-18 16:29:29.000000 das-0.32.1/docs/tutorials/realtime.ipynb
--rw-r--r--   0        0        0     5617 2021-09-25 11:24:45.000000 das-0.32.1/docs/tutorials/structparams.md
--rw-r--r--   0        0        0    56476 2021-09-24 20:23:03.000000 das-0.32.1/docs/tutorials/train.ipynb
--rw-r--r--   0        0        0     1004 2023-10-10 14:21:46.000000 das-0.32.1/docs/tutorials/tuning.ipynb
--rw-r--r--   0        0        0     1159 2022-12-27 21:36:14.976655 das-0.32.1/docs/tutorials/tutorials.rst
--rw-r--r--   0        0        0     5974 2022-07-25 11:01:30.000000 das-0.32.1/docs/tutorials_gui/annotate.md
--rw-r--r--   0        0        0     4694 2024-02-23 19:42:04.648169 das-0.32.1/docs/tutorials_gui/load.md
--rw-r--r--   0        0        0     3076 2021-09-25 16:14:59.000000 das-0.32.1/docs/tutorials_gui/predict.md
--rw-r--r--   0        0        0    10092 2022-12-27 21:42:37.000000 das-0.32.1/docs/tutorials_gui/train.md
--rw-r--r--   0        0        0      482 2023-01-25 15:03:24.000000 das-0.32.1/docs/tutorials_gui/tutorials_gui.rst
--rw-r--r--   0        0        0   738598 2020-09-22 10:35:48.000000 das-0.32.1/docs/unsupervised/banner.png
--rw-r--r--   0        0        0   621476 2021-09-24 08:39:06.000000 das-0.32.1/docs/unsupervised/birds.ipynb
--rw-r--r--   0        0        0   200988 2021-09-24 08:27:06.000000 das-0.32.1/docs/unsupervised/flies.ipynb
--rwxr-xr-x   0        0        0   720771 2021-09-24 08:22:18.000000 das-0.32.1/docs/unsupervised/mice.ipynb
--rwxr-xr-x   0        0        0      982 2020-03-18 12:54:18.000000 das-0.32.1/docs/unsupervised/ncb.mplstyle
--rw-r--r--   0        0        0     3584 2021-09-25 12:25:43.000000 das-0.32.1/docs/unsupervised/unsupervised.rst
--rw-r--r--   0        0        0      794 2022-12-21 08:31:00.000000 das-0.32.1/pyproject.toml
--rw-r--r--   0        0        0      572 2023-09-02 09:15:46.000000 das-0.32.1/setup.py
--rw-r--r--   0        0        0       33 2024-03-08 10:53:37.579692 das-0.32.1/src/das/__init__.py
--rw-r--r--   0        0        0    16462 2023-01-10 07:09:56.000000 das-0.32.1/src/das/annot.py
--rw-r--r--   0        0        0    11666 2023-01-10 07:09:56.000000 das-0.32.1/src/das/augmentation.py
--rw-r--r--   0        0        0     6598 2023-04-18 06:59:16.000000 das-0.32.1/src/das/block_stratify.py
--rw-r--r--   0        0        0     2990 2024-01-02 08:56:17.944388 das-0.32.1/src/das/cli.py
--rw-r--r--   0        0        0    13390 2023-12-15 13:43:09.000000 das-0.32.1/src/das/data.py
--rw-r--r--   0        0        0     1758 2023-01-10 07:09:55.000000 das-0.32.1/src/das/data_hash.py
--rw-r--r--   0        0        0     7765 2024-01-01 20:17:00.000000 das-0.32.1/src/das/evaluate.py
--rw-r--r--   0        0        0     6594 2024-01-01 20:16:39.000000 das-0.32.1/src/das/event_utils.py
--rw-r--r--   0        0        0     2935 2023-05-13 17:02:40.000000 das-0.32.1/src/das/io.py
--rw-r--r--   0        0        0     1069 2022-03-01 17:05:15.000000 das-0.32.1/src/das/kapre/LICENSE.txt
--rw-r--r--   0        0        0    12759 2022-03-01 17:05:15.000000 das-0.32.1/src/das/kapre/README.md
--rw-r--r--   0        0        0      237 2023-01-10 07:09:55.000000 das-0.32.1/src/das/kapre/__init__.py
--rw-r--r--   0        0        0     1520 2023-01-10 07:09:55.000000 das-0.32.1/src/das/kapre/augmentation.py
--rw-r--r--   0        0        0     4751 2023-01-10 07:09:56.000000 das-0.32.1/src/das/kapre/backend.py
--rw-r--r--   0        0        0     1076 2022-03-01 17:05:15.000000 das-0.32.1/src/das/kapre/backend_keras.py
--rw-r--r--   0        0        0     4786 2023-01-10 07:09:56.000000 das-0.32.1/src/das/kapre/filterbank.py
--rw-r--r--   0        0        0    14067 2023-04-18 06:59:17.000000 das-0.32.1/src/das/kapre/time_frequency.py
--rw-r--r--   0        0        0     5159 2023-01-10 07:09:56.000000 das-0.32.1/src/das/kapre/utils.py
--rw-r--r--   0        0        0    11601 2024-01-01 20:16:53.000000 das-0.32.1/src/das/make_dataset.py
--rw-r--r--   0        0        0     2340 2023-01-10 07:09:56.000000 das-0.32.1/src/das/menagerie.py
--rw-r--r--   0        0        0    15505 2024-01-11 20:03:42.623302 das-0.32.1/src/das/models.py
--rw-r--r--   0        0        0    30534 2023-02-12 09:24:43.789306 das-0.32.1/src/das/models_legacy.py
--rwxr-xr-x   0        0        0     1080 2023-12-20 18:49:39.909722 das-0.32.1/src/das/morpholayers/LICENSE
--rwxr-xr-x   0        0        0     2706 2023-12-20 18:49:39.909838 das-0.32.1/src/das/morpholayers/README.md
--rwxr-xr-x   0        0        0       97 2023-12-20 18:49:39.909937 das-0.32.1/src/das/morpholayers/__init__.py
--rwxr-xr-x   0        0        0     5607 2023-12-20 18:59:48.000000 das-0.32.1/src/das/morpholayers/constraints.py
--rwxr-xr-x   0        0        0     6183 2023-12-20 19:04:50.000000 das-0.32.1/src/das/morpholayers/initializers.py
--rwxr-xr-x   0        0        0   152836 2024-01-11 19:51:30.000000 das-0.32.1/src/das/morpholayers/layers.py
--rwxr-xr-x   0        0        0     1926 2024-01-11 19:47:31.980151 das-0.32.1/src/das/morpholayers/regularizers.py
--rw-r--r--   0        0        0     4030 2023-05-18 07:45:17.000000 das-0.32.1/src/das/npy_dir.py
--rw-r--r--   0        0        0     5422 2023-01-10 07:09:56.000000 das-0.32.1/src/das/postprocessing.py
--rw-r--r--   0        0        0    32122 2024-03-08 10:51:18.324615 das-0.32.1/src/das/predict.py
--rw-r--r--   0        0        0     3948 2023-02-12 09:24:43.789511 das-0.32.1/src/das/pulse_utils.py
--rw-r--r--   0        0        0     4881 2023-12-25 13:19:27.000000 das-0.32.1/src/das/segment_utils.py
--rw-r--r--   0        0        0     3081 2023-01-10 07:09:56.000000 das-0.32.1/src/das/spec_utils.py
--rwxr-xr-x   0        0        0     1071 2022-03-01 17:05:15.000000 das-0.32.1/src/das/tcn/LICENSE
--rwxr-xr-x   0        0        0    11264 2022-03-01 17:05:15.000000 das-0.32.1/src/das/tcn/README.md
--rw-r--r--   0        0        0       80 2023-01-10 07:09:56.000000 das-0.32.1/src/das/tcn/__init__.py
--rw-r--r--   0        0        0     6581 2023-02-12 09:24:43.789724 das-0.32.1/src/das/tcn/tcn.py
--rw-r--r--   0        0        0    16153 2023-04-18 06:59:17.000000 das-0.32.1/src/das/tcn/tcn_new.py
--rw-r--r--   0        0        0     3125 2023-01-10 07:09:56.000000 das-0.32.1/src/das/tracking.py
--rw-r--r--   0        0        0    24727 2024-01-12 09:08:13.000000 das-0.32.1/src/das/train.py
--rw-r--r--   0        0        0    22517 2023-02-12 09:24:43.790613 das-0.32.1/src/das/train_tune.py
--rw-r--r--   0        0        0     9062 2023-01-25 09:52:34.000000 das-0.32.1/src/das/utils.py
--rw-r--r--   0        0        0    16870 2023-05-21 13:30:50.512318 das-0.32.1/src/das/utils_plot.py
--rw-r--r--   0        0        0     2557 2021-12-16 19:07:36.398031 das-0.32.1/tests/test_augmentation.py
--rw-r--r--   0        0        0      162 2023-10-10 14:20:26.000000 das-0.32.1/tests/test_cli.py
--rw-r--r--   0        0        0      725 2023-10-10 14:20:33.000000 das-0.32.1/tests/test_import.py
--rw-r--r--   0        0        0     4425 1970-01-01 00:00:00.000000 das-0.32.1/PKG-INFO
+-rw-r--r--   0        0        0     1583 2024-03-08 11:00:02.000000 das-0.32.2/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     2320 2023-03-05 11:53:05.000000 das-0.32.2/.github/workflows/test.yml
+-rwxr-xr-x   0        0        0     1764 2022-12-28 08:32:12.000000 das-0.32.2/.gitignore
+-rw-r--r--   0        0        0     3706 2024-03-14 15:06:53.609733 das-0.32.2/README.md
+-rw-r--r--   0        0        0      177 2022-09-24 07:20:14.000000 das-0.32.2/build_env.yml
+-rw-r--r--   0        0        0   267514 2021-09-25 13:47:07.000000 das-0.32.2/colab/colab.ipynb
+-rwxr-xr-x   0        0        0      573 2024-01-01 20:55:43.000000 das-0.32.2/conda/das-osxarm/build.sh
+-rwxr-xr-x   0        0        0       33 2024-01-13 12:36:02.000000 das-0.32.2/conda/das-osxarm/conda_build_config.yaml
+-rwxr-xr-x   0        0        0     1123 2024-01-13 18:51:23.000000 das-0.32.2/conda/das-osxarm/meta.yaml
+-rwxr-xr-x   0        0        0      373 2024-01-13 21:23:04.000000 das-0.32.2/conda/das-test/build_osxarm64.sh
+-rwxr-xr-x   0        0        0      284 2023-10-10 14:22:06.000000 das-0.32.2/conda/das-test/build_unix.sh
+-rwxr-xr-x   0        0        0      307 2023-10-10 14:21:58.000000 das-0.32.2/conda/das-test/build_win.bat
+-rwxr-xr-x   0        0        0       33 2024-01-13 18:16:30.000000 das-0.32.2/conda/das-test/conda_build_config.yaml
+-rwxr-xr-x   0        0        0     1879 2024-02-03 13:48:02.000000 das-0.32.2/conda/das-test/meta.yaml
+-rwxr-xr-x   0        0        0      307 2023-10-10 14:21:58.829995 das-0.32.2/conda/das/bld.bat
+-rwxr-xr-x   0        0        0      284 2023-10-10 14:22:06.132678 das-0.32.2/conda/das/build.sh
+-rwxr-xr-x   0        0        0       40 2021-10-12 09:05:12.000000 das-0.32.2/conda/das/conda_build_config.yaml
+-rwxr-xr-x   0        0        0     1618 2024-02-03 13:08:38.000000 das-0.32.2/conda/das/meta.yaml
+-rw-r--r--   0        0        0       51 2022-09-24 07:20:14.000000 das-0.32.2/condarc.yml
+-rw-r--r--   0        0        0      774 2021-08-23 12:53:04.000000 das-0.32.2/docs/Makefile
+-rw-r--r--   0        0        0      656 2023-04-18 07:18:53.621949 das-0.32.2/docs/README.md
+-rw-r--r--   0        0        0      850 2023-12-20 18:56:23.000000 das-0.32.2/docs/api.rst
+-rw-r--r--   0        0        0       62 2021-08-15 14:38:11.000000 das-0.32.2/docs/api/das.annot.rst
+-rw-r--r--   0        0        0       83 2021-12-05 14:12:32.000000 das-0.32.2/docs/api/das.augmentation.rst
+-rw-r--r--   0        0        0       89 2022-03-04 10:09:15.000000 das-0.32.2/docs/api/das.block_stratify.rst
+-rw-r--r--   0        0        0       56 2021-08-15 14:38:12.000000 das-0.32.2/docs/api/das.cli.rst
+-rw-r--r--   0        0        0       59 2021-08-15 14:38:12.000000 das-0.32.2/docs/api/das.data.rst
+-rw-r--r--   0        0        0       74 2021-08-15 14:38:12.000000 das-0.32.2/docs/api/das.data_hash.rst
+-rw-r--r--   0        0        0       71 2021-08-15 14:38:12.000000 das-0.32.2/docs/api/das.evaluate.rst
+-rw-r--r--   0        0        0       80 2021-08-15 14:38:12.000000 das-0.32.2/docs/api/das.event_utils.rst
+-rw-r--r--   0        0        0       53 2021-08-15 14:38:12.000000 das-0.32.2/docs/api/das.io.rst
+-rw-r--r--   0        0        0      101 2021-08-15 14:38:12.000000 das-0.32.2/docs/api/das.kapre.augmentation.rst
+-rw-r--r--   0        0        0       86 2021-08-15 14:38:12.000000 das-0.32.2/docs/api/das.kapre.backend.rst
+-rw-r--r--   0        0        0      104 2021-08-15 14:38:12.000000 das-0.32.2/docs/api/das.kapre.backend_keras.rst
+-rw-r--r--   0        0        0       95 2021-08-15 14:38:12.000000 das-0.32.2/docs/api/das.kapre.filterbank.rst
+-rw-r--r--   0        0        0      107 2021-08-15 14:38:12.000000 das-0.32.2/docs/api/das.kapre.time_frequency.rst
+-rw-r--r--   0        0        0       80 2021-08-15 14:38:12.000000 das-0.32.2/docs/api/das.kapre.utils.rst
+-rw-r--r--   0        0        0       83 2021-08-15 14:38:12.000000 das-0.32.2/docs/api/das.make_dataset.rst
+-rw-r--r--   0        0        0       74 2021-09-23 16:25:49.000000 das-0.32.2/docs/api/das.menagerie.rst
+-rw-r--r--   0        0        0       65 2021-08-15 14:38:12.000000 das-0.32.2/docs/api/das.models.rst
+-rw-r--r--   0        0        0       86 2021-12-05 14:12:32.000000 das-0.32.2/docs/api/das.models_legacy.rst
+-rw-r--r--   0        0        0      119 2023-12-20 18:46:31.000000 das-0.32.2/docs/api/das.morpholayers.constraints.rst
+-rw-r--r--   0        0        0      122 2023-12-20 18:46:31.000000 das-0.32.2/docs/api/das.morpholayers.initializers.rst
+-rw-r--r--   0        0        0      104 2023-12-20 18:46:31.000000 das-0.32.2/docs/api/das.morpholayers.layers.rst
+-rw-r--r--   0        0        0      122 2023-12-20 18:46:31.000000 das-0.32.2/docs/api/das.morpholayers.regularizers.rst
+-rw-r--r--   0        0        0       68 2021-08-15 14:38:12.000000 das-0.32.2/docs/api/das.neptune.rst
+-rw-r--r--   0        0        0       68 2021-08-15 14:38:12.000000 das-0.32.2/docs/api/das.npy_dir.rst
+-rw-r--r--   0        0        0       89 2022-03-04 10:09:15.000000 das-0.32.2/docs/api/das.postprocessing.rst
+-rw-r--r--   0        0        0       68 2021-08-15 14:38:12.000000 das-0.32.2/docs/api/das.predict.rst
+-rw-r--r--   0        0        0       80 2022-07-22 08:59:26.000000 das-0.32.2/docs/api/das.predict_oom.rst
+-rw-r--r--   0        0        0       80 2021-08-15 14:38:12.000000 das-0.32.2/docs/api/das.pulse_utils.rst
+-rw-r--r--   0        0        0       86 2021-08-15 14:38:12.000000 das-0.32.2/docs/api/das.segment_utils.rst
+-rw-r--r--   0        0        0       77 2022-05-04 14:42:30.000000 das-0.32.2/docs/api/das.spec_utils.rst
+-rw-r--r--   0        0        0       68 2021-08-15 14:38:12.000000 das-0.32.2/docs/api/das.tcn.tcn.rst
+-rw-r--r--   0        0        0       80 2021-08-15 14:38:12.000000 das-0.32.2/docs/api/das.tcn.tcn_new.rst
+-rw-r--r--   0        0        0       71 2021-12-15 19:50:49.000000 das-0.32.2/docs/api/das.tracking.rst
+-rw-r--r--   0        0        0       62 2021-08-15 14:38:12.000000 das-0.32.2/docs/api/das.train.rst
+-rw-r--r--   0        0        0       89 2021-08-15 14:38:12.000000 das-0.32.2/docs/api/das.train_transfer.rst
+-rw-r--r--   0        0        0       77 2021-12-05 14:12:32.000000 das-0.32.2/docs/api/das.train_tune.rst
+-rw-r--r--   0        0        0       62 2021-08-15 14:38:12.000000 das-0.32.2/docs/api/das.utils.rst
+-rw-r--r--   0        0        0       77 2021-08-15 14:38:13.000000 das-0.32.2/docs/api/das.utils_plot.rst
+-rw-r--r--   0        0        0     3499 2022-11-09 19:08:12.000000 das-0.32.2/docs/conf.py
+-rw-r--r--   0        0        0     2649 2023-01-08 09:40:58.000000 das-0.32.2/docs/index.rst
+-rw-r--r--   0        0        0     2985 2024-03-14 15:07:01.595006 das-0.32.2/docs/installation.md
+-rw-r--r--   0        0        0   109962 2023-12-20 18:56:02.000000 das-0.32.2/docs/jupyter_execute/00b86cf553e61db9b1d9039084ecb3de176c5128f74e1d9cbf226df4fd4b098c.jpg
+-rw-r--r--   0        0        0    12227 2023-12-20 18:56:01.000000 das-0.32.2/docs/jupyter_execute/05bb23a35be292dacca29115895aa30b477b3702733812dc88eedec9108561fd.png
+-rw-r--r--   0        0        0    38383 2023-12-20 18:56:01.000000 das-0.32.2/docs/jupyter_execute/0f4e455010d95626191b2c7cf3b5bb49f9aeaa9a4b91c3d3a77728209e542b28.jpg
+-rw-r--r--   0        0        0    82121 2023-12-20 18:56:02.000000 das-0.32.2/docs/jupyter_execute/0f87b4789d1dea68deb5dbd5c8169c3307774631e0c4720e8230b5bf13ceb4ab.jpg
+-rw-r--r--   0        0        0    90389 2023-12-20 18:56:02.000000 das-0.32.2/docs/jupyter_execute/1003c63cf4d33f7a19fa2966dbb8efaebbb8cded2d1f307be357976833342305.jpg
+-rw-r--r--   0        0        0    74891 2023-12-20 18:56:02.000000 das-0.32.2/docs/jupyter_execute/15961ee4ef682feb0773b21475bcaf9571ce3cbffdcdb03e80c24b12e8c1433d.jpg
+-rw-r--r--   0        0        0    10638 2023-12-20 18:56:01.000000 das-0.32.2/docs/jupyter_execute/18f69ae6eccfcaef9677e0db0e0223dcf2011fdc33c3c65f17dcf5b56f154725.jpg
+-rw-r--r--   0        0        0    51018 2023-12-20 18:56:02.000000 das-0.32.2/docs/jupyter_execute/1f70d964adae8f5937528754bfbf018926b44f563247167c283ba3d6ec6912af.jpg
+-rw-r--r--   0        0        0    94656 2023-12-20 18:56:02.000000 das-0.32.2/docs/jupyter_execute/2d19a4031347cfcde5655f0dcfceefec27aaf73fcc741ab1ab0195ccd943b251.png
+-rw-r--r--   0        0        0    30828 2023-12-20 18:56:01.000000 das-0.32.2/docs/jupyter_execute/30eacca7324ff8d5eb2b8a221da4d1e31e83a9da73b5f02656c038110f164fc5.jpg
+-rw-r--r--   0        0        0    32606 2023-12-20 18:56:02.000000 das-0.32.2/docs/jupyter_execute/31f31c028cd32511865d9b4377790afc32485c5d30387adc29f6007cdf70df7f.jpg
+-rw-r--r--   0        0        0    64881 2023-12-20 18:56:01.000000 das-0.32.2/docs/jupyter_execute/3594e0999cf561fa210f5aa128dc8c1bdf1cd54cfc522303870b7ac0996d6d81.jpg
+-rw-r--r--   0        0        0    69902 2023-12-20 18:56:02.000000 das-0.32.2/docs/jupyter_execute/36e975676dc3c37f488f6a644a09d8b0f059858482001b8b13a7a2a830677a7a.jpg
+-rw-r--r--   0        0        0    36118 2023-12-20 18:56:01.000000 das-0.32.2/docs/jupyter_execute/411ad01b915cabb08f441d57ed6c1395642c93fdba43c5ab6a3664995bb157ab.jpg
+-rw-r--r--   0        0        0   133684 2023-12-20 18:56:01.000000 das-0.32.2/docs/jupyter_execute/42e6d26af2159c983a442fa87ce71bc8d4af03073a37f56384a0f6aa07bccd4b.jpg
+-rw-r--r--   0        0        0    74310 2023-12-20 18:56:02.000000 das-0.32.2/docs/jupyter_execute/51ad2dee4a168546bfaf845facb661b5f4436899bd96e179ff9ea85aca33ae9c.png
+-rw-r--r--   0        0        0    15662 2023-12-20 18:56:01.000000 das-0.32.2/docs/jupyter_execute/5334ee66c97affed7823118c36b355c37407fbaaa038895e0872fe8090ce816a.jpg
+-rw-r--r--   0        0        0    87812 2023-12-20 18:56:01.000000 das-0.32.2/docs/jupyter_execute/59e6ffa2a5eeba3ca1f8907236c54231658e8f1b0a9a792d95781be7d5b8c1fd.png
+-rw-r--r--   0        0        0    16787 2023-12-20 18:56:01.000000 das-0.32.2/docs/jupyter_execute/6f8b4b2ebfcd0679a3727b0192658ca56d59490c9c0362db4d3cea0224fd2429.jpg
+-rw-r--r--   0        0        0    25664 2023-12-20 18:56:02.000000 das-0.32.2/docs/jupyter_execute/7270f0505dfe5c4c4083e0aa090c5ddf270ca488482cda44c8b6c315075f226f.jpg
+-rw-r--r--   0        0        0   131884 2023-12-20 18:56:02.000000 das-0.32.2/docs/jupyter_execute/72cd6540b8d8c6b5fd1039cfe919928abc36b30a1f5e220e687cd807fe104fcc.jpg
+-rw-r--r--   0        0        0   103999 2023-12-20 18:56:02.000000 das-0.32.2/docs/jupyter_execute/7876649fe14736f36ea3121f36405b25aa875478aa7bfdd42fa94e78abe45ceb.jpg
+-rw-r--r--   0        0        0    21164 2023-12-20 18:56:01.000000 das-0.32.2/docs/jupyter_execute/7962da1c27c61360e1c35f7f230b67c31fe8dfe3fefeb90e1e63d25c2865a2ce.jpg
+-rw-r--r--   0        0        0    11245 2023-12-20 18:56:01.000000 das-0.32.2/docs/jupyter_execute/8866e0d0472b30efbee828d80f76edc46540e0bb8ac2fb22e0e38319c5287c3c.jpg
+-rw-r--r--   0        0        0    29388 2023-12-20 18:56:02.000000 das-0.32.2/docs/jupyter_execute/8aa7e22a172f489f402d455824660ee508d1837b7b4e209d2e2374fd0443f39a.jpg
+-rw-r--r--   0        0        0    79037 2023-12-20 18:56:02.000000 das-0.32.2/docs/jupyter_execute/9a879c388a68d6b65ccfd5b822a225ff9453cf3c1647ae1c3e5e6813ef9b5a83.jpg
+-rw-r--r--   0        0        0   146245 2023-12-20 18:56:02.000000 das-0.32.2/docs/jupyter_execute/a0597b24513779a6876e1003b3c0aee8bb6693276d5901190b86a2efa59e42de.jpg
+-rw-r--r--   0        0        0    12151 2023-12-20 18:56:01.000000 das-0.32.2/docs/jupyter_execute/a6f5b756241918250a1f5e8a45f2cc509c003233ff7eaaf5870f0c5ca62b7473.jpg
+-rw-r--r--   0        0        0   190352 2023-12-20 18:56:02.000000 das-0.32.2/docs/jupyter_execute/b5b6635b8c13e3b79594f06a6bd2c4fca4781f6810494c4286fc7b2aca32f2d1.jpg
+-rw-r--r--   0        0        0    14654 2023-12-20 18:56:02.000000 das-0.32.2/docs/jupyter_execute/b919c302a83f2ef38e79ccbb5c939bb0f5336a657168bc9b2e010da4cd1d56cd.jpg
+-rw-r--r--   0        0        0    25292 2023-12-20 18:56:01.000000 das-0.32.2/docs/jupyter_execute/bd4feef74fd6786267ce2fc20695be861a5c06f7e4b973ee72c6ba79292d6f5d.jpg
+-rw-r--r--   0        0        0    33580 2023-12-20 18:56:02.000000 das-0.32.2/docs/jupyter_execute/c3b46f8cc6ce88b46b7b54dec7c7182ca88ccb66249098a0101904dab6e2ee05.png
+-rw-r--r--   0        0        0    69718 2023-12-20 18:56:02.000000 das-0.32.2/docs/jupyter_execute/d9ecc34617ef75d86ce90957aca0103c23f426fdcf89347c7780d7528c30a00a.png
+-rw-r--r--   0        0        0    86769 2023-12-20 18:56:02.000000 das-0.32.2/docs/jupyter_execute/e3eb93d28f5c2028549805bd3181ff21fea996bb882fe6a99c80a2506f68339f.jpg
+-rw-r--r--   0        0        0    59110 2023-12-20 18:56:02.000000 das-0.32.2/docs/jupyter_execute/eb4201de71c8575059afc78398a57c865d785ca997ac7f55fb269ab8d605e524.jpg
+-rw-r--r--   0        0        0    52009 2023-12-20 18:56:01.000000 das-0.32.2/docs/jupyter_execute/fe1262a9629ae4f353920933ba7773c9101afee6ae8ab2c3e6f14199ca7be0b6.png
+-rw-r--r--   0        0        0    37136 2023-12-20 18:56:01.000000 das-0.32.2/docs/jupyter_execute/technical/cli.ipynb
+-rw-r--r--   0        0        0   267513 2023-12-20 18:56:01.000000 das-0.32.2/docs/jupyter_execute/tutorials/colab.ipynb
+-rw-r--r--   0        0        0     5129 2023-12-20 18:56:01.000000 das-0.32.2/docs/jupyter_execute/tutorials/continue_training.ipynb
+-rw-r--r--   0        0        0   246982 2023-12-20 18:56:01.000000 das-0.32.2/docs/jupyter_execute/tutorials/evaluate_bird.ipynb
+-rw-r--r--   0        0        0   373096 2023-12-20 18:56:01.000000 das-0.32.2/docs/jupyter_execute/tutorials/evaluate_fly.ipynb
+-rw-r--r--   0        0        0   360089 2023-12-20 18:56:02.000000 das-0.32.2/docs/jupyter_execute/tutorials/inspect_dataset.ipynb
+-rw-r--r--   0        0        0    70067 2023-12-20 18:56:02.000000 das-0.32.2/docs/jupyter_execute/tutorials/make_ds_notebook.ipynb
+-rw-r--r--   0        0        0   140002 2023-12-20 18:56:02.000000 das-0.32.2/docs/jupyter_execute/tutorials/predict.ipynb
+-rw-r--r--   0        0        0   193820 2023-12-20 18:56:02.000000 das-0.32.2/docs/jupyter_execute/tutorials/realtime.ipynb
+-rw-r--r--   0        0        0    56475 2023-12-20 18:56:02.000000 das-0.32.2/docs/jupyter_execute/tutorials/train.ipynb
+-rw-r--r--   0        0        0      981 2023-12-20 18:56:02.000000 das-0.32.2/docs/jupyter_execute/tutorials/tuning.ipynb
+-rw-r--r--   0        0        0   617950 2023-12-20 18:56:02.000000 das-0.32.2/docs/jupyter_execute/unsupervised/birds.ipynb
+-rw-r--r--   0        0        0   200095 2023-12-20 18:56:02.000000 das-0.32.2/docs/jupyter_execute/unsupervised/flies.ipynb
+-rw-r--r--   0        0        0   719003 2023-12-20 18:56:02.000000 das-0.32.2/docs/jupyter_execute/unsupervised/mice.ipynb
+-rw-r--r--   0        0        0      795 2021-08-12 19:27:18.000000 das-0.32.2/docs/make.bat
+-rw-r--r--   0        0        0     1068 2021-08-15 15:00:19.000000 das-0.32.2/docs/make_api_doctree.py
+-rw-r--r--   0        0        0     9775 2023-01-08 09:32:51.000000 das-0.32.2/docs/quickstart_bird.md
+-rw-r--r--   0        0        0    11856 2023-01-08 09:28:27.000000 das-0.32.2/docs/quickstart_fly.md
+-rw-r--r--   0        0        0    37137 2022-09-18 16:59:07.000000 das-0.32.2/docs/technical/cli.ipynb
+-rw-r--r--   0        0        0     7137 2022-02-18 11:19:41.000000 das-0.32.2/docs/technical/data_formats.md
+-rw-r--r--   0        0        0      840 2021-11-11 20:17:52.000000 das-0.32.2/docs/technical/installation_apple-arm.md
+-rw-r--r--   0        0        0      254 2021-08-23 13:21:25.000000 das-0.32.2/docs/technical/technical.rst
+-rw-r--r--   0        0        0      144 2022-01-14 14:23:10.000000 das-0.32.2/docs/tracking/fixing_identities.md
+-rw-r--r--   0        0        0     3153 2022-09-19 13:10:08.000000 das-0.32.2/docs/tutorials/architecture_tuning.md
+-rw-r--r--   0        0        0   267514 2021-09-25 13:47:07.000000 das-0.32.2/docs/tutorials/colab.ipynb
+-rw-r--r--   0        0        0     5152 2022-06-09 10:37:23.000000 das-0.32.2/docs/tutorials/continue_training.ipynb
+-rw-r--r--   0        0        0     5929 2022-02-18 11:14:07.000000 das-0.32.2/docs/tutorials/convert.md
+-rw-r--r--   0        0        0   246983 2021-09-25 13:50:30.000000 das-0.32.2/docs/tutorials/evaluate_bird.ipynb
+-rw-r--r--   0        0        0   373097 2022-09-25 17:24:36.000000 das-0.32.2/docs/tutorials/evaluate_fly.ipynb
+-rw-r--r--   0        0        0     1131 2022-09-18 17:21:36.000000 das-0.32.2/docs/tutorials/experiment_tracking.md
+-rwxr-xr-x   0        0        0   360090 2021-09-25 12:38:04.000000 das-0.32.2/docs/tutorials/inspect_dataset.ipynb
+-rw-r--r--   0        0        0      127 2020-12-07 15:26:25.000000 das-0.32.2/docs/tutorials/label_segments.md
+-rw-r--r--   0        0        0    70068 2021-09-25 12:36:01.000000 das-0.32.2/docs/tutorials/make_ds_notebook.ipynb
+-rwxr-xr-x   0        0        0      982 2020-03-18 12:54:18.000000 das-0.32.2/docs/tutorials/ncb.mplstyle
+-rw-r--r--   0        0        0   140003 2022-07-25 11:04:46.000000 das-0.32.2/docs/tutorials/predict.ipynb
+-rwxr-xr-x   0        0        0   193821 2022-09-18 16:29:29.000000 das-0.32.2/docs/tutorials/realtime.ipynb
+-rw-r--r--   0        0        0     5617 2021-09-25 11:24:45.000000 das-0.32.2/docs/tutorials/structparams.md
+-rw-r--r--   0        0        0    56476 2021-09-24 20:23:03.000000 das-0.32.2/docs/tutorials/train.ipynb
+-rw-r--r--   0        0        0     1004 2023-10-10 14:21:46.471524 das-0.32.2/docs/tutorials/tuning.ipynb
+-rw-r--r--   0        0        0     1159 2022-12-27 21:36:14.000000 das-0.32.2/docs/tutorials/tutorials.rst
+-rw-r--r--   0        0        0     5974 2022-07-25 11:01:30.000000 das-0.32.2/docs/tutorials_gui/annotate.md
+-rw-r--r--   0        0        0     4694 2024-02-23 19:41:54.000000 das-0.32.2/docs/tutorials_gui/load.md
+-rw-r--r--   0        0        0     3076 2021-09-25 16:14:59.000000 das-0.32.2/docs/tutorials_gui/predict.md
+-rw-r--r--   0        0        0    10092 2022-12-27 21:42:37.000000 das-0.32.2/docs/tutorials_gui/train.md
+-rw-r--r--   0        0        0      482 2023-01-25 15:03:24.000000 das-0.32.2/docs/tutorials_gui/tutorials_gui.rst
+-rw-r--r--   0        0        0   738598 2020-09-22 10:35:48.000000 das-0.32.2/docs/unsupervised/banner.png
+-rw-r--r--   0        0        0   621476 2021-09-24 08:39:06.000000 das-0.32.2/docs/unsupervised/birds.ipynb
+-rw-r--r--   0        0        0   200988 2021-09-24 08:27:06.000000 das-0.32.2/docs/unsupervised/flies.ipynb
+-rwxr-xr-x   0        0        0   720771 2021-09-24 08:22:18.000000 das-0.32.2/docs/unsupervised/mice.ipynb
+-rwxr-xr-x   0        0        0      982 2020-03-18 12:54:18.000000 das-0.32.2/docs/unsupervised/ncb.mplstyle
+-rw-r--r--   0        0        0     3584 2021-09-25 12:25:43.000000 das-0.32.2/docs/unsupervised/unsupervised.rst
+-rw-r--r--   0        0        0      794 2022-12-21 08:31:00.000000 das-0.32.2/pyproject.toml
+-rw-r--r--   0        0        0      572 2023-09-02 09:15:46.000000 das-0.32.2/setup.py
+-rw-r--r--   0        0        0       33 2024-03-14 15:06:15.192338 das-0.32.2/src/das/__init__.py
+-rw-r--r--   0        0        0    16462 2023-01-10 07:09:56.000000 das-0.32.2/src/das/annot.py
+-rw-r--r--   0        0        0    11666 2023-01-10 07:09:56.000000 das-0.32.2/src/das/augmentation.py
+-rw-r--r--   0        0        0     6598 2023-04-18 06:59:16.000000 das-0.32.2/src/das/block_stratify.py
+-rw-r--r--   0        0        0     2990 2024-01-02 08:56:17.000000 das-0.32.2/src/das/cli.py
+-rw-r--r--   0        0        0    13390 2023-12-15 13:43:09.000000 das-0.32.2/src/das/data.py
+-rw-r--r--   0        0        0     1758 2023-01-10 07:09:55.000000 das-0.32.2/src/das/data_hash.py
+-rw-r--r--   0        0        0     7765 2024-01-01 20:17:00.000000 das-0.32.2/src/das/evaluate.py
+-rw-r--r--   0        0        0     6594 2024-01-01 20:16:39.000000 das-0.32.2/src/das/event_utils.py
+-rw-r--r--   0        0        0     2935 2023-05-13 17:02:40.000000 das-0.32.2/src/das/io.py
+-rw-r--r--   0        0        0     1069 2022-03-01 17:05:15.000000 das-0.32.2/src/das/kapre/LICENSE.txt
+-rw-r--r--   0        0        0    12759 2022-03-01 17:05:15.000000 das-0.32.2/src/das/kapre/README.md
+-rw-r--r--   0        0        0      237 2023-01-10 07:09:55.000000 das-0.32.2/src/das/kapre/__init__.py
+-rw-r--r--   0        0        0     1520 2023-01-10 07:09:55.000000 das-0.32.2/src/das/kapre/augmentation.py
+-rw-r--r--   0        0        0     4751 2023-01-10 07:09:56.000000 das-0.32.2/src/das/kapre/backend.py
+-rw-r--r--   0        0        0     1076 2022-03-01 17:05:15.000000 das-0.32.2/src/das/kapre/backend_keras.py
+-rw-r--r--   0        0        0     4786 2023-01-10 07:09:56.000000 das-0.32.2/src/das/kapre/filterbank.py
+-rw-r--r--   0        0        0    14067 2023-04-18 06:59:17.000000 das-0.32.2/src/das/kapre/time_frequency.py
+-rw-r--r--   0        0        0     5159 2023-01-10 07:09:56.000000 das-0.32.2/src/das/kapre/utils.py
+-rw-r--r--   0        0        0    11601 2024-01-01 20:16:53.000000 das-0.32.2/src/das/make_dataset.py
+-rw-r--r--   0        0        0     2340 2023-01-10 07:09:56.000000 das-0.32.2/src/das/menagerie.py
+-rw-r--r--   0        0        0    15505 2024-01-11 20:03:42.000000 das-0.32.2/src/das/models.py
+-rw-r--r--   0        0        0    30534 2023-02-12 09:24:43.000000 das-0.32.2/src/das/models_legacy.py
+-rwxr-xr-x   0        0        0     1080 2023-12-20 18:49:39.000000 das-0.32.2/src/das/morpholayers/LICENSE
+-rwxr-xr-x   0        0        0     2706 2023-12-20 18:49:39.000000 das-0.32.2/src/das/morpholayers/README.md
+-rwxr-xr-x   0        0        0       97 2023-12-20 18:49:39.000000 das-0.32.2/src/das/morpholayers/__init__.py
+-rwxr-xr-x   0        0        0     5607 2023-12-20 18:59:48.000000 das-0.32.2/src/das/morpholayers/constraints.py
+-rwxr-xr-x   0        0        0     6183 2023-12-20 19:04:50.000000 das-0.32.2/src/das/morpholayers/initializers.py
+-rwxr-xr-x   0        0        0   152836 2024-01-11 19:51:30.000000 das-0.32.2/src/das/morpholayers/layers.py
+-rwxr-xr-x   0        0        0     1926 2024-01-11 19:47:31.000000 das-0.32.2/src/das/morpholayers/regularizers.py
+-rw-r--r--   0        0        0     4030 2023-05-18 07:45:17.000000 das-0.32.2/src/das/npy_dir.py
+-rw-r--r--   0        0        0     5422 2023-01-10 07:09:56.000000 das-0.32.2/src/das/postprocessing.py
+-rw-r--r--   0        0        0    32162 2024-03-14 15:06:33.504476 das-0.32.2/src/das/predict.py
+-rw-r--r--   0        0        0     3948 2023-02-12 09:24:43.000000 das-0.32.2/src/das/pulse_utils.py
+-rw-r--r--   0        0        0     4881 2023-12-25 13:19:27.000000 das-0.32.2/src/das/segment_utils.py
+-rw-r--r--   0        0        0     3081 2023-01-10 07:09:56.000000 das-0.32.2/src/das/spec_utils.py
+-rwxr-xr-x   0        0        0     1071 2022-03-01 17:05:15.000000 das-0.32.2/src/das/tcn/LICENSE
+-rwxr-xr-x   0        0        0    11264 2022-03-01 17:05:15.000000 das-0.32.2/src/das/tcn/README.md
+-rw-r--r--   0        0        0       80 2023-01-10 07:09:56.000000 das-0.32.2/src/das/tcn/__init__.py
+-rw-r--r--   0        0        0     6581 2023-02-12 09:24:43.000000 das-0.32.2/src/das/tcn/tcn.py
+-rw-r--r--   0        0        0    16153 2023-04-18 06:59:17.000000 das-0.32.2/src/das/tcn/tcn_new.py
+-rw-r--r--   0        0        0     3125 2023-01-10 07:09:56.000000 das-0.32.2/src/das/tracking.py
+-rw-r--r--   0        0        0    24727 2024-01-12 09:08:13.000000 das-0.32.2/src/das/train.py
+-rw-r--r--   0        0        0    22517 2023-02-12 09:24:43.000000 das-0.32.2/src/das/train_tune.py
+-rw-r--r--   0        0        0     9062 2023-01-25 09:52:34.000000 das-0.32.2/src/das/utils.py
+-rw-r--r--   0        0        0    16870 2023-05-21 13:30:50.000000 das-0.32.2/src/das/utils_plot.py
+-rw-r--r--   0        0        0     2557 2021-12-16 19:07:36.000000 das-0.32.2/tests/test_augmentation.py
+-rw-r--r--   0        0        0      162 2023-10-10 14:20:26.420845 das-0.32.2/tests/test_cli.py
+-rw-r--r--   0        0        0      725 2023-10-10 14:20:33.000000 das-0.32.2/tests/test_import.py
+-rw-r--r--   0        0        0     4425 1970-01-01 00:00:00.000000 das-0.32.2/PKG-INFO
```

### Comparing `das-0.32.1/.github/workflows/publish.yml` & `das-0.32.2/.github/workflows/publish.yml`

 * *Files 0% similar despite different names*

```diff
@@ -15,18 +15,18 @@
 
 jobs:
   publish:
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: False
       matrix:
-        # python-version: [3.9, '3.10']
-        # os: [ubuntu-latest, windows-latest, macOS-13, macOS-14]
-        python-version: ['3.10']
-        os: [windows-latest]
+        python-version: [3.9, '3.10']
+        os: [ubuntu-latest, windows-latest, macOS-13, macOS-14]
+        # python-version: ['3.10']
+        # os: [windows-latest]
     defaults:  # https://github.com/marketplace/actions/setup-miniconda#use-a-default-shell
       run:
         shell: bash -l {0}
     steps:
     - uses: actions/checkout@v3
     - name: Setup miniconda # https://github.com/marketplace/actions/setup-miniconda
       uses: conda-incubator/setup-miniconda@v3
```

### Comparing `das-0.32.1/.github/workflows/test.yml` & `das-0.32.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `das-0.32.1/.gitignore` & `das-0.32.2/.gitignore`

 * *Files identical despite different names*

### Comparing `das-0.32.1/README.md` & `das-0.32.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -31,21 +31,21 @@
 
 ### Install _DAS_
 Create an anaconda environment called `das` that contains all the required packages.
 
 On windows:
 ```shell
 conda install mamba -c conda-forge -n base -y
-mamba create python=3.9 das=0.32.0 "numpy<1.24" -c conda-forge -c ncb -c anaconda -c nvidia -n das -y
+mamba create python=3.9 das=0.32.2 "numpy<1.24" -c conda-forge -c ncb -c anaconda -c nvidia -n das -y
 ```
 
 On Linux or MacOS (intel and arm):
 ```shell
 conda install mamba -c conda-forge -n base -y
-mamba create python=3.10 das=0.32.0 -c conda-forge -c ncb -c anaconda -c nvidia -c apple -n das -y
+mamba create python=3.10 das=0.32.2 -c conda-forge -c ncb -c anaconda -c nvidia -c apple -n das -y
 ```
 
 ## Usage
 To start the graphical user interface:
 ```shell
 conda activate das
 das gui
```

### Comparing `das-0.32.1/colab/colab.ipynb` & `das-0.32.2/colab/colab.ipynb`

 * *Files identical despite different names*

### Comparing `das-0.32.1/conda/das-osxarm/build.sh` & `das-0.32.2/conda/das-osxarm/build.sh`

 * *Files identical despite different names*

### Comparing `das-0.32.1/conda/das-osxarm/meta.yaml` & `das-0.32.2/conda/das-osxarm/meta.yaml`

 * *Files identical despite different names*

### Comparing `das-0.32.1/conda/das-test/meta.yaml` & `das-0.32.2/conda/das-test/meta.yaml`

 * *Files identical despite different names*

### Comparing `das-0.32.1/conda/das/meta.yaml` & `das-0.32.2/conda/das/meta.yaml`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/Makefile` & `das-0.32.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/README.md` & `das-0.32.2/docs/README.md`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/api.rst` & `das-0.32.2/docs/api.rst`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/conf.py` & `das-0.32.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/index.rst` & `das-0.32.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/installation.md` & `das-0.32.2/docs/installation.md`

 * *Files 1% similar despite different names*

```diff
@@ -10,21 +10,21 @@
 
 ## Install _DAS_
 Create an anaconda environment called `das` that contains all the required packages.
 
 On windows
 ```shell
 conda install mamba -c conda-forge -n base -y
-mamba create python=3.9 das=0.32.0 "numpy<1.24" -c conda-forge -c ncb -c anaconda -c nvidia -n das -y
+mamba create python=3.9 das=0.32.2 "numpy<1.24" -c conda-forge -c ncb -c anaconda -c nvidia -n das -y
 ```
 
 On Linux or MacOS (intel and arm):
 ```shell
 conda install mamba -c conda-forge -n base -y
-mamba create python=3.10 das=0.32.0 -c conda-forge -c ncb -c anaconda -c nvidia -c apple -n das -y
+mamba create python=3.10 das=0.32.2 -c conda-forge -c ncb -c anaconda -c nvidia -c apple -n das -y
 ```
 
 
 ## Test the installation (Optional)
 To quickly test the installation, run these  commands in the terminal:
 ```shell
 conda activate das  # activate the conda environment
```

### Comparing `das-0.32.1/docs/jupyter_execute/00b86cf553e61db9b1d9039084ecb3de176c5128f74e1d9cbf226df4fd4b098c.jpg` & `das-0.32.2/docs/jupyter_execute/00b86cf553e61db9b1d9039084ecb3de176c5128f74e1d9cbf226df4fd4b098c.jpg`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/jupyter_execute/05bb23a35be292dacca29115895aa30b477b3702733812dc88eedec9108561fd.png` & `das-0.32.2/docs/jupyter_execute/05bb23a35be292dacca29115895aa30b477b3702733812dc88eedec9108561fd.png`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/jupyter_execute/0f4e455010d95626191b2c7cf3b5bb49f9aeaa9a4b91c3d3a77728209e542b28.jpg` & `das-0.32.2/docs/jupyter_execute/0f4e455010d95626191b2c7cf3b5bb49f9aeaa9a4b91c3d3a77728209e542b28.jpg`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/jupyter_execute/0f87b4789d1dea68deb5dbd5c8169c3307774631e0c4720e8230b5bf13ceb4ab.jpg` & `das-0.32.2/docs/jupyter_execute/0f87b4789d1dea68deb5dbd5c8169c3307774631e0c4720e8230b5bf13ceb4ab.jpg`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/jupyter_execute/1003c63cf4d33f7a19fa2966dbb8efaebbb8cded2d1f307be357976833342305.jpg` & `das-0.32.2/docs/jupyter_execute/1003c63cf4d33f7a19fa2966dbb8efaebbb8cded2d1f307be357976833342305.jpg`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/jupyter_execute/15961ee4ef682feb0773b21475bcaf9571ce3cbffdcdb03e80c24b12e8c1433d.jpg` & `das-0.32.2/docs/jupyter_execute/15961ee4ef682feb0773b21475bcaf9571ce3cbffdcdb03e80c24b12e8c1433d.jpg`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/jupyter_execute/18f69ae6eccfcaef9677e0db0e0223dcf2011fdc33c3c65f17dcf5b56f154725.jpg` & `das-0.32.2/docs/jupyter_execute/18f69ae6eccfcaef9677e0db0e0223dcf2011fdc33c3c65f17dcf5b56f154725.jpg`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/jupyter_execute/1f70d964adae8f5937528754bfbf018926b44f563247167c283ba3d6ec6912af.jpg` & `das-0.32.2/docs/jupyter_execute/1f70d964adae8f5937528754bfbf018926b44f563247167c283ba3d6ec6912af.jpg`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/jupyter_execute/2d19a4031347cfcde5655f0dcfceefec27aaf73fcc741ab1ab0195ccd943b251.png` & `das-0.32.2/docs/jupyter_execute/2d19a4031347cfcde5655f0dcfceefec27aaf73fcc741ab1ab0195ccd943b251.png`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/jupyter_execute/30eacca7324ff8d5eb2b8a221da4d1e31e83a9da73b5f02656c038110f164fc5.jpg` & `das-0.32.2/docs/jupyter_execute/30eacca7324ff8d5eb2b8a221da4d1e31e83a9da73b5f02656c038110f164fc5.jpg`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/jupyter_execute/31f31c028cd32511865d9b4377790afc32485c5d30387adc29f6007cdf70df7f.jpg` & `das-0.32.2/docs/jupyter_execute/31f31c028cd32511865d9b4377790afc32485c5d30387adc29f6007cdf70df7f.jpg`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/jupyter_execute/3594e0999cf561fa210f5aa128dc8c1bdf1cd54cfc522303870b7ac0996d6d81.jpg` & `das-0.32.2/docs/jupyter_execute/3594e0999cf561fa210f5aa128dc8c1bdf1cd54cfc522303870b7ac0996d6d81.jpg`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/jupyter_execute/36e975676dc3c37f488f6a644a09d8b0f059858482001b8b13a7a2a830677a7a.jpg` & `das-0.32.2/docs/jupyter_execute/36e975676dc3c37f488f6a644a09d8b0f059858482001b8b13a7a2a830677a7a.jpg`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/jupyter_execute/411ad01b915cabb08f441d57ed6c1395642c93fdba43c5ab6a3664995bb157ab.jpg` & `das-0.32.2/docs/jupyter_execute/411ad01b915cabb08f441d57ed6c1395642c93fdba43c5ab6a3664995bb157ab.jpg`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/jupyter_execute/42e6d26af2159c983a442fa87ce71bc8d4af03073a37f56384a0f6aa07bccd4b.jpg` & `das-0.32.2/docs/jupyter_execute/42e6d26af2159c983a442fa87ce71bc8d4af03073a37f56384a0f6aa07bccd4b.jpg`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/jupyter_execute/51ad2dee4a168546bfaf845facb661b5f4436899bd96e179ff9ea85aca33ae9c.png` & `das-0.32.2/docs/jupyter_execute/51ad2dee4a168546bfaf845facb661b5f4436899bd96e179ff9ea85aca33ae9c.png`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/jupyter_execute/5334ee66c97affed7823118c36b355c37407fbaaa038895e0872fe8090ce816a.jpg` & `das-0.32.2/docs/jupyter_execute/5334ee66c97affed7823118c36b355c37407fbaaa038895e0872fe8090ce816a.jpg`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/jupyter_execute/59e6ffa2a5eeba3ca1f8907236c54231658e8f1b0a9a792d95781be7d5b8c1fd.png` & `das-0.32.2/docs/jupyter_execute/59e6ffa2a5eeba3ca1f8907236c54231658e8f1b0a9a792d95781be7d5b8c1fd.png`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/jupyter_execute/6f8b4b2ebfcd0679a3727b0192658ca56d59490c9c0362db4d3cea0224fd2429.jpg` & `das-0.32.2/docs/jupyter_execute/6f8b4b2ebfcd0679a3727b0192658ca56d59490c9c0362db4d3cea0224fd2429.jpg`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/jupyter_execute/7270f0505dfe5c4c4083e0aa090c5ddf270ca488482cda44c8b6c315075f226f.jpg` & `das-0.32.2/docs/jupyter_execute/7270f0505dfe5c4c4083e0aa090c5ddf270ca488482cda44c8b6c315075f226f.jpg`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/jupyter_execute/72cd6540b8d8c6b5fd1039cfe919928abc36b30a1f5e220e687cd807fe104fcc.jpg` & `das-0.32.2/docs/jupyter_execute/72cd6540b8d8c6b5fd1039cfe919928abc36b30a1f5e220e687cd807fe104fcc.jpg`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/jupyter_execute/7876649fe14736f36ea3121f36405b25aa875478aa7bfdd42fa94e78abe45ceb.jpg` & `das-0.32.2/docs/jupyter_execute/7876649fe14736f36ea3121f36405b25aa875478aa7bfdd42fa94e78abe45ceb.jpg`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/jupyter_execute/7962da1c27c61360e1c35f7f230b67c31fe8dfe3fefeb90e1e63d25c2865a2ce.jpg` & `das-0.32.2/docs/jupyter_execute/7962da1c27c61360e1c35f7f230b67c31fe8dfe3fefeb90e1e63d25c2865a2ce.jpg`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/jupyter_execute/8866e0d0472b30efbee828d80f76edc46540e0bb8ac2fb22e0e38319c5287c3c.jpg` & `das-0.32.2/docs/jupyter_execute/8866e0d0472b30efbee828d80f76edc46540e0bb8ac2fb22e0e38319c5287c3c.jpg`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/jupyter_execute/8aa7e22a172f489f402d455824660ee508d1837b7b4e209d2e2374fd0443f39a.jpg` & `das-0.32.2/docs/jupyter_execute/8aa7e22a172f489f402d455824660ee508d1837b7b4e209d2e2374fd0443f39a.jpg`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/jupyter_execute/9a879c388a68d6b65ccfd5b822a225ff9453cf3c1647ae1c3e5e6813ef9b5a83.jpg` & `das-0.32.2/docs/jupyter_execute/9a879c388a68d6b65ccfd5b822a225ff9453cf3c1647ae1c3e5e6813ef9b5a83.jpg`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/jupyter_execute/a0597b24513779a6876e1003b3c0aee8bb6693276d5901190b86a2efa59e42de.jpg` & `das-0.32.2/docs/jupyter_execute/a0597b24513779a6876e1003b3c0aee8bb6693276d5901190b86a2efa59e42de.jpg`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/jupyter_execute/a6f5b756241918250a1f5e8a45f2cc509c003233ff7eaaf5870f0c5ca62b7473.jpg` & `das-0.32.2/docs/jupyter_execute/a6f5b756241918250a1f5e8a45f2cc509c003233ff7eaaf5870f0c5ca62b7473.jpg`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/jupyter_execute/b5b6635b8c13e3b79594f06a6bd2c4fca4781f6810494c4286fc7b2aca32f2d1.jpg` & `das-0.32.2/docs/jupyter_execute/b5b6635b8c13e3b79594f06a6bd2c4fca4781f6810494c4286fc7b2aca32f2d1.jpg`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/jupyter_execute/b919c302a83f2ef38e79ccbb5c939bb0f5336a657168bc9b2e010da4cd1d56cd.jpg` & `das-0.32.2/docs/jupyter_execute/b919c302a83f2ef38e79ccbb5c939bb0f5336a657168bc9b2e010da4cd1d56cd.jpg`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/jupyter_execute/bd4feef74fd6786267ce2fc20695be861a5c06f7e4b973ee72c6ba79292d6f5d.jpg` & `das-0.32.2/docs/jupyter_execute/bd4feef74fd6786267ce2fc20695be861a5c06f7e4b973ee72c6ba79292d6f5d.jpg`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/jupyter_execute/c3b46f8cc6ce88b46b7b54dec7c7182ca88ccb66249098a0101904dab6e2ee05.png` & `das-0.32.2/docs/jupyter_execute/c3b46f8cc6ce88b46b7b54dec7c7182ca88ccb66249098a0101904dab6e2ee05.png`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/jupyter_execute/d9ecc34617ef75d86ce90957aca0103c23f426fdcf89347c7780d7528c30a00a.png` & `das-0.32.2/docs/jupyter_execute/d9ecc34617ef75d86ce90957aca0103c23f426fdcf89347c7780d7528c30a00a.png`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/jupyter_execute/e3eb93d28f5c2028549805bd3181ff21fea996bb882fe6a99c80a2506f68339f.jpg` & `das-0.32.2/docs/jupyter_execute/e3eb93d28f5c2028549805bd3181ff21fea996bb882fe6a99c80a2506f68339f.jpg`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/jupyter_execute/eb4201de71c8575059afc78398a57c865d785ca997ac7f55fb269ab8d605e524.jpg` & `das-0.32.2/docs/jupyter_execute/eb4201de71c8575059afc78398a57c865d785ca997ac7f55fb269ab8d605e524.jpg`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/jupyter_execute/fe1262a9629ae4f353920933ba7773c9101afee6ae8ab2c3e6f14199ca7be0b6.png` & `das-0.32.2/docs/jupyter_execute/fe1262a9629ae4f353920933ba7773c9101afee6ae8ab2c3e6f14199ca7be0b6.png`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/jupyter_execute/technical/cli.ipynb` & `das-0.32.2/docs/jupyter_execute/technical/cli.ipynb`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/jupyter_execute/tutorials/colab.ipynb` & `das-0.32.2/docs/jupyter_execute/tutorials/colab.ipynb`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/jupyter_execute/tutorials/continue_training.ipynb` & `das-0.32.2/docs/jupyter_execute/tutorials/continue_training.ipynb`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/jupyter_execute/tutorials/evaluate_bird.ipynb` & `das-0.32.2/docs/jupyter_execute/tutorials/evaluate_bird.ipynb`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/jupyter_execute/tutorials/evaluate_fly.ipynb` & `das-0.32.2/docs/jupyter_execute/tutorials/evaluate_fly.ipynb`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/jupyter_execute/tutorials/inspect_dataset.ipynb` & `das-0.32.2/docs/jupyter_execute/tutorials/inspect_dataset.ipynb`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/jupyter_execute/tutorials/make_ds_notebook.ipynb` & `das-0.32.2/docs/jupyter_execute/tutorials/make_ds_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/jupyter_execute/tutorials/predict.ipynb` & `das-0.32.2/docs/jupyter_execute/tutorials/predict.ipynb`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/jupyter_execute/tutorials/realtime.ipynb` & `das-0.32.2/docs/jupyter_execute/tutorials/realtime.ipynb`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/jupyter_execute/tutorials/train.ipynb` & `das-0.32.2/docs/jupyter_execute/tutorials/train.ipynb`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/jupyter_execute/tutorials/tuning.ipynb` & `das-0.32.2/docs/jupyter_execute/tutorials/tuning.ipynb`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/jupyter_execute/unsupervised/birds.ipynb` & `das-0.32.2/docs/jupyter_execute/unsupervised/birds.ipynb`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/jupyter_execute/unsupervised/flies.ipynb` & `das-0.32.2/docs/jupyter_execute/unsupervised/flies.ipynb`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/jupyter_execute/unsupervised/mice.ipynb` & `das-0.32.2/docs/jupyter_execute/unsupervised/mice.ipynb`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/make.bat` & `das-0.32.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/make_api_doctree.py` & `das-0.32.2/docs/make_api_doctree.py`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/quickstart_bird.md` & `das-0.32.2/docs/quickstart_bird.md`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/quickstart_fly.md` & `das-0.32.2/docs/quickstart_fly.md`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/technical/cli.ipynb` & `das-0.32.2/docs/technical/cli.ipynb`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/technical/data_formats.md` & `das-0.32.2/docs/technical/data_formats.md`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/technical/installation_apple-arm.md` & `das-0.32.2/docs/technical/installation_apple-arm.md`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/tutorials/architecture_tuning.md` & `das-0.32.2/docs/tutorials/architecture_tuning.md`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/tutorials/colab.ipynb` & `das-0.32.2/docs/tutorials/colab.ipynb`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/tutorials/continue_training.ipynb` & `das-0.32.2/docs/tutorials/continue_training.ipynb`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/tutorials/convert.md` & `das-0.32.2/docs/tutorials/convert.md`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/tutorials/evaluate_bird.ipynb` & `das-0.32.2/docs/tutorials/evaluate_bird.ipynb`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/tutorials/evaluate_fly.ipynb` & `das-0.32.2/docs/tutorials/evaluate_fly.ipynb`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/tutorials/experiment_tracking.md` & `das-0.32.2/docs/tutorials/experiment_tracking.md`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/tutorials/inspect_dataset.ipynb` & `das-0.32.2/docs/tutorials/inspect_dataset.ipynb`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/tutorials/make_ds_notebook.ipynb` & `das-0.32.2/docs/tutorials/make_ds_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/tutorials/ncb.mplstyle` & `das-0.32.2/docs/tutorials/ncb.mplstyle`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/tutorials/predict.ipynb` & `das-0.32.2/docs/tutorials/predict.ipynb`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/tutorials/realtime.ipynb` & `das-0.32.2/docs/tutorials/realtime.ipynb`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/tutorials/structparams.md` & `das-0.32.2/docs/tutorials/structparams.md`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/tutorials/train.ipynb` & `das-0.32.2/docs/tutorials/train.ipynb`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/tutorials/tuning.ipynb` & `das-0.32.2/docs/tutorials/tuning.ipynb`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/tutorials/tutorials.rst` & `das-0.32.2/docs/tutorials/tutorials.rst`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/tutorials_gui/annotate.md` & `das-0.32.2/docs/tutorials_gui/annotate.md`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/tutorials_gui/load.md` & `das-0.32.2/docs/tutorials_gui/load.md`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/tutorials_gui/predict.md` & `das-0.32.2/docs/tutorials_gui/predict.md`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/tutorials_gui/train.md` & `das-0.32.2/docs/tutorials_gui/train.md`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/unsupervised/banner.png` & `das-0.32.2/docs/unsupervised/banner.png`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/unsupervised/birds.ipynb` & `das-0.32.2/docs/unsupervised/birds.ipynb`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/unsupervised/flies.ipynb` & `das-0.32.2/docs/unsupervised/flies.ipynb`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/unsupervised/mice.ipynb` & `das-0.32.2/docs/unsupervised/mice.ipynb`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/unsupervised/ncb.mplstyle` & `das-0.32.2/docs/unsupervised/ncb.mplstyle`

 * *Files identical despite different names*

### Comparing `das-0.32.1/docs/unsupervised/unsupervised.rst` & `das-0.32.2/docs/unsupervised/unsupervised.rst`

 * *Files identical despite different names*

### Comparing `das-0.32.1/pyproject.toml` & `das-0.32.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `das-0.32.1/setup.py` & `das-0.32.2/setup.py`

 * *Files identical despite different names*

### Comparing `das-0.32.1/src/das/annot.py` & `das-0.32.2/src/das/annot.py`

 * *Files identical despite different names*

### Comparing `das-0.32.1/src/das/augmentation.py` & `das-0.32.2/src/das/augmentation.py`

 * *Files identical despite different names*

### Comparing `das-0.32.1/src/das/block_stratify.py` & `das-0.32.2/src/das/block_stratify.py`

 * *Files identical despite different names*

### Comparing `das-0.32.1/src/das/cli.py` & `das-0.32.2/src/das/cli.py`

 * *Files identical despite different names*

### Comparing `das-0.32.1/src/das/data.py` & `das-0.32.2/src/das/data.py`

 * *Files identical despite different names*

### Comparing `das-0.32.1/src/das/data_hash.py` & `das-0.32.2/src/das/data_hash.py`

 * *Files identical despite different names*

### Comparing `das-0.32.1/src/das/evaluate.py` & `das-0.32.2/src/das/evaluate.py`

 * *Files identical despite different names*

### Comparing `das-0.32.1/src/das/event_utils.py` & `das-0.32.2/src/das/event_utils.py`

 * *Files identical despite different names*

### Comparing `das-0.32.1/src/das/io.py` & `das-0.32.2/src/das/io.py`

 * *Files identical despite different names*

### Comparing `das-0.32.1/src/das/kapre/LICENSE.txt` & `das-0.32.2/src/das/kapre/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `das-0.32.1/src/das/kapre/README.md` & `das-0.32.2/src/das/kapre/README.md`

 * *Files identical despite different names*

### Comparing `das-0.32.1/src/das/kapre/augmentation.py` & `das-0.32.2/src/das/kapre/augmentation.py`

 * *Files identical despite different names*

### Comparing `das-0.32.1/src/das/kapre/backend.py` & `das-0.32.2/src/das/kapre/backend.py`

 * *Files identical despite different names*

### Comparing `das-0.32.1/src/das/kapre/backend_keras.py` & `das-0.32.2/src/das/kapre/backend_keras.py`

 * *Files identical despite different names*

### Comparing `das-0.32.1/src/das/kapre/filterbank.py` & `das-0.32.2/src/das/kapre/filterbank.py`

 * *Files identical despite different names*

### Comparing `das-0.32.1/src/das/kapre/time_frequency.py` & `das-0.32.2/src/das/kapre/time_frequency.py`

 * *Files identical despite different names*

### Comparing `das-0.32.1/src/das/kapre/utils.py` & `das-0.32.2/src/das/kapre/utils.py`

 * *Files identical despite different names*

### Comparing `das-0.32.1/src/das/make_dataset.py` & `das-0.32.2/src/das/make_dataset.py`

 * *Files identical despite different names*

### Comparing `das-0.32.1/src/das/menagerie.py` & `das-0.32.2/src/das/menagerie.py`

 * *Files identical despite different names*

### Comparing `das-0.32.1/src/das/models.py` & `das-0.32.2/src/das/models.py`

 * *Files identical despite different names*

### Comparing `das-0.32.1/src/das/models_legacy.py` & `das-0.32.2/src/das/models_legacy.py`

 * *Files identical despite different names*

### Comparing `das-0.32.1/src/das/morpholayers/LICENSE` & `das-0.32.2/src/das/morpholayers/LICENSE`

 * *Files identical despite different names*

### Comparing `das-0.32.1/src/das/morpholayers/README.md` & `das-0.32.2/src/das/morpholayers/README.md`

 * *Files identical despite different names*

### Comparing `das-0.32.1/src/das/morpholayers/constraints.py` & `das-0.32.2/src/das/morpholayers/constraints.py`

 * *Files identical despite different names*

### Comparing `das-0.32.1/src/das/morpholayers/initializers.py` & `das-0.32.2/src/das/morpholayers/initializers.py`

 * *Files identical despite different names*

### Comparing `das-0.32.1/src/das/morpholayers/layers.py` & `das-0.32.2/src/das/morpholayers/layers.py`

 * *Files identical despite different names*

### Comparing `das-0.32.1/src/das/morpholayers/regularizers.py` & `das-0.32.2/src/das/morpholayers/regularizers.py`

 * *Files identical despite different names*

### Comparing `das-0.32.1/src/das/npy_dir.py` & `das-0.32.2/src/das/npy_dir.py`

 * *Files identical despite different names*

### Comparing `das-0.32.1/src/das/postprocessing.py` & `das-0.32.2/src/das/postprocessing.py`

 * *Files identical despite different names*

### Comparing `das-0.32.1/src/das/predict.py` & `das-0.32.2/src/das/predict.py`

 * *Files 0% similar despite different names*

```diff
@@ -539,15 +539,16 @@
         segment_minlen=segment_minlen,
         segment_fillgap=segment_fillgap,
     )
     if not save_memory:
         segments["probabilities"] = _to_np(segments["probabilities"])
         segments["samples"] = _to_np(segments["samples"])
         class_probabilities = _to_np(class_probabilities)
-    class_probabilities.temp_dir = temp_dir
+    else:
+        class_probabilities.temp_dir = temp_dir
     return events, segments, class_probabilities, params["class_names"]
 
 
 def _to_np(array):
     if isinstance(array, dask.array.core.Array):
         array = array.compute()
     return array
@@ -699,15 +700,16 @@
                 evt = annot.Events.from_predict(events, segments)
                 if save_filename is None:
                     save_filename = os.path.splitext(recording_filename)[0] + "_annotations.csv"
                 logging.info(f"   Saving results to {save_filename}.")
                 evt.to_df().to_csv(save_filename)
                 logging.info("Done.")
             # reset
-            temp_dir = class_probabilities.temp_dir
-            del class_probabilities
-            shutil.rmtree(temp_dir, ignore_errors=True)
-            print(os.path.exists(temp_dir))
+            if hasattr(class_probabilities, "temp_dir"):
+                temp_dir = class_probabilities.temp_dir
+                del class_probabilities
+                shutil.rmtree(temp_dir, ignore_errors=True)
+
             if os.path.isdir(path):
                 save_filename = None
         except Exception:
             logging.exception(f"Error processing file {recording_filename}.")
```

### Comparing `das-0.32.1/src/das/pulse_utils.py` & `das-0.32.2/src/das/pulse_utils.py`

 * *Files identical despite different names*

### Comparing `das-0.32.1/src/das/segment_utils.py` & `das-0.32.2/src/das/segment_utils.py`

 * *Files identical despite different names*

### Comparing `das-0.32.1/src/das/spec_utils.py` & `das-0.32.2/src/das/spec_utils.py`

 * *Files identical despite different names*

### Comparing `das-0.32.1/src/das/tcn/LICENSE` & `das-0.32.2/src/das/tcn/LICENSE`

 * *Files identical despite different names*

### Comparing `das-0.32.1/src/das/tcn/README.md` & `das-0.32.2/src/das/tcn/README.md`

 * *Files identical despite different names*

### Comparing `das-0.32.1/src/das/tcn/tcn.py` & `das-0.32.2/src/das/tcn/tcn.py`

 * *Files identical despite different names*

### Comparing `das-0.32.1/src/das/tcn/tcn_new.py` & `das-0.32.2/src/das/tcn/tcn_new.py`

 * *Files identical despite different names*

### Comparing `das-0.32.1/src/das/tracking.py` & `das-0.32.2/src/das/tracking.py`

 * *Files identical despite different names*

### Comparing `das-0.32.1/src/das/train.py` & `das-0.32.2/src/das/train.py`

 * *Files identical despite different names*

### Comparing `das-0.32.1/src/das/train_tune.py` & `das-0.32.2/src/das/train_tune.py`

 * *Files identical despite different names*

### Comparing `das-0.32.1/src/das/utils.py` & `das-0.32.2/src/das/utils.py`

 * *Files identical despite different names*

### Comparing `das-0.32.1/src/das/utils_plot.py` & `das-0.32.2/src/das/utils_plot.py`

 * *Files identical despite different names*

### Comparing `das-0.32.1/tests/test_augmentation.py` & `das-0.32.2/tests/test_augmentation.py`

 * *Files identical despite different names*

### Comparing `das-0.32.1/tests/test_import.py` & `das-0.32.2/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `das-0.32.1/PKG-INFO` & `das-0.32.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: das
-Version: 0.32.1
+Version: 0.32.2
 Summary: DAS
 Home-page: https://github.com/janclemenslab/das
 Author: Jan Clemens
 Author-email: clemensjan@googlemail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
@@ -60,21 +60,21 @@
 
 ### Install _DAS_
 Create an anaconda environment called `das` that contains all the required packages.
 
 On windows:
 ```shell
 conda install mamba -c conda-forge -n base -y
-mamba create python=3.9 das=0.32.0 "numpy<1.24" -c conda-forge -c ncb -c anaconda -c nvidia -n das -y
+mamba create python=3.9 das=0.32.2 "numpy<1.24" -c conda-forge -c ncb -c anaconda -c nvidia -n das -y
 ```
 
 On Linux or MacOS (intel and arm):
 ```shell
 conda install mamba -c conda-forge -n base -y
-mamba create python=3.10 das=0.32.0 -c conda-forge -c ncb -c anaconda -c nvidia -c apple -n das -y
+mamba create python=3.10 das=0.32.2 -c conda-forge -c ncb -c anaconda -c nvidia -c apple -n das -y
 ```
 
 ## Usage
 To start the graphical user interface:
 ```shell
 conda activate das
 das gui
```

