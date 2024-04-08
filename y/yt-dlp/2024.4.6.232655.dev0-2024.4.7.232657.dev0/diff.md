# Comparing `tmp/yt_dlp-2024.4.6.232655.dev0.tar.gz` & `tmp/yt_dlp-2024.4.7.232657.dev0.tar.gz`

## Comparing `yt_dlp-2024.4.6.232655.dev0.tar` & `yt_dlp-2024.4.7.232657.dev0.tar`

### file list

```diff
@@ -1,1183 +1,1183 @@
--rw-r--r--   0        0        0   421317 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/Changelog.md
--rw-r--r--   0        0        0   149513 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/README.txt
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/setup.cfg
--rw-r--r--   0        0        0    56260 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/supportedsites.md
--rw-r--r--   0        0        0   145072 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt-dlp.1
--rw-r--r--   0        0        0     6166 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/completions/bash/yt-dlp
--rw-r--r--   0        0        0    50103 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/completions/fish/yt-dlp.fish
--rw-r--r--   0        0        0     6272 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/completions/zsh/_yt-dlp
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/devscripts/__init__.py
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/devscripts/bash-completion.in
--rwxr-xr-x   0        0        0      854 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/devscripts/bash-completion.py
--rw-r--r--   0        0        0     6887 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/devscripts/changelog_override.json
--rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/devscripts/changelog_override.schema.json
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/devscripts/check-porn.py
--rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/devscripts/cli_to_api.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/devscripts/fish-completion.in
--rwxr-xr-x   0        0        0     1670 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/devscripts/fish-completion.py
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/devscripts/generate_aes_testdata.py
--rwxr-xr-x   0        0        0     2307 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/devscripts/install_deps.py
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/devscripts/lazy_load_template.py
--rw-r--r--   0        0        0    41043 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/devscripts/logo.ico
--rw-r--r--   0        0        0    18382 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/devscripts/make_changelog.py
--rwxr-xr-x   0        0        0      763 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/devscripts/make_contributing.py
--rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/devscripts/make_issue_template.py
--rw-r--r--   0        0        0     4541 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/devscripts/make_lazy_extractors.py
--rwxr-xr-x   0        0        0     2892 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/devscripts/make_readme.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/devscripts/make_supportedsites.py
--rw-r--r--   0        0        0     2875 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/devscripts/prepare_manpage.py
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/devscripts/run_tests.bat
--rwxr-xr-x   0        0        0     2082 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/devscripts/run_tests.py
--rwxr-xr-x   0        0        0      140 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/devscripts/run_tests.sh
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/devscripts/set-variant.py
--rwxr-xr-x   0        0        0     4849 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/devscripts/tomlparse.py
--rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/devscripts/update-version.py
--rwxr-xr-x   0        0        0      972 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/devscripts/update_changelog.py
--rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/devscripts/utils.py
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/devscripts/zsh-completion.in
--rwxr-xr-x   0        0        0     1381 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/devscripts/zsh-completion.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/test/__init__.py
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/test/conftest.py
--rw-r--r--   0        0        0    12759 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/test/helper.py
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/test/parameters.json
--rw-r--r--   0        0        0   100103 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/test/test_InfoExtractor.py
--rw-r--r--   0        0        0    57080 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/test/test_YoutubeDL.py
--rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/test/test_YoutubeDLCookieJar.py
--rw-r--r--   0        0        0     6862 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/test/test_aes.py
--rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/test/test_age_restriction.py
--rw-r--r--   0        0        0     6120 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/test/test_all_urls.py
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/test/test_cache.py
--rw-r--r--   0        0        0     4706 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/test/test_compat.py
--rw-r--r--   0        0        0     6721 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/test/test_config.py
--rw-r--r--   0        0        0    13665 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/test/test_cookies.py
--rwxr-xr-x   0        0        0    12247 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/test/test_download.py
--rw-r--r--   0        0        0     4887 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/test/test_downloader_external.py
--rw-r--r--   0        0        0     3307 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/test/test_downloader_http.py
--rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/test/test_execution.py
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/test/test_iqiyi_sdk_interpreter.py
--rw-r--r--   0        0        0    18408 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/test/test_jsinterp.py
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/test/test_netrc.py
--rw-r--r--   0        0        0    86601 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/test/test_networking.py
--rw-r--r--   0        0        0     7613 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/test/test_networking_utils.py
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/test/test_overwrites.py
--rw-r--r--   0        0        0     2766 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/test/test_plugins.py
--rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/test/test_post_hooks.py
--rw-r--r--   0        0        0    30542 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/test/test_postprocessors.py
--rw-r--r--   0        0        0    19659 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/test/test_socks.py
--rw-r--r--   0        0        0    17397 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/test/test_subtitles.py
--rw-r--r--   0        0        0    24248 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/test/test_traversal.py
--rw-r--r--   0        0        0    10649 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/test/test_update.py
--rw-r--r--   0        0        0    97398 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/test/test_utils.py
--rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/test/test_verbose_output.py
--rw-r--r--   0        0        0    16532 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/test/test_websockets.py
--rw-r--r--   0        0        0     2480 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/test/test_write_annotations.py.disabled
--rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/test/test_youtube_lists.py
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/test/test_youtube_misc.py
--rw-r--r--   0        0        0     9763 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/test/test_youtube_signature.py
--rw-r--r--   0        0        0     3176 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/test/testcert.pem
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/test/testdata/certificate/ca.crt
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/test/testdata/certificate/ca.key
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/test/testdata/certificate/ca.srl
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/test/testdata/certificate/client.crt
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/test/testdata/certificate/client.csr
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/test/testdata/certificate/client.key
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/test/testdata/certificate/clientencrypted.key
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/test/testdata/certificate/clientwithencryptedkey.crt
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/test/testdata/certificate/clientwithkey.crt
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/test/testdata/certificate/instructions.md
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/test/testdata/cookies/httponly_cookies.txt
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/test/testdata/cookies/malformed_cookies.txt
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/test/testdata/cookies/session_cookies.txt
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/test/testdata/f4m/custom_base_url.f4m
--rw-r--r--   0        0        0     3987 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/test/testdata/ism/ec-3_test.Manifest
--rw-r--r--   0        0        0    23179 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/test/testdata/ism/sintel.Manifest
--rw-r--r--   0        0        0     3286 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/test/testdata/m3u8/bipbop_16x9.m3u8
--rw-r--r--   0        0        0     6291 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/test/testdata/m3u8/img_bipbop_adv_example_fmp4.m3u8
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/test/testdata/mpd/float_duration.mpd
--rw-r--r--   0        0        0    10268 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/test/testdata/mpd/subtitles.mpd
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/test/testdata/mpd/unfragmented.mpd
--rw-r--r--   0        0        0    22374 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/test/testdata/mpd/urls_only.mpd
--rw-r--r--   0        0        0     3928 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/test/testdata/thumbnails/foo %d bar/foo_%d.webp
--rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/test/testdata/xspf/foo_xspf.xspf
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/test/testdata/yt_dlp_plugins/extractor/_ignore.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/test/testdata/yt_dlp_plugins/extractor/ignore.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/test/testdata/yt_dlp_plugins/extractor/normal.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/test/testdata/yt_dlp_plugins/postprocessor/normal.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/test/testdata/zipped_plugins/yt_dlp_plugins/extractor/zipped.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/test/testdata/zipped_plugins/yt_dlp_plugins/postprocessor/zipped.py
--rw-r--r--   0        0        0   210976 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/YoutubeDL.py
--rw-r--r--   0        0        0    47675 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/__init__.py
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/__main__.py
--rw-r--r--   0        0        0    22402 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/aes.py
--rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/cache.py
--rw-r--r--   0        0        0    54746 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/cookies.py
--rw-r--r--   0        0        0    34646 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/jsinterp.py
--rw-r--r--   0        0        0     5328 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/minicurses.py
--rw-r--r--   0        0        0    96530 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/options.py
--rw-r--r--   0        0        0     6358 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/plugins.py
--rw-r--r--   0        0        0     8943 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/socks.py
--rw-r--r--   0        0        0    24873 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/update.py
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/version.py
--rw-r--r--   0        0        0    11441 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/webvtt.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/__pyinstaller/__init__.py
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/__pyinstaller/hook-yt_dlp.py
--rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/compat/__init__.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/compat/_deprecated.py
--rw-r--r--   0        0        0     3976 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/compat/_legacy.py
--rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/compat/compat_utils.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/compat/functools.py
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/compat/imghdr.py
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/compat/shutil.py
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/compat/types.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/compat/urllib/__init__.py
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/compat/urllib/request.py
--rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/dependencies/Cryptodome.py
--rw-r--r--   0        0        0     2206 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/dependencies/__init__.py
--rw-r--r--   0        0        0     4497 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/downloader/__init__.py
--rw-r--r--   0        0        0    19180 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/downloader/common.py
--rw-r--r--   0        0        0     3620 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/downloader/dash.py
--rw-r--r--   0        0        0    28090 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/downloader/external.py
--rw-r--r--   0        0        0    15344 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/downloader/f4m.py
--rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/downloader/fc2.py
--rw-r--r--   0        0        0    21795 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/downloader/fragment.py
--rw-r--r--   0        0        0    17819 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/downloader/hls.py
--rw-r--r--   0        0        0    16863 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/downloader/http.py
--rw-r--r--   0        0        0    11644 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/downloader/ism.py
--rw-r--r--   0        0        0     6182 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/downloader/mhtml.py
--rw-r--r--   0        0        0     5387 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/downloader/niconico.py
--rw-r--r--   0        0        0     8923 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/downloader/rtmp.py
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/downloader/rtsp.py
--rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/downloader/websocket.py
--rw-r--r--   0        0        0    10873 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/downloader/youtube_live_chat.py
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/__init__.py
--rw-r--r--   0        0        0    52856 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/_extractors.py
--rw-r--r--   0        0        0    17696 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/abc.py
--rw-r--r--   0        0        0     6328 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/abcnews.py
--rw-r--r--   0        0        0     4596 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/abcotvs.py
--rw-r--r--   0        0        0    19939 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/abematv.py
--rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/academicearth.py
--rw-r--r--   0        0        0     5571 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/acast.py
--rw-r--r--   0        0        0     7946 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/acfun.py
--rw-r--r--   0        0        0    14123 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/adn.py
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/adobeconnect.py
--rw-r--r--   0        0        0    52679 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/adobepass.py
--rw-r--r--   0        0        0    10277 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/adobetv.py
--rw-r--r--   0        0        0     7833 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/adultswim.py
--rw-r--r--   0        0        0    13304 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/aenetworks.py
--rw-r--r--   0        0        0     3299 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/aeonco.py
--rw-r--r--   0        0        0    15841 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/afreecatv.py
--rw-r--r--   0        0        0     9821 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/agora.py
--rw-r--r--   0        0        0     4085 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/airtv.py
--rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/aitube.py
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/aliexpress.py
--rw-r--r--   0        0        0     3364 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/aljazeera.py
--rw-r--r--   0        0        0     4803 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/allocine.py
--rw-r--r--   0        0        0     9202 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/allstar.py
--rw-r--r--   0        0        0     2683 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/alphaporno.py
--rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/alsace20tv.py
--rw-r--r--   0        0        0     3976 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/altcensored.py
--rw-r--r--   0        0        0     6501 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/alura.py
--rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/amadeustv.py
--rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/amara.py
--rw-r--r--   0        0        0     6589 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/amazon.py
--rw-r--r--   0        0        0    10729 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/amazonminitv.py
--rw-r--r--   0        0        0     6154 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/amcnetworks.py
--rw-r--r--   0        0        0     8724 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/americastestkitchen.py
--rw-r--r--   0        0        0     4225 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/amp.py
--rw-r--r--   0        0        0     4800 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/anchorfm.py
--rw-r--r--   0        0        0     2550 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/angel.py
--rw-r--r--   0        0        0     5967 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/antenna.py
--rw-r--r--   0        0        0    26757 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/anvato.py
--rw-r--r--   0        0        0     5467 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/aol.py
--rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/apa.py
--rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/aparat.py
--rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/appleconnect.py
--rw-r--r--   0        0        0     3624 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/applepodcasts.py
--rw-r--r--   0        0        0    10196 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/appletrailers.py
--rw-r--r--   0        0        0    46353 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/archiveorg.py
--rw-r--r--   0        0        0     7514 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/arcpublishing.py
--rw-r--r--   0        0        0    26748 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ard.py
--rw-r--r--   0        0        0     7199 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/arkena.py
--rw-r--r--   0        0        0     3556 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/arnes.py
--rw-r--r--   0        0        0    12859 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/art19.py
--rw-r--r--   0        0        0    14734 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/arte.py
--rw-r--r--   0        0        0     6806 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/asobichannel.py
--rw-r--r--   0        0        0     6974 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/asobistage.py
--rw-r--r--   0        0        0     4149 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/atresplayer.py
--rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/atscaleconf.py
--rw-r--r--   0        0        0     4179 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/atvat.py
--rw-r--r--   0        0        0     3929 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/audimedia.py
--rw-r--r--   0        0        0     2866 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/audioboom.py
--rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/audiodraft.py
--rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/audiomack.py
--rw-r--r--   0        0        0    10773 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/audius.py
--rw-r--r--   0        0        0     7133 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/awaan.py
--rw-r--r--   0        0        0     3121 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/aws.py
--rw-r--r--   0        0        0     3328 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/axs.py
--rw-r--r--   0        0        0     2424 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/azmedien.py
--rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/baidu.py
--rw-r--r--   0        0        0     6273 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/banbye.py
--rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/bandaichannel.py
--rw-r--r--   0        0        0    18597 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/bandcamp.py
--rw-r--r--   0        0        0     5303 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/bannedvideo.py
--rw-r--r--   0        0        0    72720 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/bbc.py
--rw-r--r--   0        0        0     4614 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/beatbump.py
--rw-r--r--   0        0        0     3246 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/beatport.py
--rw-r--r--   0        0        0     3180 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/beeg.py
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/behindkink.py
--rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/bellmedia.py
--rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/berufetv.py
--rw-r--r--   0        0        0     2763 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/bet.py
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/bfi.py
--rw-r--r--   0        0        0     5422 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/bfmtv.py
--rw-r--r--   0        0        0     6831 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/bibeltv.py
--rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/bigflix.py
--rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/bigo.py
--rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/bild.py
--rw-r--r--   0        0        0    93818 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/bilibili.py
--rw-r--r--   0        0        0     3454 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/biobiochiletv.py
--rw-r--r--   0        0        0    11755 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/bitchute.py
--rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/blackboardcollaborate.py
--rw-r--r--   0        0        0     4291 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/bleacherreport.py
--rw-r--r--   0        0        0     4733 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/blerp.py
--rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/blogger.py
--rw-r--r--   0        0        0     3180 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/bloomberg.py
--rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/bokecc.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/bongacams.py
--rw-r--r--   0        0        0     8894 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/boosty.py
--rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/bostonglobe.py
--rw-r--r--   0        0        0     4229 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/box.py
--rw-r--r--   0        0        0     4756 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/boxcast.py
--rw-r--r--   0        0        0     7723 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/bpb.py
--rw-r--r--   0        0        0     7476 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/br.py
--rw-r--r--   0        0        0    12920 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/brainpop.py
--rw-r--r--   0        0        0     8277 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/bravotv.py
--rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/breitbart.py
--rw-r--r--   0        0        0    42705 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/brightcove.py
--rw-r--r--   0        0        0     5378 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/brilliantpala.py
--rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/bundesliga.py
--rw-r--r--   0        0        0     5116 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/bundestag.py
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/businessinsider.py
--rw-r--r--   0        0        0     3609 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/buzzfeed.py
--rw-r--r--   0        0        0     3929 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/byutv.py
--rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/c56.py
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/cableav.py
--rw-r--r--   0        0        0     8123 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/callin.py
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/caltrans.py
--rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/cam4.py
--rw-r--r--   0        0        0     5715 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/camdemy.py
--rw-r--r--   0        0        0     3458 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/camfm.py
--rw-r--r--   0        0        0     2826 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/cammodels.py
--rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/camsoda.py
--rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/camtasia.py
--rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/canal1.py
--rw-r--r--   0        0        0     4269 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/canalalpha.py
--rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/canalc2.py
--rw-r--r--   0        0        0     4358 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/canalplus.py
--rw-r--r--   0        0        0     5733 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/caracoltv.py
--rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/cartoonnetwork.py
--rw-r--r--   0        0        0    30351 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/cbc.py
--rw-r--r--   0        0        0    11862 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/cbs.py
--rw-r--r--   0        0        0    19544 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/cbsnews.py
--rw-r--r--   0        0        0     4883 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/cbssports.py
--rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ccc.py
--rw-r--r--   0        0        0     5381 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ccma.py
--rw-r--r--   0        0        0     7391 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/cctv.py
--rw-r--r--   0        0        0    13880 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/cda.py
--rw-r--r--   0        0        0     2837 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/cellebrite.py
--rw-r--r--   0        0        0    11811 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ceskatelevize.py
--rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/cgtn.py
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/charlierose.py
--rw-r--r--   0        0        0     3816 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/chaturbate.py
--rw-r--r--   0        0        0     4822 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/chilloutzone.py
--rw-r--r--   0        0        0     5651 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/chzzk.py
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/cinemax.py
--rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/cinetecamilano.py
--rw-r--r--   0        0        0     5774 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/cineverse.py
--rw-r--r--   0        0        0     5858 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ciscolive.py
--rw-r--r--   0        0        0     4432 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ciscowebex.py
--rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/cjsw.py
--rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/clipchamp.py
--rw-r--r--   0        0        0     2493 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/clippit.py
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/cliprs.py
--rw-r--r--   0        0        0     3016 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/closertotruth.py
--rw-r--r--   0        0        0     3235 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/cloudflarestream.py
--rw-r--r--   0        0        0     2971 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/cloudycdn.py
--rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/clubic.py
--rw-r--r--   0        0        0     3083 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/clyp.py
--rw-r--r--   0        0        0     2243 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/cmt.py
--rw-r--r--   0        0        0     4615 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/cnbc.py
--rw-r--r--   0        0        0     9171 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/cnn.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/comedycentral.py
--rw-r--r--   0        0        0   192000 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/common.py
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/commonmistakes.py
--rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/commonprotocols.py
--rw-r--r--   0        0        0     9730 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/condenast.py
--rw-r--r--   0        0        0     4102 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/contv.py
--rw-r--r--   0        0        0     6313 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/corus.py
--rw-r--r--   0        0        0     4559 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/coub.py
--rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/cozytv.py
--rw-r--r--   0        0        0     5703 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/cpac.py
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/cracked.py
--rw-r--r--   0        0        0     9681 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/crackle.py
--rw-r--r--   0        0        0     3186 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/craftsy.py
--rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/crooksandliars.py
--rw-r--r--   0        0        0     4162 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/crowdbunker.py
--rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/crtvg.py
--rw-r--r--   0        0        0    28345 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/crunchyroll.py
--rw-r--r--   0        0        0    12105 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/cspan.py
--rw-r--r--   0        0        0     3591 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ctsnews.py
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ctv.py
--rw-r--r--   0        0        0     2554 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ctvnews.py
--rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/cultureunplugged.py
--rw-r--r--   0        0        0     8391 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/curiositystream.py
--rw-r--r--   0        0        0     4002 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/cwtv.py
--rw-r--r--   0        0        0     6285 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/cybrary.py
--rw-r--r--   0        0        0     6335 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/dacast.py
--rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/dailymail.py
--rw-r--r--   0        0        0    18453 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/dailymotion.py
--rw-r--r--   0        0        0     4854 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/dailywire.py
--rw-r--r--   0        0        0     5500 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/damtomo.py
--rw-r--r--   0        0        0     9431 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/daum.py
--rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/daystar.py
--rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/dbtv.py
--rw-r--r--   0        0        0     3531 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/dctp.py
--rw-r--r--   0        0        0     5154 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/deezer.py
--rw-r--r--   0        0        0     3007 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/democracynow.py
--rw-r--r--   0        0        0     8088 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/detik.py
--rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/deuxm.py
--rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/dfb.py
--rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/dhm.py
--rw-r--r--   0        0        0     6419 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/digitalconcerthall.py
--rw-r--r--   0        0        0     3257 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/digiteka.py
--rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/discogs.py
--rw-r--r--   0        0        0     4855 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/discovery.py
--rw-r--r--   0        0        0     6002 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/discoverygo.py
--rw-r--r--   0        0        0     6770 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/disney.py
--rw-r--r--   0        0        0     4946 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/dispeak.py
--rw-r--r--   0        0        0     8692 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/dlf.py
--rw-r--r--   0        0        0     2976 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/dlive.py
--rw-r--r--   0        0        0    11836 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/douyutv.py
--rw-r--r--   0        0        0    41198 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/dplay.py
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/drbonanza.py
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/dreisat.py
--rw-r--r--   0        0        0     4187 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/drooble.py
--rw-r--r--   0        0        0     4023 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/dropbox.py
--rw-r--r--   0        0        0     9914 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/dropout.py
--rw-r--r--   0        0        0     3796 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/drtuber.py
--rw-r--r--   0        0        0    15934 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/drtv.py
--rw-r--r--   0        0        0     2742 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/dtube.py
--rw-r--r--   0        0        0     8532 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/duboku.py
--rw-r--r--   0        0        0     3999 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/dumpert.py
--rw-r--r--   0        0        0     4118 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/duoplay.py
--rw-r--r--   0        0        0     7435 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/dvtv.py
--rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/dw.py
--rw-r--r--   0        0        0     8194 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/eagleplatform.py
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ebaumsworld.py
--rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ebay.py
--rw-r--r--   0        0        0     4938 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/egghead.py
--rw-r--r--   0        0        0     5811 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/eighttracks.py
--rw-r--r--   0        0        0     3612 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/einthusan.py
--rw-r--r--   0        0        0     3167 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/eitb.py
--rw-r--r--   0        0        0     3327 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/elementorembed.py
--rw-r--r--   0        0        0     2585 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/elonet.py
--rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/elpais.py
--rw-r--r--   0        0        0     2650 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/eltrecetv.py
--rw-r--r--   0        0        0     5286 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/embedly.py
--rw-r--r--   0        0        0     4195 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/epicon.py
--rw-r--r--   0        0        0     4090 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/epidemicsound.py
--rw-r--r--   0        0        0     7863 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/eplus.py
--rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/epoch.py
--rw-r--r--   0        0        0     5047 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/eporner.py
--rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/erocast.py
--rw-r--r--   0        0        0     4467 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/eroprofile.py
--rw-r--r--   0        0        0     8855 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/err.py
--rw-r--r--   0        0        0    12620 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ertgr.py
--rw-r--r--   0        0        0    17218 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/espn.py
--rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ettutv.py
--rw-r--r--   0        0        0     6666 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/europa.py
--rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/europeantour.py
--rw-r--r--   0        0        0     6617 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/eurosport.py
--rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/euscreen.py
--rw-r--r--   0        0        0     4088 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/expressen.py
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/extractors.py
--rw-r--r--   0        0        0     2630 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/eyedotv.py
--rw-r--r--   0        0        0    48374 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/facebook.py
--rw-r--r--   0        0        0     7218 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/fancode.py
--rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/fathom.py
--rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/faz.py
--rw-r--r--   0        0        0    10584 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/fc2.py
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/fczenit.py
--rw-r--r--   0        0        0     3845 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/fifa.py
--rw-r--r--   0        0        0     5899 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/filmon.py
--rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/filmweb.py
--rw-r--r--   0        0        0     6361 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/firsttv.py
--rw-r--r--   0        0        0     3045 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/fivetv.py
--rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/flextv.py
--rw-r--r--   0        0        0     4701 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/flickr.py
--rw-r--r--   0        0        0    14314 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/floatplane.py
--rw-r--r--   0        0        0     2550 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/folketinget.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/footyroom.py
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/formula1.py
--rw-r--r--   0        0        0    11501 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/fourtube.py
--rw-r--r--   0        0        0     6849 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/fox.py
--rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/fox9.py
--rw-r--r--   0        0        0     7661 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/foxnews.py
--rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/foxsports.py
--rw-r--r--   0        0        0     4848 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/fptplay.py
--rw-r--r--   0        0        0     2158 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/franceinter.py
--rw-r--r--   0        0        0    17035 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/francetv.py
--rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/freesound.py
--rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/freespeech.py
--rw-r--r--   0        0        0     5529 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/freetv.py
--rw-r--r--   0        0        0     8597 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/frontendmasters.py
--rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/fujitv.py
--rw-r--r--   0        0        0    14971 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/funimation.py
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/funk.py
--rw-r--r--   0        0        0     3272 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/funker530.py
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/fuyintv.py
--rw-r--r--   0        0        0     5675 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/gab.py
--rw-r--r--   0        0        0     4504 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/gaia.py
--rw-r--r--   0        0        0    25081 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/gamejolt.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/gamespot.py
--rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/gamestar.py
--rw-r--r--   0        0        0     3707 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/gaskrank.py
--rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/gazeta.py
--rw-r--r--   0        0        0     8544 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/gdcvault.py
--rw-r--r--   0        0        0     8522 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/gedidigital.py
--rw-r--r--   0        0        0   119486 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/generic.py
--rw-r--r--   0        0        0     4608 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/genericembeds.py
--rw-r--r--   0        0        0     6103 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/genius.py
--rw-r--r--   0        0        0     7544 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/getcourseru.py
--rw-r--r--   0        0        0     7845 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/gettr.py
--rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/giantbomb.py
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/gigya.py
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/glide.py
--rw-r--r--   0        0        0     9446 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/globalplayer.py
--rw-r--r--   0        0        0    10140 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/globo.py
--rw-r--r--   0        0        0     8517 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/glomex.py
--rw-r--r--   0        0        0     3926 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/gmanetwork.py
--rw-r--r--   0        0        0    14143 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/go.py
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/godtube.py
--rw-r--r--   0        0        0     3543 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/gofile.py
--rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/golem.py
--rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/goodgame.py
--rw-r--r--   0        0        0    14775 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/googledrive.py
--rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/googlepodcasts.py
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/googlesearch.py
--rw-r--r--   0        0        0    16911 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/goplay.py
--rw-r--r--   0        0        0     3768 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/gopro.py
--rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/goshgay.py
--rw-r--r--   0        0        0     2727 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/gotostage.py
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/gputechconf.py
--rw-r--r--   0        0        0     4399 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/gronkh.py
--rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/groupon.py
--rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/harpodeon.py
--rw-r--r--   0        0        0     6035 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/hbo.py
--rw-r--r--   0        0        0     3489 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/hearthisat.py
--rw-r--r--   0        0        0     8432 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/heise.py
--rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/hellporno.py
--rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/hgtv.py
--rw-r--r--   0        0        0     4945 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/hidive.py
--rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/historicfilms.py
--rw-r--r--   0        0        0     2228 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/hitrecord.py
--rw-r--r--   0        0        0     6867 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/hketv.py
--rw-r--r--   0        0        0     2871 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/hollywoodreporter.py
--rw-r--r--   0        0        0     4267 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/holodex.py
--rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/hotnewhiphop.py
--rw-r--r--   0        0        0    18185 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/hotstar.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/hrefli.py
--rw-r--r--   0        0        0     3845 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/hrfensehen.py
--rw-r--r--   0        0        0     7049 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/hrti.py
--rw-r--r--   0        0        0     3600 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/hse.py
--rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/huajiao.py
--rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/huffpost.py
--rw-r--r--   0        0        0     7699 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/hungama.py
--rw-r--r--   0        0        0     4862 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/huya.py
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/hypem.py
--rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/hypergryph.py
--rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/hytale.py
--rw-r--r--   0        0        0     7391 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/icareus.py
--rw-r--r--   0        0        0     5787 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ichinanalive.py
--rw-r--r--   0        0        0     4868 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/idolplus.py
--rw-r--r--   0        0        0    16322 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ign.py
--rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/iheart.py
--rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ilpost.py
--rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/iltalehti.py
--rw-r--r--   0        0        0     5636 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/imdb.py
--rw-r--r--   0        0        0     4828 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/imggaming.py
--rw-r--r--   0        0        0    14257 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/imgur.py
--rw-r--r--   0        0        0     3617 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ina.py
--rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/inc.py
--rw-r--r--   0        0        0     4188 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/indavideo.py
--rw-r--r--   0        0        0     5112 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/infoq.py
--rw-r--r--   0        0        0    30961 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/instagram.py
--rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/internazionale.py
--rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/internetvideoarchive.py
--rw-r--r--   0        0        0    10919 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/iprima.py
--rw-r--r--   0        0        0    31244 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/iqiyi.py
--rw-r--r--   0        0        0     3177 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/islamchannel.py
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/israelnationalnews.py
--rw-r--r--   0        0        0     5343 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/itprotv.py
--rw-r--r--   0        0        0    10682 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/itv.py
--rw-r--r--   0        0        0    10052 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ivi.py
--rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ivideon.py
--rw-r--r--   0        0        0    11627 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/iwara.py
--rw-r--r--   0        0        0     3426 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ixigua.py
--rw-r--r--   0        0        0     4059 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/izlesene.py
--rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/jable.py
--rw-r--r--   0        0        0     7902 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/jamendo.py
--rw-r--r--   0        0        0    10351 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/japandiet.py
--rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/jeuxvideo.py
--rw-r--r--   0        0        0     4315 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/jiosaavn.py
--rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/jixie.py
--rw-r--r--   0        0        0     3865 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/joj.py
--rw-r--r--   0        0        0     4512 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/joqrag.py
--rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/jove.py
--rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/jstream.py
--rw-r--r--   0        0        0     6333 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/jtbc.py
--rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/jwplatform.py
--rw-r--r--   0        0        0     5912 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/kakao.py
--rw-r--r--   0        0        0    24329 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/kaltura.py
--rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/kankanews.py
--rw-r--r--   0        0        0     2283 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/karaoketv.py
--rw-r--r--   0        0        0     3488 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/kelbyone.py
--rw-r--r--   0        0        0     4103 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/khanacademy.py
--rw-r--r--   0        0        0     5571 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/kick.py
--rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/kicker.py
--rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/kickstarter.py
--rw-r--r--   0        0        0     7835 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/kinja.py
--rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/kinopoisk.py
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/kommunetv.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/kompas.py
--rw-r--r--   0        0        0     4707 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/koo.py
--rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/krasview.py
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/kth.py
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ku6.py
--rw-r--r--   0        0        0     5694 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/kukululive.py
--rw-r--r--   0        0        0    12524 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/kuwo.py
--rw-r--r--   0        0        0     9434 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/la7.py
--rw-r--r--   0        0        0     4748 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/lastfm.py
--rw-r--r--   0        0        0     2772 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/laxarxames.py
--rw-r--r--   0        0        0   771840 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/lazy_extractors.py
--rw-r--r--   0        0        0    17579 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/lbry.py
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/lci.py
--rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/lcp.py
--rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/lecture2go.py
--rw-r--r--   0        0        0     8380 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/lecturio.py
--rw-r--r--   0        0        0    12993 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/leeco.py
--rw-r--r--   0        0        0     5417 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/lefigaro.py
--rw-r--r--   0        0        0     5894 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/lego.py
--rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/lemonde.py
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/lenta.py
--rw-r--r--   0        0        0     4935 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/libraryofcongress.py
--rw-r--r--   0        0        0     3673 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/libsyn.py
--rw-r--r--   0        0        0     9524 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/lifenews.py
--rw-r--r--   0        0        0     7021 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/likee.py
--rw-r--r--   0        0        0    15006 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/limelight.py
--rw-r--r--   0        0        0    10886 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/linkedin.py
--rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/liputan6.py
--rw-r--r--   0        0        0     4167 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/listennotes.py
--rw-r--r--   0        0        0     6884 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/litv.py
--rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/livejournal.py
--rw-r--r--   0        0        0    14577 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/livestream.py
--rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/livestreamfails.py
--rw-r--r--   0        0        0     6318 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/lnkgo.py
--rw-r--r--   0        0        0    18063 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/loom.py
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/lovehomeporn.py
--rw-r--r--   0        0        0     4038 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/lrt.py
--rw-r--r--   0        0        0    12070 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/lsm.py
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/lumni.py
--rw-r--r--   0        0        0    12446 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/lynda.py
--rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/maariv.py
--rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/magellantv.py
--rw-r--r--   0        0        0     2772 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/magentamusik.py
--rw-r--r--   0        0        0    12022 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/mailru.py
--rw-r--r--   0        0        0     9235 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/mainstreaming.py
--rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/mangomolo.py
--rw-r--r--   0        0        0     5148 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/manoto.py
--rw-r--r--   0        0        0     5946 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/manyvids.py
--rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/maoritv.py
--rw-r--r--   0        0        0     4507 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/markiza.py
--rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/massengeschmacktv.py
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/masters.py
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/matchtv.py
--rw-r--r--   0        0        0     3897 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/mbn.py
--rw-r--r--   0        0        0     6836 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/mdr.py
--rw-r--r--   0        0        0     6055 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/medaltv.py
--rw-r--r--   0        0        0     4930 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/mediaite.py
--rw-r--r--   0        0        0     6890 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/mediaklikk.py
--rw-r--r--   0        0        0     4122 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/medialaan.py
--rw-r--r--   0        0        0    13331 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/mediaset.py
--rw-r--r--   0        0        0    16617 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/mediasite.py
--rw-r--r--   0        0        0    10321 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/mediastream.py
--rw-r--r--   0        0        0     4078 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/mediaworksnz.py
--rw-r--r--   0        0        0     6712 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/medici.py
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/megaphone.py
--rw-r--r--   0        0        0     6726 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/megatvcom.py
--rw-r--r--   0        0        0     3537 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/meipai.py
--rw-r--r--   0        0        0     2158 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/melonvod.py
--rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/metacritic.py
--rw-r--r--   0        0        0     6473 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/mgtv.py
--rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/microsoftembed.py
--rw-r--r--   0        0        0     5381 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/microsoftstream.py
--rw-r--r--   0        0        0     7306 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/microsoftvirtualacademy.py
--rw-r--r--   0        0        0    11551 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/mildom.py
--rw-r--r--   0        0        0     6829 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/minds.py
--rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/minoto.py
--rw-r--r--   0        0        0     4880 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/mirrativ.py
--rw-r--r--   0        0        0     4403 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/mirrorcouk.py
--rw-r--r--   0        0        0     5165 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/mit.py
--rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/mitele.py
--rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/mixch.py
--rw-r--r--   0        0        0    12793 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/mixcloud.py
--rw-r--r--   0        0        0    14610 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/mlb.py
--rw-r--r--   0        0        0     6696 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/mlssoccer.py
--rw-r--r--   0        0        0     2959 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/mocha.py
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/mojvideo.py
--rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/monstercat.py
--rw-r--r--   0        0        0    10821 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/motherless.py
--rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/motorsport.py
--rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/moviepilot.py
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/moview.py
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/moviezine.py
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/movingimage.py
--rw-r--r--   0        0        0     7501 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/msn.py
--rw-r--r--   0        0        0    25584 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/mtv.py
--rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/muenchentv.py
--rw-r--r--   0        0        0     5035 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/murrtube.py
--rw-r--r--   0        0        0     4093 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/museai.py
--rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/musescore.py
--rw-r--r--   0        0        0     7179 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/musicdex.py
--rw-r--r--   0        0        0     6379 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/mx3.py
--rw-r--r--   0        0        0    10007 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/mxplayer.py
--rw-r--r--   0        0        0     7765 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/myspace.py
--rw-r--r--   0        0        0     3714 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/myspass.py
--rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/myvideoge.py
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/myvidster.py
--rw-r--r--   0        0        0     3746 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/mzaalo.py
--rw-r--r--   0        0        0     6814 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/n1.py
--rw-r--r--   0        0        0     4303 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/nate.py
--rw-r--r--   0        0        0     3057 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/nationalgeographic.py
--rw-r--r--   0        0        0    16447 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/naver.py
--rw-r--r--   0        0        0    16157 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/nba.py
--rw-r--r--   0        0        0    35311 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/nbc.py
--rw-r--r--   0        0        0    18232 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ndr.py
--rw-r--r--   0        0        0     4502 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ndtv.py
--rw-r--r--   0        0        0    20864 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/nebula.py
--rw-r--r--   0        0        0     9389 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/nekohacker.py
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/nerdcubed.py
--rw-r--r--   0        0        0    23769 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/neteasemusic.py
--rw-r--r--   0        0        0    10988 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/netverse.py
--rw-r--r--   0        0        0     2922 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/netzkino.py
--rw-r--r--   0        0        0    11825 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/newgrounds.py
--rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/newspicks.py
--rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/newsy.py
--rw-r--r--   0        0        0     9075 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/nextmedia.py
--rw-r--r--   0        0        0    21193 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/nexx.py
--rw-r--r--   0        0        0    13126 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/nfb.py
--rw-r--r--   0        0        0     5859 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/nfhsnetwork.py
--rw-r--r--   0        0        0    15532 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/nfl.py
--rw-r--r--   0        0        0    29764 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/nhk.py
--rw-r--r--   0        0        0     4912 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/nhl.py
--rw-r--r--   0        0        0    10478 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/nick.py
--rw-r--r--   0        0        0    44728 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/niconico.py
--rw-r--r--   0        0        0    18094 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/niconicochannelplus.py
--rw-r--r--   0        0        0    10389 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ninaprotocol.py
--rw-r--r--   0        0        0     5131 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ninecninemedia.py
--rw-r--r--   0        0        0     5178 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ninegag.py
--rw-r--r--   0        0        0     3634 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ninenews.py
--rw-r--r--   0        0        0     5299 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ninenow.py
--rw-r--r--   0        0        0     5473 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/nintendo.py
--rw-r--r--   0        0        0    13650 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/nitter.py
--rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/nobelprize.py
--rw-r--r--   0        0        0     5056 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/noice.py
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/nonktube.py
--rw-r--r--   0        0        0     3441 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/noodlemagazine.py
--rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/noovo.py
--rw-r--r--   0        0        0     5817 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/nosnl.py
--rw-r--r--   0        0        0    12074 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/nova.py
--rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/novaplay.py
--rw-r--r--   0        0        0     5954 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/nowness.py
--rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/noz.py
--rw-r--r--   0        0        0    22320 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/npo.py
--rw-r--r--   0        0        0     5740 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/npr.py
--rw-r--r--   0        0        0    32207 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/nrk.py
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/nrl.py
--rw-r--r--   0        0        0     2277 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ntvcojp.py
--rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ntvde.py
--rw-r--r--   0        0        0     5666 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ntvru.py
--rw-r--r--   0        0        0     4492 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/nubilesporn.py
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/nuevo.py
--rw-r--r--   0        0        0     7311 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/nuum.py
--rw-r--r--   0        0        0     3532 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/nuvid.py
--rw-r--r--   0        0        0    17309 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/nytimes.py
--rw-r--r--   0        0        0     5896 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/nzherald.py
--rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/nzonscreen.py
--rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/nzz.py
--rw-r--r--   0        0        0     4284 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/odkmedia.py
--rw-r--r--   0        0        0    17342 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/odnoklassniki.py
--rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/oftv.py
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/oktoberfesttv.py
--rw-r--r--   0        0        0     2868 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/olympics.py
--rw-r--r--   0        0        0     3924 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/on24.py
--rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/once.py
--rw-r--r--   0        0        0     6757 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ondemandkorea.py
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/onefootball.py
--rw-r--r--   0        0        0     5136 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/onenewsnz.py
--rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/oneplace.py
--rw-r--r--   0        0        0     9845 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/onet.py
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/onionstudios.py
--rw-r--r--   0        0        0     7984 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/opencast.py
--rw-r--r--   0        0        0     8647 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/openload.py
--rw-r--r--   0        0        0     6204 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/openrec.py
--rw-r--r--   0        0        0     3126 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ora.py
--rw-r--r--   0        0        0    24396 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/orf.py
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/outsidetv.py
--rw-r--r--   0        0        0     2709 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/owncloud.py
--rw-r--r--   0        0        0     6166 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/packtpub.py
--rw-r--r--   0        0        0     4455 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/palcomp3.py
--rw-r--r--   0        0        0    25808 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/panopto.py
--rw-r--r--   0        0        0     7483 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/paramountplus.py
--rw-r--r--   0        0        0     3802 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/parler.py
--rw-r--r--   0        0        0     2772 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/parlview.py
--rw-r--r--   0        0        0    19461 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/patreon.py
--rw-r--r--   0        0        0    38530 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/pbs.py
--rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/pearvideo.py
--rw-r--r--   0        0        0     7214 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/peekvids.py
--rw-r--r--   0        0        0    78541 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/peertube.py
--rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/peertv.py
--rw-r--r--   0        0        0     8858 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/peloton.py
--rw-r--r--   0        0        0     3246 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/performgroup.py
--rw-r--r--   0        0        0     7323 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/periscope.py
--rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/pgatour.py
--rw-r--r--   0        0        0     4068 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/philharmoniedeparis.py
--rw-r--r--   0        0        0     4961 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/phoenix.py
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/photobucket.py
--rw-r--r--   0        0        0     4794 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/piapro.py
--rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/piaulizaportal.py
--rw-r--r--   0        0        0     4640 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/picarto.py
--rw-r--r--   0        0        0     6898 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/piksel.py
--rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/pinkbike.py
--rw-r--r--   0        0        0     9595 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/pinterest.py
--rw-r--r--   0        0        0     4752 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/pixivsketch.py
--rw-r--r--   0        0        0     4923 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/pladform.py
--rw-r--r--   0        0        0     2922 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/planetmarathi.py
--rw-r--r--   0        0        0     7404 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/platzi.py
--rw-r--r--   0        0        0     3655 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/playplustv.py
--rw-r--r--   0        0        0     8782 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/playsuisse.py
--rw-r--r--   0        0        0     7115 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/playtvak.py
--rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/playwire.py
--rw-r--r--   0        0        0    18375 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/pluralsight.py
--rw-r--r--   0        0        0     8093 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/plutotv.py
--rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/podbayfm.py
--rw-r--r--   0        0        0     3761 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/podchaser.py
--rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/podomatic.py
--rw-r--r--   0        0        0     5475 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/pokemon.py
--rw-r--r--   0        0        0     4180 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/pokergo.py
--rw-r--r--   0        0        0     3150 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/polsatgo.py
--rw-r--r--   0        0        0    24519 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/polskieradio.py
--rw-r--r--   0        0        0     3258 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/popcorntimes.py
--rw-r--r--   0        0        0     2630 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/popcorntv.py
--rw-r--r--   0        0        0     4047 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/porn91.py
--rw-r--r--   0        0        0     4490 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/pornbox.py
--rw-r--r--   0        0        0     3500 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/pornflip.py
--rw-r--r--   0        0        0    31546 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/pornhub.py
--rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/pornotube.py
--rw-r--r--   0        0        0     3916 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/pornovoisines.py
--rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/pornoxo.py
--rw-r--r--   0        0        0     8116 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/pr0gramm.py
--rw-r--r--   0        0        0     5722 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/prankcast.py
--rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/premiershiprugby.py
--rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/presstv.py
--rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/projectveritas.py
--rw-r--r--   0        0        0    21515 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/prosiebensat1.py
--rw-r--r--   0        0        0    16065 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/prx.py
--rw-r--r--   0        0        0     8375 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/puhutv.py
--rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/puls4.py
--rw-r--r--   0        0        0     2719 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/pyvideo.py
--rw-r--r--   0        0        0     7437 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/qdance.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/qingting.py
--rw-r--r--   0        0        0    13550 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/qqmusic.py
--rw-r--r--   0        0        0     4657 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/r7.py
--rw-r--r--   0        0        0     9799 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/radiko.py
--rw-r--r--   0        0        0     6253 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/radiocanada.py
--rw-r--r--   0        0        0     6253 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/radiocomercial.py
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/radiode.py
--rw-r--r--   0        0        0    18223 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/radiofrance.py
--rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/radiojavan.py
--rw-r--r--   0        0        0     3345 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/radiokapital.py
--rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/radiozet.py
--rw-r--r--   0        0        0     6929 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/radlive.py
--rw-r--r--   0        0        0    34159 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/rai.py
--rw-r--r--   0        0        0     6124 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/raywenderlich.py
--rw-r--r--   0        0        0     5343 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/rbgtum.py
--rw-r--r--   0        0        0    16249 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/rcs.py
--rw-r--r--   0        0        0    16483 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/rcti.py
--rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/rds.py
--rw-r--r--   0        0        0    14580 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/redbee.py
--rw-r--r--   0        0        0     9273 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/redbulltv.py
--rw-r--r--   0        0        0    14147 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/reddit.py
--rw-r--r--   0        0        0     5235 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/redge.py
--rw-r--r--   0        0        0     9523 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/redgifs.py
--rw-r--r--   0        0        0     6216 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/redtube.py
--rw-r--r--   0        0        0     4105 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/rentv.py
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/restudy.py
--rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/reuters.py
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/reverbnation.py
--rw-r--r--   0        0        0     4653 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/rheinmaintv.py
--rw-r--r--   0        0        0     4417 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ridehome.py
--rw-r--r--   0        0        0     3192 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/rinsefm.py
--rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/rmcdecouverte.py
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/rockstargames.py
--rw-r--r--   0        0        0    21043 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/rokfin.py
--rw-r--r--   0        0        0    15756 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/roosterteeth.py
--rw-r--r--   0        0        0     3045 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/rottentomatoes.py
--rw-r--r--   0        0        0    15123 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/rozhlas.py
--rw-r--r--   0        0        0     6207 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/rte.py
--rw-r--r--   0        0        0     3636 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/rtl2.py
--rw-r--r--   0        0        0    12122 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/rtlnl.py
--rw-r--r--   0        0        0     7645 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/rtnews.py
--rw-r--r--   0        0        0     3371 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/rtp.py
--rw-r--r--   0        0        0     2756 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/rtrfm.py
--rw-r--r--   0        0        0     9529 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/rts.py
--rw-r--r--   0        0        0    11224 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/rtvcplay.py
--rw-r--r--   0        0        0    12881 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/rtve.py
--rw-r--r--   0        0        0     3428 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/rtvs.py
--rw-r--r--   0        0        0     7153 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/rtvslo.py
--rw-r--r--   0        0        0     5205 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/rudovideo.py
--rw-r--r--   0        0        0     5206 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/rule34video.py
--rw-r--r--   0        0        0    15578 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/rumble.py
--rw-r--r--   0        0        0    13882 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/rutube.py
--rw-r--r--   0        0        0     8052 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/rutv.py
--rw-r--r--   0        0        0    10968 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ruutu.py
--rw-r--r--   0        0        0     6839 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ruv.py
--rw-r--r--   0        0        0     4071 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/s4c.py
--rw-r--r--   0        0        0     9807 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/safari.py
--rw-r--r--   0        0        0     3011 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/saitosan.py
--rw-r--r--   0        0        0     3817 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/samplefocus.py
--rw-r--r--   0        0        0     4398 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/sapo.py
--rw-r--r--   0        0        0     6548 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/sbs.py
--rw-r--r--   0        0        0     8280 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/sbscokr.py
--rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/screen9.py
--rw-r--r--   0        0        0     4594 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/screencast.py
--rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/screencastify.py
--rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/screencastomatic.py
--rw-r--r--   0        0        0     5975 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/scrippsnetworks.py
--rw-r--r--   0        0        0     3744 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/scrolller.py
--rw-r--r--   0        0        0     4866 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/scte.py
--rw-r--r--   0        0        0     8609 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/sejmpl.py
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/senalcolombia.py
--rw-r--r--   0        0        0     8688 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/senategov.py
--rw-r--r--   0        0        0     3940 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/sendtonews.py
--rw-r--r--   0        0        0     5410 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/servus.py
--rw-r--r--   0        0        0     4955 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/sevenplus.py
--rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/sexu.py
--rw-r--r--   0        0        0     7623 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/seznamzpravy.py
--rw-r--r--   0        0        0     8289 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/shahid.py
--rw-r--r--   0        0        0     5505 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/sharepoint.py
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/sharevideos.py
--rw-r--r--   0        0        0     4337 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/shemaroome.py
--rw-r--r--   0        0        0     3016 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/showroomlive.py
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/sibnet.py
--rw-r--r--   0        0        0     6045 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/simplecast.py
--rw-r--r--   0        0        0     4213 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/sina.py
--rw-r--r--   0        0        0     5054 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/sixplay.py
--rw-r--r--   0        0        0     5580 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/skeb.py
--rw-r--r--   0        0        0     5398 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/sky.py
--rw-r--r--   0        0        0     9225 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/skyit.py
--rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/skylinewebcams.py
--rw-r--r--   0        0        0     5367 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/skynewsarabia.py
--rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/skynewsau.py
--rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/slideshare.py
--rw-r--r--   0        0        0    21906 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/slideslive.py
--rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/slutload.py
--rw-r--r--   0        0        0     2685 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/smotrim.py
--rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/snotr.py
--rw-r--r--   0        0        0    11240 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/sohu.py
--rw-r--r--   0        0        0    10281 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/sonyliv.py
--rw-r--r--   0        0        0    37011 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/soundcloud.py
--rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/soundgasm.py
--rw-r--r--   0        0        0     7785 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/southpark.py
--rw-r--r--   0        0        0     8210 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/sovietscloset.py
--rw-r--r--   0        0        0     7193 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/spankbang.py
--rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/spiegel.py
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/spike.py
--rw-r--r--   0        0        0     3147 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/sport5.py
--rw-r--r--   0        0        0     3233 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/sportbox.py
--rw-r--r--   0        0        0     6295 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/sportdeutschland.py
--rw-r--r--   0        0        0     6341 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/spotify.py
--rw-r--r--   0        0        0     5973 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/spreaker.py
--rw-r--r--   0        0        0     3987 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/springboardplatform.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/sprout.py
--rw-r--r--   0        0        0     9937 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/srgssr.py
--rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/srmediathek.py
--rw-r--r--   0        0        0     8726 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/stacommu.py
--rw-r--r--   0        0        0    10877 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/stageplus.py
--rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/stanfordoc.py
--rw-r--r--   0        0        0     3832 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/startrek.py
--rw-r--r--   0        0        0     3530 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/startv.py
--rw-r--r--   0        0        0     6502 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/steam.py
--rw-r--r--   0        0        0     5330 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/stitcher.py
--rw-r--r--   0        0        0     4718 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/storyfire.py
--rw-r--r--   0        0        0     3917 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/streamable.py
--rw-r--r--   0        0        0     5011 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/streamcz.py
--rw-r--r--   0        0        0     3567 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/streetvoice.py
--rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/stretchinternet.py
--rw-r--r--   0        0        0     2545 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/stripchat.py
--rw-r--r--   0        0        0     3329 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/stv.py
--rw-r--r--   0        0        0     4625 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/substack.py
--rw-r--r--   0        0        0     2528 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/sunporno.py
--rw-r--r--   0        0        0     5495 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/sverigesradio.py
--rw-r--r--   0        0        0    17835 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/svt.py
--rw-r--r--   0        0        0     3399 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/swearnet.py
--rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/syfy.py
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/syvdk.py
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/sztvhu.py
--rw-r--r--   0        0        0     6194 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tagesschau.py
--rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tass.py
--rw-r--r--   0        0        0     3487 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tbs.py
--rw-r--r--   0        0        0     7105 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tbsjp.py
--rw-r--r--   0        0        0    10455 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/teachable.py
--rw-r--r--   0        0        0     4361 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/teachertube.py
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/teachingchannel.py
--rw-r--r--   0        0        0     9986 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/teamcoco.py
--rw-r--r--   0        0        0     5374 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/teamtreehouse.py
--rw-r--r--   0        0        0     9821 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ted.py
--rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tele13.py
--rw-r--r--   0        0        0     3301 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tele5.py
--rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/telebruxelles.py
--rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/telecaribe.py
--rw-r--r--   0        0        0     6110 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/telecinco.py
--rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/telegraaf.py
--rw-r--r--   0        0        0     5085 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/telegram.py
--rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/telemb.py
--rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/telemundo.py
--rw-r--r--   0        0        0     8988 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/telequebec.py
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/teletask.py
--rw-r--r--   0        0        0     5429 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/telewebion.py
--rw-r--r--   0        0        0     4888 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tempo.py
--rw-r--r--   0        0        0    19941 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tencent.py
--rw-r--r--   0        0        0     7260 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tennistv.py
--rw-r--r--   0        0        0     6695 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tenplay.py
--rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/testurl.py
--rw-r--r--   0        0        0     3855 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tf1.py
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tfo.py
--rw-r--r--   0        0        0     6132 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/theguardian.py
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/theholetv.py
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/theintercept.py
--rw-r--r--   0        0        0    18966 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/theplatform.py
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/thestar.py
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/thesun.py
--rw-r--r--   0        0        0     4105 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/theweatherchannel.py
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/thisamericanlife.py
--rw-r--r--   0        0        0     5955 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/thisoldhouse.py
--rw-r--r--   0        0        0     8617 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/thisvid.py
--rw-r--r--   0        0        0     6222 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/threeqsdn.py
--rw-r--r--   0        0        0     4005 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/threespeak.py
--rw-r--r--   0        0        0    60521 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tiktok.py
--rw-r--r--   0        0        0     9690 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tmz.py
--rw-r--r--   0        0        0    13595 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tnaflix.py
--rw-r--r--   0        0        0     8812 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/toggle.py
--rw-r--r--   0        0        0     3404 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/toggo.py
--rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tonline.py
--rw-r--r--   0        0        0     2972 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/toongoggles.py
--rw-r--r--   0        0        0     3530 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/toutv.py
--rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/toypics.py
--rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/traileraddict.py
--rw-r--r--   0        0        0    13594 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/triller.py
--rw-r--r--   0        0        0    12901 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/trovo.py
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/trtcocuk.py
--rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/trtworld.py
--rw-r--r--   0        0        0     6358 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/trueid.py
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/trunews.py
--rw-r--r--   0        0        0     2790 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/truth.py
--rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/trutv.py
--rw-r--r--   0        0        0     6293 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tube8.py
--rw-r--r--   0        0        0    10672 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tubetugraz.py
--rw-r--r--   0        0        0     6697 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tubitv.py
--rw-r--r--   0        0        0    16426 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tumblr.py
--rw-r--r--   0        0        0     9127 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tunein.py
--rw-r--r--   0        0        0    11056 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/turner.py
--rw-r--r--   0        0        0    13726 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tv2.py
--rw-r--r--   0        0        0     3645 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tv24ua.py
--rw-r--r--   0        0        0     6019 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tv2dk.py
--rw-r--r--   0        0        0     3968 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tv2hu.py
--rw-r--r--   0        0        0     5479 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tv4.py
--rw-r--r--   0        0        0     7830 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tv5mondeplus.py
--rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tv5unis.py
--rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tva.py
--rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tvanouvelles.py
--rw-r--r--   0        0        0     3671 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tvc.py
--rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tver.py
--rw-r--r--   0        0        0     5043 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tvigle.py
--rw-r--r--   0        0        0     3247 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tviplayer.py
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tvland.py
--rw-r--r--   0        0        0     3830 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tvn24.py
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tvnoe.py
--rw-r--r--   0        0        0     5209 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tvopengr.py
--rw-r--r--   0        0        0    25539 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tvp.py
--rw-r--r--   0        0        0    11849 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tvplay.py
--rw-r--r--   0        0        0     2732 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tvplayer.py
--rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tweakers.py
--rw-r--r--   0        0        0     2638 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/twentymin.py
--rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/twentythreevideo.py
--rw-r--r--   0        0        0    12681 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/twitcasting.py
--rw-r--r--   0        0        0    42809 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/twitch.py
--rw-r--r--   0        0        0    81104 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/twitter.py
--rw-r--r--   0        0        0    17683 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/txxx.py
--rw-r--r--   0        0        0    19475 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/udemy.py
--rw-r--r--   0        0        0     3578 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/udn.py
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ufctv.py
--rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ukcolumn.py
--rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/uktvplay.py
--rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/umg.py
--rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/unistra.py
--rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/unity.py
--rw-r--r--   0        0        0     7258 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/unsupported.py
--rw-r--r--   0        0        0     5376 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/uol.py
--rw-r--r--   0        0        0     3352 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/uplynk.py
--rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/urort.py
--rw-r--r--   0        0        0     6918 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/urplay.py
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/usanetwork.py
--rw-r--r--   0        0        0     2646 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/usatoday.py
--rw-r--r--   0        0        0    10545 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ustream.py
--rw-r--r--   0        0        0     4260 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ustudio.py
--rw-r--r--   0        0        0     3721 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/utreon.py
--rw-r--r--   0        0        0     3045 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/varzesh3.py
--rw-r--r--   0        0        0     3902 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/vbox7.py
--rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/veo.py
--rw-r--r--   0        0        0     6940 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/veoh.py
--rw-r--r--   0        0        0     4343 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/vesti.py
--rw-r--r--   0        0        0    13519 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/vevo.py
--rw-r--r--   0        0        0    10860 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/vgtv.py
--rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/vh1.py
--rw-r--r--   0        0        0    11845 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/vice.py
--rw-r--r--   0        0        0     4937 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/viddler.py
--rw-r--r--   0        0        0     6529 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/videa.py
--rw-r--r--   0        0        0    10740 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/videocampus_sachsen.py
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/videodetective.py
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/videofyme.py
--rw-r--r--   0        0        0    13772 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/videoken.py
--rw-r--r--   0        0        0    11324 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/videomore.py
--rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/videopress.py
--rw-r--r--   0        0        0    13750 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/vidio.py
--rw-r--r--   0        0        0     5797 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/vidlii.py
--rw-r--r--   0        0        0     3061 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/vidly.py
--rw-r--r--   0        0        0    14946 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/viewlift.py
--rw-r--r--   0        0        0     7377 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/viidea.py
--rw-r--r--   0        0        0    13492 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/viki.py
--rw-r--r--   0        0        0    62548 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/vimeo.py
--rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/vimm.py
--rw-r--r--   0        0        0     5402 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/vine.py
--rw-r--r--   0        0        0     2572 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/viously.py
--rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/viqeo.py
--rw-r--r--   0        0        0    21227 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/viu.py
--rw-r--r--   0        0        0    34047 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/vk.py
--rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/vocaroo.py
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/vodpl.py
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/vodplatform.py
--rw-r--r--   0        0        0     5405 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/voicy.py
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/volejtv.py
--rw-r--r--   0        0        0     8993 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/voot.py
--rw-r--r--   0        0        0     9519 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/voxmedia.py
--rw-r--r--   0        0        0    21514 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/vrt.py
--rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/vtm.py
--rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/vuclip.py
--rw-r--r--   0        0        0    12609 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/vvvvid.py
--rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/walla.py
--rw-r--r--   0        0        0     5816 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/washingtonpost.py
--rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/wat.py
--rw-r--r--   0        0        0    15111 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/wdr.py
--rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/webcamerapl.py
--rw-r--r--   0        0        0     3660 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/webcaster.py
--rw-r--r--   0        0        0     5456 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/webofstories.py
--rw-r--r--   0        0        0    10998 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/weibo.py
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/weiqitv.py
--rw-r--r--   0        0        0    25606 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/weverse.py
--rw-r--r--   0        0        0     4168 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/wevidi.py
--rw-r--r--   0        0        0     3497 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/weyyak.py
--rw-r--r--   0        0        0     3937 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/whowatch.py
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/whyp.py
--rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/wikimedia.py
--rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/wimbledon.py
--rw-r--r--   0        0        0     5466 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/wimtv.py
--rw-r--r--   0        0        0    15862 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/wistia.py
--rw-r--r--   0        0        0     7198 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/wordpress.py
--rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/worldstarhiphop.py
--rw-r--r--   0        0        0     6113 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/wppilot.py
--rw-r--r--   0        0        0    12727 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/wrestleuniverse.py
--rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/wsj.py
--rw-r--r--   0        0        0     4491 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/wwe.py
--rw-r--r--   0        0        0    10763 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/wykop.py
--rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/xanimu.py
--rw-r--r--   0        0        0     2315 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/xboxclips.py
--rw-r--r--   0        0        0     7408 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/xfileshare.py
--rw-r--r--   0        0        0    19584 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/xhamster.py
--rw-r--r--   0        0        0     6659 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ximalaya.py
--rw-r--r--   0        0        0     4001 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/xinpianchang.py
--rw-r--r--   0        0        0     2901 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/xminus.py
--rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/xnxx.py
--rw-r--r--   0        0        0     3881 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/xstream.py
--rw-r--r--   0        0        0     7312 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/xvideos.py
--rw-r--r--   0        0        0     2612 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/xxxymovies.py
--rw-r--r--   0        0        0    17965 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/yahoo.py
--rw-r--r--   0        0        0     5059 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/yandexdisk.py
--rw-r--r--   0        0        0    17649 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/yandexmusic.py
--rw-r--r--   0        0        0    17747 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/yandexvideo.py
--rw-r--r--   0        0        0     2960 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/yapfiles.py
--rw-r--r--   0        0        0     5647 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/yappy.py
--rw-r--r--   0        0        0     6088 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/yle_areena.py
--rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/youjizz.py
--rw-r--r--   0        0        0    10927 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/youku.py
--rw-r--r--   0        0        0     7061 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/younow.py
--rw-r--r--   0        0        0     8467 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/youporn.py
--rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/yourporn.py
--rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/yourupload.py
--rw-r--r--   0        0        0   348531 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/youtube.py
--rw-r--r--   0        0        0     5982 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/zaiko.py
--rw-r--r--   0        0        0     3832 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/zapiks.py
--rw-r--r--   0        0        0    29425 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/zattoo.py
--rw-r--r--   0        0        0    18597 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/zdf.py
--rw-r--r--   0        0        0    12040 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/zee5.py
--rw-r--r--   0        0        0     3216 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/zeenews.py
--rw-r--r--   0        0        0     4803 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/zenporn.py
--rw-r--r--   0        0        0     3916 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/zetland.py
--rw-r--r--   0        0        0     2545 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/zhihu.py
--rw-r--r--   0        0        0    23571 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/zingmp3.py
--rw-r--r--   0        0        0     7091 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/zoom.py
--rw-r--r--   0        0        0     5505 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/zype.py
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/networking/__init__.py
--rw-r--r--   0        0        0     8776 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/networking/_curlcffi.py
--rw-r--r--   0        0        0    10452 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/networking/_helper.py
--rw-r--r--   0        0        0    15012 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/networking/_requests.py
--rw-r--r--   0        0        0    15738 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/networking/_urllib.py
--rw-r--r--   0        0        0     7266 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/networking/_websockets.py
--rw-r--r--   0        0        0    21205 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/networking/common.py
--rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/networking/exceptions.py
--rw-r--r--   0        0        0     5533 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/networking/impersonate.py
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/networking/websocket.py
--rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/postprocessor/__init__.py
--rw-r--r--   0        0        0     8359 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/postprocessor/common.py
--rw-r--r--   0        0        0    10469 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/postprocessor/embedthumbnail.py
--rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/postprocessor/exec.py
--rw-r--r--   0        0        0    49509 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/postprocessor/ffmpeg.py
--rw-r--r--   0        0        0     4381 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/postprocessor/metadataparser.py
--rw-r--r--   0        0        0    17821 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/postprocessor/modify_chapters.py
--rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/postprocessor/movefilesafterdownload.py
--rw-r--r--   0        0        0     4088 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/postprocessor/sponskrub.py
--rw-r--r--   0        0        0     4249 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/postprocessor/sponsorblock.py
--rw-r--r--   0        0        0     2481 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/postprocessor/xattrpp.py
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/utils/__init__.py
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/utils/_deprecated.py
--rw-r--r--   0        0        0     9992 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/utils/_legacy.py
--rw-r--r--   0        0        0   183337 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/utils/_utils.py
--rw-r--r--   0        0        0     5404 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/utils/networking.py
--rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/utils/progress.py
--rw-r--r--   0        0        0    12620 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/yt_dlp/utils/traversal.py
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/.gitignore
--rw-r--r--   0        0        0    17261 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/AUTHORS
--rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/LICENSE
--rw-r--r--   0        0        0   161803 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/README.md
--rw-r--r--   0        0        0     3540 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/pyproject.toml
--rw-r--r--   0        0        0   165928 2020-02-02 00:00:00.000000 yt_dlp-2024.4.6.232655.dev0/PKG-INFO
+-rw-r--r--   0        0        0   422459 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/Changelog.md
+-rw-r--r--   0        0        0   149513 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/README.txt
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/setup.cfg
+-rw-r--r--   0        0        0    56287 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/supportedsites.md
+-rw-r--r--   0        0        0   145072 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt-dlp.1
+-rw-r--r--   0        0        0     6166 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/completions/bash/yt-dlp
+-rw-r--r--   0        0        0    50103 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/completions/fish/yt-dlp.fish
+-rw-r--r--   0        0        0     6272 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/completions/zsh/_yt-dlp
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/devscripts/__init__.py
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/devscripts/bash-completion.in
+-rwxr-xr-x   0        0        0      854 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/devscripts/bash-completion.py
+-rw-r--r--   0        0        0     6887 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/devscripts/changelog_override.json
+-rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/devscripts/changelog_override.schema.json
+-rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/devscripts/check-porn.py
+-rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/devscripts/cli_to_api.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/devscripts/fish-completion.in
+-rwxr-xr-x   0        0        0     1670 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/devscripts/fish-completion.py
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/devscripts/generate_aes_testdata.py
+-rwxr-xr-x   0        0        0     2307 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/devscripts/install_deps.py
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/devscripts/lazy_load_template.py
+-rw-r--r--   0        0        0    41043 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/devscripts/logo.ico
+-rw-r--r--   0        0        0    18382 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/devscripts/make_changelog.py
+-rwxr-xr-x   0        0        0      763 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/devscripts/make_contributing.py
+-rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/devscripts/make_issue_template.py
+-rw-r--r--   0        0        0     4541 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/devscripts/make_lazy_extractors.py
+-rwxr-xr-x   0        0        0     2892 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/devscripts/make_readme.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/devscripts/make_supportedsites.py
+-rw-r--r--   0        0        0     2875 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/devscripts/prepare_manpage.py
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/devscripts/run_tests.bat
+-rwxr-xr-x   0        0        0     2082 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/devscripts/run_tests.py
+-rwxr-xr-x   0        0        0      140 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/devscripts/run_tests.sh
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/devscripts/set-variant.py
+-rwxr-xr-x   0        0        0     4849 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/devscripts/tomlparse.py
+-rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/devscripts/update-version.py
+-rwxr-xr-x   0        0        0      972 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/devscripts/update_changelog.py
+-rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/devscripts/utils.py
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/devscripts/zsh-completion.in
+-rwxr-xr-x   0        0        0     1381 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/devscripts/zsh-completion.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/test/__init__.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/test/conftest.py
+-rw-r--r--   0        0        0    12759 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/test/helper.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/test/parameters.json
+-rw-r--r--   0        0        0   100103 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/test/test_InfoExtractor.py
+-rw-r--r--   0        0        0    57080 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/test/test_YoutubeDL.py
+-rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/test/test_YoutubeDLCookieJar.py
+-rw-r--r--   0        0        0     6862 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/test/test_aes.py
+-rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/test/test_age_restriction.py
+-rw-r--r--   0        0        0     6120 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/test/test_all_urls.py
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/test/test_cache.py
+-rw-r--r--   0        0        0     4706 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/test/test_compat.py
+-rw-r--r--   0        0        0     6721 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/test/test_config.py
+-rw-r--r--   0        0        0    13665 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/test/test_cookies.py
+-rwxr-xr-x   0        0        0    12247 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/test/test_download.py
+-rw-r--r--   0        0        0     4887 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/test/test_downloader_external.py
+-rw-r--r--   0        0        0     3307 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/test/test_downloader_http.py
+-rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/test/test_execution.py
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/test/test_iqiyi_sdk_interpreter.py
+-rw-r--r--   0        0        0    18408 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/test/test_jsinterp.py
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/test/test_netrc.py
+-rw-r--r--   0        0        0    86601 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/test/test_networking.py
+-rw-r--r--   0        0        0     7613 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/test/test_networking_utils.py
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/test/test_overwrites.py
+-rw-r--r--   0        0        0     2766 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/test/test_plugins.py
+-rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/test/test_post_hooks.py
+-rw-r--r--   0        0        0    30542 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/test/test_postprocessors.py
+-rw-r--r--   0        0        0    19659 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/test/test_socks.py
+-rw-r--r--   0        0        0    17397 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/test/test_subtitles.py
+-rw-r--r--   0        0        0    24248 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/test/test_traversal.py
+-rw-r--r--   0        0        0    10649 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/test/test_update.py
+-rw-r--r--   0        0        0    97398 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/test/test_utils.py
+-rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/test/test_verbose_output.py
+-rw-r--r--   0        0        0    16532 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/test/test_websockets.py
+-rw-r--r--   0        0        0     2480 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/test/test_write_annotations.py.disabled
+-rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/test/test_youtube_lists.py
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/test/test_youtube_misc.py
+-rw-r--r--   0        0        0     9763 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/test/test_youtube_signature.py
+-rw-r--r--   0        0        0     3176 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/test/testcert.pem
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/test/testdata/certificate/ca.crt
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/test/testdata/certificate/ca.key
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/test/testdata/certificate/ca.srl
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/test/testdata/certificate/client.crt
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/test/testdata/certificate/client.csr
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/test/testdata/certificate/client.key
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/test/testdata/certificate/clientencrypted.key
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/test/testdata/certificate/clientwithencryptedkey.crt
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/test/testdata/certificate/clientwithkey.crt
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/test/testdata/certificate/instructions.md
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/test/testdata/cookies/httponly_cookies.txt
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/test/testdata/cookies/malformed_cookies.txt
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/test/testdata/cookies/session_cookies.txt
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/test/testdata/f4m/custom_base_url.f4m
+-rw-r--r--   0        0        0     3987 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/test/testdata/ism/ec-3_test.Manifest
+-rw-r--r--   0        0        0    23179 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/test/testdata/ism/sintel.Manifest
+-rw-r--r--   0        0        0     3286 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/test/testdata/m3u8/bipbop_16x9.m3u8
+-rw-r--r--   0        0        0     6291 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/test/testdata/m3u8/img_bipbop_adv_example_fmp4.m3u8
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/test/testdata/mpd/float_duration.mpd
+-rw-r--r--   0        0        0    10268 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/test/testdata/mpd/subtitles.mpd
+-rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/test/testdata/mpd/unfragmented.mpd
+-rw-r--r--   0        0        0    22374 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/test/testdata/mpd/urls_only.mpd
+-rw-r--r--   0        0        0     3928 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/test/testdata/thumbnails/foo %d bar/foo_%d.webp
+-rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/test/testdata/xspf/foo_xspf.xspf
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/test/testdata/yt_dlp_plugins/extractor/_ignore.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/test/testdata/yt_dlp_plugins/extractor/ignore.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/test/testdata/yt_dlp_plugins/extractor/normal.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/test/testdata/yt_dlp_plugins/postprocessor/normal.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/test/testdata/zipped_plugins/yt_dlp_plugins/extractor/zipped.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/test/testdata/zipped_plugins/yt_dlp_plugins/postprocessor/zipped.py
+-rw-r--r--   0        0        0   210976 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/YoutubeDL.py
+-rw-r--r--   0        0        0    47675 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/__init__.py
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/__main__.py
+-rw-r--r--   0        0        0    22402 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/aes.py
+-rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/cache.py
+-rw-r--r--   0        0        0    54844 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/cookies.py
+-rw-r--r--   0        0        0    34646 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/jsinterp.py
+-rw-r--r--   0        0        0     5328 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/minicurses.py
+-rw-r--r--   0        0        0    96530 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/options.py
+-rw-r--r--   0        0        0     6358 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/plugins.py
+-rw-r--r--   0        0        0     8943 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/socks.py
+-rw-r--r--   0        0        0    24873 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/update.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/version.py
+-rw-r--r--   0        0        0    11441 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/webvtt.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/__pyinstaller/__init__.py
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/__pyinstaller/hook-yt_dlp.py
+-rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/compat/__init__.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/compat/_deprecated.py
+-rw-r--r--   0        0        0     3976 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/compat/_legacy.py
+-rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/compat/compat_utils.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/compat/functools.py
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/compat/imghdr.py
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/compat/shutil.py
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/compat/types.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/compat/urllib/__init__.py
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/compat/urllib/request.py
+-rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/dependencies/Cryptodome.py
+-rw-r--r--   0        0        0     2206 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/dependencies/__init__.py
+-rw-r--r--   0        0        0     4497 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/downloader/__init__.py
+-rw-r--r--   0        0        0    19180 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/downloader/common.py
+-rw-r--r--   0        0        0     3620 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/downloader/dash.py
+-rw-r--r--   0        0        0    28090 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/downloader/external.py
+-rw-r--r--   0        0        0    15344 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/downloader/f4m.py
+-rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/downloader/fc2.py
+-rw-r--r--   0        0        0    21795 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/downloader/fragment.py
+-rw-r--r--   0        0        0    17819 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/downloader/hls.py
+-rw-r--r--   0        0        0    16863 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/downloader/http.py
+-rw-r--r--   0        0        0    11644 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/downloader/ism.py
+-rw-r--r--   0        0        0     6182 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/downloader/mhtml.py
+-rw-r--r--   0        0        0     5387 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/downloader/niconico.py
+-rw-r--r--   0        0        0     8923 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/downloader/rtmp.py
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/downloader/rtsp.py
+-rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/downloader/websocket.py
+-rw-r--r--   0        0        0    10873 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/downloader/youtube_live_chat.py
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/__init__.py
+-rw-r--r--   0        0        0    52880 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/_extractors.py
+-rw-r--r--   0        0        0    17696 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/abc.py
+-rw-r--r--   0        0        0     6328 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/abcnews.py
+-rw-r--r--   0        0        0     4596 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/abcotvs.py
+-rw-r--r--   0        0        0    19939 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/abematv.py
+-rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/academicearth.py
+-rw-r--r--   0        0        0     5571 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/acast.py
+-rw-r--r--   0        0        0     7946 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/acfun.py
+-rw-r--r--   0        0        0    14123 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/adn.py
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/adobeconnect.py
+-rw-r--r--   0        0        0    52679 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/adobepass.py
+-rw-r--r--   0        0        0    10277 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/adobetv.py
+-rw-r--r--   0        0        0     7833 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/adultswim.py
+-rw-r--r--   0        0        0    13304 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/aenetworks.py
+-rw-r--r--   0        0        0     3299 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/aeonco.py
+-rw-r--r--   0        0        0    15841 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/afreecatv.py
+-rw-r--r--   0        0        0     9821 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/agora.py
+-rw-r--r--   0        0        0     4085 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/airtv.py
+-rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/aitube.py
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/aliexpress.py
+-rw-r--r--   0        0        0     3364 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/aljazeera.py
+-rw-r--r--   0        0        0     4803 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/allocine.py
+-rw-r--r--   0        0        0     9202 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/allstar.py
+-rw-r--r--   0        0        0     2683 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/alphaporno.py
+-rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/alsace20tv.py
+-rw-r--r--   0        0        0     3976 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/altcensored.py
+-rw-r--r--   0        0        0     6501 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/alura.py
+-rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/amadeustv.py
+-rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/amara.py
+-rw-r--r--   0        0        0     6589 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/amazon.py
+-rw-r--r--   0        0        0    10729 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/amazonminitv.py
+-rw-r--r--   0        0        0     6154 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/amcnetworks.py
+-rw-r--r--   0        0        0     8724 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/americastestkitchen.py
+-rw-r--r--   0        0        0     4225 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/amp.py
+-rw-r--r--   0        0        0     4800 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/anchorfm.py
+-rw-r--r--   0        0        0     2550 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/angel.py
+-rw-r--r--   0        0        0     5967 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/antenna.py
+-rw-r--r--   0        0        0    26757 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/anvato.py
+-rw-r--r--   0        0        0     5467 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/aol.py
+-rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/apa.py
+-rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/aparat.py
+-rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/appleconnect.py
+-rw-r--r--   0        0        0     3624 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/applepodcasts.py
+-rw-r--r--   0        0        0    10196 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/appletrailers.py
+-rw-r--r--   0        0        0    46353 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/archiveorg.py
+-rw-r--r--   0        0        0     7514 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/arcpublishing.py
+-rw-r--r--   0        0        0    26748 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ard.py
+-rw-r--r--   0        0        0     7199 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/arkena.py
+-rw-r--r--   0        0        0     3556 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/arnes.py
+-rw-r--r--   0        0        0    12859 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/art19.py
+-rw-r--r--   0        0        0    14734 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/arte.py
+-rw-r--r--   0        0        0     6806 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/asobichannel.py
+-rw-r--r--   0        0        0     6974 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/asobistage.py
+-rw-r--r--   0        0        0     4149 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/atresplayer.py
+-rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/atscaleconf.py
+-rw-r--r--   0        0        0     4179 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/atvat.py
+-rw-r--r--   0        0        0     3929 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/audimedia.py
+-rw-r--r--   0        0        0     2866 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/audioboom.py
+-rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/audiodraft.py
+-rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/audiomack.py
+-rw-r--r--   0        0        0    10773 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/audius.py
+-rw-r--r--   0        0        0     7133 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/awaan.py
+-rw-r--r--   0        0        0     3121 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/aws.py
+-rw-r--r--   0        0        0     3328 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/axs.py
+-rw-r--r--   0        0        0     2424 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/azmedien.py
+-rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/baidu.py
+-rw-r--r--   0        0        0     6273 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/banbye.py
+-rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/bandaichannel.py
+-rw-r--r--   0        0        0    18597 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/bandcamp.py
+-rw-r--r--   0        0        0     5303 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/bannedvideo.py
+-rw-r--r--   0        0        0    72720 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/bbc.py
+-rw-r--r--   0        0        0     4614 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/beatbump.py
+-rw-r--r--   0        0        0     3246 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/beatport.py
+-rw-r--r--   0        0        0     3180 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/beeg.py
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/behindkink.py
+-rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/bellmedia.py
+-rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/berufetv.py
+-rw-r--r--   0        0        0     2763 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/bet.py
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/bfi.py
+-rw-r--r--   0        0        0     5422 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/bfmtv.py
+-rw-r--r--   0        0        0     6831 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/bibeltv.py
+-rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/bigflix.py
+-rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/bigo.py
+-rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/bild.py
+-rw-r--r--   0        0        0    93818 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/bilibili.py
+-rw-r--r--   0        0        0     3454 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/biobiochiletv.py
+-rw-r--r--   0        0        0    11755 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/bitchute.py
+-rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/blackboardcollaborate.py
+-rw-r--r--   0        0        0     4291 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/bleacherreport.py
+-rw-r--r--   0        0        0     4733 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/blerp.py
+-rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/blogger.py
+-rw-r--r--   0        0        0     3180 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/bloomberg.py
+-rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/bokecc.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/bongacams.py
+-rw-r--r--   0        0        0     8894 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/boosty.py
+-rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/bostonglobe.py
+-rw-r--r--   0        0        0     4229 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/box.py
+-rw-r--r--   0        0        0     4756 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/boxcast.py
+-rw-r--r--   0        0        0     7723 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/bpb.py
+-rw-r--r--   0        0        0     7476 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/br.py
+-rw-r--r--   0        0        0    12920 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/brainpop.py
+-rw-r--r--   0        0        0     8277 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/bravotv.py
+-rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/breitbart.py
+-rw-r--r--   0        0        0    42705 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/brightcove.py
+-rw-r--r--   0        0        0     5378 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/brilliantpala.py
+-rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/bundesliga.py
+-rw-r--r--   0        0        0     5116 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/bundestag.py
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/businessinsider.py
+-rw-r--r--   0        0        0     3609 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/buzzfeed.py
+-rw-r--r--   0        0        0     3929 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/byutv.py
+-rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/c56.py
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/cableav.py
+-rw-r--r--   0        0        0     8123 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/callin.py
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/caltrans.py
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/cam4.py
+-rw-r--r--   0        0        0     5715 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/camdemy.py
+-rw-r--r--   0        0        0     3458 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/camfm.py
+-rw-r--r--   0        0        0     2826 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/cammodels.py
+-rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/camsoda.py
+-rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/camtasia.py
+-rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/canal1.py
+-rw-r--r--   0        0        0     4269 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/canalalpha.py
+-rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/canalc2.py
+-rw-r--r--   0        0        0     4358 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/canalplus.py
+-rw-r--r--   0        0        0     5733 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/caracoltv.py
+-rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/cartoonnetwork.py
+-rw-r--r--   0        0        0    30351 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/cbc.py
+-rw-r--r--   0        0        0    11862 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/cbs.py
+-rw-r--r--   0        0        0    19544 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/cbsnews.py
+-rw-r--r--   0        0        0     4883 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/cbssports.py
+-rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ccc.py
+-rw-r--r--   0        0        0     5381 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ccma.py
+-rw-r--r--   0        0        0     7391 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/cctv.py
+-rw-r--r--   0        0        0    13880 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/cda.py
+-rw-r--r--   0        0        0     2837 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/cellebrite.py
+-rw-r--r--   0        0        0    11811 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ceskatelevize.py
+-rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/cgtn.py
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/charlierose.py
+-rw-r--r--   0        0        0     3816 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/chaturbate.py
+-rw-r--r--   0        0        0     4822 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/chilloutzone.py
+-rw-r--r--   0        0        0     5651 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/chzzk.py
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/cinemax.py
+-rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/cinetecamilano.py
+-rw-r--r--   0        0        0     5774 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/cineverse.py
+-rw-r--r--   0        0        0     5858 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ciscolive.py
+-rw-r--r--   0        0        0     4432 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ciscowebex.py
+-rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/cjsw.py
+-rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/clipchamp.py
+-rw-r--r--   0        0        0     2493 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/clippit.py
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/cliprs.py
+-rw-r--r--   0        0        0     3016 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/closertotruth.py
+-rw-r--r--   0        0        0     3235 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/cloudflarestream.py
+-rw-r--r--   0        0        0     2971 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/cloudycdn.py
+-rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/clubic.py
+-rw-r--r--   0        0        0     3083 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/clyp.py
+-rw-r--r--   0        0        0     2243 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/cmt.py
+-rw-r--r--   0        0        0     4615 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/cnbc.py
+-rw-r--r--   0        0        0     9171 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/cnn.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/comedycentral.py
+-rw-r--r--   0        0        0   192000 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/common.py
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/commonmistakes.py
+-rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/commonprotocols.py
+-rw-r--r--   0        0        0     9730 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/condenast.py
+-rw-r--r--   0        0        0     4102 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/contv.py
+-rw-r--r--   0        0        0     6313 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/corus.py
+-rw-r--r--   0        0        0     4559 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/coub.py
+-rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/cozytv.py
+-rw-r--r--   0        0        0     5703 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/cpac.py
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/cracked.py
+-rw-r--r--   0        0        0     9681 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/crackle.py
+-rw-r--r--   0        0        0     3186 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/craftsy.py
+-rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/crooksandliars.py
+-rw-r--r--   0        0        0     4162 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/crowdbunker.py
+-rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/crtvg.py
+-rw-r--r--   0        0        0    28345 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/crunchyroll.py
+-rw-r--r--   0        0        0    12105 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/cspan.py
+-rw-r--r--   0        0        0     3591 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ctsnews.py
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ctv.py
+-rw-r--r--   0        0        0     2554 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ctvnews.py
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/cultureunplugged.py
+-rw-r--r--   0        0        0     8391 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/curiositystream.py
+-rw-r--r--   0        0        0     4002 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/cwtv.py
+-rw-r--r--   0        0        0     6285 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/cybrary.py
+-rw-r--r--   0        0        0     6335 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/dacast.py
+-rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/dailymail.py
+-rw-r--r--   0        0        0    18453 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/dailymotion.py
+-rw-r--r--   0        0        0     4854 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/dailywire.py
+-rw-r--r--   0        0        0     5500 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/damtomo.py
+-rw-r--r--   0        0        0     9431 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/daum.py
+-rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/daystar.py
+-rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/dbtv.py
+-rw-r--r--   0        0        0     3531 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/dctp.py
+-rw-r--r--   0        0        0     5154 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/deezer.py
+-rw-r--r--   0        0        0     3007 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/democracynow.py
+-rw-r--r--   0        0        0     8088 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/detik.py
+-rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/deuxm.py
+-rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/dfb.py
+-rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/dhm.py
+-rw-r--r--   0        0        0     6419 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/digitalconcerthall.py
+-rw-r--r--   0        0        0     3257 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/digiteka.py
+-rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/discogs.py
+-rw-r--r--   0        0        0     4855 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/discovery.py
+-rw-r--r--   0        0        0     6002 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/discoverygo.py
+-rw-r--r--   0        0        0     6770 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/disney.py
+-rw-r--r--   0        0        0     4946 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/dispeak.py
+-rw-r--r--   0        0        0     8692 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/dlf.py
+-rw-r--r--   0        0        0     2976 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/dlive.py
+-rw-r--r--   0        0        0    11836 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/douyutv.py
+-rw-r--r--   0        0        0    41198 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/dplay.py
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/drbonanza.py
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/dreisat.py
+-rw-r--r--   0        0        0     4187 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/drooble.py
+-rw-r--r--   0        0        0     4023 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/dropbox.py
+-rw-r--r--   0        0        0     9914 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/dropout.py
+-rw-r--r--   0        0        0     3796 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/drtuber.py
+-rw-r--r--   0        0        0    15934 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/drtv.py
+-rw-r--r--   0        0        0     2742 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/dtube.py
+-rw-r--r--   0        0        0     8532 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/duboku.py
+-rw-r--r--   0        0        0     3999 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/dumpert.py
+-rw-r--r--   0        0        0     4118 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/duoplay.py
+-rw-r--r--   0        0        0     7435 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/dvtv.py
+-rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/dw.py
+-rw-r--r--   0        0        0     8194 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/eagleplatform.py
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ebaumsworld.py
+-rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ebay.py
+-rw-r--r--   0        0        0     4938 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/egghead.py
+-rw-r--r--   0        0        0     5811 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/eighttracks.py
+-rw-r--r--   0        0        0     3612 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/einthusan.py
+-rw-r--r--   0        0        0     3167 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/eitb.py
+-rw-r--r--   0        0        0     3327 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/elementorembed.py
+-rw-r--r--   0        0        0     2585 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/elonet.py
+-rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/elpais.py
+-rw-r--r--   0        0        0     2650 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/eltrecetv.py
+-rw-r--r--   0        0        0     5286 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/embedly.py
+-rw-r--r--   0        0        0     4195 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/epicon.py
+-rw-r--r--   0        0        0     4090 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/epidemicsound.py
+-rw-r--r--   0        0        0     7863 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/eplus.py
+-rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/epoch.py
+-rw-r--r--   0        0        0     5047 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/eporner.py
+-rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/erocast.py
+-rw-r--r--   0        0        0     4467 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/eroprofile.py
+-rw-r--r--   0        0        0     8855 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/err.py
+-rw-r--r--   0        0        0    12620 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ertgr.py
+-rw-r--r--   0        0        0    17218 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/espn.py
+-rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ettutv.py
+-rw-r--r--   0        0        0     6666 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/europa.py
+-rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/europeantour.py
+-rw-r--r--   0        0        0     6617 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/eurosport.py
+-rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/euscreen.py
+-rw-r--r--   0        0        0     4088 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/expressen.py
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/extractors.py
+-rw-r--r--   0        0        0     2630 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/eyedotv.py
+-rw-r--r--   0        0        0    48374 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/facebook.py
+-rw-r--r--   0        0        0     7218 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/fancode.py
+-rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/fathom.py
+-rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/faz.py
+-rw-r--r--   0        0        0    10584 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/fc2.py
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/fczenit.py
+-rw-r--r--   0        0        0     3845 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/fifa.py
+-rw-r--r--   0        0        0     5899 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/filmon.py
+-rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/filmweb.py
+-rw-r--r--   0        0        0     6361 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/firsttv.py
+-rw-r--r--   0        0        0     3045 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/fivetv.py
+-rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/flextv.py
+-rw-r--r--   0        0        0     4701 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/flickr.py
+-rw-r--r--   0        0        0    14314 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/floatplane.py
+-rw-r--r--   0        0        0     2550 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/folketinget.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/footyroom.py
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/formula1.py
+-rw-r--r--   0        0        0    11501 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/fourtube.py
+-rw-r--r--   0        0        0     6849 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/fox.py
+-rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/fox9.py
+-rw-r--r--   0        0        0     7661 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/foxnews.py
+-rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/foxsports.py
+-rw-r--r--   0        0        0     4848 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/fptplay.py
+-rw-r--r--   0        0        0     2158 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/franceinter.py
+-rw-r--r--   0        0        0    17035 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/francetv.py
+-rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/freesound.py
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/freespeech.py
+-rw-r--r--   0        0        0     5529 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/freetv.py
+-rw-r--r--   0        0        0     8597 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/frontendmasters.py
+-rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/fujitv.py
+-rw-r--r--   0        0        0    14971 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/funimation.py
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/funk.py
+-rw-r--r--   0        0        0     3272 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/funker530.py
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/fuyintv.py
+-rw-r--r--   0        0        0     5675 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/gab.py
+-rw-r--r--   0        0        0     4504 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/gaia.py
+-rw-r--r--   0        0        0    25081 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/gamejolt.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/gamespot.py
+-rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/gamestar.py
+-rw-r--r--   0        0        0     3707 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/gaskrank.py
+-rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/gazeta.py
+-rw-r--r--   0        0        0     8544 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/gdcvault.py
+-rw-r--r--   0        0        0     8522 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/gedidigital.py
+-rw-r--r--   0        0        0   119486 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/generic.py
+-rw-r--r--   0        0        0     4608 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/genericembeds.py
+-rw-r--r--   0        0        0     6103 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/genius.py
+-rw-r--r--   0        0        0     7544 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/getcourseru.py
+-rw-r--r--   0        0        0     7845 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/gettr.py
+-rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/giantbomb.py
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/gigya.py
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/glide.py
+-rw-r--r--   0        0        0     9446 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/globalplayer.py
+-rw-r--r--   0        0        0    10140 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/globo.py
+-rw-r--r--   0        0        0     8517 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/glomex.py
+-rw-r--r--   0        0        0     3926 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/gmanetwork.py
+-rw-r--r--   0        0        0    14143 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/go.py
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/godtube.py
+-rw-r--r--   0        0        0     3543 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/gofile.py
+-rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/golem.py
+-rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/goodgame.py
+-rw-r--r--   0        0        0    14775 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/googledrive.py
+-rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/googlepodcasts.py
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/googlesearch.py
+-rw-r--r--   0        0        0    16911 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/goplay.py
+-rw-r--r--   0        0        0     3768 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/gopro.py
+-rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/goshgay.py
+-rw-r--r--   0        0        0     2727 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/gotostage.py
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/gputechconf.py
+-rw-r--r--   0        0        0     4399 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/gronkh.py
+-rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/groupon.py
+-rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/harpodeon.py
+-rw-r--r--   0        0        0     6035 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/hbo.py
+-rw-r--r--   0        0        0     3489 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/hearthisat.py
+-rw-r--r--   0        0        0     8432 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/heise.py
+-rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/hellporno.py
+-rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/hgtv.py
+-rw-r--r--   0        0        0     4945 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/hidive.py
+-rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/historicfilms.py
+-rw-r--r--   0        0        0     2228 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/hitrecord.py
+-rw-r--r--   0        0        0     6867 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/hketv.py
+-rw-r--r--   0        0        0     2871 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/hollywoodreporter.py
+-rw-r--r--   0        0        0     4267 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/holodex.py
+-rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/hotnewhiphop.py
+-rw-r--r--   0        0        0    18185 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/hotstar.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/hrefli.py
+-rw-r--r--   0        0        0     3845 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/hrfensehen.py
+-rw-r--r--   0        0        0     7049 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/hrti.py
+-rw-r--r--   0        0        0     3600 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/hse.py
+-rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/huajiao.py
+-rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/huffpost.py
+-rw-r--r--   0        0        0     7699 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/hungama.py
+-rw-r--r--   0        0        0     4862 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/huya.py
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/hypem.py
+-rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/hypergryph.py
+-rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/hytale.py
+-rw-r--r--   0        0        0     7391 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/icareus.py
+-rw-r--r--   0        0        0     5787 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ichinanalive.py
+-rw-r--r--   0        0        0     4868 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/idolplus.py
+-rw-r--r--   0        0        0    16322 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ign.py
+-rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/iheart.py
+-rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ilpost.py
+-rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/iltalehti.py
+-rw-r--r--   0        0        0     5636 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/imdb.py
+-rw-r--r--   0        0        0     4828 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/imggaming.py
+-rw-r--r--   0        0        0    14257 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/imgur.py
+-rw-r--r--   0        0        0     3617 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ina.py
+-rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/inc.py
+-rw-r--r--   0        0        0     4188 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/indavideo.py
+-rw-r--r--   0        0        0     5112 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/infoq.py
+-rw-r--r--   0        0        0    30961 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/instagram.py
+-rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/internazionale.py
+-rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/internetvideoarchive.py
+-rw-r--r--   0        0        0    10919 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/iprima.py
+-rw-r--r--   0        0        0    31244 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/iqiyi.py
+-rw-r--r--   0        0        0     3177 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/islamchannel.py
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/israelnationalnews.py
+-rw-r--r--   0        0        0     5343 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/itprotv.py
+-rw-r--r--   0        0        0    10682 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/itv.py
+-rw-r--r--   0        0        0    10052 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ivi.py
+-rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ivideon.py
+-rw-r--r--   0        0        0    11627 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/iwara.py
+-rw-r--r--   0        0        0     3426 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ixigua.py
+-rw-r--r--   0        0        0     4059 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/izlesene.py
+-rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/jable.py
+-rw-r--r--   0        0        0     7902 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/jamendo.py
+-rw-r--r--   0        0        0    10351 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/japandiet.py
+-rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/jeuxvideo.py
+-rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/jiosaavn.py
+-rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/jixie.py
+-rw-r--r--   0        0        0     3865 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/joj.py
+-rw-r--r--   0        0        0     4512 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/joqrag.py
+-rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/jove.py
+-rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/jstream.py
+-rw-r--r--   0        0        0     6333 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/jtbc.py
+-rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/jwplatform.py
+-rw-r--r--   0        0        0     5912 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/kakao.py
+-rw-r--r--   0        0        0    24329 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/kaltura.py
+-rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/kankanews.py
+-rw-r--r--   0        0        0     2283 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/karaoketv.py
+-rw-r--r--   0        0        0     3488 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/kelbyone.py
+-rw-r--r--   0        0        0     4103 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/khanacademy.py
+-rw-r--r--   0        0        0     5571 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/kick.py
+-rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/kicker.py
+-rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/kickstarter.py
+-rw-r--r--   0        0        0     7835 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/kinja.py
+-rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/kinopoisk.py
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/kommunetv.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/kompas.py
+-rw-r--r--   0        0        0     4707 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/koo.py
+-rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/krasview.py
+-rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/kth.py
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ku6.py
+-rw-r--r--   0        0        0     5694 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/kukululive.py
+-rw-r--r--   0        0        0    12524 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/kuwo.py
+-rw-r--r--   0        0        0     9434 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/la7.py
+-rw-r--r--   0        0        0     4748 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/lastfm.py
+-rw-r--r--   0        0        0     2772 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/laxarxames.py
+-rw-r--r--   0        0        0   772427 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/lazy_extractors.py
+-rw-r--r--   0        0        0    17579 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/lbry.py
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/lci.py
+-rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/lcp.py
+-rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/lecture2go.py
+-rw-r--r--   0        0        0     8380 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/lecturio.py
+-rw-r--r--   0        0        0    12993 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/leeco.py
+-rw-r--r--   0        0        0     5417 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/lefigaro.py
+-rw-r--r--   0        0        0     5894 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/lego.py
+-rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/lemonde.py
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/lenta.py
+-rw-r--r--   0        0        0     4935 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/libraryofcongress.py
+-rw-r--r--   0        0        0     3673 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/libsyn.py
+-rw-r--r--   0        0        0     9524 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/lifenews.py
+-rw-r--r--   0        0        0     7021 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/likee.py
+-rw-r--r--   0        0        0    15006 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/limelight.py
+-rw-r--r--   0        0        0    10886 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/linkedin.py
+-rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/liputan6.py
+-rw-r--r--   0        0        0     4167 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/listennotes.py
+-rw-r--r--   0        0        0     6884 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/litv.py
+-rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/livejournal.py
+-rw-r--r--   0        0        0    14577 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/livestream.py
+-rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/livestreamfails.py
+-rw-r--r--   0        0        0     6318 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/lnkgo.py
+-rw-r--r--   0        0        0    18063 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/loom.py
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/lovehomeporn.py
+-rw-r--r--   0        0        0     4038 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/lrt.py
+-rw-r--r--   0        0        0    12070 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/lsm.py
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/lumni.py
+-rw-r--r--   0        0        0    12446 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/lynda.py
+-rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/maariv.py
+-rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/magellantv.py
+-rw-r--r--   0        0        0     2772 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/magentamusik.py
+-rw-r--r--   0        0        0    12022 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/mailru.py
+-rw-r--r--   0        0        0     9235 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/mainstreaming.py
+-rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/mangomolo.py
+-rw-r--r--   0        0        0     5148 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/manoto.py
+-rw-r--r--   0        0        0     5946 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/manyvids.py
+-rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/maoritv.py
+-rw-r--r--   0        0        0     4507 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/markiza.py
+-rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/massengeschmacktv.py
+-rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/masters.py
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/matchtv.py
+-rw-r--r--   0        0        0     3897 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/mbn.py
+-rw-r--r--   0        0        0     6836 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/mdr.py
+-rw-r--r--   0        0        0     6055 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/medaltv.py
+-rw-r--r--   0        0        0     4930 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/mediaite.py
+-rw-r--r--   0        0        0     6890 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/mediaklikk.py
+-rw-r--r--   0        0        0     4122 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/medialaan.py
+-rw-r--r--   0        0        0    13331 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/mediaset.py
+-rw-r--r--   0        0        0    16617 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/mediasite.py
+-rw-r--r--   0        0        0    10321 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/mediastream.py
+-rw-r--r--   0        0        0     4078 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/mediaworksnz.py
+-rw-r--r--   0        0        0     6712 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/medici.py
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/megaphone.py
+-rw-r--r--   0        0        0     6726 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/megatvcom.py
+-rw-r--r--   0        0        0     3537 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/meipai.py
+-rw-r--r--   0        0        0     2158 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/melonvod.py
+-rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/metacritic.py
+-rw-r--r--   0        0        0     6473 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/mgtv.py
+-rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/microsoftembed.py
+-rw-r--r--   0        0        0     5381 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/microsoftstream.py
+-rw-r--r--   0        0        0     7306 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/microsoftvirtualacademy.py
+-rw-r--r--   0        0        0    11551 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/mildom.py
+-rw-r--r--   0        0        0     6829 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/minds.py
+-rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/minoto.py
+-rw-r--r--   0        0        0     4880 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/mirrativ.py
+-rw-r--r--   0        0        0     4403 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/mirrorcouk.py
+-rw-r--r--   0        0        0     5165 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/mit.py
+-rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/mitele.py
+-rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/mixch.py
+-rw-r--r--   0        0        0    12793 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/mixcloud.py
+-rw-r--r--   0        0        0    14610 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/mlb.py
+-rw-r--r--   0        0        0     6696 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/mlssoccer.py
+-rw-r--r--   0        0        0     2959 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/mocha.py
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/mojvideo.py
+-rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/monstercat.py
+-rw-r--r--   0        0        0    10821 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/motherless.py
+-rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/motorsport.py
+-rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/moviepilot.py
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/moview.py
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/moviezine.py
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/movingimage.py
+-rw-r--r--   0        0        0     7501 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/msn.py
+-rw-r--r--   0        0        0    25584 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/mtv.py
+-rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/muenchentv.py
+-rw-r--r--   0        0        0     5035 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/murrtube.py
+-rw-r--r--   0        0        0     4093 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/museai.py
+-rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/musescore.py
+-rw-r--r--   0        0        0     7179 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/musicdex.py
+-rw-r--r--   0        0        0     6379 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/mx3.py
+-rw-r--r--   0        0        0    10007 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/mxplayer.py
+-rw-r--r--   0        0        0     7765 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/myspace.py
+-rw-r--r--   0        0        0     3714 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/myspass.py
+-rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/myvideoge.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/myvidster.py
+-rw-r--r--   0        0        0     3746 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/mzaalo.py
+-rw-r--r--   0        0        0     6814 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/n1.py
+-rw-r--r--   0        0        0     4303 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/nate.py
+-rw-r--r--   0        0        0     3057 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/nationalgeographic.py
+-rw-r--r--   0        0        0    16447 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/naver.py
+-rw-r--r--   0        0        0    16157 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/nba.py
+-rw-r--r--   0        0        0    35311 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/nbc.py
+-rw-r--r--   0        0        0    18232 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ndr.py
+-rw-r--r--   0        0        0     4502 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ndtv.py
+-rw-r--r--   0        0        0    20864 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/nebula.py
+-rw-r--r--   0        0        0     9389 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/nekohacker.py
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/nerdcubed.py
+-rw-r--r--   0        0        0    23769 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/neteasemusic.py
+-rw-r--r--   0        0        0    10988 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/netverse.py
+-rw-r--r--   0        0        0     2922 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/netzkino.py
+-rw-r--r--   0        0        0    11825 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/newgrounds.py
+-rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/newspicks.py
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/newsy.py
+-rw-r--r--   0        0        0     9075 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/nextmedia.py
+-rw-r--r--   0        0        0    21193 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/nexx.py
+-rw-r--r--   0        0        0    13126 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/nfb.py
+-rw-r--r--   0        0        0     5859 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/nfhsnetwork.py
+-rw-r--r--   0        0        0    15532 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/nfl.py
+-rw-r--r--   0        0        0    34642 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/nhk.py
+-rw-r--r--   0        0        0     4912 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/nhl.py
+-rw-r--r--   0        0        0    10478 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/nick.py
+-rw-r--r--   0        0        0    44728 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/niconico.py
+-rw-r--r--   0        0        0    18094 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/niconicochannelplus.py
+-rw-r--r--   0        0        0    10389 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ninaprotocol.py
+-rw-r--r--   0        0        0     5131 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ninecninemedia.py
+-rw-r--r--   0        0        0     5178 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ninegag.py
+-rw-r--r--   0        0        0     3634 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ninenews.py
+-rw-r--r--   0        0        0     5299 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ninenow.py
+-rw-r--r--   0        0        0     5473 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/nintendo.py
+-rw-r--r--   0        0        0    13650 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/nitter.py
+-rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/nobelprize.py
+-rw-r--r--   0        0        0     5056 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/noice.py
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/nonktube.py
+-rw-r--r--   0        0        0     3441 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/noodlemagazine.py
+-rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/noovo.py
+-rw-r--r--   0        0        0     5817 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/nosnl.py
+-rw-r--r--   0        0        0    12074 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/nova.py
+-rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/novaplay.py
+-rw-r--r--   0        0        0     5954 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/nowness.py
+-rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/noz.py
+-rw-r--r--   0        0        0    22320 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/npo.py
+-rw-r--r--   0        0        0     5740 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/npr.py
+-rw-r--r--   0        0        0    32207 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/nrk.py
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/nrl.py
+-rw-r--r--   0        0        0     2277 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ntvcojp.py
+-rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ntvde.py
+-rw-r--r--   0        0        0     5666 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ntvru.py
+-rw-r--r--   0        0        0     4492 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/nubilesporn.py
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/nuevo.py
+-rw-r--r--   0        0        0     7311 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/nuum.py
+-rw-r--r--   0        0        0     3532 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/nuvid.py
+-rw-r--r--   0        0        0    17309 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/nytimes.py
+-rw-r--r--   0        0        0     5896 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/nzherald.py
+-rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/nzonscreen.py
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/nzz.py
+-rw-r--r--   0        0        0     4284 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/odkmedia.py
+-rw-r--r--   0        0        0    17342 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/odnoklassniki.py
+-rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/oftv.py
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/oktoberfesttv.py
+-rw-r--r--   0        0        0     2868 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/olympics.py
+-rw-r--r--   0        0        0     3924 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/on24.py
+-rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/once.py
+-rw-r--r--   0        0        0     6757 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ondemandkorea.py
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/onefootball.py
+-rw-r--r--   0        0        0     5136 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/onenewsnz.py
+-rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/oneplace.py
+-rw-r--r--   0        0        0     9845 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/onet.py
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/onionstudios.py
+-rw-r--r--   0        0        0     7984 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/opencast.py
+-rw-r--r--   0        0        0     8647 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/openload.py
+-rw-r--r--   0        0        0     6204 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/openrec.py
+-rw-r--r--   0        0        0     3126 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ora.py
+-rw-r--r--   0        0        0    24396 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/orf.py
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/outsidetv.py
+-rw-r--r--   0        0        0     2709 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/owncloud.py
+-rw-r--r--   0        0        0     6166 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/packtpub.py
+-rw-r--r--   0        0        0     4455 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/palcomp3.py
+-rw-r--r--   0        0        0    25808 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/panopto.py
+-rw-r--r--   0        0        0     7483 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/paramountplus.py
+-rw-r--r--   0        0        0     3802 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/parler.py
+-rw-r--r--   0        0        0     2772 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/parlview.py
+-rw-r--r--   0        0        0    20496 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/patreon.py
+-rw-r--r--   0        0        0    38530 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/pbs.py
+-rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/pearvideo.py
+-rw-r--r--   0        0        0     7214 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/peekvids.py
+-rw-r--r--   0        0        0    78541 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/peertube.py
+-rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/peertv.py
+-rw-r--r--   0        0        0     8858 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/peloton.py
+-rw-r--r--   0        0        0     3246 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/performgroup.py
+-rw-r--r--   0        0        0     7323 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/periscope.py
+-rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/pgatour.py
+-rw-r--r--   0        0        0     4068 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/philharmoniedeparis.py
+-rw-r--r--   0        0        0     4961 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/phoenix.py
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/photobucket.py
+-rw-r--r--   0        0        0     4794 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/piapro.py
+-rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/piaulizaportal.py
+-rw-r--r--   0        0        0     4640 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/picarto.py
+-rw-r--r--   0        0        0     6898 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/piksel.py
+-rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/pinkbike.py
+-rw-r--r--   0        0        0     9595 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/pinterest.py
+-rw-r--r--   0        0        0     4752 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/pixivsketch.py
+-rw-r--r--   0        0        0     4923 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/pladform.py
+-rw-r--r--   0        0        0     2922 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/planetmarathi.py
+-rw-r--r--   0        0        0     7404 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/platzi.py
+-rw-r--r--   0        0        0     3655 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/playplustv.py
+-rw-r--r--   0        0        0     8782 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/playsuisse.py
+-rw-r--r--   0        0        0     7115 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/playtvak.py
+-rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/playwire.py
+-rw-r--r--   0        0        0    18375 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/pluralsight.py
+-rw-r--r--   0        0        0     8093 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/plutotv.py
+-rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/podbayfm.py
+-rw-r--r--   0        0        0     3761 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/podchaser.py
+-rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/podomatic.py
+-rw-r--r--   0        0        0     5475 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/pokemon.py
+-rw-r--r--   0        0        0     4180 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/pokergo.py
+-rw-r--r--   0        0        0     3150 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/polsatgo.py
+-rw-r--r--   0        0        0    24519 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/polskieradio.py
+-rw-r--r--   0        0        0     3258 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/popcorntimes.py
+-rw-r--r--   0        0        0     2630 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/popcorntv.py
+-rw-r--r--   0        0        0     4047 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/porn91.py
+-rw-r--r--   0        0        0     4490 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/pornbox.py
+-rw-r--r--   0        0        0     3500 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/pornflip.py
+-rw-r--r--   0        0        0    31546 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/pornhub.py
+-rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/pornotube.py
+-rw-r--r--   0        0        0     3916 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/pornovoisines.py
+-rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/pornoxo.py
+-rw-r--r--   0        0        0     8116 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/pr0gramm.py
+-rw-r--r--   0        0        0     5722 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/prankcast.py
+-rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/premiershiprugby.py
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/presstv.py
+-rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/projectveritas.py
+-rw-r--r--   0        0        0    21515 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/prosiebensat1.py
+-rw-r--r--   0        0        0    16065 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/prx.py
+-rw-r--r--   0        0        0     8375 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/puhutv.py
+-rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/puls4.py
+-rw-r--r--   0        0        0     2719 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/pyvideo.py
+-rw-r--r--   0        0        0     7437 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/qdance.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/qingting.py
+-rw-r--r--   0        0        0    13550 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/qqmusic.py
+-rw-r--r--   0        0        0     4657 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/r7.py
+-rw-r--r--   0        0        0     9799 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/radiko.py
+-rw-r--r--   0        0        0     6253 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/radiocanada.py
+-rw-r--r--   0        0        0     6253 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/radiocomercial.py
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/radiode.py
+-rw-r--r--   0        0        0    18223 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/radiofrance.py
+-rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/radiojavan.py
+-rw-r--r--   0        0        0     3345 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/radiokapital.py
+-rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/radiozet.py
+-rw-r--r--   0        0        0     6929 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/radlive.py
+-rw-r--r--   0        0        0    34159 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/rai.py
+-rw-r--r--   0        0        0     6124 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/raywenderlich.py
+-rw-r--r--   0        0        0     5343 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/rbgtum.py
+-rw-r--r--   0        0        0    16249 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/rcs.py
+-rw-r--r--   0        0        0    16483 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/rcti.py
+-rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/rds.py
+-rw-r--r--   0        0        0    14580 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/redbee.py
+-rw-r--r--   0        0        0     9273 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/redbulltv.py
+-rw-r--r--   0        0        0    14147 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/reddit.py
+-rw-r--r--   0        0        0     5235 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/redge.py
+-rw-r--r--   0        0        0     9523 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/redgifs.py
+-rw-r--r--   0        0        0     6216 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/redtube.py
+-rw-r--r--   0        0        0     4105 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/rentv.py
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/restudy.py
+-rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/reuters.py
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/reverbnation.py
+-rw-r--r--   0        0        0     4653 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/rheinmaintv.py
+-rw-r--r--   0        0        0     4417 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ridehome.py
+-rw-r--r--   0        0        0     3192 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/rinsefm.py
+-rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/rmcdecouverte.py
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/rockstargames.py
+-rw-r--r--   0        0        0    21043 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/rokfin.py
+-rw-r--r--   0        0        0    15756 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/roosterteeth.py
+-rw-r--r--   0        0        0     3045 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/rottentomatoes.py
+-rw-r--r--   0        0        0    15123 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/rozhlas.py
+-rw-r--r--   0        0        0     6207 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/rte.py
+-rw-r--r--   0        0        0     3636 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/rtl2.py
+-rw-r--r--   0        0        0    12122 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/rtlnl.py
+-rw-r--r--   0        0        0     7645 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/rtnews.py
+-rw-r--r--   0        0        0     3371 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/rtp.py
+-rw-r--r--   0        0        0     2756 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/rtrfm.py
+-rw-r--r--   0        0        0     9529 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/rts.py
+-rw-r--r--   0        0        0    11224 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/rtvcplay.py
+-rw-r--r--   0        0        0    12881 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/rtve.py
+-rw-r--r--   0        0        0     3428 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/rtvs.py
+-rw-r--r--   0        0        0     7153 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/rtvslo.py
+-rw-r--r--   0        0        0     5205 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/rudovideo.py
+-rw-r--r--   0        0        0     5206 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/rule34video.py
+-rw-r--r--   0        0        0    15578 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/rumble.py
+-rw-r--r--   0        0        0    13882 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/rutube.py
+-rw-r--r--   0        0        0     8052 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/rutv.py
+-rw-r--r--   0        0        0    10968 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ruutu.py
+-rw-r--r--   0        0        0     6839 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ruv.py
+-rw-r--r--   0        0        0     4071 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/s4c.py
+-rw-r--r--   0        0        0     9807 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/safari.py
+-rw-r--r--   0        0        0     3011 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/saitosan.py
+-rw-r--r--   0        0        0     3817 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/samplefocus.py
+-rw-r--r--   0        0        0     4398 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/sapo.py
+-rw-r--r--   0        0        0     6548 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/sbs.py
+-rw-r--r--   0        0        0     8280 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/sbscokr.py
+-rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/screen9.py
+-rw-r--r--   0        0        0     4594 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/screencast.py
+-rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/screencastify.py
+-rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/screencastomatic.py
+-rw-r--r--   0        0        0     5975 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/scrippsnetworks.py
+-rw-r--r--   0        0        0     3744 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/scrolller.py
+-rw-r--r--   0        0        0     4866 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/scte.py
+-rw-r--r--   0        0        0     8609 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/sejmpl.py
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/senalcolombia.py
+-rw-r--r--   0        0        0     8688 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/senategov.py
+-rw-r--r--   0        0        0     3940 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/sendtonews.py
+-rw-r--r--   0        0        0     5410 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/servus.py
+-rw-r--r--   0        0        0     4955 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/sevenplus.py
+-rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/sexu.py
+-rw-r--r--   0        0        0     7623 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/seznamzpravy.py
+-rw-r--r--   0        0        0     8289 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/shahid.py
+-rw-r--r--   0        0        0     5505 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/sharepoint.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/sharevideos.py
+-rw-r--r--   0        0        0     4337 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/shemaroome.py
+-rw-r--r--   0        0        0     3016 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/showroomlive.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/sibnet.py
+-rw-r--r--   0        0        0     6045 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/simplecast.py
+-rw-r--r--   0        0        0     4213 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/sina.py
+-rw-r--r--   0        0        0     5054 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/sixplay.py
+-rw-r--r--   0        0        0     5580 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/skeb.py
+-rw-r--r--   0        0        0     5398 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/sky.py
+-rw-r--r--   0        0        0     9225 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/skyit.py
+-rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/skylinewebcams.py
+-rw-r--r--   0        0        0     5367 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/skynewsarabia.py
+-rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/skynewsau.py
+-rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/slideshare.py
+-rw-r--r--   0        0        0    21906 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/slideslive.py
+-rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/slutload.py
+-rw-r--r--   0        0        0     2685 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/smotrim.py
+-rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/snotr.py
+-rw-r--r--   0        0        0    11240 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/sohu.py
+-rw-r--r--   0        0        0    10281 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/sonyliv.py
+-rw-r--r--   0        0        0    37011 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/soundcloud.py
+-rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/soundgasm.py
+-rw-r--r--   0        0        0     7785 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/southpark.py
+-rw-r--r--   0        0        0     8210 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/sovietscloset.py
+-rw-r--r--   0        0        0     7193 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/spankbang.py
+-rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/spiegel.py
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/spike.py
+-rw-r--r--   0        0        0     3147 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/sport5.py
+-rw-r--r--   0        0        0     3233 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/sportbox.py
+-rw-r--r--   0        0        0     6295 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/sportdeutschland.py
+-rw-r--r--   0        0        0     6341 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/spotify.py
+-rw-r--r--   0        0        0     5973 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/spreaker.py
+-rw-r--r--   0        0        0     3987 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/springboardplatform.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/sprout.py
+-rw-r--r--   0        0        0     9937 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/srgssr.py
+-rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/srmediathek.py
+-rw-r--r--   0        0        0     8726 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/stacommu.py
+-rw-r--r--   0        0        0    10877 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/stageplus.py
+-rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/stanfordoc.py
+-rw-r--r--   0        0        0     3832 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/startrek.py
+-rw-r--r--   0        0        0     3530 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/startv.py
+-rw-r--r--   0        0        0     6502 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/steam.py
+-rw-r--r--   0        0        0     5330 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/stitcher.py
+-rw-r--r--   0        0        0     4718 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/storyfire.py
+-rw-r--r--   0        0        0     3917 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/streamable.py
+-rw-r--r--   0        0        0     5011 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/streamcz.py
+-rw-r--r--   0        0        0     3567 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/streetvoice.py
+-rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/stretchinternet.py
+-rw-r--r--   0        0        0     2545 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/stripchat.py
+-rw-r--r--   0        0        0     3329 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/stv.py
+-rw-r--r--   0        0        0     4625 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/substack.py
+-rw-r--r--   0        0        0     2528 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/sunporno.py
+-rw-r--r--   0        0        0     5495 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/sverigesradio.py
+-rw-r--r--   0        0        0    17835 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/svt.py
+-rw-r--r--   0        0        0     3399 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/swearnet.py
+-rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/syfy.py
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/syvdk.py
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/sztvhu.py
+-rw-r--r--   0        0        0     6194 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tagesschau.py
+-rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tass.py
+-rw-r--r--   0        0        0     3487 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tbs.py
+-rw-r--r--   0        0        0     7105 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tbsjp.py
+-rw-r--r--   0        0        0    10455 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/teachable.py
+-rw-r--r--   0        0        0     4361 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/teachertube.py
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/teachingchannel.py
+-rw-r--r--   0        0        0     9986 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/teamcoco.py
+-rw-r--r--   0        0        0     5374 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/teamtreehouse.py
+-rw-r--r--   0        0        0     9821 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ted.py
+-rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tele13.py
+-rw-r--r--   0        0        0     3301 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tele5.py
+-rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/telebruxelles.py
+-rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/telecaribe.py
+-rw-r--r--   0        0        0     6110 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/telecinco.py
+-rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/telegraaf.py
+-rw-r--r--   0        0        0     5085 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/telegram.py
+-rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/telemb.py
+-rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/telemundo.py
+-rw-r--r--   0        0        0     8988 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/telequebec.py
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/teletask.py
+-rw-r--r--   0        0        0     5429 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/telewebion.py
+-rw-r--r--   0        0        0     4888 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tempo.py
+-rw-r--r--   0        0        0    19941 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tencent.py
+-rw-r--r--   0        0        0     7260 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tennistv.py
+-rw-r--r--   0        0        0     6695 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tenplay.py
+-rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/testurl.py
+-rw-r--r--   0        0        0     3855 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tf1.py
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tfo.py
+-rw-r--r--   0        0        0     6132 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/theguardian.py
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/theholetv.py
+-rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/theintercept.py
+-rw-r--r--   0        0        0    18966 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/theplatform.py
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/thestar.py
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/thesun.py
+-rw-r--r--   0        0        0     4105 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/theweatherchannel.py
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/thisamericanlife.py
+-rw-r--r--   0        0        0     5955 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/thisoldhouse.py
+-rw-r--r--   0        0        0     8617 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/thisvid.py
+-rw-r--r--   0        0        0     6222 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/threeqsdn.py
+-rw-r--r--   0        0        0     4005 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/threespeak.py
+-rw-r--r--   0        0        0    60557 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tiktok.py
+-rw-r--r--   0        0        0     9690 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tmz.py
+-rw-r--r--   0        0        0    13595 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tnaflix.py
+-rw-r--r--   0        0        0     8812 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/toggle.py
+-rw-r--r--   0        0        0     3404 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/toggo.py
+-rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tonline.py
+-rw-r--r--   0        0        0     2972 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/toongoggles.py
+-rw-r--r--   0        0        0     3530 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/toutv.py
+-rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/toypics.py
+-rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/traileraddict.py
+-rw-r--r--   0        0        0    13594 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/triller.py
+-rw-r--r--   0        0        0    12901 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/trovo.py
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/trtcocuk.py
+-rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/trtworld.py
+-rw-r--r--   0        0        0     6358 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/trueid.py
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/trunews.py
+-rw-r--r--   0        0        0     2790 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/truth.py
+-rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/trutv.py
+-rw-r--r--   0        0        0     6293 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tube8.py
+-rw-r--r--   0        0        0    10672 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tubetugraz.py
+-rw-r--r--   0        0        0     6697 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tubitv.py
+-rw-r--r--   0        0        0    16426 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tumblr.py
+-rw-r--r--   0        0        0     9127 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tunein.py
+-rw-r--r--   0        0        0    11056 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/turner.py
+-rw-r--r--   0        0        0    13726 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tv2.py
+-rw-r--r--   0        0        0     3645 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tv24ua.py
+-rw-r--r--   0        0        0     6019 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tv2dk.py
+-rw-r--r--   0        0        0     3968 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tv2hu.py
+-rw-r--r--   0        0        0     5479 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tv4.py
+-rw-r--r--   0        0        0     7830 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tv5mondeplus.py
+-rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tv5unis.py
+-rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tva.py
+-rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tvanouvelles.py
+-rw-r--r--   0        0        0     3671 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tvc.py
+-rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tver.py
+-rw-r--r--   0        0        0     5043 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tvigle.py
+-rw-r--r--   0        0        0     3247 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tviplayer.py
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tvland.py
+-rw-r--r--   0        0        0     3830 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tvn24.py
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tvnoe.py
+-rw-r--r--   0        0        0     5209 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tvopengr.py
+-rw-r--r--   0        0        0    25539 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tvp.py
+-rw-r--r--   0        0        0    11849 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tvplay.py
+-rw-r--r--   0        0        0     2732 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tvplayer.py
+-rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tweakers.py
+-rw-r--r--   0        0        0     2638 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/twentymin.py
+-rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/twentythreevideo.py
+-rw-r--r--   0        0        0    12681 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/twitcasting.py
+-rw-r--r--   0        0        0    42809 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/twitch.py
+-rw-r--r--   0        0        0    81104 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/twitter.py
+-rw-r--r--   0        0        0    17683 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/txxx.py
+-rw-r--r--   0        0        0    19475 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/udemy.py
+-rw-r--r--   0        0        0     3578 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/udn.py
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ufctv.py
+-rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ukcolumn.py
+-rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/uktvplay.py
+-rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/umg.py
+-rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/unistra.py
+-rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/unity.py
+-rw-r--r--   0        0        0     7258 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/unsupported.py
+-rw-r--r--   0        0        0     5376 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/uol.py
+-rw-r--r--   0        0        0     3352 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/uplynk.py
+-rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/urort.py
+-rw-r--r--   0        0        0     6918 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/urplay.py
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/usanetwork.py
+-rw-r--r--   0        0        0     2646 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/usatoday.py
+-rw-r--r--   0        0        0    10545 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ustream.py
+-rw-r--r--   0        0        0     4260 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ustudio.py
+-rw-r--r--   0        0        0     3721 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/utreon.py
+-rw-r--r--   0        0        0     3045 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/varzesh3.py
+-rw-r--r--   0        0        0     3902 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/vbox7.py
+-rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/veo.py
+-rw-r--r--   0        0        0     6940 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/veoh.py
+-rw-r--r--   0        0        0     4343 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/vesti.py
+-rw-r--r--   0        0        0    13519 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/vevo.py
+-rw-r--r--   0        0        0    10860 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/vgtv.py
+-rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/vh1.py
+-rw-r--r--   0        0        0    11845 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/vice.py
+-rw-r--r--   0        0        0     4937 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/viddler.py
+-rw-r--r--   0        0        0     6529 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/videa.py
+-rw-r--r--   0        0        0    10740 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/videocampus_sachsen.py
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/videodetective.py
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/videofyme.py
+-rw-r--r--   0        0        0    13772 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/videoken.py
+-rw-r--r--   0        0        0    11324 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/videomore.py
+-rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/videopress.py
+-rw-r--r--   0        0        0    13750 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/vidio.py
+-rw-r--r--   0        0        0     5797 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/vidlii.py
+-rw-r--r--   0        0        0     3061 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/vidly.py
+-rw-r--r--   0        0        0    14946 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/viewlift.py
+-rw-r--r--   0        0        0     7377 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/viidea.py
+-rw-r--r--   0        0        0    13492 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/viki.py
+-rw-r--r--   0        0        0    62548 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/vimeo.py
+-rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/vimm.py
+-rw-r--r--   0        0        0     5402 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/vine.py
+-rw-r--r--   0        0        0     2572 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/viously.py
+-rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/viqeo.py
+-rw-r--r--   0        0        0    21227 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/viu.py
+-rw-r--r--   0        0        0    34047 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/vk.py
+-rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/vocaroo.py
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/vodpl.py
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/vodplatform.py
+-rw-r--r--   0        0        0     5405 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/voicy.py
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/volejtv.py
+-rw-r--r--   0        0        0     8993 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/voot.py
+-rw-r--r--   0        0        0     9519 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/voxmedia.py
+-rw-r--r--   0        0        0    21514 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/vrt.py
+-rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/vtm.py
+-rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/vuclip.py
+-rw-r--r--   0        0        0    12609 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/vvvvid.py
+-rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/walla.py
+-rw-r--r--   0        0        0     5816 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/washingtonpost.py
+-rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/wat.py
+-rw-r--r--   0        0        0    15111 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/wdr.py
+-rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/webcamerapl.py
+-rw-r--r--   0        0        0     3660 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/webcaster.py
+-rw-r--r--   0        0        0     5456 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/webofstories.py
+-rw-r--r--   0        0        0    10998 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/weibo.py
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/weiqitv.py
+-rw-r--r--   0        0        0    25606 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/weverse.py
+-rw-r--r--   0        0        0     4168 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/wevidi.py
+-rw-r--r--   0        0        0     3497 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/weyyak.py
+-rw-r--r--   0        0        0     3937 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/whowatch.py
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/whyp.py
+-rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/wikimedia.py
+-rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/wimbledon.py
+-rw-r--r--   0        0        0     5466 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/wimtv.py
+-rw-r--r--   0        0        0    15862 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/wistia.py
+-rw-r--r--   0        0        0     7198 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/wordpress.py
+-rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/worldstarhiphop.py
+-rw-r--r--   0        0        0     6113 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/wppilot.py
+-rw-r--r--   0        0        0    12727 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/wrestleuniverse.py
+-rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/wsj.py
+-rw-r--r--   0        0        0     4491 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/wwe.py
+-rw-r--r--   0        0        0    10763 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/wykop.py
+-rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/xanimu.py
+-rw-r--r--   0        0        0     2315 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/xboxclips.py
+-rw-r--r--   0        0        0     7408 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/xfileshare.py
+-rw-r--r--   0        0        0    19584 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/xhamster.py
+-rw-r--r--   0        0        0     6659 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ximalaya.py
+-rw-r--r--   0        0        0     4001 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/xinpianchang.py
+-rw-r--r--   0        0        0     2901 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/xminus.py
+-rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/xnxx.py
+-rw-r--r--   0        0        0     3881 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/xstream.py
+-rw-r--r--   0        0        0     7312 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/xvideos.py
+-rw-r--r--   0        0        0     2612 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/xxxymovies.py
+-rw-r--r--   0        0        0    17965 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/yahoo.py
+-rw-r--r--   0        0        0     5059 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/yandexdisk.py
+-rw-r--r--   0        0        0    17649 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/yandexmusic.py
+-rw-r--r--   0        0        0    17747 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/yandexvideo.py
+-rw-r--r--   0        0        0     2960 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/yapfiles.py
+-rw-r--r--   0        0        0     5647 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/yappy.py
+-rw-r--r--   0        0        0     6088 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/yle_areena.py
+-rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/youjizz.py
+-rw-r--r--   0        0        0    10927 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/youku.py
+-rw-r--r--   0        0        0     7061 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/younow.py
+-rw-r--r--   0        0        0     8467 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/youporn.py
+-rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/yourporn.py
+-rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/yourupload.py
+-rw-r--r--   0        0        0   348531 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/youtube.py
+-rw-r--r--   0        0        0     5982 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/zaiko.py
+-rw-r--r--   0        0        0     3832 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/zapiks.py
+-rw-r--r--   0        0        0    29425 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/zattoo.py
+-rw-r--r--   0        0        0    18597 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/zdf.py
+-rw-r--r--   0        0        0    12040 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/zee5.py
+-rw-r--r--   0        0        0     3216 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/zeenews.py
+-rw-r--r--   0        0        0     4803 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/zenporn.py
+-rw-r--r--   0        0        0     3916 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/zetland.py
+-rw-r--r--   0        0        0     2545 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/zhihu.py
+-rw-r--r--   0        0        0    23571 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/zingmp3.py
+-rw-r--r--   0        0        0     7091 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/zoom.py
+-rw-r--r--   0        0        0     5505 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/zype.py
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/networking/__init__.py
+-rw-r--r--   0        0        0     8776 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/networking/_curlcffi.py
+-rw-r--r--   0        0        0    10452 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/networking/_helper.py
+-rw-r--r--   0        0        0    15012 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/networking/_requests.py
+-rw-r--r--   0        0        0    15738 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/networking/_urllib.py
+-rw-r--r--   0        0        0     7266 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/networking/_websockets.py
+-rw-r--r--   0        0        0    21205 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/networking/common.py
+-rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/networking/exceptions.py
+-rw-r--r--   0        0        0     5533 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/networking/impersonate.py
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/networking/websocket.py
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/postprocessor/__init__.py
+-rw-r--r--   0        0        0     8359 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/postprocessor/common.py
+-rw-r--r--   0        0        0    10469 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/postprocessor/embedthumbnail.py
+-rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/postprocessor/exec.py
+-rw-r--r--   0        0        0    49509 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/postprocessor/ffmpeg.py
+-rw-r--r--   0        0        0     4381 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/postprocessor/metadataparser.py
+-rw-r--r--   0        0        0    17821 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/postprocessor/modify_chapters.py
+-rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/postprocessor/movefilesafterdownload.py
+-rw-r--r--   0        0        0     4088 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/postprocessor/sponskrub.py
+-rw-r--r--   0        0        0     4249 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/postprocessor/sponsorblock.py
+-rw-r--r--   0        0        0     2481 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/postprocessor/xattrpp.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/utils/__init__.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/utils/_deprecated.py
+-rw-r--r--   0        0        0     9992 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/utils/_legacy.py
+-rw-r--r--   0        0        0   183337 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/utils/_utils.py
+-rw-r--r--   0        0        0     5404 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/utils/networking.py
+-rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/utils/progress.py
+-rw-r--r--   0        0        0    12620 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/yt_dlp/utils/traversal.py
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/.gitignore
+-rw-r--r--   0        0        0    17261 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/AUTHORS
+-rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/LICENSE
+-rw-r--r--   0        0        0   161803 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/README.md
+-rw-r--r--   0        0        0     3540 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/pyproject.toml
+-rw-r--r--   0        0        0   165928 2020-02-02 00:00:00.000000 yt_dlp-2024.4.7.232657.dev0/PKG-INFO
```

### Comparing `yt_dlp-2024.4.6.232655.dev0/Changelog.md` & `yt_dlp-2024.4.7.232657.dev0/Changelog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # Changelog
 
 <!--
 # To create a release, dispatch the https://github.com/yt-dlp/yt-dlp/actions/workflows/release.yml workflow on master
 -->
 
-### 2024.04.06.232655
+### 2024.04.07.232657
 
 #### Core changes
 - [Add new options `--impersonate` and `--list-impersonate-targets`](https://github.com/yt-dlp/yt-dlp/commit/0b81d4d252bd065ccd352722987ea34fe17f9244) by [bashonly](https://github.com/bashonly), [coletdjnz](https://github.com/coletdjnz), [Grub4K](https://github.com/Grub4K), [pukkandan](https://github.com/pukkandan)
 - [Add option `--no-break-on-existing`](https://github.com/yt-dlp/yt-dlp/commit/16be117729150b2784f3b17755c886cb0cf73374) ([#9610](https://github.com/yt-dlp/yt-dlp/issues/9610)) by [bashonly](https://github.com/bashonly)
 - [Fix `filesize_approx` calculation](https://github.com/yt-dlp/yt-dlp/commit/86e3b82261e8ebc6c6707c09544c9dfb8907c0fd) ([#9560](https://github.com/yt-dlp/yt-dlp/issues/9560)) by [pukkandan](https://github.com/pukkandan), [seproDev](https://github.com/seproDev)
 - [Infer `acodec` for single-codec containers](https://github.com/yt-dlp/yt-dlp/commit/86a972033e05fea80e5fe7f2aff6723dbe2f3952) by [pukkandan](https://github.com/pukkandan)
+- **cookies**: [Add `--cookies-from-browser` support for Firefox Flatpak](https://github.com/yt-dlp/yt-dlp/commit/2ab2651a4a7be18939e2b4cb21be79fe477c797a) ([#9619](https://github.com/yt-dlp/yt-dlp/issues/9619)) by [un-def](https://github.com/un-def)
 - **utils**
     - `traverse_obj`
         - [Allow unbranching using `all` and `any`](https://github.com/yt-dlp/yt-dlp/commit/3699eeb67cad333272b14a42dd3843d93fda1a2e) ([#9571](https://github.com/yt-dlp/yt-dlp/issues/9571)) by [Grub4K](https://github.com/Grub4K)
         - [Convenience improvements](https://github.com/yt-dlp/yt-dlp/commit/32abfb00bdbd119ca675fdc6d1719331f0a2741a) ([#9577](https://github.com/yt-dlp/yt-dlp/issues/9577)) by [Grub4K](https://github.com/Grub4K)
 
 #### Extractor changes
 - [Add extractor impersonate API](https://github.com/yt-dlp/yt-dlp/commit/50c29352312f5662acf9a64b0012766f5c40af61) ([#9474](https://github.com/yt-dlp/yt-dlp/issues/9474)) by [bashonly](https://github.com/bashonly), [Grub4K](https://github.com/Grub4K), [pukkandan](https://github.com/pukkandan)
@@ -31,32 +32,36 @@
 - **dropbox**: [Fix formats extraction](https://github.com/yt-dlp/yt-dlp/commit/a48cc86d6f6b20427553620c2ddb990ede6a4b41) ([#9627](https://github.com/yt-dlp/yt-dlp/issues/9627)) by [bashonly](https://github.com/bashonly)
 - **fathom**: [Add extractor](https://github.com/yt-dlp/yt-dlp/commit/bc2b8c0596fd6b75af24822c4f0f1da6783d71f7) ([#9495](https://github.com/yt-dlp/yt-dlp/issues/9495)) by [src-tinkerer](https://github.com/src-tinkerer)
 - **gofile**: [Fix extractor](https://github.com/yt-dlp/yt-dlp/commit/0da66980d3193cad3dae0120cddddbfcabddf7a1) ([#9446](https://github.com/yt-dlp/yt-dlp/issues/9446)) by [jazz1611](https://github.com/jazz1611)
 - **imgur**: [Fix extraction](https://github.com/yt-dlp/yt-dlp/commit/86d2f4d24849af0d1f3af7c0e2ac43bf8a058f74) ([#9471](https://github.com/yt-dlp/yt-dlp/issues/9471)) by [trwstin](https://github.com/trwstin)
 - **jiosaavn**
     - [Extract artists](https://github.com/yt-dlp/yt-dlp/commit/0ae16ceb1846cc4e609b70ce7c5d8e7458efceb2) ([#9612](https://github.com/yt-dlp/yt-dlp/issues/9612)) by [bashonly](https://github.com/bashonly)
     - [Fix format extensions](https://github.com/yt-dlp/yt-dlp/commit/443e206ec41e64ca2aef61d8ef91640fb69b3113) ([#9609](https://github.com/yt-dlp/yt-dlp/issues/9609)) by [bashonly](https://github.com/bashonly)
+    - [Support playlists](https://github.com/yt-dlp/yt-dlp/commit/2e94602f241f6e41bdc48576c61089435529339b) ([#9622](https://github.com/yt-dlp/yt-dlp/issues/9622)) by [bashonly](https://github.com/bashonly)
 - **joqrag**: [Fix live status detection](https://github.com/yt-dlp/yt-dlp/commit/f2fd449b46c4058222e1744f7a35caa20b2d003d) ([#9624](https://github.com/yt-dlp/yt-dlp/issues/9624)) by [pzhlkj6612](https://github.com/pzhlkj6612)
 - **kick**: [Support browser impersonation](https://github.com/yt-dlp/yt-dlp/commit/c8a61a910096c77ce08dad5e1b2fbda5eb964156) ([#9611](https://github.com/yt-dlp/yt-dlp/issues/9611)) by [bashonly](https://github.com/bashonly)
 - **loom**: [Add extractors](https://github.com/yt-dlp/yt-dlp/commit/f859ed3ba1e8b129ae6a467592c65687e73fbca1) ([#8686](https://github.com/yt-dlp/yt-dlp/issues/8686)) by [bashonly](https://github.com/bashonly), [hruzgar](https://github.com/hruzgar)
 - **medici**: [Fix extractor](https://github.com/yt-dlp/yt-dlp/commit/4cd9e251b9abada107b10830de997bf4d79ca369) ([#9518](https://github.com/yt-dlp/yt-dlp/issues/9518)) by [Offert4324](https://github.com/Offert4324)
 - **mixch**
     - [Fix extractor](https://github.com/yt-dlp/yt-dlp/commit/4c3b7a0769706f7f0ea24adf1f219d5ae82d2b07) ([#9608](https://github.com/yt-dlp/yt-dlp/issues/9608)) by [bashonly](https://github.com/bashonly), [nipotan](https://github.com/nipotan)
     - archive: [Fix extractor](https://github.com/yt-dlp/yt-dlp/commit/c59de48e2bb4c681b03b93b584a05f52609ce4a0) ([#8761](https://github.com/yt-dlp/yt-dlp/issues/8761)) by [pzhlkj6612](https://github.com/pzhlkj6612)
+- **nhk**: [Fix NHK World extractors](https://github.com/yt-dlp/yt-dlp/commit/4af9d5c2f6aa81403ae2a8a5ae3cc824730f0b86) ([#9623](https://github.com/yt-dlp/yt-dlp/issues/9623)) by [bashonly](https://github.com/bashonly)
+- **patreon**: [Do not extract dead embed URLs](https://github.com/yt-dlp/yt-dlp/commit/36b240f9a72af57eb2c9d927ebb7fd1c917ebf18) ([#9613](https://github.com/yt-dlp/yt-dlp/issues/9613)) by [johnvictorfs](https://github.com/johnvictorfs)
 - **radio1be**: [Add extractor](https://github.com/yt-dlp/yt-dlp/commit/36baaa10e06715ccba06b78885b2042c4844c826) ([#9122](https://github.com/yt-dlp/yt-dlp/issues/9122)) by [HobbyistDev](https://github.com/HobbyistDev)
 - **sharepoint**: [Add extractor](https://github.com/yt-dlp/yt-dlp/commit/ff349ff94aae0b2b148bd3670f7c91d39c2f1d8e) ([#6531](https://github.com/yt-dlp/yt-dlp/issues/6531)) by [bashonly](https://github.com/bashonly), [C0D3D3V](https://github.com/C0D3D3V)
 - **sonylivseries**: [Fix season extraction](https://github.com/yt-dlp/yt-dlp/commit/f2868b26e917354203f82a370ad2396646edb813) ([#9423](https://github.com/yt-dlp/yt-dlp/issues/9423)) by [bashonly](https://github.com/bashonly)
 - **soundcloud**
     - [Adjust format sorting](https://github.com/yt-dlp/yt-dlp/commit/a2d0840739cddd585d24e0ce4796394fc8a4fa2e) ([#9584](https://github.com/yt-dlp/yt-dlp/issues/9584)) by [bashonly](https://github.com/bashonly)
     - [Support cookies](https://github.com/yt-dlp/yt-dlp/commit/97362712a1f2b04e735bdf54f749ad99165a62fe) ([#9586](https://github.com/yt-dlp/yt-dlp/issues/9586)) by [bashonly](https://github.com/bashonly)
     - [Support retries for API rate-limit](https://github.com/yt-dlp/yt-dlp/commit/246571ae1d867df8bf31a056bdf3bbbfd398366a) ([#9585](https://github.com/yt-dlp/yt-dlp/issues/9585)) by [bashonly](https://github.com/bashonly)
 - **thisoldhouse**: [Support Brightcove embeds](https://github.com/yt-dlp/yt-dlp/commit/0df63cce69026d2f4c0cbb4dd36163e83eac93dc) ([#9576](https://github.com/yt-dlp/yt-dlp/issues/9576)) by [bashonly](https://github.com/bashonly)
 - **tiktok**
     - [Fix API extraction](https://github.com/yt-dlp/yt-dlp/commit/cb61e20c266facabb7a30f9ce53bd79dfc158475) ([#9548](https://github.com/yt-dlp/yt-dlp/issues/9548)) by [bashonly](https://github.com/bashonly), [Grub4K](https://github.com/Grub4K)
     - [Prefer non-bytevc2 formats](https://github.com/yt-dlp/yt-dlp/commit/63f685f341f35f6f02b0368d1ba53bdb5b520410) ([#9575](https://github.com/yt-dlp/yt-dlp/issues/9575)) by [bashonly](https://github.com/bashonly)
+    - [Restore `carrier_region` API parameter](https://github.com/yt-dlp/yt-dlp/commit/fc53ec13ff1ee926a3e533a68cfca8acc887b661) ([#9637](https://github.com/yt-dlp/yt-dlp/issues/9637)) by [bashonly](https://github.com/bashonly)
     - [Update API hostname](https://github.com/yt-dlp/yt-dlp/commit/8c05b3ebae23c5b444857549a85b84004c01a536) ([#9444](https://github.com/yt-dlp/yt-dlp/issues/9444)) by [bashonly](https://github.com/bashonly)
 - **twitch**: [Extract AV1 and HEVC formats](https://github.com/yt-dlp/yt-dlp/commit/02f93ff51b3ff9436d60c4993562b366eaae8851) ([#9158](https://github.com/yt-dlp/yt-dlp/issues/9158)) by [kasper93](https://github.com/kasper93)
 - **vkplay**: [Fix `_VALID_URL`](https://github.com/yt-dlp/yt-dlp/commit/b15b0c1d2106437ec61a5c436c543e8760eac160) ([#9636](https://github.com/yt-dlp/yt-dlp/issues/9636)) by [bashonly](https://github.com/bashonly)
 - **xvideos**: [Support new URL format (#9493)](https://github.com/yt-dlp/yt-dlp/commit/aa7e9ae4f48276bd5d0173966c77db9484f65a0a) ([#9502](https://github.com/yt-dlp/yt-dlp/issues/9502)) by [sta1us](https://github.com/sta1us)
 - **youtube**
     - [Calculate more accurate `filesize`](https://github.com/yt-dlp/yt-dlp/commit/a25a424323267e3f6f9f63c0b62df499bd7b8d46) by [pukkandan](https://github.com/pukkandan)
     - [Update `android` params](https://github.com/yt-dlp/yt-dlp/commit/e7b17fce14775bd2448695c8eb7379b8d31d3537) by [pukkandan](https://github.com/pukkandan)
```

### Comparing `yt_dlp-2024.4.6.232655.dev0/README.txt` & `yt_dlp-2024.4.7.232657.dev0/README.txt`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/setup.cfg` & `yt_dlp-2024.4.7.232657.dev0/setup.cfg`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/supportedsites.md` & `yt_dlp-2024.4.7.232657.dev0/supportedsites.md`

 * *Files 1% similar despite different names*

```diff
@@ -632,16 +632,17 @@
  - **Ixigua**
  - **Izlesene**
  - **Jable**
  - **JablePlaylist**
  - **Jamendo**
  - **JamendoAlbum**
  - **JeuxVideo**: (**Currently broken**)
- - **JioSaavnAlbum**
- - **JioSaavnSong**
+ - **jiosaavn:album**
+ - **jiosaavn:playlist**
+ - **jiosaavn:song**
  - **Joj**
  - **JoqrAg**: 超!A&G+ 文化放送 (f.k.a. AGQR) Nippon Cultural Broadcasting, Inc. (JOQR)
  - **Jove**
  - **JStream**
  - **JTBC**: jtbc.co.kr
  - **JTBC:program**
  - **JWPlatform**
```

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt-dlp.1` & `yt_dlp-2024.4.7.232657.dev0/yt-dlp.1`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/completions/bash/yt-dlp` & `yt_dlp-2024.4.7.232657.dev0/completions/bash/yt-dlp`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/completions/fish/yt-dlp.fish` & `yt_dlp-2024.4.7.232657.dev0/completions/fish/yt-dlp.fish`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/completions/zsh/_yt-dlp` & `yt_dlp-2024.4.7.232657.dev0/completions/zsh/_yt-dlp`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/devscripts/bash-completion.in` & `yt_dlp-2024.4.7.232657.dev0/devscripts/bash-completion.in`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/devscripts/bash-completion.py` & `yt_dlp-2024.4.7.232657.dev0/devscripts/bash-completion.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/devscripts/changelog_override.json` & `yt_dlp-2024.4.7.232657.dev0/devscripts/changelog_override.json`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/devscripts/changelog_override.schema.json` & `yt_dlp-2024.4.7.232657.dev0/devscripts/changelog_override.schema.json`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/devscripts/check-porn.py` & `yt_dlp-2024.4.7.232657.dev0/devscripts/check-porn.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/devscripts/cli_to_api.py` & `yt_dlp-2024.4.7.232657.dev0/devscripts/cli_to_api.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/devscripts/fish-completion.py` & `yt_dlp-2024.4.7.232657.dev0/devscripts/fish-completion.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/devscripts/generate_aes_testdata.py` & `yt_dlp-2024.4.7.232657.dev0/devscripts/generate_aes_testdata.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/devscripts/install_deps.py` & `yt_dlp-2024.4.7.232657.dev0/devscripts/install_deps.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/devscripts/lazy_load_template.py` & `yt_dlp-2024.4.7.232657.dev0/devscripts/lazy_load_template.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/devscripts/logo.ico` & `yt_dlp-2024.4.7.232657.dev0/devscripts/logo.ico`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/devscripts/make_changelog.py` & `yt_dlp-2024.4.7.232657.dev0/devscripts/make_changelog.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/devscripts/make_contributing.py` & `yt_dlp-2024.4.7.232657.dev0/devscripts/make_contributing.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/devscripts/make_issue_template.py` & `yt_dlp-2024.4.7.232657.dev0/devscripts/make_issue_template.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/devscripts/make_lazy_extractors.py` & `yt_dlp-2024.4.7.232657.dev0/devscripts/make_lazy_extractors.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/devscripts/make_readme.py` & `yt_dlp-2024.4.7.232657.dev0/devscripts/make_readme.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/devscripts/prepare_manpage.py` & `yt_dlp-2024.4.7.232657.dev0/devscripts/prepare_manpage.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/devscripts/run_tests.py` & `yt_dlp-2024.4.7.232657.dev0/devscripts/run_tests.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/devscripts/set-variant.py` & `yt_dlp-2024.4.7.232657.dev0/devscripts/set-variant.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/devscripts/tomlparse.py` & `yt_dlp-2024.4.7.232657.dev0/devscripts/tomlparse.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/devscripts/update-version.py` & `yt_dlp-2024.4.7.232657.dev0/devscripts/update-version.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/devscripts/update_changelog.py` & `yt_dlp-2024.4.7.232657.dev0/devscripts/update_changelog.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/devscripts/utils.py` & `yt_dlp-2024.4.7.232657.dev0/devscripts/utils.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/devscripts/zsh-completion.in` & `yt_dlp-2024.4.7.232657.dev0/devscripts/zsh-completion.in`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/devscripts/zsh-completion.py` & `yt_dlp-2024.4.7.232657.dev0/devscripts/zsh-completion.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/test/conftest.py` & `yt_dlp-2024.4.7.232657.dev0/test/conftest.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/test/helper.py` & `yt_dlp-2024.4.7.232657.dev0/test/helper.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/test/parameters.json` & `yt_dlp-2024.4.7.232657.dev0/test/parameters.json`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/test/test_InfoExtractor.py` & `yt_dlp-2024.4.7.232657.dev0/test/test_InfoExtractor.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/test/test_YoutubeDL.py` & `yt_dlp-2024.4.7.232657.dev0/test/test_YoutubeDL.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/test/test_YoutubeDLCookieJar.py` & `yt_dlp-2024.4.7.232657.dev0/test/test_YoutubeDLCookieJar.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/test/test_aes.py` & `yt_dlp-2024.4.7.232657.dev0/test/test_aes.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/test/test_age_restriction.py` & `yt_dlp-2024.4.7.232657.dev0/test/test_age_restriction.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/test/test_all_urls.py` & `yt_dlp-2024.4.7.232657.dev0/test/test_all_urls.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/test/test_cache.py` & `yt_dlp-2024.4.7.232657.dev0/test/test_cache.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/test/test_compat.py` & `yt_dlp-2024.4.7.232657.dev0/test/test_compat.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/test/test_config.py` & `yt_dlp-2024.4.7.232657.dev0/test/test_config.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/test/test_cookies.py` & `yt_dlp-2024.4.7.232657.dev0/test/test_cookies.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/test/test_download.py` & `yt_dlp-2024.4.7.232657.dev0/test/test_download.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/test/test_downloader_external.py` & `yt_dlp-2024.4.7.232657.dev0/test/test_downloader_external.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/test/test_downloader_http.py` & `yt_dlp-2024.4.7.232657.dev0/test/test_downloader_http.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/test/test_execution.py` & `yt_dlp-2024.4.7.232657.dev0/test/test_execution.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/test/test_iqiyi_sdk_interpreter.py` & `yt_dlp-2024.4.7.232657.dev0/test/test_iqiyi_sdk_interpreter.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/test/test_jsinterp.py` & `yt_dlp-2024.4.7.232657.dev0/test/test_jsinterp.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/test/test_netrc.py` & `yt_dlp-2024.4.7.232657.dev0/test/test_netrc.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/test/test_networking.py` & `yt_dlp-2024.4.7.232657.dev0/test/test_networking.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/test/test_networking_utils.py` & `yt_dlp-2024.4.7.232657.dev0/test/test_networking_utils.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/test/test_overwrites.py` & `yt_dlp-2024.4.7.232657.dev0/test/test_overwrites.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/test/test_plugins.py` & `yt_dlp-2024.4.7.232657.dev0/test/test_plugins.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/test/test_post_hooks.py` & `yt_dlp-2024.4.7.232657.dev0/test/test_post_hooks.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/test/test_postprocessors.py` & `yt_dlp-2024.4.7.232657.dev0/test/test_postprocessors.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/test/test_socks.py` & `yt_dlp-2024.4.7.232657.dev0/test/test_socks.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/test/test_subtitles.py` & `yt_dlp-2024.4.7.232657.dev0/test/test_subtitles.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/test/test_traversal.py` & `yt_dlp-2024.4.7.232657.dev0/test/test_traversal.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/test/test_update.py` & `yt_dlp-2024.4.7.232657.dev0/test/test_update.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/test/test_utils.py` & `yt_dlp-2024.4.7.232657.dev0/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/test/test_verbose_output.py` & `yt_dlp-2024.4.7.232657.dev0/test/test_verbose_output.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/test/test_websockets.py` & `yt_dlp-2024.4.7.232657.dev0/test/test_websockets.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/test/test_write_annotations.py.disabled` & `yt_dlp-2024.4.7.232657.dev0/test/test_write_annotations.py.disabled`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/test/test_youtube_lists.py` & `yt_dlp-2024.4.7.232657.dev0/test/test_youtube_lists.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/test/test_youtube_misc.py` & `yt_dlp-2024.4.7.232657.dev0/test/test_youtube_misc.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/test/test_youtube_signature.py` & `yt_dlp-2024.4.7.232657.dev0/test/test_youtube_signature.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/test/testcert.pem` & `yt_dlp-2024.4.7.232657.dev0/test/testcert.pem`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/test/testdata/certificate/ca.crt` & `yt_dlp-2024.4.7.232657.dev0/test/testdata/certificate/ca.crt`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/test/testdata/certificate/clientwithencryptedkey.crt` & `yt_dlp-2024.4.7.232657.dev0/test/testdata/certificate/clientwithencryptedkey.crt`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/test/testdata/certificate/clientwithkey.crt` & `yt_dlp-2024.4.7.232657.dev0/test/testdata/certificate/clientwithkey.crt`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/test/testdata/certificate/instructions.md` & `yt_dlp-2024.4.7.232657.dev0/test/testdata/certificate/instructions.md`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/test/testdata/f4m/custom_base_url.f4m` & `yt_dlp-2024.4.7.232657.dev0/test/testdata/f4m/custom_base_url.f4m`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/test/testdata/ism/ec-3_test.Manifest` & `yt_dlp-2024.4.7.232657.dev0/test/testdata/ism/ec-3_test.Manifest`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/test/testdata/ism/sintel.Manifest` & `yt_dlp-2024.4.7.232657.dev0/test/testdata/ism/sintel.Manifest`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/test/testdata/m3u8/bipbop_16x9.m3u8` & `yt_dlp-2024.4.7.232657.dev0/test/testdata/m3u8/bipbop_16x9.m3u8`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/test/testdata/m3u8/img_bipbop_adv_example_fmp4.m3u8` & `yt_dlp-2024.4.7.232657.dev0/test/testdata/m3u8/img_bipbop_adv_example_fmp4.m3u8`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/test/testdata/mpd/float_duration.mpd` & `yt_dlp-2024.4.7.232657.dev0/test/testdata/mpd/float_duration.mpd`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/test/testdata/mpd/subtitles.mpd` & `yt_dlp-2024.4.7.232657.dev0/test/testdata/mpd/subtitles.mpd`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/test/testdata/mpd/unfragmented.mpd` & `yt_dlp-2024.4.7.232657.dev0/test/testdata/mpd/unfragmented.mpd`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/test/testdata/mpd/urls_only.mpd` & `yt_dlp-2024.4.7.232657.dev0/test/testdata/mpd/urls_only.mpd`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/test/testdata/thumbnails/foo %d bar/foo_%d.webp` & `yt_dlp-2024.4.7.232657.dev0/test/testdata/thumbnails/foo %d bar/foo_%d.webp`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/test/testdata/xspf/foo_xspf.xspf` & `yt_dlp-2024.4.7.232657.dev0/test/testdata/xspf/foo_xspf.xspf`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/YoutubeDL.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/YoutubeDL.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/__init__.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/__init__.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/aes.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/aes.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/cache.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/cache.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/cookies.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/cookies.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,15 +190,19 @@
     if sys.platform in ('cygwin', 'win32'):
         yield os.path.expandvars(R'%APPDATA%\Mozilla\Firefox\Profiles')
 
     elif sys.platform == 'darwin':
         yield os.path.expanduser('~/Library/Application Support/Firefox/Profiles')
 
     else:
-        yield from map(os.path.expanduser, ('~/.mozilla/firefox', '~/snap/firefox/common/.mozilla/firefox'))
+        yield from map(os.path.expanduser, (
+            '~/.mozilla/firefox',
+            '~/snap/firefox/common/.mozilla/firefox',
+            '~/.var/app/org.mozilla.firefox/.mozilla/firefox',
+        ))
 
 
 def _firefox_cookie_dbs(roots):
     for root in map(os.path.abspath, roots):
         for pattern in ('', '*/', 'Profiles/*/'):
             yield from glob.iglob(os.path.join(root, pattern, 'cookies.sqlite'))
```

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/jsinterp.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/jsinterp.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/minicurses.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/minicurses.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/options.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/options.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/plugins.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/plugins.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/socks.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/socks.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/update.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/update.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/webvtt.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/webvtt.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/__pyinstaller/hook-yt_dlp.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/__pyinstaller/hook-yt_dlp.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/compat/__init__.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/compat/_deprecated.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/compat/_deprecated.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/compat/_legacy.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/compat/_legacy.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/compat/compat_utils.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/compat/compat_utils.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/compat/imghdr.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/compat/imghdr.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/compat/shutil.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/compat/shutil.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/compat/urllib/request.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/compat/urllib/request.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/dependencies/Cryptodome.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/dependencies/Cryptodome.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/dependencies/__init__.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/dependencies/__init__.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/downloader/__init__.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/downloader/__init__.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/downloader/common.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/downloader/common.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/downloader/dash.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/downloader/dash.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/downloader/external.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/downloader/external.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/downloader/f4m.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/downloader/f4m.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/downloader/fc2.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/downloader/fc2.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/downloader/fragment.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/downloader/fragment.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/downloader/hls.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/downloader/hls.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/downloader/http.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/downloader/http.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/downloader/ism.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/downloader/ism.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/downloader/mhtml.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/downloader/mhtml.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/downloader/niconico.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/downloader/niconico.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/downloader/rtmp.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/downloader/rtmp.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/downloader/rtsp.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/downloader/rtsp.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/downloader/websocket.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/downloader/websocket.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/downloader/youtube_live_chat.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/downloader/youtube_live_chat.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/__init__.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/__init__.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/_extractors.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/_extractors.py`

 * *Files 0% similar despite different names*

```diff
@@ -872,14 +872,15 @@
     SangiinInstructionIE,
     SangiinIE,
 )
 from .jeuxvideo import JeuxVideoIE
 from .jiosaavn import (
     JioSaavnSongIE,
     JioSaavnAlbumIE,
+    JioSaavnPlaylistIE,
 )
 from .jove import JoveIE
 from .joj import JojIE
 from .joqrag import JoqrAgIE
 from .jstream import JStreamIE
 from .jtbc import (
     JTBCIE,
```

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/abc.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/abc.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/abcnews.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/abcnews.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/abcotvs.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/abcotvs.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/abematv.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/abematv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/academicearth.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/academicearth.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/acast.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/acast.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/acfun.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/acfun.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/adn.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/adn.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/adobeconnect.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/adobeconnect.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/adobepass.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/adobepass.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/adobetv.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/adobetv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/adultswim.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/adultswim.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/aenetworks.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/aenetworks.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/aeonco.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/aeonco.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/afreecatv.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/afreecatv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/agora.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/agora.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/airtv.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/airtv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/aitube.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/aitube.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/aliexpress.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/aliexpress.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/aljazeera.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/aljazeera.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/allocine.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/allocine.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/allstar.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/allstar.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/alphaporno.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/alphaporno.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/alsace20tv.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/alsace20tv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/altcensored.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/altcensored.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/alura.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/alura.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/amadeustv.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/amadeustv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/amara.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/amara.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/amazon.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/amazon.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/amazonminitv.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/amazonminitv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/amcnetworks.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/amcnetworks.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/americastestkitchen.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/americastestkitchen.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/amp.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/amp.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/anchorfm.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/anchorfm.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/angel.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/angel.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/antenna.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/antenna.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/anvato.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/anvato.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/aol.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/aol.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/apa.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/apa.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/aparat.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/aparat.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/appleconnect.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/appleconnect.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/applepodcasts.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/applepodcasts.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/appletrailers.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/appletrailers.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/archiveorg.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/archiveorg.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/arcpublishing.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/arcpublishing.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ard.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ard.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/arkena.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/arkena.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/arnes.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/arnes.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/art19.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/art19.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/arte.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/arte.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/asobichannel.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/asobichannel.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/asobistage.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/asobistage.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/atresplayer.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/atresplayer.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/atscaleconf.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/atscaleconf.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/atvat.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/atvat.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/audimedia.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/audimedia.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/audioboom.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/audioboom.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/audiodraft.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/audiodraft.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/audiomack.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/audiomack.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/audius.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/audius.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/awaan.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/awaan.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/aws.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/aws.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/axs.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/axs.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/azmedien.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/azmedien.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/baidu.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/baidu.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/banbye.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/banbye.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/bandaichannel.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/bandaichannel.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/bandcamp.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/bandcamp.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/bannedvideo.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/bannedvideo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/bbc.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/bbc.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/beatbump.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/beatbump.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/beatport.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/beatport.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/beeg.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/beeg.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/behindkink.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/behindkink.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/bellmedia.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/bellmedia.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/berufetv.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/berufetv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/bet.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/bet.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/bfi.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/bfi.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/bfmtv.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/bfmtv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/bibeltv.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/bibeltv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/bigflix.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/bigflix.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/bigo.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/bigo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/bild.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/bild.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/bilibili.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/bilibili.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/biobiochiletv.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/biobiochiletv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/bitchute.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/bitchute.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/blackboardcollaborate.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/blackboardcollaborate.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/bleacherreport.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/bleacherreport.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/blerp.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/blerp.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/blogger.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/blogger.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/bloomberg.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/bloomberg.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/bokecc.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/bokecc.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/bongacams.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/bongacams.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/boosty.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/boosty.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/bostonglobe.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/bostonglobe.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/box.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/box.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/boxcast.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/boxcast.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/bpb.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/bpb.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/br.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/br.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/brainpop.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/brainpop.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/bravotv.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/bravotv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/breitbart.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/breitbart.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/brightcove.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/brightcove.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/brilliantpala.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/brilliantpala.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/bundesliga.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/bundesliga.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/bundestag.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/bundestag.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/businessinsider.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/businessinsider.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/buzzfeed.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/buzzfeed.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/byutv.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/byutv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/c56.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/c56.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/cableav.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/cableav.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/callin.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/callin.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/caltrans.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/caltrans.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/cam4.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/cam4.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/camdemy.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/camdemy.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/camfm.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/camfm.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/cammodels.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/cammodels.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/camsoda.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/camsoda.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/camtasia.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/camtasia.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/canal1.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/canal1.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/canalalpha.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/canalalpha.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/canalc2.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/canalc2.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/canalplus.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/canalplus.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/caracoltv.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/caracoltv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/cartoonnetwork.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/cartoonnetwork.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/cbc.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/cbc.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/cbs.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/cbs.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/cbsnews.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/cbsnews.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/cbssports.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/cbssports.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ccc.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ccc.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ccma.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ccma.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/cctv.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/cctv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/cda.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/cda.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/cellebrite.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/cellebrite.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ceskatelevize.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ceskatelevize.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/cgtn.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/cgtn.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/charlierose.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/charlierose.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/chaturbate.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/chaturbate.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/chilloutzone.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/chilloutzone.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/chzzk.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/chzzk.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/cinemax.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/cinemax.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/cinetecamilano.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/cinetecamilano.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/cineverse.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/cineverse.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ciscolive.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ciscolive.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ciscowebex.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ciscowebex.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/cjsw.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/cjsw.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/clipchamp.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/clipchamp.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/clippit.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/clippit.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/cliprs.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/cliprs.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/closertotruth.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/closertotruth.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/cloudflarestream.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/cloudflarestream.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/cloudycdn.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/cloudycdn.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/clubic.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/clubic.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/clyp.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/clyp.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/cmt.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/cmt.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/cnbc.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/cnbc.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/cnn.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/cnn.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/comedycentral.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/comedycentral.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/common.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/common.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/commonmistakes.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/commonmistakes.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/commonprotocols.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/commonprotocols.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/condenast.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/condenast.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/contv.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/contv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/corus.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/corus.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/coub.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/coub.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/cozytv.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/cozytv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/cpac.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/cpac.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/cracked.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/cracked.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/crackle.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/crackle.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/craftsy.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/craftsy.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/crooksandliars.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/crooksandliars.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/crowdbunker.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/crowdbunker.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/crtvg.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/crtvg.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/crunchyroll.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/crunchyroll.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/cspan.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/cspan.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ctsnews.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ctsnews.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ctv.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ctv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ctvnews.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ctvnews.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/cultureunplugged.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/cultureunplugged.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/curiositystream.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/curiositystream.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/cwtv.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/cwtv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/cybrary.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/cybrary.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/dacast.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/dacast.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/dailymail.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/dailymail.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/dailymotion.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/dailymotion.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/dailywire.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/dailywire.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/damtomo.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/damtomo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/daum.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/daum.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/daystar.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/daystar.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/dbtv.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/dbtv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/dctp.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/dctp.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/deezer.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/deezer.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/democracynow.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/democracynow.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/detik.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/detik.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/deuxm.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/deuxm.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/dfb.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/dfb.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/dhm.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/dhm.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/digitalconcerthall.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/digitalconcerthall.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/digiteka.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/digiteka.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/discogs.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/discogs.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/discovery.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/discovery.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/discoverygo.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/discoverygo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/disney.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/disney.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/dispeak.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/dispeak.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/dlf.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/dlf.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/dlive.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/dlive.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/douyutv.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/douyutv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/dplay.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/dplay.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/drbonanza.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/drbonanza.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/dreisat.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/dreisat.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/drooble.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/drooble.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/dropbox.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/dropbox.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/dropout.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/dropout.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/drtuber.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/drtuber.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/drtv.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/drtv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/dtube.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/dtube.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/duboku.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/duboku.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/dumpert.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/dumpert.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/duoplay.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/duoplay.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/dvtv.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/dvtv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/dw.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/dw.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/eagleplatform.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/eagleplatform.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ebaumsworld.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ebaumsworld.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ebay.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ebay.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/egghead.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/egghead.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/eighttracks.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/eighttracks.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/einthusan.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/einthusan.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/eitb.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/eitb.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/elementorembed.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/elementorembed.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/elonet.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/elonet.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/elpais.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/elpais.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/eltrecetv.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/eltrecetv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/embedly.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/embedly.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/epicon.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/epicon.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/epidemicsound.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/epidemicsound.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/eplus.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/eplus.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/epoch.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/epoch.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/eporner.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/eporner.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/erocast.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/erocast.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/eroprofile.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/eroprofile.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/err.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/err.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ertgr.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ertgr.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/espn.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/espn.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ettutv.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ettutv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/europa.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/europa.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/europeantour.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/europeantour.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/eurosport.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/eurosport.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/euscreen.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/euscreen.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/expressen.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/expressen.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/extractors.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/extractors.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/eyedotv.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/eyedotv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/facebook.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/facebook.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/fancode.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/fancode.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/fathom.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/fathom.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/faz.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/faz.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/fc2.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/fc2.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/fczenit.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/fczenit.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/fifa.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/fifa.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/filmon.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/filmon.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/filmweb.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/filmweb.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/firsttv.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/firsttv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/fivetv.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/fivetv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/flextv.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/flextv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/flickr.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/flickr.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/floatplane.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/floatplane.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/folketinget.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/folketinget.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/footyroom.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/footyroom.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/formula1.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/formula1.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/fourtube.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/fourtube.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/fox.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/fox.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/fox9.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/fox9.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/foxnews.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/foxnews.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/foxsports.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/foxsports.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/fptplay.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/fptplay.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/franceinter.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/franceinter.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/francetv.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/francetv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/freesound.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/freesound.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/freespeech.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/freespeech.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/freetv.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/freetv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/frontendmasters.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/frontendmasters.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/fujitv.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/fujitv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/funimation.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/funimation.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/funk.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/funk.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/funker530.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/funker530.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/fuyintv.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/fuyintv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/gab.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/gab.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/gaia.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/gaia.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/gamejolt.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/gamejolt.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/gamespot.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/gamespot.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/gamestar.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/gamestar.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/gaskrank.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/gaskrank.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/gazeta.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/gazeta.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/gdcvault.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/gdcvault.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/gedidigital.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/gedidigital.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/generic.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/generic.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/genericembeds.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/genericembeds.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/genius.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/genius.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/getcourseru.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/getcourseru.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/gettr.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/gettr.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/giantbomb.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/giantbomb.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/gigya.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/gigya.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/glide.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/glide.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/globalplayer.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/globalplayer.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/globo.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/globo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/glomex.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/glomex.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/gmanetwork.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/gmanetwork.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/go.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/go.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/godtube.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/godtube.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/gofile.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/gofile.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/golem.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/golem.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/goodgame.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/goodgame.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/googledrive.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/googledrive.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/googlepodcasts.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/googlepodcasts.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/googlesearch.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/googlesearch.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/goplay.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/goplay.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/gopro.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/gopro.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/goshgay.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/goshgay.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/gotostage.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/gotostage.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/gputechconf.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/gputechconf.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/gronkh.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/gronkh.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/groupon.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/groupon.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/harpodeon.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/harpodeon.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/hbo.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/hbo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/hearthisat.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/hearthisat.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/heise.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/heise.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/hellporno.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/hellporno.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/hgtv.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/hgtv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/hidive.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/hidive.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/historicfilms.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/historicfilms.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/hitrecord.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/hitrecord.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/hketv.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/hketv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/hollywoodreporter.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/hollywoodreporter.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/holodex.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/holodex.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/hotnewhiphop.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/hotnewhiphop.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/hotstar.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/hotstar.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/hrefli.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/hrefli.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/hrfensehen.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/hrfensehen.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/hrti.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/hrti.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/hse.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/hse.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/huajiao.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/huajiao.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/huffpost.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/huffpost.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/hungama.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/hungama.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/huya.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/huya.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/hypem.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/hypem.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/hypergryph.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/hypergryph.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/hytale.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/hytale.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/icareus.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/icareus.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ichinanalive.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ichinanalive.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/idolplus.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/idolplus.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ign.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ign.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/iheart.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/iheart.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ilpost.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ilpost.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/iltalehti.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/iltalehti.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/imdb.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/imdb.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/imggaming.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/imggaming.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/imgur.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/imgur.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ina.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ina.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/inc.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/inc.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/indavideo.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/indavideo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/infoq.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/infoq.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/instagram.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/instagram.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/internazionale.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/internazionale.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/internetvideoarchive.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/internetvideoarchive.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/iprima.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/iprima.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/iqiyi.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/iqiyi.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/islamchannel.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/islamchannel.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/israelnationalnews.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/israelnationalnews.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/itprotv.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/itprotv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/itv.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/itv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ivi.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ivi.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ivideon.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ivideon.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/iwara.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/iwara.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ixigua.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ixigua.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/izlesene.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/izlesene.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/jable.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/jable.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/jamendo.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/jamendo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/japandiet.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/japandiet.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/jeuxvideo.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/jeuxvideo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/jiosaavn.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/wwe.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,109 +1,138 @@
+import re
+
 from .common import InfoExtractor
+from ..compat import compat_str
 from ..utils import (
-    int_or_none,
-    js_to_json,
-    orderedSet,
+    try_get,
+    unescapeHTML,
     url_or_none,
-    urlencode_postdata,
     urljoin,
 )
-from ..utils.traversal import traverse_obj
 
 
-class JioSaavnBaseIE(InfoExtractor):
-    def _extract_initial_data(self, url, audio_id):
-        webpage = self._download_webpage(url, audio_id)
-        return self._search_json(
-            r'window\.__INITIAL_DATA__\s*=', webpage,
-            'init json', audio_id, transform_source=js_to_json)
+class WWEBaseIE(InfoExtractor):
+    _SUBTITLE_LANGS = {
+        'English': 'en',
+        'Deutsch': 'de',
+    }
+
+    def _extract_entry(self, data, url, video_id=None):
+        video_id = compat_str(video_id or data['nid'])
+        title = data['title']
+
+        formats = self._extract_m3u8_formats(
+            data['file'], video_id, 'mp4', entry_protocol='m3u8_native',
+            m3u8_id='hls')
+
+        description = data.get('description')
+        thumbnail = urljoin(url, data.get('image'))
+        series = data.get('show_name')
+        episode = data.get('episode_name')
+
+        subtitles = {}
+        tracks = data.get('tracks')
+        if isinstance(tracks, list):
+            for track in tracks:
+                if not isinstance(track, dict):
+                    continue
+                if track.get('kind') != 'captions':
+                    continue
+                track_file = url_or_none(track.get('file'))
+                if not track_file:
+                    continue
+                label = track.get('label')
+                lang = self._SUBTITLE_LANGS.get(label, label) or 'en'
+                subtitles.setdefault(lang, []).append({
+                    'url': track_file,
+                })
+
+        return {
+            'id': video_id,
+            'title': title,
+            'description': description,
+            'thumbnail': thumbnail,
+            'series': series,
+            'episode': episode,
+            'formats': formats,
+            'subtitles': subtitles,
+        }
 
 
-class JioSaavnSongIE(JioSaavnBaseIE):
-    _VALID_URL = r'https?://(?:www\.)?(?:jiosaavn\.com/song/[^/?#]+/|saavn\.com/s/song/(?:[^/?#]+/){3})(?P<id>[^/?#]+)'
+class WWEIE(WWEBaseIE):
+    _VALID_URL = r'https?://(?:[^/]+\.)?wwe\.com/(?:[^/]+/)*videos/(?P<id>[^/?#&]+)'
     _TESTS = [{
-        'url': 'https://www.jiosaavn.com/song/leja-re/OQsEfQFVUXk',
-        'md5': '3b84396d15ed9e083c3106f1fa589c04',
+        'url': 'https://www.wwe.com/videos/daniel-bryan-vs-andrade-cien-almas-smackdown-live-sept-4-2018',
+        'md5': '92811c6a14bfc206f7a6a9c5d9140184',
         'info_dict': {
-            'id': 'OQsEfQFVUXk',
-            'ext': 'm4a',
-            'title': 'Leja Re',
-            'album': 'Leja Re',
-            'thumbnail': 'https://c.saavncdn.com/258/Leja-Re-Hindi-2018-20181124024539-500x500.jpg',
-            'duration': 205,
-            'view_count': int,
-            'release_year': 2018,
-            'artists': ['Sandesh Shandilya', 'Dhvani Bhanushali', 'Tanishk Bagchi', 'Rashmi Virag', 'Irshad Kamil'],
-        },
+            'id': '40048199',
+            'ext': 'mp4',
+            'title': 'Daniel Bryan vs. Andrade "Cien" Almas: SmackDown LIVE, Sept. 4, 2018',
+            'description': 'md5:2d7424dbc6755c61a0e649d2a8677f67',
+            'thumbnail': r're:^https?://.*\.jpg$',
+        }
     }, {
-        'url': 'https://www.saavn.com/s/song/hindi/Saathiya/O-Humdum-Suniyo-Re/KAMiazoCblU',
+        'url': 'https://de.wwe.com/videos/gran-metalik-vs-tony-nese-wwe-205-live-sept-4-2018',
         'only_matching': True,
     }]
 
-    _VALID_BITRATES = ('16', '32', '64', '128', '320')
-
     def _real_extract(self, url):
-        audio_id = self._match_id(url)
-        extract_bitrates = self._configuration_arg('bitrate', ['128', '320'], ie_key='JioSaavn')
-        if invalid_bitrates := [br for br in extract_bitrates if br not in self._VALID_BITRATES]:
-            raise ValueError(
-                f'Invalid bitrate(s): {", ".join(invalid_bitrates)}. '
-                + f'Valid bitrates are: {", ".join(self._VALID_BITRATES)}')
-
-        song_data = self._extract_initial_data(url, audio_id)['song']['song']
-        formats = []
-        for bitrate in extract_bitrates:
-            media_data = self._download_json(
-                'https://www.jiosaavn.com/api.php', audio_id, f'Downloading format info for {bitrate}',
-                fatal=False, data=urlencode_postdata({
-                    '__call': 'song.generateAuthToken',
-                    '_format': 'json',
-                    'bitrate': bitrate,
-                    'url': song_data['encrypted_media_url'],
-                }))
-            if not media_data.get('auth_url'):
-                self.report_warning(f'Unable to extract format info for {bitrate}')
-                continue
-            ext = media_data.get('type')
-            formats.append({
-                'url': media_data['auth_url'],
-                'ext': 'm4a' if ext == 'mp4' else ext,
-                'format_id': bitrate,
-                'abr': int(bitrate),
-                'vcodec': 'none',
-            })
+        display_id = self._match_id(url)
+        webpage = self._download_webpage(url, display_id)
 
-        return {
-            'id': audio_id,
-            'formats': formats,
-            **traverse_obj(song_data, {
-                'title': ('title', 'text'),
-                'album': ('album', 'text'),
-                'thumbnail': ('image', 0, {url_or_none}),
-                'duration': ('duration', {int_or_none}),
-                'view_count': ('play_count', {int_or_none}),
-                'release_year': ('year', {int_or_none}),
-                'artists': ('artists', ..., 'name', {str}, all, {orderedSet}),
-            }),
-        }
+        landing = self._parse_json(
+            self._html_search_regex(
+                r'(?s)Drupal\.settings\s*,\s*({.+?})\s*\)\s*;',
+                webpage, 'drupal settings'),
+            display_id)['WWEVideoLanding']
 
+        data = landing['initialVideo']['playlist'][0]
+        video_id = landing.get('initialVideoId')
 
-class JioSaavnAlbumIE(JioSaavnBaseIE):
-    _VALID_URL = r'https?://(?:www\.)?(?:jio)?saavn\.com/album/[^/?#]+/(?P<id>[^/?#]+)'
+        info = self._extract_entry(data, url, video_id)
+        info['display_id'] = display_id
+        return info
+
+
+class WWEPlaylistIE(WWEBaseIE):
+    _VALID_URL = r'https?://(?:[^/]+\.)?wwe\.com/(?:[^/]+/)*(?P<id>[^/?#&]+)'
     _TESTS = [{
-        'url': 'https://www.jiosaavn.com/album/96/buIOjYZDrNA_',
+        'url': 'https://www.wwe.com/shows/raw/2018-11-12',
         'info_dict': {
-            'id': 'buIOjYZDrNA_',
-            'title': '96',
+            'id': '2018-11-12',
         },
-        'playlist_count': 10,
+        'playlist_mincount': 11,
+    }, {
+        'url': 'http://www.wwe.com/article/walk-the-prank-wwe-edition',
+        'only_matching': True,
+    }, {
+        'url': 'https://www.wwe.com/shows/wwenxt/article/matt-riddle-interview',
+        'only_matching': True,
     }]
 
+    @classmethod
+    def suitable(cls, url):
+        return False if WWEIE.suitable(url) else super(WWEPlaylistIE, cls).suitable(url)
+
     def _real_extract(self, url):
-        album_id = self._match_id(url)
-        album_view = self._extract_initial_data(url, album_id)['albumView']
+        display_id = self._match_id(url)
+        webpage = self._download_webpage(url, display_id)
+
+        entries = []
+        for mobj in re.finditer(
+                r'data-video\s*=\s*(["\'])(?P<data>{.+?})\1', webpage):
+            video = self._parse_json(
+                mobj.group('data'), display_id, transform_source=unescapeHTML,
+                fatal=False)
+            if not video:
+                continue
+            data = try_get(video, lambda x: x['playlist'][0], dict)
+            if not data:
+                continue
+            try:
+                entry = self._extract_entry(data, url)
+            except Exception:
+                continue
+            entry['extractor_key'] = WWEIE.ie_key()
+            entries.append(entry)
 
-        return self.playlist_from_matches(
-            traverse_obj(album_view, (
-                'modules', lambda _, x: x['key'] == 'list', 'data', ..., 'title', 'action', {str})),
-            album_id, traverse_obj(album_view, ('album', 'title', 'text', {str})), ie=JioSaavnSongIE,
-            getter=lambda x: urljoin('https://www.jiosaavn.com/', x))
+        return self.playlist_result(entries, display_id)
```

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/jixie.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/jixie.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/joj.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/joj.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/joqrag.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/joqrag.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/jove.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/jove.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/jstream.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/jstream.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/jtbc.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/jtbc.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/jwplatform.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/jwplatform.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/kakao.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/kakao.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/kaltura.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/kaltura.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/kankanews.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/kankanews.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/karaoketv.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/karaoketv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/kelbyone.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/kelbyone.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/khanacademy.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/khanacademy.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/kick.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/kick.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/kicker.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/kicker.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/kickstarter.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/kickstarter.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/kinja.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/kinja.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/kinopoisk.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/kinopoisk.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/kommunetv.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/kommunetv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/kompas.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/kompas.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/koo.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/koo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/krasview.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/krasview.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/kth.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/kth.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ku6.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ku6.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/kukululive.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/kukululive.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/kuwo.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/kuwo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/la7.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/la7.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/lastfm.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/lastfm.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/laxarxames.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/laxarxames.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/lazy_extractors.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/lazy_extractors.py`

 * *Files 0% similar despite different names*

```diff
@@ -5316,26 +5316,33 @@
 class JioSaavnBaseIE(LazyLoadExtractor):
     _module = 'yt_dlp.extractor.jiosaavn'
     IE_NAME = 'JioSaavnBase'
 
 
 class JioSaavnSongIE(JioSaavnBaseIE):
     _module = 'yt_dlp.extractor.jiosaavn'
-    IE_NAME = 'JioSaavnSong'
+    IE_NAME = 'jiosaavn:song'
     _VALID_URL = 'https?://(?:www\\.)?(?:jiosaavn\\.com/song/[^/?#]+/|saavn\\.com/s/song/(?:[^/?#]+/){3})(?P<id>[^/?#]+)'
     _RETURN_TYPE = 'video'
 
 
 class JioSaavnAlbumIE(JioSaavnBaseIE):
     _module = 'yt_dlp.extractor.jiosaavn'
-    IE_NAME = 'JioSaavnAlbum'
+    IE_NAME = 'jiosaavn:album'
     _VALID_URL = 'https?://(?:www\\.)?(?:jio)?saavn\\.com/album/[^/?#]+/(?P<id>[^/?#]+)'
     _RETURN_TYPE = 'playlist'
 
 
+class JioSaavnPlaylistIE(JioSaavnBaseIE):
+    _module = 'yt_dlp.extractor.jiosaavn'
+    IE_NAME = 'jiosaavn:playlist'
+    _VALID_URL = 'https?://(?:www\\.)?(?:jio)?saavn\\.com/s/playlist/(?:[^/?#]+/){2}(?P<id>[^/?#]+)'
+    _RETURN_TYPE = 'playlist'
+
+
 class JoveIE(LazyLoadExtractor):
     _module = 'yt_dlp.extractor.jove'
     IE_NAME = 'Jove'
     _VALID_URL = 'https?://(?:www\\.)?jove\\.com/video/(?P<id>[0-9]+)'
     _RETURN_TYPE = 'video'
 
 
@@ -7467,24 +7474,28 @@
     _module = 'yt_dlp.extractor.nhk'
     IE_NAME = 'NhkBase'
 
 
 class NhkVodIE(NhkBaseIE):
     _module = 'yt_dlp.extractor.nhk'
     IE_NAME = 'NhkVod'
-    _VALID_URL = ['https?://www3\\.nhk\\.or\\.jp/nhkworld/(?P<lang>[a-z]{2})/ondemand/(?P<type>video)/(?P<id>[0-9a-z]+)', 'https?://www3\\.nhk\\.or\\.jp/nhkworld/(?P<lang>[a-z]{2})/ondemand/(?P<type>audio)/(?P<id>[^/?#]+?-\\d{8}-[0-9a-z]+)']
+    _VALID_URL = ['https?://www3\\.nhk\\.or\\.jp/nhkworld/(?P<lang>[a-z]{2})/shows/(?:(?P<type>video)/)?(?P<id>\\d{4}[\\da-z]\\d+)/?(?:$|[?#])', 'https?://www3\\.nhk\\.or\\.jp/nhkworld/(?P<lang>[a-z]{2})/(?:ondemand|shows)/(?P<type>audio)/(?P<id>[^/?#]+?-\\d{8}-[\\da-z]+)', 'https?://www3\\.nhk\\.or\\.jp/nhkworld/(?P<lang>[a-z]{2})/ondemand/(?P<type>video)/(?P<id>\\d{4}[\\da-z]\\d+)']
     _RETURN_TYPE = 'video'
 
 
 class NhkVodProgramIE(NhkBaseIE):
     _module = 'yt_dlp.extractor.nhk'
     IE_NAME = 'NhkVodProgram'
-    _VALID_URL = 'https?://www3\\.nhk\\.or\\.jp/nhkworld/(?P<lang>[a-z]{2})/ondemand/program/(?P<type>video|audio)/(?P<id>\\w+)(?:.+?\\btype=(?P<episode_type>clip|(?:radio|tv)Episode))?'
+    _VALID_URL = '(?x)\n        https?://www3\\.nhk\\.or\\.jp/nhkworld/(?P<lang>[a-z]{2})/(?:shows|tv)/\n        (?:(?P<type>audio)/programs/)?(?P<id>\\w+)/?\n        (?:\\?(?:[^#]+&)?type=(?P<episode_type>clip|(?:radio|tv)Episode))?'
     _RETURN_TYPE = 'playlist'
 
+    @classmethod
+    def suitable(cls, url):
+        return False if NhkVodIE.suitable(url) else super().suitable(url)
+
 
 class NhkForSchoolBangumiIE(LazyLoadExtractor):
     _module = 'yt_dlp.extractor.nhk'
     IE_NAME = 'NhkForSchoolBangumi'
     _VALID_URL = 'https?://www2\\.nhk\\.or\\.jp/school/movie/(?P<type>bangumi|clip)\\.cgi\\?das_id=(?P<id>[a-zA-Z0-9_-]+)'
     _RETURN_TYPE = 'video'
 
@@ -15418,8 +15429,8 @@
     _VALID_URL = '.*'
     IE_DESC = 'Generic downloader that works on some sites'
     _NETRC_MACHINE = False
     age_limit = 18
     _RETURN_TYPE = 'any'
 
 
-_ALL_CLASSES = [YoutubeIE, YoutubeClipIE, YoutubeFavouritesIE, YoutubeNotificationsIE, YoutubeHistoryIE, YoutubeTabIE, YoutubeLivestreamEmbedIE, YoutubePlaylistIE, YoutubeRecommendedIE, YoutubeSearchDateIE, YoutubeSearchIE, YoutubeSearchURLIE, YoutubeMusicSearchURLIE, YoutubeSubscriptionsIE, YoutubeTruncatedIDIE, YoutubeTruncatedURLIE, YoutubeYtBeIE, YoutubeYtUserIE, YoutubeWatchLaterIE, YoutubeShortsAudioPivotIE, YoutubeConsentRedirectIE, ABCIE, ABCIViewIE, ABCIViewShowSeriesIE, AbcNewsIE, AbcNewsVideoIE, ABCOTVSIE, ABCOTVSClipsIE, AbemaTVIE, AbemaTVTitleIE, AcademicEarthCourseIE, ACastIE, ACastChannelIE, AcFunVideoIE, AcFunBangumiIE, ADNIE, ADNSeasonIE, AdobeConnectIE, AdobeTVEmbedIE, AdobeTVIE, AdobeTVShowIE, AdobeTVChannelIE, AdobeTVVideoIE, AdultSwimIE, AeonCoIE, AfreecaTVIE, AfreecaTVLiveIE, AfreecaTVUserIE, TokFMAuditionIE, TokFMPodcastIE, WyborczaPodcastIE, WyborczaVideoIE, AirTVIE, AitubeKZVideoIE, AlJazeeraIE, AllstarIE, AllstarProfileIE, AlphaPornoIE, AltCensoredIE, AltCensoredChannelIE, AluraIE, AluraCourseIE, AmadeusTVIE, AmaraIE, AmazonStoreIE, AmazonReviewsIE, AmazonMiniTVIE, AmazonMiniTVSeasonIE, AmazonMiniTVSeriesIE, AmericasTestKitchenIE, AmericasTestKitchenSeasonIE, AnchorFMEpisodeIE, AngelIE, AnvatoIE, AllocineIE, AliExpressLiveIE, Alsace20TVIE, Alsace20TVEmbedIE, APAIE, AparatIE, AppleConnectIE, AppleTrailersIE, AppleTrailersSectionIE, ApplePodcastsIE, ArchiveOrgIE, YoutubeWebArchiveIE, ArcPublishingIE, ArkenaIE, ARDBetaMediathekIE, ARDMediathekCollectionIE, ARDIE, Art19IE, Art19ShowIE, ArteTVIE, ArteTVEmbedIE, ArteTVPlaylistIE, ArteTVCategoryIE, ArnesIE, AsobiChannelIE, AsobiChannelTagURLIE, AsobiStageIE, AtresPlayerIE, AtScaleConfEventIE, ATVAtIE, AudiMediaIE, AudioBoomIE, AudiodraftCustomIE, AudiodraftGenericIE, AudiomackIE, AudiomackAlbumIE, AudiusIE, AudiusTrackIE, AudiusPlaylistIE, AudiusProfileIE, AWAANIE, AWAANVideoIE, AWAANLiveIE, AWAANSeasonIE, AxsIE, AZMedienIE, BaiduVideoIE, BanByeIE, BanByeChannelIE, BandaiChannelIE, BandcampIE, BandcampAlbumIE, BandcampWeeklyIE, BandcampUserIE, BannedVideoIE, BBCCoUkIE, BBCCoUkArticleIE, BBCCoUkIPlayerEpisodesIE, BBCCoUkIPlayerGroupIE, BBCCoUkPlaylistIE, BBCIE, BeegIE, BehindKinkIE, BellMediaIE, BeatBumpVideoIE, BeatBumpPlaylistIE, BeatportIE, BerufeTVIE, BetIE, BFIPlayerIE, BFMTVIE, BFMTVLiveIE, BFMTVArticleIE, BibelTVLiveIE, BibelTVSeriesIE, BibelTVVideoIE, BigflixIE, BigoIE, BildIE, BiliBiliIE, BiliBiliBangumiIE, BiliBiliBangumiSeasonIE, BiliBiliBangumiMediaIE, BilibiliCheeseIE, BilibiliCheeseSeasonIE, BiliBiliSearchIE, BilibiliCategoryIE, BilibiliAudioIE, BilibiliAudioAlbumIE, BiliBiliPlayerIE, BilibiliSpaceVideoIE, BilibiliSpaceAudioIE, BilibiliCollectionListIE, BilibiliSeriesListIE, BilibiliFavoritesListIE, BilibiliWatchlaterIE, BilibiliPlaylistIE, BiliIntlIE, BiliIntlSeriesIE, BiliLiveIE, BioBioChileTVIE, BitChuteIE, BitChuteChannelIE, BlackboardCollaborateIE, BleacherReportIE, BleacherReportCMSIE, BlerpIE, BloggerIE, BloombergIE, BokeCCIE, BongaCamsIE, BoostyIE, BostonGlobeIE, BoxIE, BoxCastVideoIE, BpbIE, BRIE, BravoTVIE, BrainPOPIE, BrainPOPJrIE, BrainPOPELLIE, BrainPOPEspIE, BrainPOPFrIE, BrainPOPIlIE, BreitBartIE, BrightcoveLegacyIE, BrightcoveNewIE, BrilliantpalaElearnIE, BrilliantpalaClassesIE, BusinessInsiderIE, BundesligaIE, BundestagIE, BuzzFeedIE, BYUtvIE, C56IE, CableAVIE, CallinIE, CaltransIE, CAM4IE, CamdemyIE, CamdemyFolderIE, CamFMEpisodeIE, CamFMShowIE, CamModelsIE, CamsodaIE, CamtasiaEmbedIE, Canal1IE, CanalAlphaIE, CanalplusIE, Canalc2IE, CaracolTvPlayIE, CartoonNetworkIE, CBCIE, CBCPlayerIE, CBCPlayerPlaylistIE, CBCGemIE, CBCGemPlaylistIE, CBCGemLiveIE, ParamountPressExpressIE, CBSNewsEmbedIE, CBSNewsIE, CBSLocalIE, CBSLocalArticleIE, CBSLocalLiveIE, CBSNewsLiveIE, CBSNewsLiveVideoIE, CBSSportsEmbedIE, CBSSportsIE, TwentyFourSevenSportsIE, CCCIE, CCCPlaylistIE, CCMAIE, CCTVIE, CDAIE, CellebriteIE, CeskaTelevizeIE, CGTNIE, CharlieRoseIE, ChaturbateIE, ChilloutzoneIE, CHZZKLiveIE, CHZZKVideoIE, CinemaxIE, CinetecaMilanoIE, CineverseIE, CineverseDetailsIE, CiscoLiveSessionIE, CiscoLiveSearchIE, CiscoWebexIE, CJSWIE, ClipchampIE, ClippitIE, ClipRsIE, CloserToTruthIE, CloudflareStreamIE, CloudyCDNIE, ClubicIE, ClypIE, CNBCVideoIE, CNNIE, CNNBlogsIE, CNNArticleIE, CNNIndonesiaIE, CoubIE, ComedyCentralIE, ComedyCentralTVIE, CommonMistakesIE, UnicodeBOMIE, MmsIE, RtmpIE, ViewSourceIE, CondeNastIE, CONtvIE, CPACIE, CPACPlaylistIE, CozyTVIE, CrackedIE, CrackleIE, CraftsyIE, CrooksAndLiarsIE, CrowdBunkerIE, CrowdBunkerChannelIE, CrtvgIE, CrunchyrollBetaIE, CrunchyrollBetaShowIE, CrunchyrollMusicIE, CrunchyrollArtistIE, CSpanIE, CSpanCongressIE, CtsNewsIE, CTVIE, CTVNewsIE, CultureUnpluggedIE, CuriosityStreamIE, CuriosityStreamCollectionsIE, CuriosityStreamSeriesIE, CWTVIE, CybraryIE, CybraryCourseIE, DacastVODIE, DacastPlaylistIE, DailyMailIE, DailymotionIE, DailymotionPlaylistIE, DailymotionSearchIE, DailymotionUserIE, DailyWireIE, DailyWirePodcastIE, DamtomoRecordIE, DamtomoVideoIE, DaumIE, DaumClipIE, DaumPlaylistIE, DaumUserIE, DaystarClipIE, DBTVIE, DctpTvIE, DeezerPlaylistIE, DeezerAlbumIE, DemocracynowIE, DetikEmbedIE, DLFIE, DLFCorpusIE, DFBIE, DHMIE, DouyuShowIE, DouyuTVIE, DPlayIE, DiscoveryPlusIE, HGTVDeIE, GoDiscoveryIE, TravelChannelIE, CookingChannelIE, HGTVUsaIE, FoodNetworkIE, InvestigationDiscoveryIE, DestinationAmericaIE, AmHistoryChannelIE, ScienceChannelIE, DIYNetworkIE, DiscoveryLifeIE, AnimalPlanetIE, TLCIE, MotorTrendIE, MotorTrendOnDemandIE, DiscoveryPlusIndiaIE, DiscoveryNetworksDeIE, DiscoveryPlusItalyIE, DiscoveryPlusItalyShowIE, DiscoveryPlusIndiaShowIE, GlobalCyclingNetworkPlusIE, DRBonanzaIE, DrTuberIE, DRTVIE, DRTVLiveIE, DRTVSeasonIE, DRTVSeriesIE, DTubeIE, DVTVIE, DubokuIE, DubokuPlaylistIE, DumpertIE, DeuxMIE, DeuxMNewsIE, DigitalConcertHallIE, DiscogsReleasePlaylistIE, DiscoveryIE, DisneyIE, DigitallySpeakingIE, DropboxIE, DropoutSeasonIE, DropoutIE, DuoplayIE, DWIE, DWArticleIE, EaglePlatformIE, ClipYouEmbedIE, EbaumsWorldIE, EbayIE, EggheadCourseIE, EggheadLessonIE, EightTracksIE, EinthusanIE, EitbIE, ElementorEmbedIE, ElonetIE, ElPaisIE, ElTreceTVIE, EmbedlyIE, EpiconIE, EpiconSeriesIE, EpidemicSoundIE, EplusIbIE, EpochIE, EpornerIE, ErocastIE, EroProfileIE, EroProfileAlbumIE, ERRJupiterIE, ERTFlixCodenameIE, ERTFlixIE, ERTWebtvEmbedIE, ESPNIE, WatchESPNIE, ESPNArticleIE, FiveThirtyEightIE, ESPNCricInfoIE, EttuTvIE, EuropaIE, EuroParlWebstreamIE, EuropeanTourIE, EurosportIE, EUScreenIE, ExpressenIE, EyedoTVIE, FacebookIE, FacebookPluginsVideoIE, FacebookRedirectURLIE, FacebookReelIE, FacebookAdsIE, FathomIE, FancodeVodIE, FancodeLiveIE, FazIE, FC2IE, FC2EmbedIE, FC2LiveIE, FczenitIE, FifaIE, FilmOnIE, FilmOnChannelIE, FilmwebIE, FirstTVIE, FiveTVIE, FlexTVIE, FlickrIE, FloatplaneIE, FloatplaneChannelIE, FolketingetIE, FootyRoomIE, Formula1IE, FourTubeIE, PornTubeIE, PornerBrosIE, FuxIE, FOXIE, FOX9IE, FOX9NewsIE, FoxNewsIE, FoxNewsArticleIE, FoxNewsVideoIE, FoxSportsIE, FptplayIE, FranceInterIE, FranceTVIE, FranceTVSiteIE, FranceTVInfoIE, FreesoundIE, FreespeechIE, FrontendMastersIE, FrontendMastersLessonIE, FrontendMastersCourseIE, FreeTvIE, FreeTvMoviesIE, FujiTVFODPlus7IE, FunimationIE, FunimationPageIE, FunimationShowIE, FunkIE, Funker530IE, FuyinTVIE, GabTVIE, GabIE, GaiaIE, GameJoltIE, GameJoltUserIE, GameJoltGameIE, GameJoltGameSoundtrackIE, GameJoltCommunityIE, GameJoltSearchIE, GameSpotIE, GameStarIE, GaskrankIE, GazetaIE, GDCVaultIE, GediDigitalIE, GeniusIE, GeniusLyricsIE, GetCourseRuPlayerIE, GetCourseRuIE, GettrIE, GettrStreamingIE, GiantBombIE, GlideIE, GlobalPlayerLiveIE, GlobalPlayerLivePlaylistIE, GlobalPlayerAudioIE, GlobalPlayerAudioEpisodeIE, GlobalPlayerVideoIE, GloboIE, GloboArticleIE, GMANetworkVideoIE, GoIE, GodTubeIE, GofileIE, GolemIE, GoodGameIE, GoogleDriveIE, GoogleDriveFolderIE, GooglePodcastsIE, GooglePodcastsFeedIE, GoogleSearchIE, GoProIE, GoPlayIE, GoshgayIE, GoToStageIE, GPUTechConfIE, GronkhIE, GronkhFeedIE, GronkhVodsIE, GrouponIE, HarpodeonIE, HBOIE, HearThisAtIE, HeiseIE, HellPornoIE, HGTVComShowIE, HKETVIE, HiDiveIE, HistoricFilmsIE, HitRecordIE, HollywoodReporterIE, HollywoodReporterPlaylistIE, HolodexIE, HotNewHipHopIE, HotStarIE, HotStarPrefixIE, HotStarPlaylistIE, HotStarSeasonIE, HotStarSeriesIE, HrefLiRedirectIE, HRFernsehenIE, HRTiIE, HRTiPlaylistIE, HSEShowIE, HSEProductIE, HTML5MediaEmbedIE, QuotedHTMLIE, HuajiaoIE, HuyaLiveIE, HuffPostIE, HungamaIE, HungamaSongIE, HungamaAlbumPlaylistIE, HypemIE, MonsterSirenHypergryphMusicIE, HytaleIE, IcareusIE, IchinanaLiveIE, IchinanaLiveClipIE, IdolPlusIE, IGNIE, IGNVideoIE, IGNArticleIE, IHeartRadioIE, IHeartRadioPodcastIE, IlPostIE, IltalehtiIE, ImdbIE, ImdbListIE, ImgurIE, ImgurAlbumIE, ImgurGalleryIE, InaIE, IncIE, IndavideoEmbedIE, InfoQIE, InstagramIE, InstagramIOSIE, InstagramUserIE, InstagramTagIE, InstagramStoryIE, InternazionaleIE, InternetVideoArchiveIE, IPrimaIE, IPrimaCNNIE, IqiyiIE, IqIE, IqAlbumIE, IslamChannelIE, IslamChannelSeriesIE, IsraelNationalNewsIE, ITProTVIE, ITProTVCourseIE, ITVIE, ITVBTCCIE, IviIE, IviCompilationIE, IvideonIE, IwaraIE, IwaraPlaylistIE, IwaraUserIE, IxiguaIE, IzleseneIE, JableIE, JablePlaylistIE, JamendoIE, JamendoAlbumIE, ShugiinItvLiveIE, ShugiinItvLiveRoomIE, ShugiinItvVodIE, SangiinInstructionIE, SangiinIE, JeuxVideoIE, JioSaavnSongIE, JioSaavnAlbumIE, JoveIE, JojIE, JoqrAgIE, JStreamIE, JTBCIE, JTBCProgramIE, JWPlatformIE, KakaoIE, KalturaIE, KankaNewsIE, KaraoketvIE, KelbyOneIE, KhanAcademyIE, KhanAcademyUnitIE, KickIE, KickVODIE, KickerIE, KickStarterIE, KinjaEmbedIE, KinoPoiskIE, KommunetvIE, KompasVideoIE, KooIE, KTHIE, KrasViewIE, Ku6IE, KukuluLiveIE, KuwoIE, KuwoAlbumIE, KuwoChartIE, KuwoSingerIE, KuwoCategoryIE, KuwoMvIE, LA7IE, LA7PodcastEpisodeIE, LA7PodcastIE, LastFMIE, LastFMPlaylistIE, LastFMUserIE, LaXarxaMesIE, LBRYIE, LBRYChannelIE, LBRYPlaylistIE, LCIIE, LcpPlayIE, LcpIE, Lecture2GoIE, LecturioIE, LecturioCourseIE, LecturioDeCourseIE, LeIE, LePlaylistIE, LetvCloudIE, LeFigaroVideoEmbedIE, LeFigaroVideoSectionIE, LEGOIE, LemondeIE, LentaIE, LibraryOfCongressIE, LibsynIE, LifeNewsIE, LifeEmbedIE, LikeeIE, LikeeUserIE, LimelightMediaIE, LimelightChannelIE, LimelightChannelListIE, LinkedInIE, LinkedInLearningIE, LinkedInLearningCourseIE, Liputan6IE, ListenNotesIE, LiTVIE, LiveJournalIE, LivestreamIE, LivestreamOriginalIE, LivestreamShortenerIE, LivestreamfailsIE, LnkGoIE, LnkIE, LoomIE, LoomFolderIE, LoveHomePornIE, LRTVODIE, LRTStreamIE, LSMLREmbedIE, LSMLTVEmbedIE, LSMReplayIE, LumniIE, LyndaIE, LyndaCourseIE, MaarivIE, MagellanTVIE, MagentaMusikIE, MailRuIE, MailRuMusicIE, MailRuMusicSearchIE, MainStreamingIE, MangomoloVideoIE, MangomoloLiveIE, ManotoTVIE, ManotoTVShowIE, ManotoTVLiveIE, ManyVidsIE, MaoriTVIE, MarkizaIE, MarkizaPageIE, MassengeschmackTVIE, MastersIE, MatchTVIE, MBNIE, MDRIE, MedalTVIE, MediaiteIE, MediaKlikkIE, MediasetIE, MediasetShowIE, MediasiteIE, MediasiteCatalogIE, MediasiteNamedCatalogIE, MediaStreamIE, WinSportsVideoIE, MediaWorksNZVODIE, MediciIE, MegaphoneIE, MeipaiIE, MelonVODIE, MetacriticIE, MGTVIE, MicrosoftStreamIE, MicrosoftVirtualAcademyIE, MicrosoftVirtualAcademyCourseIE, MicrosoftEmbedIE, MildomIE, MildomVodIE, MildomClipIE, MildomUserVodIE, MindsIE, MindsChannelIE, MindsGroupIE, MinotoIE, MirrativIE, MirrativUserIE, MirrorCoUKIE, TechTVMITIE, OCWMITIE, MixchIE, MixchArchiveIE, MixcloudIE, MixcloudUserIE, MixcloudPlaylistIE, MLBIE, MLBVideoIE, MLBTVIE, MLBArticleIE, MLSSoccerIE, MochaVideoIE, MojvideoIE, MonstercatIE, MotherlessIE, MotherlessGroupIE, MotherlessGalleryIE, MotherlessUploaderIE, MotorsportIE, MoviepilotIE, MoviewPlayIE, MoviezineIE, MovingImageIE, MSNIE, MTVIE, CMTIE, MTVVideoIE, MTVServicesEmbeddedIE, MTVDEIE, MTVJapanIE, MTVItaliaIE, MTVItaliaProgrammaIE, MuenchenTVIE, MurrtubeIE, MurrtubeUserIE, MuseAIIE, MuseScoreIE, MusicdexSongIE, MusicdexAlbumIE, MusicdexArtistIE, MusicdexPlaylistIE, Mx3IE, Mx3NeoIE, Mx3VolksmusikIE, MxplayerIE, MxplayerShowIE, MySpaceIE, MySpaceAlbumIE, MySpassIE, MyVideoGeIE, MyVidsterIE, MzaaloIE, N1InfoAssetIE, N1InfoIIE, NateIE, NateProgramIE, NationalGeographicVideoIE, NationalGeographicTVIE, NaverIE, NaverLiveIE, NaverNowIE, NBAWatchEmbedIE, NBAWatchIE, NBAWatchCollectionIE, NBAEmbedIE, NBAIE, NBAChannelIE, NBCOlympicsIE, NBCOlympicsStreamIE, NBCSportsIE, NBCSportsStreamIE, NBCSportsVPlayerIE, NBCStationsIE, NDRIE, NJoyIE, NDREmbedBaseIE, NDREmbedIE, NJoyEmbedIE, NDTVIE, NebulaIE, NebulaClassIE, NebulaSubscriptionsIE, NebulaChannelIE, NekoHackerIE, NerdCubedFeedIE, NetzkinoIE, NetEaseMusicIE, NetEaseMusicAlbumIE, NetEaseMusicSingerIE, NetEaseMusicListIE, NetEaseMusicMvIE, NetEaseMusicProgramIE, NetEaseMusicDjRadioIE, NetverseIE, NetversePlaylistIE, NetverseSearchIE, NewgroundsIE, NewgroundsPlaylistIE, NewgroundsUserIE, NewsPicksIE, NewsyIE, NextMediaIE, NextMediaActionNewsIE, AppleDailyIE, NextTVIE, NexxIE, NexxEmbedIE, NFBIE, NFBSeriesIE, NFHSNetworkIE, NFLIE, NFLArticleIE, NFLPlusEpisodeIE, NFLPlusReplayIE, NhkVodIE, NhkVodProgramIE, NhkForSchoolBangumiIE, NhkForSchoolSubjectIE, NhkForSchoolProgramListIE, NhkRadioNewsPageIE, NhkRadiruIE, NhkRadiruLiveIE, NHLIE, NickIE, NickBrIE, NickDeIE, NickRuIE, NiconicoIE, NiconicoPlaylistIE, NiconicoUserIE, NiconicoSeriesIE, NiconicoHistoryIE, NicovideoSearchDateIE, NicovideoSearchIE, NicovideoSearchURLIE, NicovideoTagURLIE, NiconicoLiveIE, NinaProtocolIE, NineCNineMediaIE, CPTwentyFourIE, NiconicoChannelPlusIE, NiconicoChannelPlusChannelVideosIE, NiconicoChannelPlusChannelLivesIE, NineGagIE, NineNewsIE, NineNowIE, NintendoIE, NitterIE, NobelPrizeIE, NoicePodcastIE, NonkTubeIE, NoodleMagazineIE, NoovoIE, NOSNLArticleIE, NovaEmbedIE, NovaIE, NovaPlayIE, NownessIE, NownessPlaylistIE, NownessSeriesIE, NozIE, NPOIE, AndereTijdenIE, NPOLiveIE, NPORadioIE, NPORadioFragmentIE, SchoolTVIE, HetKlokhuisIE, VPROIE, WNLIE, NprIE, NRKIE, NRKPlaylistIE, NRKSkoleIE, NRKTVIE, NRKTVDirekteIE, NRKRadioPodkastIE, NRKTVEpisodeIE, NRKTVEpisodesIE, NRKTVSeasonIE, NRKTVSeriesIE, NRLTVIE, NTVCoJpCUIE, NTVDeIE, NTVRuIE, NubilesPornIE, NYTimesIE, NYTimesArticleIE, NYTimesCookingIE, NYTimesCookingRecipeIE, NuumLiveIE, NuumTabIE, NuumMediaIE, NuvidIE, NZHeraldIE, NZOnScreenIE, NZZIE, OnDemandChinaEpisodeIE, OdnoklassnikiIE, OfTVIE, OfTVPlaylistIE, OktoberfestTVIE, OlympicsReplayIE, On24IE, OnDemandKoreaIE, OnDemandKoreaProgramIE, OneFootballIE, OneNewsNZIE, OnePlacePodcastIE, OnetIE, OnetChannelIE, OnetMVPIE, OnetPlIE, OnionStudiosIE, OpencastIE, OpencastPlaylistIE, OpenRecIE, OpenRecCaptureIE, OpenRecMovieIE, OraTVIE, ORFTVthekIE, ORFFM4StoryIE, ORFONIE, ORFRadioIE, ORFPodcastIE, ORFIPTVIE, OutsideTVIE, OwnCloudIE, PacktPubIE, PacktPubCourseIE, PalcoMP3IE, PalcoMP3ArtistIE, PalcoMP3VideoIE, PanoptoIE, PanoptoListIE, PanoptoPlaylistIE, ParamountPlusSeriesIE, ParlerIE, ParlviewIE, PatreonIE, PatreonCampaignIE, PBSIE, PBSKidsIE, PearVideoIE, PeekVidsIE, PlayVidsIE, PeerTubeIE, PeerTubePlaylistIE, PeerTVIE, PelotonIE, PelotonLiveIE, PerformGroupIE, PeriscopeIE, PeriscopeUserIE, PGATourIE, PhilharmonieDeParisIE, PhoenixIE, PhotobucketIE, PiaproIE, PIAULIZAPortalIE, PicartoIE, PicartoVodIE, PikselIE, PinkbikeIE, PinterestIE, PinterestCollectionIE, PixivSketchIE, PixivSketchUserIE, PladformIE, PlanetMarathiIE, PlatziIE, PlatziCourseIE, PlayPlusTVIE, PlaySuisseIE, PlaytvakIE, PlaywireIE, PlutoTVIE, PluralsightIE, PluralsightCourseIE, PodbayFMIE, PodbayFMChannelIE, PodchaserIE, PodomaticIE, PokemonIE, PokemonWatchIE, PokerGoIE, PokerGoCollectionIE, PolsatGoIE, PolskieRadioIE, PolskieRadioLegacyIE, PolskieRadioAuditionIE, PolskieRadioCategoryIE, PolskieRadioPlayerIE, PolskieRadioPodcastIE, PolskieRadioPodcastListIE, PopcorntimesIE, PopcornTVIE, Porn91IE, PornboxIE, PornFlipIE, PornHubIE, PornHubUserIE, PornHubPlaylistIE, PornHubPagedVideoListIE, PornHubUserVideosUploadIE, PornotubeIE, PornoVoisinesIE, PornoXOIE, PuhuTVIE, PuhuTVSerieIE, Pr0grammIE, PrankCastIE, PrankCastPostIE, PremiershipRugbyIE, PressTVIE, ProjectVeritasIE, ProSiebenSat1IE, PRXStoryIE, PRXSeriesIE, PRXAccountIE, PRXStoriesSearchIE, PRXSeriesSearchIE, Puls4IE, PyvideoIE, QDanceIE, QingTingIE, QQMusicIE, QQMusicSingerIE, QQMusicAlbumIE, QQMusicToplistIE, QQMusicPlaylistIE, R7IE, R7ArticleIE, RadikoIE, RadikoRadioIE, RadioCanadaIE, RadioCanadaAudioVideoIE, RadioComercialIE, RadioComercialPlaylistIE, RadioDeIE, RadioJavanIE, FranceCultureIE, RadioFranceIE, RadioFranceLiveIE, RadioFrancePodcastIE, RadioFranceProfileIE, RadioFranceProgramScheduleIE, RadioZetPodcastIE, RadioKapitalIE, RadioKapitalShowIE, RadLiveIE, RadLiveChannelIE, RadLiveSeasonIE, RaiIE, RaiPlayIE, RaiPlayLiveIE, RaiPlayPlaylistIE, RaiPlaySoundIE, RaiPlaySoundLiveIE, RaiPlaySoundPlaylistIE, RaiNewsIE, RaiCulturaIE, RaiSudtirolIE, RayWenderlichIE, RayWenderlichCourseIE, RbgTumIE, RbgTumCourseIE, RbgTumNewCourseIE, RCSIE, RCSEmbedsIE, RCSVariousIE, RCTIPlusIE, RCTIPlusSeriesIE, RCTIPlusTVIE, RDSIE, ParliamentLiveUKIE, RTBFIE, RedBullTVIE, RedBullEmbedIE, RedBullTVRrnContentIE, RedBullIE, RedditIE, RedCDNLivxIE, RedGifsIE, RedGifsSearchIE, RedGifsUserIE, RedTubeIE, RENTVIE, RENTVArticleIE, RestudyIE, ReutersIE, ReverbNationIE, RheinMainTVIE, RideHomeIE, RinseFMIE, RinseFMArtistPlaylistIE, RMCDecouverteIE, RockstarGamesIE, RokfinIE, RokfinStackIE, RokfinChannelIE, RokfinSearchIE, RoosterTeethIE, RoosterTeethSeriesIE, RottenTomatoesIE, RozhlasIE, RozhlasVltavaIE, MujRozhlasIE, RteIE, RteRadioIE, RtlNlIE, RTLLuTeleVODIE, RTLLuArticleIE, RTLLuLiveIE, RTLLuRadioIE, RTL2IE, RTNewsIE, RTDocumentryIE, RTDocumentryPlaylistIE, RuptlyIE, RTPIE, RTRFMIE, RTVCPlayIE, RTVCPlayEmbedIE, RTVCKalturaIE, RTVEALaCartaIE, RTVEAudioIE, RTVELiveIE, RTVEInfantilIE, RTVETelevisionIE, RTVSIE, RTVSLOIE, Rule34VideoIE, RumbleEmbedIE, RumbleIE, RumbleChannelIE, RudoVideoIE, RutubeIE, RutubeChannelIE, RutubeEmbedIE, RutubeMovieIE, RutubePersonIE, RutubePlaylistIE, RutubeTagsIE, GlomexIE, GlomexEmbedIE, MegaTVComIE, MegaTVComEmbedIE, AntennaGrWatchIE, Ant1NewsGrArticleIE, Ant1NewsGrEmbedIE, RUTVIE, RuutuIE, RuvIE, RuvSpilaIE, S4CIE, S4CSeriesIE, SafariIE, SafariApiIE, SafariCourseIE, SaitosanIE, SampleFocusIE, SapoIE, SBSIE, SBSCoKrIE, SBSCoKrAllvodProgramIE, SBSCoKrProgramsVodIE, Screen9IE, ScreencastIE, ScreencastifyIE, ScreencastOMaticIE, ScrippsNetworksWatchIE, ScrippsNetworksIE, SCTEIE, SCTECourseIE, ScrolllerIE, SejmIE, SenalColombiaLiveIE, SenateISVPIE, SenateGovIE, SendtoNewsIE, ServusIE, SevenPlusIE, SexuIE, SeznamZpravyIE, SeznamZpravyArticleIE, ShahidIE, ShahidShowIE, SharePointIE, ShareVideosEmbedIE, SibnetEmbedIE, ShemarooMeIE, ShowRoomLiveIE, SimplecastIE, SimplecastEpisodeIE, SimplecastPodcastIE, SinaIE, SixPlayIE, SkebIE, SkyItPlayerIE, SkyItVideoIE, SkyItVideoLiveIE, SkyItIE, SkyItArteIE, CieloTVItIE, TV8ItIE, SkylineWebcamsIE, SkyNewsArabiaIE, SkyNewsArabiaArticleIE, SkyNewsAUIE, SkyNewsIE, SkyNewsStoryIE, SkySportsIE, SkySportsNewsIE, SlideshareIE, SlidesLiveIE, SlutloadIE, SmotrimIE, SnotrIE, SohuIE, SohuVIE, SonyLIVIE, SonyLIVSeriesIE, SoundcloudEmbedIE, SoundcloudIE, SoundcloudSetIE, SoundcloudRelatedIE, SoundcloudUserIE, SoundcloudUserPermalinkIE, SoundcloudTrackStationIE, SoundcloudPlaylistIE, SoundcloudSearchIE, SoundgasmIE, SoundgasmProfileIE, SouthParkIE, SouthParkDeIE, SouthParkDkIE, SouthParkEsIE, SouthParkLatIE, SouthParkNlIE, SovietsClosetIE, SovietsClosetPlaylistIE, SpankBangIE, SpankBangPlaylistIE, SpiegelIE, BellatorIE, ParamountNetworkIE, StagePlusVODConcertIE, StarTrekIE, StitcherIE, StitcherShowIE, Sport5IE, SportBoxIE, SportDeutschlandIE, SpotifyIE, SpotifyShowIE, SpreakerIE, SpreakerPageIE, SpreakerShowIE, SpreakerShowPageIE, SpringboardPlatformIE, SproutIE, SRGSSRIE, RTSIE, SRGSSRPlayIE, SRMediathekIE, StacommuLiveIE, StacommuVODIE, TheaterComplexTownVODIE, TheaterComplexTownPPVIE, StanfordOpenClassroomIE, StarTVIE, SteamIE, SteamCommunityBroadcastIE, StoryFireIE, StoryFireUserIE, StoryFireSeriesIE, StreamableIE, StreamCZIE, StreetVoiceIE, StretchInternetIE, StripchatIE, STVPlayerIE, SubstackIE, SunPornoIE, SverigesRadioEpisodeIE, SverigesRadioPublicationIE, SVTIE, SVTPageIE, SVTPlayIE, SVTSeriesIE, SwearnetEpisodeIE, SYVDKIE, SyfyIE, SztvHuIE, TagesschauIE, TassIE, TBSIE, TBSJPEpisodeIE, TBSJPProgramIE, TBSJPPlaylistIE, TeachableIE, TeachableCourseIE, TeacherTubeIE, TeacherTubeUserIE, TeachingChannelIE, TeamcocoIE, ConanClassicIE, TeamTreeHouseIE, TedEmbedIE, TedPlaylistIE, TedSeriesIE, TedTalkIE, Tele5IE, Tele13IE, TeleBruxellesIE, TelecaribePlayIE, TelecincoIE, MiTeleIE, TelegraafIE, TelegramEmbedIE, TeleMBIE, TelemundoIE, TeleQuebecIE, TeleQuebecSquatIE, TeleQuebecEmissionIE, TeleQuebecLiveIE, TeleQuebecVideoIE, TeleTaskIE, TelewebionIE, TempoIE, IVXPlayerIE, IflixEpisodeIE, IflixSeriesIE, VQQSeriesIE, VQQVideoIE, WeTvEpisodeIE, WeTvSeriesIE, TennisTVIE, TenPlayIE, TenPlaySeasonIE, TestURLIE, TF1IE, TFOIE, TheGuardianPodcastIE, TheGuardianPodcastPlaylistIE, TheHoleTvIE, TheInterceptIE, ThePlatformIE, AENetworksIE, AENetworksCollectionIE, AENetworksShowIE, HistoryTopicIE, HistoryPlayerIE, BiographyIE, AMCNetworksIE, NBCIE, NBCNewsIE, ThePlatformFeedIE, CBSIE, CorusIE, ParamountPlusIE, TheStarIE, TheSunIE, TheWeatherChannelIE, ThisAmericanLifeIE, ThisOldHouseIE, ThisVidIE, ThisVidMemberIE, ThisVidPlaylistIE, ThreeSpeakIE, ThreeSpeakUserIE, ThreeQSDNIE, TikTokIE, TikTokUserIE, TikTokSoundIE, TikTokEffectIE, TikTokTagIE, TikTokVMIE, TikTokLiveIE, DouyinIE, TMZIE, TNAFlixNetworkEmbedIE, TNAFlixIE, EMPFlixIE, MovieFapIE, ToggleIE, MeWatchIE, ToggoIE, TOnlineIE, ToonGogglesIE, TouTvIE, ToypicsUserIE, ToypicsIE, TrailerAddictIE, TrillerIE, TrillerUserIE, TrillerShortIE, TrovoIE, TrovoVodIE, TrovoChannelVodIE, TrovoChannelClipIE, TrtCocukVideoIE, TrtWorldIE, TrueIDIE, TruNewsIE, TruthIE, TruTVIE, Tube8IE, TubeTuGrazIE, TubeTuGrazSeriesIE, TubiTvIE, TubiTvShowIE, TumblrIE, TuneInStationIE, TuneInPodcastIE, TuneInPodcastEpisodeIE, TuneInShortenerIE, TV2IE, TV2ArticleIE, KatsomoIE, MTVUutisetArticleIE, TV24UAVideoIE, TV2DKIE, TV2DKBornholmPlayIE, TV2HuIE, TV2HuSeriesIE, TV4IE, TV5MondePlusIE, TV5UnisVideoIE, TV5UnisIE, TVAIE, QubIE, TVANouvellesIE, TVANouvellesArticleIE, TVCIE, TVCArticleIE, TVerIE, TvigleIE, TVIPlayerIE, TVLandIE, TVN24IE, TVNoeIE, TVOpenGrWatchIE, TVOpenGrEmbedIE, TVPEmbedIE, TVPIE, TVPStreamIE, TVPVODSeriesIE, TVPVODVideoIE, TVPlayIE, TVPlayHomeIE, TVPlayerIE, TweakersIE, TwentyMinutenIE, TwentyThreeVideoIE, TwitCastingIE, TwitCastingLiveIE, TwitCastingUserIE, TwitchVodIE, TwitchCollectionIE, TwitchVideosIE, TwitchVideosClipsIE, TwitchVideosCollectionsIE, TwitchStreamIE, TwitchClipsIE, TwitterCardIE, TwitterIE, TwitterAmplifyIE, TwitterBroadcastIE, TwitterSpacesIE, TwitterShortenerIE, TxxxIE, PornTopIE, UdemyIE, UdemyCourseIE, UDNEmbedIE, UFCTVIE, UFCArabiaIE, UkColumnIE, UKTVPlayIE, DigitekaIE, DLiveVODIE, DLiveStreamIE, DroobleIE, UMGDeIE, UnistraIE, UnityIE, KnownDRMIE, KnownPiracyIE, UOLIE, UplynkIE, UplynkPreplayIE, UrortIE, URPlayIE, USANetworkIE, USATodayIE, UstreamIE, UstreamChannelIE, UstudioIE, UstudioEmbedIE, UtreonIE, Varzesh3IE, Vbox7IE, VeoIE, VeohIE, VeohUserIE, VestiIE, VevoIE, VevoPlaylistIE, BTArticleIE, BTVestlendingenIE, VH1IE, ViceIE, ViceArticleIE, ViceShowIE, ViddlerIE, VideaIE, VideocampusSachsenIE, ViMPPlaylistIE, VideoDetectiveIE, VideofyMeIE, VideoKenIE, VideoKenPlayerIE, VideoKenPlaylistIE, VideoKenCategoryIE, VideoKenTopicIE, VideomoreIE, VideomoreVideoIE, VideomoreSeasonIE, VideoPressIE, VidioIE, VidioPremierIE, VidioLiveIE, VidLiiIE, VidlyIE, ViewLiftIE, ViewLiftEmbedIE, ViideaIE, VimeoIE, VimeoAlbumIE, VimeoChannelIE, VimeoGroupsIE, VimeoLikesIE, VimeoOndemandIE, VimeoProIE, VimeoReviewIE, VimeoUserIE, VimeoWatchLaterIE, VHXEmbedIE, VimmIE, VimmRecordingIE, VineIE, VineUserIE, VikiIE, VikiChannelIE, ViouslyIE, ViqeoIE, ViuIE, ViuPlaylistIE, ViuOTTIE, ViuOTTIndonesiaIE, VKIE, VKUserVideosIE, VKWallPostIE, VKPlayIE, VKPlayLiveIE, VocarooIE, VODPlIE, VODPlatformIE, VoicyIE, VoicyChannelIE, VolejTVIE, VootIE, VootSeriesIE, VoxMediaVolumeIE, VoxMediaIE, VRTIE, VrtNUIE, KetnetIE, DagelijkseKostIE, Radio1BeIE, VTMIE, MedialaanIE, VuClipIE, VVVVIDIE, VVVVIDShowIE, WallaIE, WashingtonPostIE, WashingtonPostArticleIE, WatIE, WDRIE, WDRPageIE, WDRElefantIE, WDRMobileIE, WebcameraplIE, WebcasterIE, WebcasterFeedIE, WebOfStoriesIE, WebOfStoriesPlaylistIE, WeiboIE, WeiboVideoIE, WeiboUserIE, WeiqiTVIE, WeverseIE, WeverseMediaIE, WeverseMomentIE, WeverseLiveTabIE, WeverseMediaTabIE, WeverseLiveIE, WeVidiIE, WeyyakIE, WhypIE, WikimediaIE, WimbledonIE, WimTVIE, WhoWatchIE, WistiaIE, WistiaPlaylistIE, WistiaChannelIE, WordpressPlaylistEmbedIE, WordpressMiniAudioPlayerEmbedIE, WorldStarHipHopIE, WPPilotIE, WPPilotChannelsIE, WrestleUniverseVODIE, WrestleUniversePPVIE, WSJIE, WSJArticleIE, WWEIE, WykopDigIE, WykopDigCommentIE, WykopPostIE, WykopPostCommentIE, XanimuIE, XboxClipsIE, XFileShareIE, XHamsterIE, XHamsterEmbedIE, XHamsterUserIE, XimalayaIE, XimalayaAlbumIE, XinpianchangIE, XMinusIE, XNXXIE, XstreamIE, VGTVIE, XVideosIE, XVideosQuickiesIE, XXXYMoviesIE, YahooIE, AolIE, YahooSearchIE, YahooJapanNewsIE, YandexDiskIE, YandexMusicTrackIE, YandexMusicAlbumIE, YandexMusicPlaylistIE, YandexMusicArtistTracksIE, YandexMusicArtistAlbumsIE, YandexVideoIE, YandexVideoPreviewIE, ZenYandexIE, ZenYandexChannelIE, YapFilesIE, YappyIE, YappyProfileIE, YleAreenaIE, YouJizzIE, YoukuIE, YoukuShowIE, YouNowLiveIE, YouNowChannelIE, YouNowMomentIE, YouPornIE, YourPornIE, YourUploadIE, ZaikoIE, ZaikoETicketIE, ZapiksIE, BBVTVIE, BBVTVLiveIE, BBVTVRecordingsIE, EinsUndEinsTVIE, EinsUndEinsTVLiveIE, EinsUndEinsTVRecordingsIE, EWETVIE, EWETVLiveIE, EWETVRecordingsIE, GlattvisionTVIE, GlattvisionTVLiveIE, GlattvisionTVRecordingsIE, MNetTVIE, MNetTVLiveIE, MNetTVRecordingsIE, NetPlusTVIE, NetPlusTVLiveIE, NetPlusTVRecordingsIE, OsnatelTVIE, OsnatelTVLiveIE, OsnatelTVRecordingsIE, QuantumTVIE, QuantumTVLiveIE, QuantumTVRecordingsIE, SaltTVIE, SaltTVLiveIE, SaltTVRecordingsIE, SAKTVIE, SAKTVLiveIE, SAKTVRecordingsIE, VTXTVIE, VTXTVLiveIE, VTXTVRecordingsIE, WalyTVIE, WalyTVLiveIE, WalyTVRecordingsIE, ZattooIE, ZattooLiveIE, ZattooMoviesIE, ZattooRecordingsIE, ZDFIE, DreiSatIE, ZDFChannelIE, Zee5IE, Zee5SeriesIE, ZeeNewsIE, ZenPornIE, ZetlandDKArticleIE, ZhihuIE, ZingMp3IE, ZingMp3AlbumIE, ZingMp3ChartHomeIE, ZingMp3WeekChartIE, ZingMp3ChartMusicVideoIE, ZingMp3UserIE, ZingMp3HubIE, ZingMp3LiveRadioIE, ZingMp3PodcastEpisodeIE, ZingMp3PodcastIE, ZoomIE, ZypeIE, GenericIE]
+_ALL_CLASSES = [YoutubeIE, YoutubeClipIE, YoutubeFavouritesIE, YoutubeNotificationsIE, YoutubeHistoryIE, YoutubeTabIE, YoutubeLivestreamEmbedIE, YoutubePlaylistIE, YoutubeRecommendedIE, YoutubeSearchDateIE, YoutubeSearchIE, YoutubeSearchURLIE, YoutubeMusicSearchURLIE, YoutubeSubscriptionsIE, YoutubeTruncatedIDIE, YoutubeTruncatedURLIE, YoutubeYtBeIE, YoutubeYtUserIE, YoutubeWatchLaterIE, YoutubeShortsAudioPivotIE, YoutubeConsentRedirectIE, ABCIE, ABCIViewIE, ABCIViewShowSeriesIE, AbcNewsIE, AbcNewsVideoIE, ABCOTVSIE, ABCOTVSClipsIE, AbemaTVIE, AbemaTVTitleIE, AcademicEarthCourseIE, ACastIE, ACastChannelIE, AcFunVideoIE, AcFunBangumiIE, ADNIE, ADNSeasonIE, AdobeConnectIE, AdobeTVEmbedIE, AdobeTVIE, AdobeTVShowIE, AdobeTVChannelIE, AdobeTVVideoIE, AdultSwimIE, AeonCoIE, AfreecaTVIE, AfreecaTVLiveIE, AfreecaTVUserIE, TokFMAuditionIE, TokFMPodcastIE, WyborczaPodcastIE, WyborczaVideoIE, AirTVIE, AitubeKZVideoIE, AlJazeeraIE, AllstarIE, AllstarProfileIE, AlphaPornoIE, AltCensoredIE, AltCensoredChannelIE, AluraIE, AluraCourseIE, AmadeusTVIE, AmaraIE, AmazonStoreIE, AmazonReviewsIE, AmazonMiniTVIE, AmazonMiniTVSeasonIE, AmazonMiniTVSeriesIE, AmericasTestKitchenIE, AmericasTestKitchenSeasonIE, AnchorFMEpisodeIE, AngelIE, AnvatoIE, AllocineIE, AliExpressLiveIE, Alsace20TVIE, Alsace20TVEmbedIE, APAIE, AparatIE, AppleConnectIE, AppleTrailersIE, AppleTrailersSectionIE, ApplePodcastsIE, ArchiveOrgIE, YoutubeWebArchiveIE, ArcPublishingIE, ArkenaIE, ARDBetaMediathekIE, ARDMediathekCollectionIE, ARDIE, Art19IE, Art19ShowIE, ArteTVIE, ArteTVEmbedIE, ArteTVPlaylistIE, ArteTVCategoryIE, ArnesIE, AsobiChannelIE, AsobiChannelTagURLIE, AsobiStageIE, AtresPlayerIE, AtScaleConfEventIE, ATVAtIE, AudiMediaIE, AudioBoomIE, AudiodraftCustomIE, AudiodraftGenericIE, AudiomackIE, AudiomackAlbumIE, AudiusIE, AudiusTrackIE, AudiusPlaylistIE, AudiusProfileIE, AWAANIE, AWAANVideoIE, AWAANLiveIE, AWAANSeasonIE, AxsIE, AZMedienIE, BaiduVideoIE, BanByeIE, BanByeChannelIE, BandaiChannelIE, BandcampIE, BandcampAlbumIE, BandcampWeeklyIE, BandcampUserIE, BannedVideoIE, BBCCoUkIE, BBCCoUkArticleIE, BBCCoUkIPlayerEpisodesIE, BBCCoUkIPlayerGroupIE, BBCCoUkPlaylistIE, BBCIE, BeegIE, BehindKinkIE, BellMediaIE, BeatBumpVideoIE, BeatBumpPlaylistIE, BeatportIE, BerufeTVIE, BetIE, BFIPlayerIE, BFMTVIE, BFMTVLiveIE, BFMTVArticleIE, BibelTVLiveIE, BibelTVSeriesIE, BibelTVVideoIE, BigflixIE, BigoIE, BildIE, BiliBiliIE, BiliBiliBangumiIE, BiliBiliBangumiSeasonIE, BiliBiliBangumiMediaIE, BilibiliCheeseIE, BilibiliCheeseSeasonIE, BiliBiliSearchIE, BilibiliCategoryIE, BilibiliAudioIE, BilibiliAudioAlbumIE, BiliBiliPlayerIE, BilibiliSpaceVideoIE, BilibiliSpaceAudioIE, BilibiliCollectionListIE, BilibiliSeriesListIE, BilibiliFavoritesListIE, BilibiliWatchlaterIE, BilibiliPlaylistIE, BiliIntlIE, BiliIntlSeriesIE, BiliLiveIE, BioBioChileTVIE, BitChuteIE, BitChuteChannelIE, BlackboardCollaborateIE, BleacherReportIE, BleacherReportCMSIE, BlerpIE, BloggerIE, BloombergIE, BokeCCIE, BongaCamsIE, BoostyIE, BostonGlobeIE, BoxIE, BoxCastVideoIE, BpbIE, BRIE, BravoTVIE, BrainPOPIE, BrainPOPJrIE, BrainPOPELLIE, BrainPOPEspIE, BrainPOPFrIE, BrainPOPIlIE, BreitBartIE, BrightcoveLegacyIE, BrightcoveNewIE, BrilliantpalaElearnIE, BrilliantpalaClassesIE, BusinessInsiderIE, BundesligaIE, BundestagIE, BuzzFeedIE, BYUtvIE, C56IE, CableAVIE, CallinIE, CaltransIE, CAM4IE, CamdemyIE, CamdemyFolderIE, CamFMEpisodeIE, CamFMShowIE, CamModelsIE, CamsodaIE, CamtasiaEmbedIE, Canal1IE, CanalAlphaIE, CanalplusIE, Canalc2IE, CaracolTvPlayIE, CartoonNetworkIE, CBCIE, CBCPlayerIE, CBCPlayerPlaylistIE, CBCGemIE, CBCGemPlaylistIE, CBCGemLiveIE, ParamountPressExpressIE, CBSNewsEmbedIE, CBSNewsIE, CBSLocalIE, CBSLocalArticleIE, CBSLocalLiveIE, CBSNewsLiveIE, CBSNewsLiveVideoIE, CBSSportsEmbedIE, CBSSportsIE, TwentyFourSevenSportsIE, CCCIE, CCCPlaylistIE, CCMAIE, CCTVIE, CDAIE, CellebriteIE, CeskaTelevizeIE, CGTNIE, CharlieRoseIE, ChaturbateIE, ChilloutzoneIE, CHZZKLiveIE, CHZZKVideoIE, CinemaxIE, CinetecaMilanoIE, CineverseIE, CineverseDetailsIE, CiscoLiveSessionIE, CiscoLiveSearchIE, CiscoWebexIE, CJSWIE, ClipchampIE, ClippitIE, ClipRsIE, CloserToTruthIE, CloudflareStreamIE, CloudyCDNIE, ClubicIE, ClypIE, CNBCVideoIE, CNNIE, CNNBlogsIE, CNNArticleIE, CNNIndonesiaIE, CoubIE, ComedyCentralIE, ComedyCentralTVIE, CommonMistakesIE, UnicodeBOMIE, MmsIE, RtmpIE, ViewSourceIE, CondeNastIE, CONtvIE, CPACIE, CPACPlaylistIE, CozyTVIE, CrackedIE, CrackleIE, CraftsyIE, CrooksAndLiarsIE, CrowdBunkerIE, CrowdBunkerChannelIE, CrtvgIE, CrunchyrollBetaIE, CrunchyrollBetaShowIE, CrunchyrollMusicIE, CrunchyrollArtistIE, CSpanIE, CSpanCongressIE, CtsNewsIE, CTVIE, CTVNewsIE, CultureUnpluggedIE, CuriosityStreamIE, CuriosityStreamCollectionsIE, CuriosityStreamSeriesIE, CWTVIE, CybraryIE, CybraryCourseIE, DacastVODIE, DacastPlaylistIE, DailyMailIE, DailymotionIE, DailymotionPlaylistIE, DailymotionSearchIE, DailymotionUserIE, DailyWireIE, DailyWirePodcastIE, DamtomoRecordIE, DamtomoVideoIE, DaumIE, DaumClipIE, DaumPlaylistIE, DaumUserIE, DaystarClipIE, DBTVIE, DctpTvIE, DeezerPlaylistIE, DeezerAlbumIE, DemocracynowIE, DetikEmbedIE, DLFIE, DLFCorpusIE, DFBIE, DHMIE, DouyuShowIE, DouyuTVIE, DPlayIE, DiscoveryPlusIE, HGTVDeIE, GoDiscoveryIE, TravelChannelIE, CookingChannelIE, HGTVUsaIE, FoodNetworkIE, InvestigationDiscoveryIE, DestinationAmericaIE, AmHistoryChannelIE, ScienceChannelIE, DIYNetworkIE, DiscoveryLifeIE, AnimalPlanetIE, TLCIE, MotorTrendIE, MotorTrendOnDemandIE, DiscoveryPlusIndiaIE, DiscoveryNetworksDeIE, DiscoveryPlusItalyIE, DiscoveryPlusItalyShowIE, DiscoveryPlusIndiaShowIE, GlobalCyclingNetworkPlusIE, DRBonanzaIE, DrTuberIE, DRTVIE, DRTVLiveIE, DRTVSeasonIE, DRTVSeriesIE, DTubeIE, DVTVIE, DubokuIE, DubokuPlaylistIE, DumpertIE, DeuxMIE, DeuxMNewsIE, DigitalConcertHallIE, DiscogsReleasePlaylistIE, DiscoveryIE, DisneyIE, DigitallySpeakingIE, DropboxIE, DropoutSeasonIE, DropoutIE, DuoplayIE, DWIE, DWArticleIE, EaglePlatformIE, ClipYouEmbedIE, EbaumsWorldIE, EbayIE, EggheadCourseIE, EggheadLessonIE, EightTracksIE, EinthusanIE, EitbIE, ElementorEmbedIE, ElonetIE, ElPaisIE, ElTreceTVIE, EmbedlyIE, EpiconIE, EpiconSeriesIE, EpidemicSoundIE, EplusIbIE, EpochIE, EpornerIE, ErocastIE, EroProfileIE, EroProfileAlbumIE, ERRJupiterIE, ERTFlixCodenameIE, ERTFlixIE, ERTWebtvEmbedIE, ESPNIE, WatchESPNIE, ESPNArticleIE, FiveThirtyEightIE, ESPNCricInfoIE, EttuTvIE, EuropaIE, EuroParlWebstreamIE, EuropeanTourIE, EurosportIE, EUScreenIE, ExpressenIE, EyedoTVIE, FacebookIE, FacebookPluginsVideoIE, FacebookRedirectURLIE, FacebookReelIE, FacebookAdsIE, FathomIE, FancodeVodIE, FancodeLiveIE, FazIE, FC2IE, FC2EmbedIE, FC2LiveIE, FczenitIE, FifaIE, FilmOnIE, FilmOnChannelIE, FilmwebIE, FirstTVIE, FiveTVIE, FlexTVIE, FlickrIE, FloatplaneIE, FloatplaneChannelIE, FolketingetIE, FootyRoomIE, Formula1IE, FourTubeIE, PornTubeIE, PornerBrosIE, FuxIE, FOXIE, FOX9IE, FOX9NewsIE, FoxNewsIE, FoxNewsArticleIE, FoxNewsVideoIE, FoxSportsIE, FptplayIE, FranceInterIE, FranceTVIE, FranceTVSiteIE, FranceTVInfoIE, FreesoundIE, FreespeechIE, FrontendMastersIE, FrontendMastersLessonIE, FrontendMastersCourseIE, FreeTvIE, FreeTvMoviesIE, FujiTVFODPlus7IE, FunimationIE, FunimationPageIE, FunimationShowIE, FunkIE, Funker530IE, FuyinTVIE, GabTVIE, GabIE, GaiaIE, GameJoltIE, GameJoltUserIE, GameJoltGameIE, GameJoltGameSoundtrackIE, GameJoltCommunityIE, GameJoltSearchIE, GameSpotIE, GameStarIE, GaskrankIE, GazetaIE, GDCVaultIE, GediDigitalIE, GeniusIE, GeniusLyricsIE, GetCourseRuPlayerIE, GetCourseRuIE, GettrIE, GettrStreamingIE, GiantBombIE, GlideIE, GlobalPlayerLiveIE, GlobalPlayerLivePlaylistIE, GlobalPlayerAudioIE, GlobalPlayerAudioEpisodeIE, GlobalPlayerVideoIE, GloboIE, GloboArticleIE, GMANetworkVideoIE, GoIE, GodTubeIE, GofileIE, GolemIE, GoodGameIE, GoogleDriveIE, GoogleDriveFolderIE, GooglePodcastsIE, GooglePodcastsFeedIE, GoogleSearchIE, GoProIE, GoPlayIE, GoshgayIE, GoToStageIE, GPUTechConfIE, GronkhIE, GronkhFeedIE, GronkhVodsIE, GrouponIE, HarpodeonIE, HBOIE, HearThisAtIE, HeiseIE, HellPornoIE, HGTVComShowIE, HKETVIE, HiDiveIE, HistoricFilmsIE, HitRecordIE, HollywoodReporterIE, HollywoodReporterPlaylistIE, HolodexIE, HotNewHipHopIE, HotStarIE, HotStarPrefixIE, HotStarPlaylistIE, HotStarSeasonIE, HotStarSeriesIE, HrefLiRedirectIE, HRFernsehenIE, HRTiIE, HRTiPlaylistIE, HSEShowIE, HSEProductIE, HTML5MediaEmbedIE, QuotedHTMLIE, HuajiaoIE, HuyaLiveIE, HuffPostIE, HungamaIE, HungamaSongIE, HungamaAlbumPlaylistIE, HypemIE, MonsterSirenHypergryphMusicIE, HytaleIE, IcareusIE, IchinanaLiveIE, IchinanaLiveClipIE, IdolPlusIE, IGNIE, IGNVideoIE, IGNArticleIE, IHeartRadioIE, IHeartRadioPodcastIE, IlPostIE, IltalehtiIE, ImdbIE, ImdbListIE, ImgurIE, ImgurAlbumIE, ImgurGalleryIE, InaIE, IncIE, IndavideoEmbedIE, InfoQIE, InstagramIE, InstagramIOSIE, InstagramUserIE, InstagramTagIE, InstagramStoryIE, InternazionaleIE, InternetVideoArchiveIE, IPrimaIE, IPrimaCNNIE, IqiyiIE, IqIE, IqAlbumIE, IslamChannelIE, IslamChannelSeriesIE, IsraelNationalNewsIE, ITProTVIE, ITProTVCourseIE, ITVIE, ITVBTCCIE, IviIE, IviCompilationIE, IvideonIE, IwaraIE, IwaraPlaylistIE, IwaraUserIE, IxiguaIE, IzleseneIE, JableIE, JablePlaylistIE, JamendoIE, JamendoAlbumIE, ShugiinItvLiveIE, ShugiinItvLiveRoomIE, ShugiinItvVodIE, SangiinInstructionIE, SangiinIE, JeuxVideoIE, JioSaavnSongIE, JioSaavnAlbumIE, JioSaavnPlaylistIE, JoveIE, JojIE, JoqrAgIE, JStreamIE, JTBCIE, JTBCProgramIE, JWPlatformIE, KakaoIE, KalturaIE, KankaNewsIE, KaraoketvIE, KelbyOneIE, KhanAcademyIE, KhanAcademyUnitIE, KickIE, KickVODIE, KickerIE, KickStarterIE, KinjaEmbedIE, KinoPoiskIE, KommunetvIE, KompasVideoIE, KooIE, KTHIE, KrasViewIE, Ku6IE, KukuluLiveIE, KuwoIE, KuwoAlbumIE, KuwoChartIE, KuwoSingerIE, KuwoCategoryIE, KuwoMvIE, LA7IE, LA7PodcastEpisodeIE, LA7PodcastIE, LastFMIE, LastFMPlaylistIE, LastFMUserIE, LaXarxaMesIE, LBRYIE, LBRYChannelIE, LBRYPlaylistIE, LCIIE, LcpPlayIE, LcpIE, Lecture2GoIE, LecturioIE, LecturioCourseIE, LecturioDeCourseIE, LeIE, LePlaylistIE, LetvCloudIE, LeFigaroVideoEmbedIE, LeFigaroVideoSectionIE, LEGOIE, LemondeIE, LentaIE, LibraryOfCongressIE, LibsynIE, LifeNewsIE, LifeEmbedIE, LikeeIE, LikeeUserIE, LimelightMediaIE, LimelightChannelIE, LimelightChannelListIE, LinkedInIE, LinkedInLearningIE, LinkedInLearningCourseIE, Liputan6IE, ListenNotesIE, LiTVIE, LiveJournalIE, LivestreamIE, LivestreamOriginalIE, LivestreamShortenerIE, LivestreamfailsIE, LnkGoIE, LnkIE, LoomIE, LoomFolderIE, LoveHomePornIE, LRTVODIE, LRTStreamIE, LSMLREmbedIE, LSMLTVEmbedIE, LSMReplayIE, LumniIE, LyndaIE, LyndaCourseIE, MaarivIE, MagellanTVIE, MagentaMusikIE, MailRuIE, MailRuMusicIE, MailRuMusicSearchIE, MainStreamingIE, MangomoloVideoIE, MangomoloLiveIE, ManotoTVIE, ManotoTVShowIE, ManotoTVLiveIE, ManyVidsIE, MaoriTVIE, MarkizaIE, MarkizaPageIE, MassengeschmackTVIE, MastersIE, MatchTVIE, MBNIE, MDRIE, MedalTVIE, MediaiteIE, MediaKlikkIE, MediasetIE, MediasetShowIE, MediasiteIE, MediasiteCatalogIE, MediasiteNamedCatalogIE, MediaStreamIE, WinSportsVideoIE, MediaWorksNZVODIE, MediciIE, MegaphoneIE, MeipaiIE, MelonVODIE, MetacriticIE, MGTVIE, MicrosoftStreamIE, MicrosoftVirtualAcademyIE, MicrosoftVirtualAcademyCourseIE, MicrosoftEmbedIE, MildomIE, MildomVodIE, MildomClipIE, MildomUserVodIE, MindsIE, MindsChannelIE, MindsGroupIE, MinotoIE, MirrativIE, MirrativUserIE, MirrorCoUKIE, TechTVMITIE, OCWMITIE, MixchIE, MixchArchiveIE, MixcloudIE, MixcloudUserIE, MixcloudPlaylistIE, MLBIE, MLBVideoIE, MLBTVIE, MLBArticleIE, MLSSoccerIE, MochaVideoIE, MojvideoIE, MonstercatIE, MotherlessIE, MotherlessGroupIE, MotherlessGalleryIE, MotherlessUploaderIE, MotorsportIE, MoviepilotIE, MoviewPlayIE, MoviezineIE, MovingImageIE, MSNIE, MTVIE, CMTIE, MTVVideoIE, MTVServicesEmbeddedIE, MTVDEIE, MTVJapanIE, MTVItaliaIE, MTVItaliaProgrammaIE, MuenchenTVIE, MurrtubeIE, MurrtubeUserIE, MuseAIIE, MuseScoreIE, MusicdexSongIE, MusicdexAlbumIE, MusicdexArtistIE, MusicdexPlaylistIE, Mx3IE, Mx3NeoIE, Mx3VolksmusikIE, MxplayerIE, MxplayerShowIE, MySpaceIE, MySpaceAlbumIE, MySpassIE, MyVideoGeIE, MyVidsterIE, MzaaloIE, N1InfoAssetIE, N1InfoIIE, NateIE, NateProgramIE, NationalGeographicVideoIE, NationalGeographicTVIE, NaverIE, NaverLiveIE, NaverNowIE, NBAWatchEmbedIE, NBAWatchIE, NBAWatchCollectionIE, NBAEmbedIE, NBAIE, NBAChannelIE, NBCOlympicsIE, NBCOlympicsStreamIE, NBCSportsIE, NBCSportsStreamIE, NBCSportsVPlayerIE, NBCStationsIE, NDRIE, NJoyIE, NDREmbedBaseIE, NDREmbedIE, NJoyEmbedIE, NDTVIE, NebulaIE, NebulaClassIE, NebulaSubscriptionsIE, NebulaChannelIE, NekoHackerIE, NerdCubedFeedIE, NetzkinoIE, NetEaseMusicIE, NetEaseMusicAlbumIE, NetEaseMusicSingerIE, NetEaseMusicListIE, NetEaseMusicMvIE, NetEaseMusicProgramIE, NetEaseMusicDjRadioIE, NetverseIE, NetversePlaylistIE, NetverseSearchIE, NewgroundsIE, NewgroundsPlaylistIE, NewgroundsUserIE, NewsPicksIE, NewsyIE, NextMediaIE, NextMediaActionNewsIE, AppleDailyIE, NextTVIE, NexxIE, NexxEmbedIE, NFBIE, NFBSeriesIE, NFHSNetworkIE, NFLIE, NFLArticleIE, NFLPlusEpisodeIE, NFLPlusReplayIE, NhkVodIE, NhkVodProgramIE, NhkForSchoolBangumiIE, NhkForSchoolSubjectIE, NhkForSchoolProgramListIE, NhkRadioNewsPageIE, NhkRadiruIE, NhkRadiruLiveIE, NHLIE, NickIE, NickBrIE, NickDeIE, NickRuIE, NiconicoIE, NiconicoPlaylistIE, NiconicoUserIE, NiconicoSeriesIE, NiconicoHistoryIE, NicovideoSearchDateIE, NicovideoSearchIE, NicovideoSearchURLIE, NicovideoTagURLIE, NiconicoLiveIE, NinaProtocolIE, NineCNineMediaIE, CPTwentyFourIE, NiconicoChannelPlusIE, NiconicoChannelPlusChannelVideosIE, NiconicoChannelPlusChannelLivesIE, NineGagIE, NineNewsIE, NineNowIE, NintendoIE, NitterIE, NobelPrizeIE, NoicePodcastIE, NonkTubeIE, NoodleMagazineIE, NoovoIE, NOSNLArticleIE, NovaEmbedIE, NovaIE, NovaPlayIE, NownessIE, NownessPlaylistIE, NownessSeriesIE, NozIE, NPOIE, AndereTijdenIE, NPOLiveIE, NPORadioIE, NPORadioFragmentIE, SchoolTVIE, HetKlokhuisIE, VPROIE, WNLIE, NprIE, NRKIE, NRKPlaylistIE, NRKSkoleIE, NRKTVIE, NRKTVDirekteIE, NRKRadioPodkastIE, NRKTVEpisodeIE, NRKTVEpisodesIE, NRKTVSeasonIE, NRKTVSeriesIE, NRLTVIE, NTVCoJpCUIE, NTVDeIE, NTVRuIE, NubilesPornIE, NYTimesIE, NYTimesArticleIE, NYTimesCookingIE, NYTimesCookingRecipeIE, NuumLiveIE, NuumTabIE, NuumMediaIE, NuvidIE, NZHeraldIE, NZOnScreenIE, NZZIE, OnDemandChinaEpisodeIE, OdnoklassnikiIE, OfTVIE, OfTVPlaylistIE, OktoberfestTVIE, OlympicsReplayIE, On24IE, OnDemandKoreaIE, OnDemandKoreaProgramIE, OneFootballIE, OneNewsNZIE, OnePlacePodcastIE, OnetIE, OnetChannelIE, OnetMVPIE, OnetPlIE, OnionStudiosIE, OpencastIE, OpencastPlaylistIE, OpenRecIE, OpenRecCaptureIE, OpenRecMovieIE, OraTVIE, ORFTVthekIE, ORFFM4StoryIE, ORFONIE, ORFRadioIE, ORFPodcastIE, ORFIPTVIE, OutsideTVIE, OwnCloudIE, PacktPubIE, PacktPubCourseIE, PalcoMP3IE, PalcoMP3ArtistIE, PalcoMP3VideoIE, PanoptoIE, PanoptoListIE, PanoptoPlaylistIE, ParamountPlusSeriesIE, ParlerIE, ParlviewIE, PatreonIE, PatreonCampaignIE, PBSIE, PBSKidsIE, PearVideoIE, PeekVidsIE, PlayVidsIE, PeerTubeIE, PeerTubePlaylistIE, PeerTVIE, PelotonIE, PelotonLiveIE, PerformGroupIE, PeriscopeIE, PeriscopeUserIE, PGATourIE, PhilharmonieDeParisIE, PhoenixIE, PhotobucketIE, PiaproIE, PIAULIZAPortalIE, PicartoIE, PicartoVodIE, PikselIE, PinkbikeIE, PinterestIE, PinterestCollectionIE, PixivSketchIE, PixivSketchUserIE, PladformIE, PlanetMarathiIE, PlatziIE, PlatziCourseIE, PlayPlusTVIE, PlaySuisseIE, PlaytvakIE, PlaywireIE, PlutoTVIE, PluralsightIE, PluralsightCourseIE, PodbayFMIE, PodbayFMChannelIE, PodchaserIE, PodomaticIE, PokemonIE, PokemonWatchIE, PokerGoIE, PokerGoCollectionIE, PolsatGoIE, PolskieRadioIE, PolskieRadioLegacyIE, PolskieRadioAuditionIE, PolskieRadioCategoryIE, PolskieRadioPlayerIE, PolskieRadioPodcastIE, PolskieRadioPodcastListIE, PopcorntimesIE, PopcornTVIE, Porn91IE, PornboxIE, PornFlipIE, PornHubIE, PornHubUserIE, PornHubPlaylistIE, PornHubPagedVideoListIE, PornHubUserVideosUploadIE, PornotubeIE, PornoVoisinesIE, PornoXOIE, PuhuTVIE, PuhuTVSerieIE, Pr0grammIE, PrankCastIE, PrankCastPostIE, PremiershipRugbyIE, PressTVIE, ProjectVeritasIE, ProSiebenSat1IE, PRXStoryIE, PRXSeriesIE, PRXAccountIE, PRXStoriesSearchIE, PRXSeriesSearchIE, Puls4IE, PyvideoIE, QDanceIE, QingTingIE, QQMusicIE, QQMusicSingerIE, QQMusicAlbumIE, QQMusicToplistIE, QQMusicPlaylistIE, R7IE, R7ArticleIE, RadikoIE, RadikoRadioIE, RadioCanadaIE, RadioCanadaAudioVideoIE, RadioComercialIE, RadioComercialPlaylistIE, RadioDeIE, RadioJavanIE, FranceCultureIE, RadioFranceIE, RadioFranceLiveIE, RadioFrancePodcastIE, RadioFranceProfileIE, RadioFranceProgramScheduleIE, RadioZetPodcastIE, RadioKapitalIE, RadioKapitalShowIE, RadLiveIE, RadLiveChannelIE, RadLiveSeasonIE, RaiIE, RaiPlayIE, RaiPlayLiveIE, RaiPlayPlaylistIE, RaiPlaySoundIE, RaiPlaySoundLiveIE, RaiPlaySoundPlaylistIE, RaiNewsIE, RaiCulturaIE, RaiSudtirolIE, RayWenderlichIE, RayWenderlichCourseIE, RbgTumIE, RbgTumCourseIE, RbgTumNewCourseIE, RCSIE, RCSEmbedsIE, RCSVariousIE, RCTIPlusIE, RCTIPlusSeriesIE, RCTIPlusTVIE, RDSIE, ParliamentLiveUKIE, RTBFIE, RedBullTVIE, RedBullEmbedIE, RedBullTVRrnContentIE, RedBullIE, RedditIE, RedCDNLivxIE, RedGifsIE, RedGifsSearchIE, RedGifsUserIE, RedTubeIE, RENTVIE, RENTVArticleIE, RestudyIE, ReutersIE, ReverbNationIE, RheinMainTVIE, RideHomeIE, RinseFMIE, RinseFMArtistPlaylistIE, RMCDecouverteIE, RockstarGamesIE, RokfinIE, RokfinStackIE, RokfinChannelIE, RokfinSearchIE, RoosterTeethIE, RoosterTeethSeriesIE, RottenTomatoesIE, RozhlasIE, RozhlasVltavaIE, MujRozhlasIE, RteIE, RteRadioIE, RtlNlIE, RTLLuTeleVODIE, RTLLuArticleIE, RTLLuLiveIE, RTLLuRadioIE, RTL2IE, RTNewsIE, RTDocumentryIE, RTDocumentryPlaylistIE, RuptlyIE, RTPIE, RTRFMIE, RTVCPlayIE, RTVCPlayEmbedIE, RTVCKalturaIE, RTVEALaCartaIE, RTVEAudioIE, RTVELiveIE, RTVEInfantilIE, RTVETelevisionIE, RTVSIE, RTVSLOIE, Rule34VideoIE, RumbleEmbedIE, RumbleIE, RumbleChannelIE, RudoVideoIE, RutubeIE, RutubeChannelIE, RutubeEmbedIE, RutubeMovieIE, RutubePersonIE, RutubePlaylistIE, RutubeTagsIE, GlomexIE, GlomexEmbedIE, MegaTVComIE, MegaTVComEmbedIE, AntennaGrWatchIE, Ant1NewsGrArticleIE, Ant1NewsGrEmbedIE, RUTVIE, RuutuIE, RuvIE, RuvSpilaIE, S4CIE, S4CSeriesIE, SafariIE, SafariApiIE, SafariCourseIE, SaitosanIE, SampleFocusIE, SapoIE, SBSIE, SBSCoKrIE, SBSCoKrAllvodProgramIE, SBSCoKrProgramsVodIE, Screen9IE, ScreencastIE, ScreencastifyIE, ScreencastOMaticIE, ScrippsNetworksWatchIE, ScrippsNetworksIE, SCTEIE, SCTECourseIE, ScrolllerIE, SejmIE, SenalColombiaLiveIE, SenateISVPIE, SenateGovIE, SendtoNewsIE, ServusIE, SevenPlusIE, SexuIE, SeznamZpravyIE, SeznamZpravyArticleIE, ShahidIE, ShahidShowIE, SharePointIE, ShareVideosEmbedIE, SibnetEmbedIE, ShemarooMeIE, ShowRoomLiveIE, SimplecastIE, SimplecastEpisodeIE, SimplecastPodcastIE, SinaIE, SixPlayIE, SkebIE, SkyItPlayerIE, SkyItVideoIE, SkyItVideoLiveIE, SkyItIE, SkyItArteIE, CieloTVItIE, TV8ItIE, SkylineWebcamsIE, SkyNewsArabiaIE, SkyNewsArabiaArticleIE, SkyNewsAUIE, SkyNewsIE, SkyNewsStoryIE, SkySportsIE, SkySportsNewsIE, SlideshareIE, SlidesLiveIE, SlutloadIE, SmotrimIE, SnotrIE, SohuIE, SohuVIE, SonyLIVIE, SonyLIVSeriesIE, SoundcloudEmbedIE, SoundcloudIE, SoundcloudSetIE, SoundcloudRelatedIE, SoundcloudUserIE, SoundcloudUserPermalinkIE, SoundcloudTrackStationIE, SoundcloudPlaylistIE, SoundcloudSearchIE, SoundgasmIE, SoundgasmProfileIE, SouthParkIE, SouthParkDeIE, SouthParkDkIE, SouthParkEsIE, SouthParkLatIE, SouthParkNlIE, SovietsClosetIE, SovietsClosetPlaylistIE, SpankBangIE, SpankBangPlaylistIE, SpiegelIE, BellatorIE, ParamountNetworkIE, StagePlusVODConcertIE, StarTrekIE, StitcherIE, StitcherShowIE, Sport5IE, SportBoxIE, SportDeutschlandIE, SpotifyIE, SpotifyShowIE, SpreakerIE, SpreakerPageIE, SpreakerShowIE, SpreakerShowPageIE, SpringboardPlatformIE, SproutIE, SRGSSRIE, RTSIE, SRGSSRPlayIE, SRMediathekIE, StacommuLiveIE, StacommuVODIE, TheaterComplexTownVODIE, TheaterComplexTownPPVIE, StanfordOpenClassroomIE, StarTVIE, SteamIE, SteamCommunityBroadcastIE, StoryFireIE, StoryFireUserIE, StoryFireSeriesIE, StreamableIE, StreamCZIE, StreetVoiceIE, StretchInternetIE, StripchatIE, STVPlayerIE, SubstackIE, SunPornoIE, SverigesRadioEpisodeIE, SverigesRadioPublicationIE, SVTIE, SVTPageIE, SVTPlayIE, SVTSeriesIE, SwearnetEpisodeIE, SYVDKIE, SyfyIE, SztvHuIE, TagesschauIE, TassIE, TBSIE, TBSJPEpisodeIE, TBSJPProgramIE, TBSJPPlaylistIE, TeachableIE, TeachableCourseIE, TeacherTubeIE, TeacherTubeUserIE, TeachingChannelIE, TeamcocoIE, ConanClassicIE, TeamTreeHouseIE, TedEmbedIE, TedPlaylistIE, TedSeriesIE, TedTalkIE, Tele5IE, Tele13IE, TeleBruxellesIE, TelecaribePlayIE, TelecincoIE, MiTeleIE, TelegraafIE, TelegramEmbedIE, TeleMBIE, TelemundoIE, TeleQuebecIE, TeleQuebecSquatIE, TeleQuebecEmissionIE, TeleQuebecLiveIE, TeleQuebecVideoIE, TeleTaskIE, TelewebionIE, TempoIE, IVXPlayerIE, IflixEpisodeIE, IflixSeriesIE, VQQSeriesIE, VQQVideoIE, WeTvEpisodeIE, WeTvSeriesIE, TennisTVIE, TenPlayIE, TenPlaySeasonIE, TestURLIE, TF1IE, TFOIE, TheGuardianPodcastIE, TheGuardianPodcastPlaylistIE, TheHoleTvIE, TheInterceptIE, ThePlatformIE, AENetworksIE, AENetworksCollectionIE, AENetworksShowIE, HistoryTopicIE, HistoryPlayerIE, BiographyIE, AMCNetworksIE, NBCIE, NBCNewsIE, ThePlatformFeedIE, CBSIE, CorusIE, ParamountPlusIE, TheStarIE, TheSunIE, TheWeatherChannelIE, ThisAmericanLifeIE, ThisOldHouseIE, ThisVidIE, ThisVidMemberIE, ThisVidPlaylistIE, ThreeSpeakIE, ThreeSpeakUserIE, ThreeQSDNIE, TikTokIE, TikTokUserIE, TikTokSoundIE, TikTokEffectIE, TikTokTagIE, TikTokVMIE, TikTokLiveIE, DouyinIE, TMZIE, TNAFlixNetworkEmbedIE, TNAFlixIE, EMPFlixIE, MovieFapIE, ToggleIE, MeWatchIE, ToggoIE, TOnlineIE, ToonGogglesIE, TouTvIE, ToypicsUserIE, ToypicsIE, TrailerAddictIE, TrillerIE, TrillerUserIE, TrillerShortIE, TrovoIE, TrovoVodIE, TrovoChannelVodIE, TrovoChannelClipIE, TrtCocukVideoIE, TrtWorldIE, TrueIDIE, TruNewsIE, TruthIE, TruTVIE, Tube8IE, TubeTuGrazIE, TubeTuGrazSeriesIE, TubiTvIE, TubiTvShowIE, TumblrIE, TuneInStationIE, TuneInPodcastIE, TuneInPodcastEpisodeIE, TuneInShortenerIE, TV2IE, TV2ArticleIE, KatsomoIE, MTVUutisetArticleIE, TV24UAVideoIE, TV2DKIE, TV2DKBornholmPlayIE, TV2HuIE, TV2HuSeriesIE, TV4IE, TV5MondePlusIE, TV5UnisVideoIE, TV5UnisIE, TVAIE, QubIE, TVANouvellesIE, TVANouvellesArticleIE, TVCIE, TVCArticleIE, TVerIE, TvigleIE, TVIPlayerIE, TVLandIE, TVN24IE, TVNoeIE, TVOpenGrWatchIE, TVOpenGrEmbedIE, TVPEmbedIE, TVPIE, TVPStreamIE, TVPVODSeriesIE, TVPVODVideoIE, TVPlayIE, TVPlayHomeIE, TVPlayerIE, TweakersIE, TwentyMinutenIE, TwentyThreeVideoIE, TwitCastingIE, TwitCastingLiveIE, TwitCastingUserIE, TwitchVodIE, TwitchCollectionIE, TwitchVideosIE, TwitchVideosClipsIE, TwitchVideosCollectionsIE, TwitchStreamIE, TwitchClipsIE, TwitterCardIE, TwitterIE, TwitterAmplifyIE, TwitterBroadcastIE, TwitterSpacesIE, TwitterShortenerIE, TxxxIE, PornTopIE, UdemyIE, UdemyCourseIE, UDNEmbedIE, UFCTVIE, UFCArabiaIE, UkColumnIE, UKTVPlayIE, DigitekaIE, DLiveVODIE, DLiveStreamIE, DroobleIE, UMGDeIE, UnistraIE, UnityIE, KnownDRMIE, KnownPiracyIE, UOLIE, UplynkIE, UplynkPreplayIE, UrortIE, URPlayIE, USANetworkIE, USATodayIE, UstreamIE, UstreamChannelIE, UstudioIE, UstudioEmbedIE, UtreonIE, Varzesh3IE, Vbox7IE, VeoIE, VeohIE, VeohUserIE, VestiIE, VevoIE, VevoPlaylistIE, BTArticleIE, BTVestlendingenIE, VH1IE, ViceIE, ViceArticleIE, ViceShowIE, ViddlerIE, VideaIE, VideocampusSachsenIE, ViMPPlaylistIE, VideoDetectiveIE, VideofyMeIE, VideoKenIE, VideoKenPlayerIE, VideoKenPlaylistIE, VideoKenCategoryIE, VideoKenTopicIE, VideomoreIE, VideomoreVideoIE, VideomoreSeasonIE, VideoPressIE, VidioIE, VidioPremierIE, VidioLiveIE, VidLiiIE, VidlyIE, ViewLiftIE, ViewLiftEmbedIE, ViideaIE, VimeoIE, VimeoAlbumIE, VimeoChannelIE, VimeoGroupsIE, VimeoLikesIE, VimeoOndemandIE, VimeoProIE, VimeoReviewIE, VimeoUserIE, VimeoWatchLaterIE, VHXEmbedIE, VimmIE, VimmRecordingIE, VineIE, VineUserIE, VikiIE, VikiChannelIE, ViouslyIE, ViqeoIE, ViuIE, ViuPlaylistIE, ViuOTTIE, ViuOTTIndonesiaIE, VKIE, VKUserVideosIE, VKWallPostIE, VKPlayIE, VKPlayLiveIE, VocarooIE, VODPlIE, VODPlatformIE, VoicyIE, VoicyChannelIE, VolejTVIE, VootIE, VootSeriesIE, VoxMediaVolumeIE, VoxMediaIE, VRTIE, VrtNUIE, KetnetIE, DagelijkseKostIE, Radio1BeIE, VTMIE, MedialaanIE, VuClipIE, VVVVIDIE, VVVVIDShowIE, WallaIE, WashingtonPostIE, WashingtonPostArticleIE, WatIE, WDRIE, WDRPageIE, WDRElefantIE, WDRMobileIE, WebcameraplIE, WebcasterIE, WebcasterFeedIE, WebOfStoriesIE, WebOfStoriesPlaylistIE, WeiboIE, WeiboVideoIE, WeiboUserIE, WeiqiTVIE, WeverseIE, WeverseMediaIE, WeverseMomentIE, WeverseLiveTabIE, WeverseMediaTabIE, WeverseLiveIE, WeVidiIE, WeyyakIE, WhypIE, WikimediaIE, WimbledonIE, WimTVIE, WhoWatchIE, WistiaIE, WistiaPlaylistIE, WistiaChannelIE, WordpressPlaylistEmbedIE, WordpressMiniAudioPlayerEmbedIE, WorldStarHipHopIE, WPPilotIE, WPPilotChannelsIE, WrestleUniverseVODIE, WrestleUniversePPVIE, WSJIE, WSJArticleIE, WWEIE, WykopDigIE, WykopDigCommentIE, WykopPostIE, WykopPostCommentIE, XanimuIE, XboxClipsIE, XFileShareIE, XHamsterIE, XHamsterEmbedIE, XHamsterUserIE, XimalayaIE, XimalayaAlbumIE, XinpianchangIE, XMinusIE, XNXXIE, XstreamIE, VGTVIE, XVideosIE, XVideosQuickiesIE, XXXYMoviesIE, YahooIE, AolIE, YahooSearchIE, YahooJapanNewsIE, YandexDiskIE, YandexMusicTrackIE, YandexMusicAlbumIE, YandexMusicPlaylistIE, YandexMusicArtistTracksIE, YandexMusicArtistAlbumsIE, YandexVideoIE, YandexVideoPreviewIE, ZenYandexIE, ZenYandexChannelIE, YapFilesIE, YappyIE, YappyProfileIE, YleAreenaIE, YouJizzIE, YoukuIE, YoukuShowIE, YouNowLiveIE, YouNowChannelIE, YouNowMomentIE, YouPornIE, YourPornIE, YourUploadIE, ZaikoIE, ZaikoETicketIE, ZapiksIE, BBVTVIE, BBVTVLiveIE, BBVTVRecordingsIE, EinsUndEinsTVIE, EinsUndEinsTVLiveIE, EinsUndEinsTVRecordingsIE, EWETVIE, EWETVLiveIE, EWETVRecordingsIE, GlattvisionTVIE, GlattvisionTVLiveIE, GlattvisionTVRecordingsIE, MNetTVIE, MNetTVLiveIE, MNetTVRecordingsIE, NetPlusTVIE, NetPlusTVLiveIE, NetPlusTVRecordingsIE, OsnatelTVIE, OsnatelTVLiveIE, OsnatelTVRecordingsIE, QuantumTVIE, QuantumTVLiveIE, QuantumTVRecordingsIE, SaltTVIE, SaltTVLiveIE, SaltTVRecordingsIE, SAKTVIE, SAKTVLiveIE, SAKTVRecordingsIE, VTXTVIE, VTXTVLiveIE, VTXTVRecordingsIE, WalyTVIE, WalyTVLiveIE, WalyTVRecordingsIE, ZattooIE, ZattooLiveIE, ZattooMoviesIE, ZattooRecordingsIE, ZDFIE, DreiSatIE, ZDFChannelIE, Zee5IE, Zee5SeriesIE, ZeeNewsIE, ZenPornIE, ZetlandDKArticleIE, ZhihuIE, ZingMp3IE, ZingMp3AlbumIE, ZingMp3ChartHomeIE, ZingMp3WeekChartIE, ZingMp3ChartMusicVideoIE, ZingMp3UserIE, ZingMp3HubIE, ZingMp3LiveRadioIE, ZingMp3PodcastEpisodeIE, ZingMp3PodcastIE, ZoomIE, ZypeIE, GenericIE]
```

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/lbry.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/lbry.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/lci.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/lci.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/lcp.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/lcp.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/lecture2go.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/lecture2go.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/lecturio.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/lecturio.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/leeco.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/leeco.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/lefigaro.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/lefigaro.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/lego.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/lego.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/lemonde.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/lemonde.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/lenta.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/lenta.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/libraryofcongress.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/libraryofcongress.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/libsyn.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/libsyn.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/lifenews.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/lifenews.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/likee.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/likee.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/limelight.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/limelight.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/linkedin.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/linkedin.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/liputan6.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/liputan6.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/listennotes.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/listennotes.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/litv.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/litv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/livejournal.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/livejournal.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/livestream.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/livestream.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/livestreamfails.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/livestreamfails.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/lnkgo.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/lnkgo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/loom.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/loom.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/lovehomeporn.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/lovehomeporn.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/lrt.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/lrt.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/lsm.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/lsm.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/lumni.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/lumni.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/lynda.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/lynda.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/maariv.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/maariv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/magellantv.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/magellantv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/magentamusik.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/magentamusik.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/mailru.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/mailru.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/mainstreaming.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/mainstreaming.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/mangomolo.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/mangomolo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/manoto.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/manoto.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/manyvids.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/manyvids.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/maoritv.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/maoritv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/markiza.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/markiza.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/massengeschmacktv.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/massengeschmacktv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/masters.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/masters.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/matchtv.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/matchtv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/mbn.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/mbn.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/mdr.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/mdr.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/medaltv.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/medaltv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/mediaite.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/mediaite.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/mediaklikk.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/mediaklikk.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/medialaan.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/medialaan.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/mediaset.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/mediaset.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/mediasite.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/mediasite.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/mediastream.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/mediastream.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/mediaworksnz.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/mediaworksnz.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/medici.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/medici.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/megaphone.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/megaphone.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/megatvcom.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/megatvcom.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/meipai.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/meipai.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/melonvod.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/melonvod.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/metacritic.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/metacritic.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/mgtv.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/mgtv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/microsoftembed.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/microsoftembed.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/microsoftstream.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/microsoftstream.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/microsoftvirtualacademy.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/microsoftvirtualacademy.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/mildom.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/mildom.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/minds.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/minds.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/minoto.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/minoto.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/mirrativ.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/mirrativ.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/mirrorcouk.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/mirrorcouk.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/mit.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/mit.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/mitele.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/mitele.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/mixch.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/mixch.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/mixcloud.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/mixcloud.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/mlb.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/mlb.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/mlssoccer.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/mlssoccer.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/mocha.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/mocha.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/mojvideo.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/mojvideo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/monstercat.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/monstercat.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/motherless.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/motherless.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/motorsport.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/motorsport.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/moviepilot.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/moviepilot.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/moview.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/moview.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/moviezine.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/moviezine.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/movingimage.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/movingimage.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/msn.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/msn.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/mtv.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/mtv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/muenchentv.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/muenchentv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/murrtube.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/murrtube.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/museai.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/museai.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/musescore.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/musescore.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/musicdex.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/musicdex.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/mx3.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/mx3.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/mxplayer.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/mxplayer.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/myspace.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/myspace.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/myspass.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/myspass.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/myvideoge.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/myvideoge.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/myvidster.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/myvidster.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/mzaalo.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/mzaalo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/n1.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/n1.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/nate.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/nate.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/nationalgeographic.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/nationalgeographic.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/naver.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/naver.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/nba.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/nba.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/nbc.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/nbc.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ndr.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ndr.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ndtv.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ndtv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/nebula.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/nebula.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/nekohacker.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/nekohacker.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/nerdcubed.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/nerdcubed.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/neteasemusic.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/neteasemusic.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/netverse.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/netverse.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/netzkino.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/netzkino.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/newgrounds.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/newgrounds.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/newspicks.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/newspicks.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/newsy.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/newsy.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/nextmedia.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/nextmedia.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/nexx.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/nexx.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/nfb.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/nfb.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/nfhsnetwork.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/nfhsnetwork.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/nfl.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/nfl.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/nhk.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/nhk.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 from ..utils import (
     ExtractorError,
     clean_html,
     get_element_by_class,
     int_or_none,
     join_nonempty,
     parse_duration,
+    remove_end,
     traverse_obj,
     try_call,
     unescapeHTML,
     unified_timestamp,
     url_or_none,
     urljoin,
 )
 
 
 class NhkBaseIE(InfoExtractor):
     _API_URL_TEMPLATE = 'https://nwapi.nhk.jp/nhkworld/%sod%slist/v7b/%s/%s/%s/all%s.json'
-    _BASE_URL_REGEX = r'https?://www3\.nhk\.or\.jp/nhkworld/(?P<lang>[a-z]{2})/ondemand'
-    _TYPE_REGEX = r'/(?P<type>video|audio)/'
+    _BASE_URL_REGEX = r'https?://www3\.nhk\.or\.jp/nhkworld/(?P<lang>[a-z]{2})/'
 
     def _call_api(self, m_id, lang, is_video, is_episode, is_clip):
         return self._download_json(
             self._API_URL_TEMPLATE % (
                 'v' if is_video else 'r',
                 'clip' if is_clip else 'esd',
                 'episode' if is_episode else 'program',
@@ -79,15 +79,15 @@
                     'subtitles': subtitles,
                 }
         raise ExtractorError('Unable to extract stream url')
 
     def _extract_episode_info(self, url, episode=None):
         fetch_episode = episode is None
         lang, m_type, episode_id = NhkVodIE._match_valid_url(url).group('lang', 'type', 'id')
-        is_video = m_type == 'video'
+        is_video = m_type != 'audio'
 
         if is_video:
             episode_id = episode_id[:4] + '-' + episode_id[4:]
 
         if fetch_episode:
             episode = self._call_api(
                 episode_id, lang, is_video, True, episode_id[:4] == '9999')[0]
@@ -134,85 +134,87 @@
             info.update({
                 **self._extract_stream_info(vod_id),
                 'id': vod_id,
             })
 
         else:
             if fetch_episode:
-                audio_path = episode['audio']['audio']
+                # From https://www3.nhk.or.jp/nhkworld/common/player/radio/inline/rod.html
+                audio_path = remove_end(episode['audio']['audio'], '.m4a')
                 info['formats'] = self._extract_m3u8_formats(
-                    'https://nhkworld-vh.akamaihd.net/i%s/master.m3u8' % audio_path,
+                    f'{urljoin("https://vod-stream.nhk.jp", audio_path)}/index.m3u8',
                     episode_id, 'm4a', entry_protocol='m3u8_native',
                     m3u8_id='hls', fatal=False)
                 for f in info['formats']:
                     f['language'] = lang
             else:
                 info.update({
                     '_type': 'url_transparent',
                     'ie_key': NhkVodIE.ie_key(),
                     'url': url,
                 })
         return info
 
 
 class NhkVodIE(NhkBaseIE):
-    # the 7-character IDs can have alphabetic chars too: assume [a-z] rather than just [a-f], eg
-    _VALID_URL = [rf'{NhkBaseIE._BASE_URL_REGEX}/(?P<type>video)/(?P<id>[0-9a-z]+)',
-                  rf'{NhkBaseIE._BASE_URL_REGEX}/(?P<type>audio)/(?P<id>[^/?#]+?-\d{{8}}-[0-9a-z]+)']
+    _VALID_URL = [
+        rf'{NhkBaseIE._BASE_URL_REGEX}shows/(?:(?P<type>video)/)?(?P<id>\d{{4}}[\da-z]\d+)/?(?:$|[?#])',
+        rf'{NhkBaseIE._BASE_URL_REGEX}(?:ondemand|shows)/(?P<type>audio)/(?P<id>[^/?#]+?-\d{{8}}-[\da-z]+)',
+        rf'{NhkBaseIE._BASE_URL_REGEX}ondemand/(?P<type>video)/(?P<id>\d{{4}}[\da-z]\d+)',  # deprecated
+    ]
     # Content available only for a limited period of time. Visit
     # https://www3.nhk.or.jp/nhkworld/en/ondemand/ for working samples.
     _TESTS = [{
         'url': 'https://www3.nhk.or.jp/nhkworld/en/ondemand/video/2049126/',
         'info_dict': {
             'id': 'nw_vod_v_en_2049_126_20230413233000_01_1681398302',
             'ext': 'mp4',
             'title': 'Japan Railway Journal - The Tohoku Shinkansen: Full Speed Ahead',
             'description': 'md5:49f7c5b206e03868a2fdf0d0814b92f6',
-            'thumbnail': 'md5:51bcef4a21936e7fea1ff4e06353f463',
+            'thumbnail': r're:https://.+/.+\.jpg',
             'episode': 'The Tohoku Shinkansen: Full Speed Ahead',
             'series': 'Japan Railway Journal',
-            'modified_timestamp': 1694243656,
+            'modified_timestamp': 1707217907,
             'timestamp': 1681428600,
             'release_timestamp': 1693883728,
             'duration': 1679,
             'upload_date': '20230413',
-            'modified_date': '20230909',
+            'modified_date': '20240206',
             'release_date': '20230905',
-
         },
     }, {
         # video clip
         'url': 'https://www3.nhk.or.jp/nhkworld/en/ondemand/video/9999011/',
         'md5': '153c3016dfd252ba09726588149cf0e7',
         'info_dict': {
             'id': 'lpZXIwaDE6_Z-976CPsFdxyICyWUzlT5',
             'ext': 'mp4',
             'title': 'Dining with the Chef - Chef Saito\'s Family recipe: MENCHI-KATSU',
             'description': 'md5:5aee4a9f9d81c26281862382103b0ea5',
-            'thumbnail': 'md5:d6a4d9b6e9be90aaadda0bcce89631ed',
+            'thumbnail': r're:https://.+/.+\.jpg',
             'series': 'Dining with the Chef',
             'episode': 'Chef Saito\'s Family recipe: MENCHI-KATSU',
             'duration': 148,
             'upload_date': '20190816',
             'release_date': '20230902',
             'release_timestamp': 1693619292,
-            'modified_timestamp': 1694168033,
-            'modified_date': '20230908',
+            'modified_timestamp': 1707217907,
+            'modified_date': '20240206',
             'timestamp': 1565997540,
         },
     }, {
         # radio
         'url': 'https://www3.nhk.or.jp/nhkworld/en/ondemand/audio/livinginjapan-20231001-1/',
         'info_dict': {
             'id': 'livinginjapan-20231001-1-en',
             'ext': 'm4a',
             'title': 'Living in Japan - Tips for Travelers to Japan / Ramen Vending Machines',
             'series': 'Living in Japan',
             'description': 'md5:0a0e2077d8f07a03071e990a6f51bfab',
-            'thumbnail': 'md5:960622fb6e06054a4a1a0c97ea752545',
+            'thumbnail': r're:https://.+/.+\.jpg',
             'episode': 'Tips for Travelers to Japan / Ramen Vending Machines'
         },
     }, {
         'url': 'https://www3.nhk.or.jp/nhkworld/en/ondemand/video/2015173/',
         'only_matching': True,
     }, {
         'url': 'https://www3.nhk.or.jp/nhkworld/en/ondemand/audio/plugin-20190404-1/',
@@ -241,96 +243,210 @@
         'url': 'https://www3.nhk.or.jp/nhkworld/ja/ondemand/video/0020271111/',
         'info_dict': {
             'id': 'nw_ja_v_jvod_ohayou_20231008',
             'ext': 'mp4',
             'title': 'おはよう日本（7時台） - 10月8日放送',
             'series': 'おはよう日本（7時台）',
             'episode': '10月8日放送',
-            'thumbnail': 'md5:d733b1c8e965ab68fb02b2d347d0e9b4',
+            'thumbnail': r're:https://.+/.+\.jpg',
             'description': 'md5:9c1d6cbeadb827b955b20e99ab920ff0',
         },
         'skip': 'expires 2023-10-15',
     }, {
         # a one-off (single-episode series). title from the api is just '<p></p>'
         'url': 'https://www3.nhk.or.jp/nhkworld/en/ondemand/video/3004952/',
         'info_dict': {
             'id': 'nw_vod_v_en_3004_952_20230723091000_01_1690074552',
             'ext': 'mp4',
-            'title': 'Barakan Discovers AMAMI OSHIMA: Isson\'s Treasure Island',
+            'title': 'Barakan Discovers - AMAMI OSHIMA: Isson\'s Treasure Isla',
             'description': 'md5:5db620c46a0698451cc59add8816b797',
-            'thumbnail': 'md5:67d9ff28009ba379bfa85ad1aaa0e2bd',
+            'thumbnail': r're:https://.+/.+\.jpg',
             'release_date': '20230905',
             'timestamp': 1690103400,
             'duration': 2939,
             'release_timestamp': 1693898699,
-            'modified_timestamp': 1698057495,
-            'modified_date': '20231023',
             'upload_date': '20230723',
+            'modified_timestamp': 1707217907,
+            'modified_date': '20240206',
+            'episode': 'AMAMI OSHIMA: Isson\'s Treasure Isla',
+            'series': 'Barakan Discovers',
+        },
+    }, {
+        # /ondemand/video/ url with alphabetical character in 5th position of id
+        'url': 'https://www3.nhk.or.jp/nhkworld/en/ondemand/video/9999a07/',
+        'info_dict': {
+            'id': 'nw_c_en_9999-a07',
+            'ext': 'mp4',
+            'episode': 'Mini-Dramas on SDGs: Ep 1 Close the Gender Gap [Director\'s Cut]',
+            'series': 'Mini-Dramas on SDGs',
+            'modified_date': '20240206',
+            'title': 'Mini-Dramas on SDGs - Mini-Dramas on SDGs: Ep 1 Close the Gender Gap [Director\'s Cut]',
+            'description': 'md5:3f9dcb4db22fceb675d90448a040d3f6',
+            'timestamp': 1621962360,
+            'duration': 189,
+            'release_date': '20230903',
+            'modified_timestamp': 1707217907,
+            'upload_date': '20210525',
+            'thumbnail': r're:https://.+/.+\.jpg',
+            'release_timestamp': 1693713487,
+        },
+    }, {
+        'url': 'https://www3.nhk.or.jp/nhkworld/en/ondemand/video/9999d17/',
+        'info_dict': {
+            'id': 'nw_c_en_9999-d17',
+            'ext': 'mp4',
+            'title': 'Flowers of snow blossom - The 72 Pentads of Yamato',
+            'description': 'Today’s focus: Snow',
+            'release_timestamp': 1693792402,
+            'release_date': '20230904',
+            'upload_date': '20220128',
+            'timestamp': 1643370960,
+            'thumbnail': r're:https://.+/.+\.jpg',
+            'duration': 136,
+            'series': '',
+            'modified_date': '20240206',
+            'modified_timestamp': 1707217907,
+        },
+    }, {
+        # new /shows/ url format
+        'url': 'https://www3.nhk.or.jp/nhkworld/en/shows/2032307/',
+        'info_dict': {
+            'id': 'nw_vod_v_en_2032_307_20240321113000_01_1710990282',
+            'ext': 'mp4',
+            'title': 'Japanology Plus - 20th Anniversary Special Part 1',
+            'description': 'md5:817d41fc8e54339ad2a916161ea24faf',
+            'episode': '20th Anniversary Special Part 1',
+            'series': 'Japanology Plus',
+            'thumbnail': r're:https://.+/.+\.jpg',
+            'duration': 1680,
+            'timestamp': 1711020600,
+            'upload_date': '20240321',
+            'release_timestamp': 1711022683,
+            'release_date': '20240321',
+            'modified_timestamp': 1711031012,
+            'modified_date': '20240321',
+        },
+    }, {
+        'url': 'https://www3.nhk.or.jp/nhkworld/en/shows/3020025/',
+        'info_dict': {
+            'id': 'nw_vod_v_en_3020_025_20230325144000_01_1679723944',
+            'ext': 'mp4',
+            'title': '100 Ideas to Save the World - Working Styles Evolve',
+            'description': 'md5:9e6c7778eaaf4f7b4af83569649f84d9',
+            'episode': 'Working Styles Evolve',
+            'series': '100 Ideas to Save the World',
+            'thumbnail': r're:https://.+/.+\.jpg',
+            'duration': 899,
+            'upload_date': '20230325',
+            'timestamp': 1679755200,
+            'release_date': '20230905',
+            'release_timestamp': 1693880540,
+            'modified_date': '20240206',
+            'modified_timestamp': 1707217907,
         },
+    }, {
+        # new /shows/audio/ url format
+        'url': 'https://www3.nhk.or.jp/nhkworld/en/shows/audio/livinginjapan-20231001-1/',
+        'only_matching': True,
+    }, {
+        # valid url even if can't be found in wild; support needed for clip entries extraction
+        'url': 'https://www3.nhk.or.jp/nhkworld/en/shows/9999o80/',
+        'only_matching': True,
     }]
 
     def _real_extract(self, url):
         return self._extract_episode_info(url)
 
 
 class NhkVodProgramIE(NhkBaseIE):
-    _VALID_URL = rf'{NhkBaseIE._BASE_URL_REGEX}/program{NhkBaseIE._TYPE_REGEX}(?P<id>\w+)(?:.+?\btype=(?P<episode_type>clip|(?:radio|tv)Episode))?'
+    _VALID_URL = rf'''(?x)
+        {NhkBaseIE._BASE_URL_REGEX}(?:shows|tv)/
+        (?:(?P<type>audio)/programs/)?(?P<id>\w+)/?
+        (?:\?(?:[^#]+&)?type=(?P<episode_type>clip|(?:radio|tv)Episode))?'''
     _TESTS = [{
         # video program episodes
-        'url': 'https://www3.nhk.or.jp/nhkworld/en/ondemand/program/video/sumo',
+        'url': 'https://www3.nhk.or.jp/nhkworld/en/shows/sumo/',
         'info_dict': {
             'id': 'sumo',
             'title': 'GRAND SUMO Highlights',
             'description': 'md5:fc20d02dc6ce85e4b72e0273aa52fdbf',
         },
-        'playlist_mincount': 0,
+        'playlist_mincount': 1,
     }, {
-        'url': 'https://www3.nhk.or.jp/nhkworld/en/ondemand/program/video/japanrailway',
+        'url': 'https://www3.nhk.or.jp/nhkworld/en/shows/japanrailway/',
         'info_dict': {
             'id': 'japanrailway',
             'title': 'Japan Railway Journal',
             'description': 'md5:ea39d93af7d05835baadf10d1aae0e3f',
         },
         'playlist_mincount': 12,
     }, {
         # video program clips
-        'url': 'https://www3.nhk.or.jp/nhkworld/en/ondemand/program/video/japanrailway/?type=clip',
+        'url': 'https://www3.nhk.or.jp/nhkworld/en/shows/japanrailway/?type=clip',
         'info_dict': {
             'id': 'japanrailway',
             'title': 'Japan Railway Journal',
             'description': 'md5:ea39d93af7d05835baadf10d1aae0e3f',
         },
-        'playlist_mincount': 5,
-    }, {
-        'url': 'https://www3.nhk.or.jp/nhkworld/en/ondemand/program/video/10yearshayaomiyazaki/',
-        'only_matching': True,
+        'playlist_mincount': 12,
     }, {
         # audio program
-        'url': 'https://www3.nhk.or.jp/nhkworld/en/ondemand/program/audio/listener/',
+        'url': 'https://www3.nhk.or.jp/nhkworld/en/shows/audio/programs/livinginjapan/',
+        'info_dict': {
+            'id': 'livinginjapan',
+            'title': 'Living in Japan',
+            'description': 'md5:665bb36ec2a12c5a7f598ee713fc2b54',
+        },
+        'playlist_mincount': 12,
+    }, {
+        # /tv/ program url
+        'url': 'https://www3.nhk.or.jp/nhkworld/en/tv/designtalksplus/',
+        'info_dict': {
+            'id': 'designtalksplus',
+            'title': 'DESIGN TALKS plus',
+            'description': 'md5:47b3b3a9f10d4ac7b33b53b70a7d2837',
+        },
+        'playlist_mincount': 20,
+    }, {
+        'url': 'https://www3.nhk.or.jp/nhkworld/en/shows/10yearshayaomiyazaki/',
         'only_matching': True,
     }]
 
+    @classmethod
+    def suitable(cls, url):
+        return False if NhkVodIE.suitable(url) else super().suitable(url)
+
+    def _extract_meta_from_class_elements(self, class_values, html):
+        for class_value in class_values:
+            if value := clean_html(get_element_by_class(class_value, html)):
+                return value
+
     def _real_extract(self, url):
         lang, m_type, program_id, episode_type = self._match_valid_url(url).group('lang', 'type', 'id', 'episode_type')
         episodes = self._call_api(
-            program_id, lang, m_type == 'video', False, episode_type == 'clip')
+            program_id, lang, m_type != 'audio', False, episode_type == 'clip')
 
-        entries = []
-        for episode in episodes:
-            episode_path = episode.get('url')
-            if not episode_path:
-                continue
-            entries.append(self._extract_episode_info(
-                urljoin(url, episode_path), episode))
+        def entries():
+            for episode in episodes:
+                if episode_path := episode.get('url'):
+                    yield self._extract_episode_info(urljoin(url, episode_path), episode)
 
         html = self._download_webpage(url, program_id)
-        program_title = clean_html(get_element_by_class('p-programDetail__title', html))
-        program_description = clean_html(get_element_by_class('p-programDetail__text', html))
+        program_title = self._extract_meta_from_class_elements([
+            'p-programDetail__title',  # /ondemand/program/
+            'pProgramHero__logoText',  # /shows/
+            'tAudioProgramMain__title',  # /shows/audio/programs/
+            'p-program-name'], html)  # /tv/
+        program_description = self._extract_meta_from_class_elements([
+            'p-programDetail__text',  # /ondemand/program/
+            'pProgramHero__description',  # /shows/
+            'tAudioProgramMain__info',  # /shows/audio/programs/
+            'p-program-description'], html)  # /tv/
 
-        return self.playlist_result(entries, program_id, program_title, program_description)
+        return self.playlist_result(entries(), program_id, program_title, program_description)
 
 
 class NhkForSchoolBangumiIE(InfoExtractor):
     _VALID_URL = r'https?://www2\.nhk\.or\.jp/school/movie/(?P<type>bangumi|clip)\.cgi\?das_id=(?P<id>[a-zA-Z0-9_-]+)'
     _TESTS = [{
         'url': 'https://www2.nhk.or.jp/school/movie/bangumi.cgi?das_id=D0005150191_00000',
         'info_dict': {
```

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/nhl.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/nhl.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/nick.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/nick.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/niconico.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/niconico.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/niconicochannelplus.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/niconicochannelplus.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ninaprotocol.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ninaprotocol.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ninecninemedia.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ninecninemedia.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ninegag.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ninegag.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ninenews.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ninenews.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ninenow.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ninenow.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/nintendo.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/nintendo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/nitter.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/nitter.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/nobelprize.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/nobelprize.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/noice.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/noice.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/nonktube.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/nonktube.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/noodlemagazine.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/noodlemagazine.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/noovo.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/noovo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/nosnl.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/nosnl.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/nova.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/nova.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/novaplay.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/novaplay.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/nowness.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/nowness.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/noz.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/noz.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/npo.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/npo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/npr.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/npr.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/nrk.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/nrk.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/nrl.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/nrl.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ntvcojp.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ntvcojp.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ntvde.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ntvde.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ntvru.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ntvru.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/nubilesporn.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/nubilesporn.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/nuevo.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/nuevo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/nuum.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/nuum.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/nuvid.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/nuvid.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/nytimes.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/nytimes.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/nzherald.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/nzherald.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/nzonscreen.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/nzonscreen.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/nzz.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/nzz.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/odkmedia.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/odkmedia.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/odnoklassniki.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/odnoklassniki.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/oftv.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/oftv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/oktoberfesttv.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/oktoberfesttv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/olympics.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/olympics.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/on24.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/on24.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/once.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/once.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ondemandkorea.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ondemandkorea.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/onefootball.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/onefootball.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/onenewsnz.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/onenewsnz.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/oneplace.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/oneplace.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/onet.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/onet.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/onionstudios.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/onionstudios.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/opencast.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/opencast.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/openload.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/openload.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/openrec.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/openrec.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ora.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ora.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/orf.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/orf.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/outsidetv.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/outsidetv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/owncloud.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/owncloud.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/packtpub.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/packtpub.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/palcomp3.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/palcomp3.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/panopto.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/panopto.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/paramountplus.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/paramountplus.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/parler.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/parler.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/parlview.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/parlview.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/patreon.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/patreon.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,30 +88,32 @@
             'id': 'SU4fj_aEMVw',
             'ext': 'mp4',
             'title': 'I\'m on Patreon!',
             'uploader': 'TraciJHines',
             'thumbnail': 're:^https?://.*$',
             'upload_date': '20150211',
             'description': 'md5:8af6425f50bd46fbf29f3db0fc3a8364',
-            'uploader_id': 'TraciJHines',
+            'uploader_id': '@TraciHinesMusic',
             'categories': ['Entertainment'],
             'duration': 282,
             'view_count': int,
             'tags': 'count:39',
             'age_limit': 0,
             'channel': 'TraciJHines',
             'channel_url': 'https://www.youtube.com/channel/UCGLim4T2loE5rwCMdpCIPVg',
             'live_status': 'not_live',
             'like_count': int,
             'channel_id': 'UCGLim4T2loE5rwCMdpCIPVg',
             'availability': 'public',
             'channel_follower_count': int,
             'playable_in_embed': True,
-            'uploader_url': 'http://www.youtube.com/user/TraciJHines',
+            'uploader_url': 'https://www.youtube.com/@TraciHinesMusic',
             'comment_count': int,
+            'channel_is_verified': True,
+            'chapters': 'count:4',
         },
         'params': {
             'noplaylist': True,
             'skip_download': True,
         }
     }, {
         'url': 'https://www.patreon.com/posts/episode-166-of-743933',
@@ -172,14 +174,35 @@
             'channel_follower_count': int,
             'like_count': int,
             'timestamp': 1660052820,
             'tags': ['The Office', 'early access', 'uncut'],
             'uploader_url': 'https://www.patreon.com/thenormies',
         },
         'skip': 'Patron-only content',
+    }, {
+        # dead vimeo and embed URLs, need to extract post_file
+        'url': 'https://www.patreon.com/posts/hunter-x-hunter-34007913',
+        'info_dict': {
+            'id': '34007913',
+            'ext': 'mp4',
+            'title': 'Hunter x Hunter | Kurapika DESTROYS Uvogin!!!',
+            'like_count': int,
+            'uploader': 'YaBoyRoshi',
+            'timestamp': 1581636833,
+            'channel_url': 'https://www.patreon.com/yaboyroshi',
+            'thumbnail': r're:^https?://.*$',
+            'tags': ['Hunter x Hunter'],
+            'uploader_id': '14264111',
+            'comment_count': int,
+            'channel_follower_count': int,
+            'description': 'Kurapika is a walking cheat code!',
+            'upload_date': '20200213',
+            'channel_id': '2147162',
+            'uploader_url': 'https://www.patreon.com/yaboyroshi',
+        },
     }]
 
     def _real_extract(self, url):
         video_id = self._match_id(url)
         post = self._call_api(
             f'posts/{video_id}', video_id, query={
                 'fields[media]': 'download_url,mimetype,size_bytes',
@@ -246,28 +269,21 @@
 
         # handle Vimeo embeds
         if try_get(attributes, lambda x: x['embed']['provider']) == 'Vimeo':
             embed_html = try_get(attributes, lambda x: x['embed']['html'])
             v_url = url_or_none(compat_urllib_parse_unquote(
                 self._search_regex(r'(https(?:%3A%2F%2F|://)player\.vimeo\.com.+app_id(?:=|%3D)+\d+)', embed_html, 'vimeo url', fatal=False)))
             if v_url:
-                return {
-                    **info,
-                    '_type': 'url_transparent',
-                    'url': VimeoIE._smuggle_referrer(v_url, 'https://patreon.com'),
-                    'ie_key': 'Vimeo',
-                }
+                v_url = VimeoIE._smuggle_referrer(v_url, 'https://patreon.com')
+                if self._request_webpage(v_url, video_id, 'Checking Vimeo embed URL', fatal=False, errnote=False):
+                    return self.url_result(v_url, VimeoIE, url_transparent=True, **info)
 
         embed_url = try_get(attributes, lambda x: x['embed']['url'])
-        if embed_url:
-            return {
-                **info,
-                '_type': 'url',
-                'url': embed_url,
-            }
+        if embed_url and self._request_webpage(embed_url, video_id, 'Checking embed URL', fatal=False, errnote=False):
+            return self.url_result(embed_url, **info)
 
         post_file = traverse_obj(attributes, 'post_file')
         if post_file:
             name = post_file.get('name')
             ext = determine_ext(name)
             if ext in KNOWN_EXTENSIONS:
                 return {
```

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/pbs.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/pbs.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/pearvideo.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/pearvideo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/peekvids.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/peekvids.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/peertube.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/peertube.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/peertv.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/peertv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/peloton.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/peloton.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/performgroup.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/performgroup.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/periscope.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/periscope.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/pgatour.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/pgatour.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/philharmoniedeparis.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/philharmoniedeparis.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/phoenix.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/phoenix.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/photobucket.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/photobucket.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/piapro.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/piapro.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/piaulizaportal.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/piaulizaportal.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/picarto.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/picarto.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/piksel.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/piksel.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/pinkbike.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/pinkbike.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/pinterest.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/pinterest.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/pixivsketch.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/pixivsketch.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/pladform.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/pladform.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/planetmarathi.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/planetmarathi.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/platzi.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/platzi.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/playplustv.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/playplustv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/playsuisse.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/playsuisse.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/playtvak.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/playtvak.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/playwire.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/playwire.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/pluralsight.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/pluralsight.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/plutotv.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/plutotv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/podbayfm.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/podbayfm.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/podchaser.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/podchaser.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/podomatic.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/podomatic.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/pokemon.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/pokemon.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/pokergo.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/pokergo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/polsatgo.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/polsatgo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/polskieradio.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/polskieradio.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/popcorntimes.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/popcorntimes.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/popcorntv.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/popcorntv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/porn91.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/porn91.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/pornbox.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/pornbox.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/pornflip.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/pornflip.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/pornhub.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/pornhub.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/pornotube.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/pornotube.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/pornovoisines.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/pornovoisines.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/pornoxo.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/pornoxo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/pr0gramm.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/pr0gramm.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/prankcast.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/prankcast.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/premiershiprugby.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/premiershiprugby.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/presstv.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/presstv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/projectveritas.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/projectveritas.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/prosiebensat1.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/prosiebensat1.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/prx.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/prx.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/puhutv.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/puhutv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/puls4.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/puls4.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/pyvideo.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/pyvideo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/qdance.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/qdance.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/qingting.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/qingting.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/qqmusic.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/qqmusic.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/r7.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/r7.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/radiko.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/radiko.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/radiocanada.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/radiocanada.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/radiocomercial.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/radiocomercial.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/radiode.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/radiode.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/radiofrance.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/radiofrance.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/radiojavan.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/radiojavan.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/radiokapital.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/radiokapital.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/radiozet.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/radiozet.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/radlive.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/radlive.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/rai.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/rai.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/raywenderlich.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/raywenderlich.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/rbgtum.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/rbgtum.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/rcs.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/rcs.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/rcti.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/rcti.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/rds.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/rds.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/redbee.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/redbee.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/redbulltv.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/redbulltv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/reddit.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/reddit.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/redge.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/redge.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/redgifs.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/redgifs.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/redtube.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/redtube.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/rentv.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/rentv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/restudy.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/restudy.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/reuters.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/reuters.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/reverbnation.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/reverbnation.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/rheinmaintv.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/rheinmaintv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ridehome.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ridehome.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/rinsefm.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/rinsefm.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/rmcdecouverte.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/rmcdecouverte.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/rockstargames.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/rockstargames.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/rokfin.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/rokfin.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/roosterteeth.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/roosterteeth.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/rottentomatoes.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/rottentomatoes.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/rozhlas.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/rozhlas.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/rte.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/rte.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/rtl2.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/rtl2.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/rtlnl.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/rtlnl.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/rtnews.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/rtnews.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/rtp.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/rtp.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/rtrfm.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/rtrfm.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/rts.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/rts.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/rtvcplay.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/rtvcplay.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/rtve.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/rtve.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/rtvs.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/rtvs.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/rtvslo.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/rtvslo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/rudovideo.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/rudovideo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/rule34video.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/rule34video.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/rumble.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/rumble.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/rutube.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/rutube.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/rutv.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/rutv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ruutu.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ruutu.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ruv.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ruv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/s4c.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/s4c.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/safari.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/safari.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/saitosan.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/saitosan.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/samplefocus.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/samplefocus.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/sapo.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/sapo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/sbs.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/sbs.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/sbscokr.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/sbscokr.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/screen9.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/screen9.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/screencast.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/screencast.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/screencastify.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/screencastify.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/screencastomatic.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/screencastomatic.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/scrippsnetworks.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/scrippsnetworks.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/scrolller.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/scrolller.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/scte.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/scte.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/sejmpl.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/sejmpl.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/senalcolombia.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/senalcolombia.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/senategov.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/senategov.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/sendtonews.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/sendtonews.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/servus.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/servus.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/sevenplus.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/sevenplus.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/sexu.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/sexu.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/seznamzpravy.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/seznamzpravy.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/shahid.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/shahid.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/sharepoint.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/sharepoint.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/shemaroome.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/shemaroome.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/showroomlive.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/showroomlive.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/sibnet.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/sibnet.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/simplecast.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/simplecast.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/sina.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/sina.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/sixplay.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/sixplay.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/skeb.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/skeb.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/sky.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/sky.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/skyit.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/skyit.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/skylinewebcams.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/skylinewebcams.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/skynewsarabia.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/skynewsarabia.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/skynewsau.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/skynewsau.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/slideshare.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/slideshare.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/slideslive.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/slideslive.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/slutload.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/slutload.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/smotrim.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/smotrim.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/snotr.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/snotr.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/sohu.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/sohu.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/sonyliv.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/sonyliv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/soundcloud.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/soundcloud.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/soundgasm.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/soundgasm.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/southpark.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/southpark.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/sovietscloset.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/sovietscloset.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/spankbang.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/spankbang.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/spiegel.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/spiegel.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/spike.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/spike.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/sport5.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/sport5.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/sportbox.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/sportbox.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/sportdeutschland.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/sportdeutschland.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/spotify.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/spotify.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/spreaker.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/spreaker.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/springboardplatform.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/springboardplatform.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/sprout.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/sprout.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/srgssr.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/srgssr.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/srmediathek.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/srmediathek.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/stacommu.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/stacommu.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/stageplus.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/stageplus.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/stanfordoc.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/stanfordoc.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/startrek.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/startrek.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/startv.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/startv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/steam.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/steam.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/stitcher.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/stitcher.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/storyfire.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/storyfire.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/streamable.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/streamable.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/streamcz.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/streamcz.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/streetvoice.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/streetvoice.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/stretchinternet.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/stretchinternet.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/stripchat.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/stripchat.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/stv.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/stv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/substack.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/substack.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/sunporno.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/sunporno.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/sverigesradio.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/sverigesradio.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/svt.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/svt.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/swearnet.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/swearnet.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/syfy.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/syfy.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/syvdk.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/syvdk.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/sztvhu.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/sztvhu.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tagesschau.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tagesschau.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tass.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tass.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tbs.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tbs.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tbsjp.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tbsjp.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/teachable.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/teachable.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/teachertube.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/teachertube.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/teachingchannel.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/teachingchannel.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/teamcoco.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/teamcoco.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/teamtreehouse.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/teamtreehouse.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ted.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ted.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tele13.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tele13.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tele5.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tele5.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/telebruxelles.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/telebruxelles.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/telecaribe.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/telecaribe.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/telecinco.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/telecinco.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/telegraaf.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/telegraaf.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/telegram.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/telegram.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/telemb.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/telemb.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/telemundo.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/telemundo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/telequebec.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/telequebec.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/teletask.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/teletask.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/telewebion.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/telewebion.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tempo.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tempo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tencent.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tencent.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tennistv.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tennistv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tenplay.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tenplay.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/testurl.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/testurl.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tf1.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tf1.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tfo.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tfo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/theguardian.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/theguardian.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/theholetv.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/theholetv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/theintercept.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/theintercept.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/theplatform.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/theplatform.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/thestar.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/thestar.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/thesun.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/thesun.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/theweatherchannel.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/theweatherchannel.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/thisamericanlife.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/thisamericanlife.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/thisoldhouse.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/thisoldhouse.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/thisvid.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/thisvid.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/threeqsdn.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/threeqsdn.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/threespeak.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/threespeak.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tiktok.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tiktok.py`

 * *Files 0% similar despite different names*

```diff
@@ -151,14 +151,15 @@
             'residence': 'US',
             'app_language': 'en',
             'timezone_offset': '-14400',
             'host_abi': 'armeabi-v7a',
             'locale': 'en',
             'ac2': 'wifi5g',
             'uoo': '1',
+            'carrier_region': 'US',
             'op_region': 'US',
             'build_number': self._APP_INFO['app_version'],
             'region': 'US',
             'ts': int(time.time()),
             'iid': self._APP_INFO['iid'],
             'device_id': random.randint(7250000000000000000, 7351147085025500000),
             'openudid': ''.join(random.choices('0123456789abcdef', k=16)),
```

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tmz.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tmz.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tnaflix.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tnaflix.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/toggle.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/toggle.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/toggo.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/toggo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tonline.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tonline.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/toongoggles.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/toongoggles.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/toutv.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/toutv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/toypics.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/toypics.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/traileraddict.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/traileraddict.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/triller.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/triller.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/trovo.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/trovo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/trtcocuk.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/trtcocuk.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/trtworld.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/trtworld.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/trueid.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/trueid.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/trunews.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/trunews.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/truth.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/truth.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/trutv.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/trutv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tube8.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tube8.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tubetugraz.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tubetugraz.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tubitv.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tubitv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tumblr.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tumblr.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tunein.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tunein.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/turner.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/turner.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tv2.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tv2.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tv24ua.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tv24ua.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tv2dk.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tv2dk.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tv2hu.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tv2hu.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tv4.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tv4.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tv5mondeplus.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tv5mondeplus.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tv5unis.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tv5unis.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tva.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tva.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tvanouvelles.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tvanouvelles.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tvc.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tvc.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tver.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tver.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tvigle.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tvigle.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tviplayer.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tviplayer.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tvland.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tvland.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tvn24.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tvn24.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tvnoe.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tvnoe.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tvopengr.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tvopengr.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tvp.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tvp.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tvplay.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tvplay.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tvplayer.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tvplayer.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/tweakers.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/tweakers.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/twentymin.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/twentymin.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/twentythreevideo.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/twentythreevideo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/twitcasting.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/twitcasting.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/twitch.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/twitch.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/twitter.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/twitter.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/txxx.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/txxx.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/udemy.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/udemy.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/udn.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/udn.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ukcolumn.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ukcolumn.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/uktvplay.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/uktvplay.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/umg.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/umg.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/unistra.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/unistra.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/unity.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/unity.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/unsupported.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/unsupported.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/uol.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/uol.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/uplynk.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/uplynk.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/urort.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/urort.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/urplay.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/urplay.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/usanetwork.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/usanetwork.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/usatoday.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/usatoday.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ustream.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ustream.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ustudio.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ustudio.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/utreon.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/utreon.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/varzesh3.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/varzesh3.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/vbox7.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/vbox7.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/veo.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/veo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/veoh.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/veoh.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/vesti.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/vesti.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/vevo.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/vevo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/vgtv.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/vgtv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/vh1.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/vh1.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/vice.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/vice.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/viddler.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/viddler.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/videa.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/videa.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/videocampus_sachsen.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/videocampus_sachsen.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/videodetective.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/videodetective.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/videofyme.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/videofyme.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/videoken.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/videoken.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/videomore.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/videomore.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/videopress.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/videopress.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/vidio.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/vidio.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/vidlii.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/vidlii.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/vidly.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/vidly.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/viewlift.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/viewlift.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/viidea.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/viidea.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/viki.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/viki.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/vimeo.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/vimeo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/vimm.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/vimm.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/vine.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/vine.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/viously.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/viously.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/viqeo.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/viqeo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/viu.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/viu.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/vk.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/vk.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/vocaroo.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/vocaroo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/vodpl.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/vodpl.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/vodplatform.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/vodplatform.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/voicy.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/voicy.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/volejtv.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/volejtv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/voot.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/voot.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/voxmedia.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/voxmedia.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/vrt.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/vrt.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/vtm.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/vtm.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/vuclip.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/vuclip.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/vvvvid.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/vvvvid.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/walla.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/walla.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/washingtonpost.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/washingtonpost.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/wat.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/wat.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/wdr.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/wdr.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/webcamerapl.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/webcamerapl.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/webcaster.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/webcaster.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/webofstories.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/webofstories.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/weibo.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/weibo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/weiqitv.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/weiqitv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/weverse.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/weverse.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/wevidi.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/wevidi.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/weyyak.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/weyyak.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/whowatch.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/whowatch.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/whyp.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/whyp.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/wikimedia.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/wikimedia.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/wimbledon.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/wimbledon.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/wimtv.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/wimtv.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/wistia.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/wistia.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/wordpress.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/wordpress.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/worldstarhiphop.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/worldstarhiphop.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/wppilot.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/wppilot.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/wrestleuniverse.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/wrestleuniverse.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/wsj.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/wsj.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/wwe.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/xinpianchang.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,138 +1,92 @@
-import re
-
 from .common import InfoExtractor
-from ..compat import compat_str
 from ..utils import (
+    int_or_none,
+    str_or_none,
     try_get,
-    unescapeHTML,
+    update_url_query,
     url_or_none,
-    urljoin,
 )
 
 
-class WWEBaseIE(InfoExtractor):
-    _SUBTITLE_LANGS = {
-        'English': 'en',
-        'Deutsch': 'de',
-    }
-
-    def _extract_entry(self, data, url, video_id=None):
-        video_id = compat_str(video_id or data['nid'])
-        title = data['title']
-
-        formats = self._extract_m3u8_formats(
-            data['file'], video_id, 'mp4', entry_protocol='m3u8_native',
-            m3u8_id='hls')
-
-        description = data.get('description')
-        thumbnail = urljoin(url, data.get('image'))
-        series = data.get('show_name')
-        episode = data.get('episode_name')
-
-        subtitles = {}
-        tracks = data.get('tracks')
-        if isinstance(tracks, list):
-            for track in tracks:
-                if not isinstance(track, dict):
-                    continue
-                if track.get('kind') != 'captions':
-                    continue
-                track_file = url_or_none(track.get('file'))
-                if not track_file:
-                    continue
-                label = track.get('label')
-                lang = self._SUBTITLE_LANGS.get(label, label) or 'en'
-                subtitles.setdefault(lang, []).append({
-                    'url': track_file,
-                })
-
-        return {
-            'id': video_id,
-            'title': title,
-            'description': description,
-            'thumbnail': thumbnail,
-            'series': series,
-            'episode': episode,
-            'formats': formats,
-            'subtitles': subtitles,
-        }
-
-
-class WWEIE(WWEBaseIE):
-    _VALID_URL = r'https?://(?:[^/]+\.)?wwe\.com/(?:[^/]+/)*videos/(?P<id>[^/?#&]+)'
+class XinpianchangIE(InfoExtractor):
+    _WORKING = False
+    _VALID_URL = r'https?://www\.xinpianchang\.com/(?P<id>[^/]+?)(?:\D|$)'
+    IE_NAME = 'xinpianchang'
+    IE_DESC = 'xinpianchang.com'
     _TESTS = [{
-        'url': 'https://www.wwe.com/videos/daniel-bryan-vs-andrade-cien-almas-smackdown-live-sept-4-2018',
-        'md5': '92811c6a14bfc206f7a6a9c5d9140184',
+        'url': 'https://www.xinpianchang.com/a11766551',
         'info_dict': {
-            'id': '40048199',
+            'id': 'a11766551',
             'ext': 'mp4',
-            'title': 'Daniel Bryan vs. Andrade "Cien" Almas: SmackDown LIVE, Sept. 4, 2018',
-            'description': 'md5:2d7424dbc6755c61a0e649d2a8677f67',
-            'thumbnail': r're:^https?://.*\.jpg$',
-        }
+            'title': '北京2022冬奥会闭幕式再见短片-冰墩墩下班了',
+            'description': 'md5:4a730c10639a82190fabe921c0fa4b87',
+            'duration': 151,
+            'thumbnail': r're:^https?://oss-xpc0\.xpccdn\.com.+/assets/',
+            'uploader': '正时文创',
+            'uploader_id': '10357277',
+            'categories': ['宣传片', '国家城市', '广告', '其他'],
+            'tags': ['北京冬奥会', '冰墩墩', '再见', '告别', '冰墩墩哭了', '感动', '闭幕式', '熄火']
+        },
     }, {
-        'url': 'https://de.wwe.com/videos/gran-metalik-vs-tony-nese-wwe-205-live-sept-4-2018',
-        'only_matching': True,
-    }]
-
-    def _real_extract(self, url):
-        display_id = self._match_id(url)
-        webpage = self._download_webpage(url, display_id)
-
-        landing = self._parse_json(
-            self._html_search_regex(
-                r'(?s)Drupal\.settings\s*,\s*({.+?})\s*\)\s*;',
-                webpage, 'drupal settings'),
-            display_id)['WWEVideoLanding']
-
-        data = landing['initialVideo']['playlist'][0]
-        video_id = landing.get('initialVideoId')
-
-        info = self._extract_entry(data, url, video_id)
-        info['display_id'] = display_id
-        return info
-
-
-class WWEPlaylistIE(WWEBaseIE):
-    _VALID_URL = r'https?://(?:[^/]+\.)?wwe\.com/(?:[^/]+/)*(?P<id>[^/?#&]+)'
-    _TESTS = [{
-        'url': 'https://www.wwe.com/shows/raw/2018-11-12',
+        'url': 'https://www.xinpianchang.com/a11762904',
         'info_dict': {
-            'id': '2018-11-12',
+            'id': 'a11762904',
+            'ext': 'mp4',
+            'title': '冬奥会决胜时刻《法国派出三只鸡？》',
+            'description': 'md5:55cb139ef8f48f0c877932d1f196df8b',
+            'duration': 136,
+            'thumbnail': r're:^https?://oss-xpc0\.xpccdn\.com.+/assets/',
+            'uploader': '精品动画',
+            'uploader_id': '10858927',
+            'categories': ['动画', '三维CG'],
+            'tags': ['France Télévisions', '法国3台', '蠢萌', '冬奥会']
         },
-        'playlist_mincount': 11,
     }, {
-        'url': 'http://www.wwe.com/article/walk-the-prank-wwe-edition',
-        'only_matching': True,
-    }, {
-        'url': 'https://www.wwe.com/shows/wwenxt/article/matt-riddle-interview',
+        'url': 'https://www.xinpianchang.com/a11779743?from=IndexPick&part=%E7%BC%96%E8%BE%91%E7%B2%BE%E9%80%89&index=2',
         'only_matching': True,
     }]
 
-    @classmethod
-    def suitable(cls, url):
-        return False if WWEIE.suitable(url) else super(WWEPlaylistIE, cls).suitable(url)
-
     def _real_extract(self, url):
-        display_id = self._match_id(url)
-        webpage = self._download_webpage(url, display_id)
+        video_id = self._match_id(url)
+        webpage = self._download_webpage(url, video_id=video_id)
+        domain = self.find_value_with_regex(var='requireNewDomain', webpage=webpage)
+        vid = self.find_value_with_regex(var='vid', webpage=webpage)
+        app_key = self.find_value_with_regex(var='modeServerAppKey', webpage=webpage)
+        api = update_url_query(f'{domain}/mod/api/v2/media/{vid}', {'appKey': app_key})
+        data = self._download_json(api, video_id=video_id)['data']
+        formats, subtitles = [], {}
+        for k, v in data.get('resource').items():
+            if k in ('dash', 'hls'):
+                v_url = v.get('url')
+                if not v_url:
+                    continue
+                if k == 'dash':
+                    fmts, subs = self._extract_mpd_formats_and_subtitles(v_url, video_id=video_id)
+                elif k == 'hls':
+                    fmts, subs = self._extract_m3u8_formats_and_subtitles(v_url, video_id=video_id)
+                formats.extend(fmts)
+                subtitles = self._merge_subtitles(subtitles, subs)
+            elif k == 'progressive':
+                formats.extend([{
+                    'url': url_or_none(prog.get('url')),
+                    'width': int_or_none(prog.get('width')),
+                    'height': int_or_none(prog.get('height')),
+                    'ext': 'mp4',
+                } for prog in v if prog.get('url') or []])
 
-        entries = []
-        for mobj in re.finditer(
-                r'data-video\s*=\s*(["\'])(?P<data>{.+?})\1', webpage):
-            video = self._parse_json(
-                mobj.group('data'), display_id, transform_source=unescapeHTML,
-                fatal=False)
-            if not video:
-                continue
-            data = try_get(video, lambda x: x['playlist'][0], dict)
-            if not data:
-                continue
-            try:
-                entry = self._extract_entry(data, url)
-            except Exception:
-                continue
-            entry['extractor_key'] = WWEIE.ie_key()
-            entries.append(entry)
+        return {
+            'id': video_id,
+            'title': data.get('title'),
+            'description': data.get('description'),
+            'duration': int_or_none(data.get('duration')),
+            'categories': data.get('categories'),
+            'tags': data.get('keywords'),
+            'thumbnail': data.get('cover'),
+            'uploader': try_get(data, lambda x: x['owner']['username']),
+            'uploader_id': str_or_none(try_get(data, lambda x: x['owner']['id'])),
+            'formats': formats,
+            'subtitles': subtitles,
+        }
 
-        return self.playlist_result(entries, display_id)
+    def find_value_with_regex(self, var, webpage):
+        return self._search_regex(rf'var\s{var}\s=\s\"(?P<vid>[^\"]+)\"', webpage, name=var)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/wykop.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/wykop.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/xanimu.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/xanimu.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/xboxclips.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/xboxclips.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/xfileshare.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/xfileshare.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/xhamster.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/xhamster.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/ximalaya.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/ximalaya.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/xinpianchang.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/xstream.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,92 +1,115 @@
+import re
+
 from .common import InfoExtractor
 from ..utils import (
     int_or_none,
-    str_or_none,
-    try_get,
-    update_url_query,
-    url_or_none,
+    parse_iso8601,
+    xpath_with_ns,
+    xpath_text,
+    find_xpath_attr,
 )
 
 
-class XinpianchangIE(InfoExtractor):
-    _WORKING = False
-    _VALID_URL = r'https?://www\.xinpianchang\.com/(?P<id>[^/]+?)(?:\D|$)'
-    IE_NAME = 'xinpianchang'
-    IE_DESC = 'xinpianchang.com'
+class XstreamIE(InfoExtractor):
+    _VALID_URL = r'''(?x)
+                    (?:
+                        xstream:|
+                        https?://frontend\.xstream\.(?:dk|net)/
+                    )
+                    (?P<partner_id>[^/]+)
+                    (?:
+                        :|
+                        /feed/video/\?.*?\bid=
+                    )
+                    (?P<id>\d+)
+                    '''
     _TESTS = [{
-        'url': 'https://www.xinpianchang.com/a11766551',
-        'info_dict': {
-            'id': 'a11766551',
-            'ext': 'mp4',
-            'title': '北京2022冬奥会闭幕式再见短片-冰墩墩下班了',
-            'description': 'md5:4a730c10639a82190fabe921c0fa4b87',
-            'duration': 151,
-            'thumbnail': r're:^https?://oss-xpc0\.xpccdn\.com.+/assets/',
-            'uploader': '正时文创',
-            'uploader_id': '10357277',
-            'categories': ['宣传片', '国家城市', '广告', '其他'],
-            'tags': ['北京冬奥会', '冰墩墩', '再见', '告别', '冰墩墩哭了', '感动', '闭幕式', '熄火']
-        },
-    }, {
-        'url': 'https://www.xinpianchang.com/a11762904',
+        'url': 'http://frontend.xstream.dk/btno/feed/video/?platform=web&id=86588',
+        'md5': 'd7d17e3337dc80de6d3a540aefbe441b',
         'info_dict': {
-            'id': 'a11762904',
-            'ext': 'mp4',
-            'title': '冬奥会决胜时刻《法国派出三只鸡？》',
-            'description': 'md5:55cb139ef8f48f0c877932d1f196df8b',
-            'duration': 136,
-            'thumbnail': r're:^https?://oss-xpc0\.xpccdn\.com.+/assets/',
-            'uploader': '精品动画',
-            'uploader_id': '10858927',
-            'categories': ['动画', '三维CG'],
-            'tags': ['France Télévisions', '法国3台', '蠢萌', '冬奥会']
+            'id': '86588',
+            'ext': 'mov',
+            'title': 'Otto Wollertsen',
+            'description': 'Vestlendingen Otto Fredrik Wollertsen',
+            'timestamp': 1430473209,
+            'upload_date': '20150501',
         },
     }, {
-        'url': 'https://www.xinpianchang.com/a11779743?from=IndexPick&part=%E7%BC%96%E8%BE%91%E7%B2%BE%E9%80%89&index=2',
+        'url': 'http://frontend.xstream.dk/ap/feed/video/?platform=web&id=21039',
         'only_matching': True,
     }]
 
-    def _real_extract(self, url):
-        video_id = self._match_id(url)
-        webpage = self._download_webpage(url, video_id=video_id)
-        domain = self.find_value_with_regex(var='requireNewDomain', webpage=webpage)
-        vid = self.find_value_with_regex(var='vid', webpage=webpage)
-        app_key = self.find_value_with_regex(var='modeServerAppKey', webpage=webpage)
-        api = update_url_query(f'{domain}/mod/api/v2/media/{vid}', {'appKey': app_key})
-        data = self._download_json(api, video_id=video_id)['data']
-        formats, subtitles = [], {}
-        for k, v in data.get('resource').items():
-            if k in ('dash', 'hls'):
-                v_url = v.get('url')
-                if not v_url:
-                    continue
-                if k == 'dash':
-                    fmts, subs = self._extract_mpd_formats_and_subtitles(v_url, video_id=video_id)
-                elif k == 'hls':
-                    fmts, subs = self._extract_m3u8_formats_and_subtitles(v_url, video_id=video_id)
-                formats.extend(fmts)
-                subtitles = self._merge_subtitles(subtitles, subs)
-            elif k == 'progressive':
-                formats.extend([{
-                    'url': url_or_none(prog.get('url')),
-                    'width': int_or_none(prog.get('width')),
-                    'height': int_or_none(prog.get('height')),
-                    'ext': 'mp4',
-                } for prog in v if prog.get('url') or []])
+    def _extract_video_info(self, partner_id, video_id):
+        data = self._download_xml(
+            'http://frontend.xstream.dk/%s/feed/video/?platform=web&id=%s'
+            % (partner_id, video_id),
+            video_id)
+
+        NS_MAP = {
+            'atom': 'http://www.w3.org/2005/Atom',
+            'xt': 'http://xstream.dk/',
+            'media': 'http://search.yahoo.com/mrss/',
+        }
+
+        entry = data.find(xpath_with_ns('./atom:entry', NS_MAP))
+
+        title = xpath_text(
+            entry, xpath_with_ns('./atom:title', NS_MAP), 'title')
+        description = xpath_text(
+            entry, xpath_with_ns('./atom:summary', NS_MAP), 'description')
+        timestamp = parse_iso8601(xpath_text(
+            entry, xpath_with_ns('./atom:published', NS_MAP), 'upload date'))
+
+        formats = []
+        media_group = entry.find(xpath_with_ns('./media:group', NS_MAP))
+        for media_content in media_group.findall(xpath_with_ns('./media:content', NS_MAP)):
+            media_url = media_content.get('url')
+            if not media_url:
+                continue
+            tbr = int_or_none(media_content.get('bitrate'))
+            mobj = re.search(r'^(?P<url>rtmp://[^/]+/(?P<app>[^/]+))/(?P<playpath>.+)$', media_url)
+            if mobj:
+                formats.append({
+                    'url': mobj.group('url'),
+                    'play_path': 'mp4:%s' % mobj.group('playpath'),
+                    'app': mobj.group('app'),
+                    'ext': 'flv',
+                    'tbr': tbr,
+                    'format_id': 'rtmp-%d' % tbr,
+                })
+            else:
+                formats.append({
+                    'url': media_url,
+                    'tbr': tbr,
+                })
+
+        link = find_xpath_attr(
+            entry, xpath_with_ns('./atom:link', NS_MAP), 'rel', 'original')
+        if link is not None:
+            formats.append({
+                'url': link.get('href'),
+                'format_id': link.get('rel'),
+                'quality': 1,
+            })
+
+        thumbnails = [{
+            'url': splash.get('url'),
+            'width': int_or_none(splash.get('width')),
+            'height': int_or_none(splash.get('height')),
+        } for splash in media_group.findall(xpath_with_ns('./xt:splash', NS_MAP))]
 
         return {
             'id': video_id,
-            'title': data.get('title'),
-            'description': data.get('description'),
-            'duration': int_or_none(data.get('duration')),
-            'categories': data.get('categories'),
-            'tags': data.get('keywords'),
-            'thumbnail': data.get('cover'),
-            'uploader': try_get(data, lambda x: x['owner']['username']),
-            'uploader_id': str_or_none(try_get(data, lambda x: x['owner']['id'])),
+            'title': title,
+            'description': description,
+            'timestamp': timestamp,
             'formats': formats,
-            'subtitles': subtitles,
+            'thumbnails': thumbnails,
         }
 
-    def find_value_with_regex(self, var, webpage):
-        return self._search_regex(rf'var\s{var}\s=\s\"(?P<vid>[^\"]+)\"', webpage, name=var)
+    def _real_extract(self, url):
+        mobj = self._match_valid_url(url)
+        partner_id = mobj.group('partner_id')
+        video_id = mobj.group('id')
+
+        return self._extract_video_info(partner_id, video_id)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/xminus.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/xminus.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/xnxx.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/xnxx.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/xvideos.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/xvideos.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/xxxymovies.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/xxxymovies.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/yahoo.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/yahoo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/yandexdisk.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/yandexdisk.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/yandexmusic.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/yandexmusic.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/yandexvideo.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/yandexvideo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/yapfiles.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/yapfiles.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/yappy.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/yappy.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/yle_areena.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/yle_areena.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/youjizz.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/youjizz.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/youku.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/youku.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/younow.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/younow.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/youporn.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/youporn.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/yourporn.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/yourporn.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/yourupload.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/yourupload.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/youtube.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/youtube.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/zaiko.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/zaiko.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/zapiks.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/zapiks.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/zattoo.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/zattoo.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/zdf.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/zdf.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/zee5.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/zee5.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/zeenews.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/zeenews.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/zenporn.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/zenporn.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/zetland.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/zetland.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/zhihu.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/zhihu.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/zingmp3.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/zingmp3.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/zoom.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/zoom.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/extractor/zype.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/extractor/zype.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/networking/__init__.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/networking/__init__.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/networking/_curlcffi.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/networking/_curlcffi.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/networking/_helper.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/networking/_helper.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/networking/_requests.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/networking/_requests.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/networking/_urllib.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/networking/_urllib.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/networking/_websockets.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/networking/_websockets.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/networking/common.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/networking/common.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/networking/exceptions.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/networking/exceptions.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/networking/impersonate.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/networking/impersonate.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/postprocessor/__init__.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/postprocessor/__init__.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/postprocessor/common.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/postprocessor/common.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/postprocessor/embedthumbnail.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/postprocessor/embedthumbnail.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/postprocessor/exec.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/postprocessor/exec.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/postprocessor/ffmpeg.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/postprocessor/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/postprocessor/metadataparser.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/postprocessor/metadataparser.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/postprocessor/modify_chapters.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/postprocessor/modify_chapters.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/postprocessor/movefilesafterdownload.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/postprocessor/movefilesafterdownload.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/postprocessor/sponskrub.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/postprocessor/sponskrub.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/postprocessor/sponsorblock.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/postprocessor/sponsorblock.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/postprocessor/xattrpp.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/postprocessor/xattrpp.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/utils/_deprecated.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/utils/_deprecated.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/utils/_legacy.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/utils/_legacy.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/utils/_utils.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/utils/_utils.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/utils/networking.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/utils/networking.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/utils/progress.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/utils/progress.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/yt_dlp/utils/traversal.py` & `yt_dlp-2024.4.7.232657.dev0/yt_dlp/utils/traversal.py`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/.gitignore` & `yt_dlp-2024.4.7.232657.dev0/.gitignore`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/AUTHORS` & `yt_dlp-2024.4.7.232657.dev0/AUTHORS`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/LICENSE` & `yt_dlp-2024.4.7.232657.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/README.md` & `yt_dlp-2024.4.7.232657.dev0/README.md`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/pyproject.toml` & `yt_dlp-2024.4.7.232657.dev0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `yt_dlp-2024.4.6.232655.dev0/PKG-INFO` & `yt_dlp-2024.4.7.232657.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 330a 4e61 6d65 3a20 7974 2d64  : 2.3.Name: yt-d
 00000020: 6c70 0a56 6572 7369 6f6e 3a20 3230 3234  lp.Version: 2024
-00000030: 2e34 2e36 2e32 3332 3635 352e 6465 7630  .4.6.232655.dev0
+00000030: 2e34 2e37 2e32 3332 3635 372e 6465 7630  .4.7.232657.dev0
 00000040: 0a53 756d 6d61 7279 3a20 4120 6665 6174  .Summary: A feat
 00000050: 7572 652d 7269 6368 2063 6f6d 6d61 6e64  ure-rich command
 00000060: 2d6c 696e 6520 6175 6469 6f2f 7669 6465  -line audio/vide
 00000070: 6f20 646f 776e 6c6f 6164 6572 0a50 726f  o downloader.Pro
 00000080: 6a65 6374 2d55 524c 3a20 446f 6375 6d65  ject-URL: Docume
 00000090: 6e74 6174 696f 6e2c 2068 7474 7073 3a2f  ntation, https:/
 000000a0: 2f67 6974 6875 622e 636f 6d2f 7974 2d64  /github.com/yt-d
```

