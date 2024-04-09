# Comparing `tmp/gzspidertools-0.0.8.tar.gz` & `tmp/gzspidertools-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gzspidertools-0.0.8.tar", max compression
+gzip compressed data, was "gzspidertools-0.0.9.tar", max compression
```

## Comparing `gzspidertools-0.0.8.tar` & `gzspidertools-0.0.9.tar`

### file list

```diff
@@ -1,100 +1,100 @@
--rw-r--r--   0        0        0      463 2024-02-23 03:50:46.199860 gzspidertools-0.0.8/gzspidertools/__init__.py
--rw-r--r--   0        0        0        0 2024-02-21 08:35:30.075886 gzspidertools-0.0.8/gzspidertools/commands/__init__.py
--rw-r--r--   0        0        0       84 2024-02-21 08:35:30.075886 gzspidertools-0.0.8/gzspidertools/commands/crawl.py
--rw-r--r--   0        0        0      340 2024-02-21 15:31:53.542253 gzspidertools-0.0.8/gzspidertools/commands/genspider.py
--rw-r--r--   0        0        0     3868 2024-02-23 03:45:17.690705 gzspidertools-0.0.8/gzspidertools/commands/startproject.py
--rw-r--r--   0        0        0      272 2024-02-21 15:48:10.983633 gzspidertools-0.0.8/gzspidertools/commands/version.py
--rw-r--r--   0        0        0        0 2024-02-21 08:35:30.078883 gzspidertools-0.0.8/gzspidertools/common/__init__.py
--rw-r--r--   0        0        0     2502 2024-02-21 15:31:53.640233 gzspidertools-0.0.8/gzspidertools/common/encryption.py
--rw-r--r--   0        0        0    10541 2024-02-21 15:31:53.686204 gzspidertools-0.0.8/gzspidertools/common/expend.py
--rw-r--r--   0        0        0     6031 2024-02-21 15:31:53.490204 gzspidertools-0.0.8/gzspidertools/common/mongodbpipe.py
--rw-r--r--   0        0        0    19881 2024-02-21 15:31:52.979206 gzspidertools-0.0.8/gzspidertools/common/multiplexing.py
--rw-r--r--   0        0        0    10538 2024-02-21 15:31:53.969208 gzspidertools-0.0.8/gzspidertools/common/mysqlerrhandle.py
--rw-r--r--   0        0        0    30778 2024-02-21 08:35:30.082854 gzspidertools-0.0.8/gzspidertools/common/params.py
--rw-r--r--   0        0        0     4806 2024-02-21 15:31:52.738209 gzspidertools-0.0.8/gzspidertools/common/postgreserrhandle.py
--rw-r--r--   0        0        0    13530 2024-02-21 15:31:54.016233 gzspidertools-0.0.8/gzspidertools/common/spiderconf.py
--rw-r--r--   0        0        0     3710 2024-02-21 08:35:30.083883 gzspidertools-0.0.8/gzspidertools/common/sqlformat.py
--rw-r--r--   0        0        0     5366 2024-02-21 08:35:30.083883 gzspidertools-0.0.8/gzspidertools/common/typevars.py
--rw-r--r--   0        0        0    12159 2024-02-21 15:31:53.662233 gzspidertools-0.0.8/gzspidertools/common/utils.py
--rw-r--r--   0        0        0      376 2024-02-21 08:35:30.084883 gzspidertools-0.0.8/gzspidertools/config.py
--rw-r--r--   0        0        0       69 2024-02-21 08:35:30.085879 gzspidertools-0.0.8/gzspidertools/extras/__init__.py
--rw-r--r--   0        0        0    16619 2024-02-21 15:31:54.216205 gzspidertools-0.0.8/gzspidertools/extras/cvnpil.py
--rw-r--r--   0        0        0     2005 2024-02-21 15:31:53.692204 gzspidertools-0.0.8/gzspidertools/extras/ext.py
--rw-r--r--   0        0        0     2216 2024-02-21 15:31:53.672203 gzspidertools-0.0.8/gzspidertools/extras/oss.py
--rw-r--r--   0        0        0     7242 2024-02-21 08:35:30.087884 gzspidertools-0.0.8/gzspidertools/formatdata.py
--rw-r--r--   0        0        0     5590 2024-02-21 15:31:52.805205 gzspidertools-0.0.8/gzspidertools/items.py
--rw-r--r--   0        0        0      660 2024-02-21 15:31:52.729204 gzspidertools-0.0.8/gzspidertools/middlewares.py
--rw-r--r--   0        0        0     4028 2024-02-21 15:31:53.223213 gzspidertools-0.0.8/gzspidertools/mongoclient.py
--rw-r--r--   0        0        0     1132 2024-02-21 08:35:30.089883 gzspidertools-0.0.8/gzspidertools/mysqlclient.py
--rw-r--r--   0        0        0     2130 2024-02-21 15:31:53.231206 gzspidertools-0.0.8/gzspidertools/pipelines.py
--rw-r--r--   0        0        0      203 2024-02-21 15:31:54.148272 gzspidertools-0.0.8/gzspidertools/request.py
--rw-r--r--   0        0        0        0 2024-02-21 08:35:30.091885 gzspidertools-0.0.8/gzspidertools/scraper/__init__.py
--rw-r--r--   0        0        0      203 2024-02-21 15:31:52.878204 gzspidertools-0.0.8/gzspidertools/scraper/http/__init__.py
--rw-r--r--   0        0        0     1556 2024-02-21 15:31:53.291206 gzspidertools-0.0.8/gzspidertools/scraper/http/request/__init__.py
--rw-r--r--   0        0        0     1137 2024-02-21 15:31:54.209203 gzspidertools-0.0.8/gzspidertools/scraper/http/request/form.py
--rw-r--r--   0        0        0      808 2024-02-21 15:31:53.699207 gzspidertools-0.0.8/gzspidertools/scraper/middlewares/__init__.py
--rw-r--r--   0        0        0        0 2024-02-21 08:35:30.095883 gzspidertools-0.0.8/gzspidertools/scraper/middlewares/headers/__init__.py
--rw-r--r--   0        0        0     1678 2024-02-21 15:31:53.562203 gzspidertools-0.0.8/gzspidertools/scraper/middlewares/headers/ua.py
--rw-r--r--   0        0        0      158 2024-02-21 15:31:53.948213 gzspidertools-0.0.8/gzspidertools/scraper/middlewares/netlib/__init__.py
--rw-r--r--   0        0        0    10137 2024-02-21 15:31:53.887208 gzspidertools-0.0.8/gzspidertools/scraper/middlewares/netlib/aiohttplib.py
--rw-r--r--   0        0        0      402 2024-02-21 15:31:53.047204 gzspidertools-0.0.8/gzspidertools/scraper/middlewares/proxy/__init__.py
--rw-r--r--   0        0        0     3602 2024-02-21 15:31:54.289205 gzspidertools-0.0.8/gzspidertools/scraper/middlewares/proxy/dynamic.py
--rw-r--r--   0        0        0     2417 2024-02-21 08:35:30.099878 gzspidertools-0.0.8/gzspidertools/scraper/middlewares/proxy/exclusive.py
--rw-r--r--   0        0        0     2288 2024-02-21 15:31:53.278205 gzspidertools-0.0.8/gzspidertools/scraper/pipelines/__init__.py
--rw-r--r--   0        0        0        0 2024-02-21 08:35:30.101882 gzspidertools-0.0.8/gzspidertools/scraper/pipelines/download/__init__.py
--rw-r--r--   0        0        0     2971 2024-02-21 15:31:52.820203 gzspidertools-0.0.8/gzspidertools/scraper/pipelines/download/file.py
--rw-r--r--   0        0        0     2259 2024-02-21 15:31:53.582235 gzspidertools-0.0.8/gzspidertools/scraper/pipelines/es/__init__.py
--rw-r--r--   0        0        0     2927 2024-02-21 15:31:52.913204 gzspidertools-0.0.8/gzspidertools/scraper/pipelines/es/asynced.py
--rw-r--r--   0        0        0      149 2024-02-21 15:31:52.956207 gzspidertools-0.0.8/gzspidertools/scraper/pipelines/es/fantasy.py
--rw-r--r--   0        0        0        0 2024-02-21 08:35:30.104882 gzspidertools-0.0.8/gzspidertools/scraper/pipelines/mongo/__init__.py
--rw-r--r--   0        0        0     1620 2024-02-21 15:31:54.271204 gzspidertools-0.0.8/gzspidertools/scraper/pipelines/mongo/asynced.py
--rw-r--r--   0        0        0     1498 2024-02-21 15:31:53.961203 gzspidertools-0.0.8/gzspidertools/scraper/pipelines/mongo/fantasy.py
--rw-r--r--   0        0        0      910 2024-02-21 15:31:53.416207 gzspidertools-0.0.8/gzspidertools/scraper/pipelines/mongo/twisted.py
--rw-r--r--   0        0        0      150 2024-02-21 08:35:30.107884 gzspidertools-0.0.8/gzspidertools/scraper/pipelines/msgproducer/__init__.py
--rw-r--r--   0        0        0     3130 2024-02-21 15:31:53.313205 gzspidertools-0.0.8/gzspidertools/scraper/pipelines/msgproducer/kafkapub.py
--rw-r--r--   0        0        0     2092 2024-02-21 15:31:54.249208 gzspidertools-0.0.8/gzspidertools/scraper/pipelines/msgproducer/mqpub.py
--rw-r--r--   0        0        0     2645 2024-02-21 15:31:53.427205 gzspidertools-0.0.8/gzspidertools/scraper/pipelines/mysql/__init__.py
--rw-r--r--   0        0        0     2319 2024-02-21 15:31:53.481203 gzspidertools-0.0.8/gzspidertools/scraper/pipelines/mysql/asynced.py
--rw-r--r--   0        0        0      164 2024-02-21 15:31:54.181209 gzspidertools-0.0.8/gzspidertools/scraper/pipelines/mysql/fantasy.py
--rw-r--r--   0        0        0     7055 2024-02-21 15:31:52.624209 gzspidertools-0.0.8/gzspidertools/scraper/pipelines/mysql/stats.py
--rw-r--r--   0        0        0     2376 2024-02-21 15:31:53.635233 gzspidertools-0.0.8/gzspidertools/scraper/pipelines/mysql/turbo.py
--rw-r--r--   0        0        0     3096 2024-02-21 15:31:53.341217 gzspidertools-0.0.8/gzspidertools/scraper/pipelines/mysql/twisted.py
--rw-r--r--   0        0        0     1402 2024-02-21 15:31:53.981205 gzspidertools-0.0.8/gzspidertools/scraper/pipelines/oracle/__init__.py
--rw-r--r--   0        0        0      169 2024-02-21 15:31:53.831210 gzspidertools-0.0.8/gzspidertools/scraper/pipelines/oracle/fantasy.py
--rw-r--r--   0        0        0     2229 2024-02-21 15:31:54.202257 gzspidertools-0.0.8/gzspidertools/scraper/pipelines/oracle/twisted.py
--rw-r--r--   0        0        0        0 2024-02-21 08:35:30.114883 gzspidertools-0.0.8/gzspidertools/scraper/pipelines/oss/__init__.py
--rw-r--r--   0        0        0     2760 2024-02-21 15:31:52.637205 gzspidertools-0.0.8/gzspidertools/scraper/pipelines/oss/ali.py
--rw-r--r--   0        0        0     2140 2024-02-21 15:31:53.360206 gzspidertools-0.0.8/gzspidertools/scraper/pipelines/postgres/__init__.py
--rw-r--r--   0        0        0     1995 2024-02-21 15:31:53.241209 gzspidertools-0.0.8/gzspidertools/scraper/pipelines/postgres/asynced.py
--rw-r--r--   0        0        0      179 2024-02-21 15:31:54.087210 gzspidertools-0.0.8/gzspidertools/scraper/pipelines/postgres/fantasy.py
--rw-r--r--   0        0        0     2874 2024-02-21 15:31:52.892208 gzspidertools-0.0.8/gzspidertools/scraper/pipelines/postgres/twisted.py
--rw-r--r--   0        0        0     6164 2024-02-21 15:31:54.194203 gzspidertools-0.0.8/gzspidertools/scraper/spiders/__init__.py
--rw-r--r--   0        0        0      333 2024-02-21 15:31:53.179206 gzspidertools-0.0.8/gzspidertools/scraper/spiders/crawl.py
--rw-r--r--   0        0        0      176 2024-02-21 15:31:53.797234 gzspidertools-0.0.8/gzspidertools/spiders.py
--rw-r--r--   0        0        0        0 2024-02-21 08:35:30.120856 gzspidertools-0.0.8/gzspidertools/templates/project/module/__init__.py
--rw-r--r--   0        0        0      282 2024-02-21 08:35:30.121883 gzspidertools-0.0.8/gzspidertools/templates/project/module/items.py.tmpl
--rw-r--r--   0        0        0     3765 2024-02-21 08:35:30.121883 gzspidertools-0.0.8/gzspidertools/templates/project/module/middlewares.py.tmpl
--rw-r--r--   0        0        0      381 2024-02-21 08:35:30.122883 gzspidertools-0.0.8/gzspidertools/templates/project/module/pipelines.py.tmpl
--rw-r--r--   0        0        0       87 2024-02-21 08:35:30.122883 gzspidertools-0.0.8/gzspidertools/templates/project/module/run.py.tmpl
--rw-r--r--   0        0        0      164 2024-02-21 08:35:30.123882 gzspidertools-0.0.8/gzspidertools/templates/project/module/run.sh.tmpl
--rw-r--r--   0        0        0     1113 2024-02-21 08:35:30.123882 gzspidertools-0.0.8/gzspidertools/templates/project/module/settings.py.tmpl
--rw-r--r--   0        0        0      165 2024-02-21 08:35:30.124883 gzspidertools-0.0.8/gzspidertools/templates/project/module/spiders/__init__.py
--rw-r--r--   0        0        0     5519 2024-02-21 15:48:10.747624 gzspidertools-0.0.8/gzspidertools/templates/project/module/VIT/.conf
--rw-r--r--   0        0        0       67 2024-02-21 08:35:30.125880 gzspidertools-0.0.8/gzspidertools/templates/project/pyproject.toml
--rw-r--r--   0        0        0      133 2024-02-23 03:11:20.437318 gzspidertools-0.0.8/gzspidertools/templates/project/README.md
--rw-r--r--   0        0        0        0 2024-02-21 08:35:30.193490 gzspidertools-0.0.8/gzspidertools/templates/project/requirements.txt
--rw-r--r--   0        0        0      284 2024-02-21 08:35:30.194484 gzspidertools-0.0.8/gzspidertools/templates/project/scrapy.cfg
--rw-r--r--   0        0        0    18012 2024-02-22 14:23:01.132000 gzspidertools-0.0.8/gzspidertools/templates/project/scrapy_redis-0.7.3-py2.py3-none-any.whl
--rw-r--r--   0        0        0     1391 2024-02-21 15:48:11.117622 gzspidertools-0.0.8/gzspidertools/templates/spiders/async.tmpl
--rw-r--r--   0        0        0     4371 2024-02-22 06:08:00.756821 gzspidertools-0.0.8/gzspidertools/templates/spiders/basic.tmpl
--rw-r--r--   0        0        0     1255 2024-02-21 15:48:10.911623 gzspidertools-0.0.8/gzspidertools/templates/spiders/crawl.tmpl
--rw-r--r--   0        0        0      565 2024-02-21 08:35:30.197483 gzspidertools-0.0.8/gzspidertools/templates/spiders/csvfeed.tmpl
--rw-r--r--   0        0        0     5483 2024-02-23 03:45:04.860042 gzspidertools-0.0.8/gzspidertools/templates/spiders/sr.tmpl
--rw-r--r--   0        0        0      559 2024-02-21 08:35:30.197483 gzspidertools-0.0.8/gzspidertools/templates/spiders/xmlfeed.tmpl
--rw-r--r--   0        0        0        0 2024-02-21 08:35:30.198483 gzspidertools-0.0.8/gzspidertools/utils/__init__.py
--rw-r--r--   0        0        0     6024 2024-02-22 06:29:33.478836 gzspidertools-0.0.8/gzspidertools/utils/cmdline.py
--rw-r--r--   0        0        0     3077 2024-02-22 06:56:49.258000 gzspidertools-0.0.8/gzspidertools/utils/text_verification.py
--rw-r--r--   0        0        0     1091 2024-02-21 08:35:30.069878 gzspidertools-0.0.8/LICENSE
--rw-r--r--   0        0        0     4503 2024-02-23 03:50:46.219140 gzspidertools-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1278 2024-02-23 03:47:42.228442 gzspidertools-0.0.8/README.md
--rw-r--r--   0        0        0     3743 1970-01-01 00:00:00.000000 gzspidertools-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      463 2024-02-23 04:06:56.428979 gzspidertools-0.0.9/gzspidertools/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-21 08:35:30.075886 gzspidertools-0.0.9/gzspidertools/commands/__init__.py
+-rw-r--r--   0        0        0       84 2024-02-21 08:35:30.075886 gzspidertools-0.0.9/gzspidertools/commands/crawl.py
+-rw-r--r--   0        0        0      340 2024-02-21 15:31:53.542253 gzspidertools-0.0.9/gzspidertools/commands/genspider.py
+-rw-r--r--   0        0        0     3868 2024-02-23 03:45:17.690705 gzspidertools-0.0.9/gzspidertools/commands/startproject.py
+-rw-r--r--   0        0        0      272 2024-02-21 15:48:10.983633 gzspidertools-0.0.9/gzspidertools/commands/version.py
+-rw-r--r--   0        0        0        0 2024-02-21 08:35:30.078883 gzspidertools-0.0.9/gzspidertools/common/__init__.py
+-rw-r--r--   0        0        0     2502 2024-02-21 15:31:53.640233 gzspidertools-0.0.9/gzspidertools/common/encryption.py
+-rw-r--r--   0        0        0    10541 2024-02-21 15:31:53.686204 gzspidertools-0.0.9/gzspidertools/common/expend.py
+-rw-r--r--   0        0        0     6031 2024-02-21 15:31:53.490204 gzspidertools-0.0.9/gzspidertools/common/mongodbpipe.py
+-rw-r--r--   0        0        0    19881 2024-02-21 15:31:52.979206 gzspidertools-0.0.9/gzspidertools/common/multiplexing.py
+-rw-r--r--   0        0        0    10538 2024-02-21 15:31:53.969208 gzspidertools-0.0.9/gzspidertools/common/mysqlerrhandle.py
+-rw-r--r--   0        0        0    30778 2024-02-21 08:35:30.082854 gzspidertools-0.0.9/gzspidertools/common/params.py
+-rw-r--r--   0        0        0     4806 2024-02-21 15:31:52.738209 gzspidertools-0.0.9/gzspidertools/common/postgreserrhandle.py
+-rw-r--r--   0        0        0    13530 2024-02-21 15:31:54.016233 gzspidertools-0.0.9/gzspidertools/common/spiderconf.py
+-rw-r--r--   0        0        0     3710 2024-02-21 08:35:30.083883 gzspidertools-0.0.9/gzspidertools/common/sqlformat.py
+-rw-r--r--   0        0        0     5366 2024-02-21 08:35:30.083883 gzspidertools-0.0.9/gzspidertools/common/typevars.py
+-rw-r--r--   0        0        0    12159 2024-02-21 15:31:53.662233 gzspidertools-0.0.9/gzspidertools/common/utils.py
+-rw-r--r--   0        0        0      376 2024-02-21 08:35:30.084883 gzspidertools-0.0.9/gzspidertools/config.py
+-rw-r--r--   0        0        0       69 2024-02-21 08:35:30.085879 gzspidertools-0.0.9/gzspidertools/extras/__init__.py
+-rw-r--r--   0        0        0    16619 2024-02-21 15:31:54.216205 gzspidertools-0.0.9/gzspidertools/extras/cvnpil.py
+-rw-r--r--   0        0        0     2005 2024-02-21 15:31:53.692204 gzspidertools-0.0.9/gzspidertools/extras/ext.py
+-rw-r--r--   0        0        0     2216 2024-02-21 15:31:53.672203 gzspidertools-0.0.9/gzspidertools/extras/oss.py
+-rw-r--r--   0        0        0     7242 2024-02-21 08:35:30.087884 gzspidertools-0.0.9/gzspidertools/formatdata.py
+-rw-r--r--   0        0        0     5590 2024-02-21 15:31:52.805205 gzspidertools-0.0.9/gzspidertools/items.py
+-rw-r--r--   0        0        0      660 2024-02-21 15:31:52.729204 gzspidertools-0.0.9/gzspidertools/middlewares.py
+-rw-r--r--   0        0        0     4028 2024-02-21 15:31:53.223213 gzspidertools-0.0.9/gzspidertools/mongoclient.py
+-rw-r--r--   0        0        0     1132 2024-02-21 08:35:30.089883 gzspidertools-0.0.9/gzspidertools/mysqlclient.py
+-rw-r--r--   0        0        0     2130 2024-02-21 15:31:53.231206 gzspidertools-0.0.9/gzspidertools/pipelines.py
+-rw-r--r--   0        0        0      203 2024-02-21 15:31:54.148272 gzspidertools-0.0.9/gzspidertools/request.py
+-rw-r--r--   0        0        0        0 2024-02-21 08:35:30.091885 gzspidertools-0.0.9/gzspidertools/scraper/__init__.py
+-rw-r--r--   0        0        0      203 2024-02-21 15:31:52.878204 gzspidertools-0.0.9/gzspidertools/scraper/http/__init__.py
+-rw-r--r--   0        0        0     1556 2024-02-21 15:31:53.291206 gzspidertools-0.0.9/gzspidertools/scraper/http/request/__init__.py
+-rw-r--r--   0        0        0     1137 2024-02-21 15:31:54.209203 gzspidertools-0.0.9/gzspidertools/scraper/http/request/form.py
+-rw-r--r--   0        0        0      808 2024-02-21 15:31:53.699207 gzspidertools-0.0.9/gzspidertools/scraper/middlewares/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-21 08:35:30.095883 gzspidertools-0.0.9/gzspidertools/scraper/middlewares/headers/__init__.py
+-rw-r--r--   0        0        0     1678 2024-02-21 15:31:53.562203 gzspidertools-0.0.9/gzspidertools/scraper/middlewares/headers/ua.py
+-rw-r--r--   0        0        0      158 2024-02-21 15:31:53.948213 gzspidertools-0.0.9/gzspidertools/scraper/middlewares/netlib/__init__.py
+-rw-r--r--   0        0        0    10137 2024-02-21 15:31:53.887208 gzspidertools-0.0.9/gzspidertools/scraper/middlewares/netlib/aiohttplib.py
+-rw-r--r--   0        0        0      402 2024-02-21 15:31:53.047204 gzspidertools-0.0.9/gzspidertools/scraper/middlewares/proxy/__init__.py
+-rw-r--r--   0        0        0     3602 2024-02-21 15:31:54.289205 gzspidertools-0.0.9/gzspidertools/scraper/middlewares/proxy/dynamic.py
+-rw-r--r--   0        0        0     2417 2024-02-21 08:35:30.099878 gzspidertools-0.0.9/gzspidertools/scraper/middlewares/proxy/exclusive.py
+-rw-r--r--   0        0        0     2288 2024-02-21 15:31:53.278205 gzspidertools-0.0.9/gzspidertools/scraper/pipelines/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-21 08:35:30.101882 gzspidertools-0.0.9/gzspidertools/scraper/pipelines/download/__init__.py
+-rw-r--r--   0        0        0     2971 2024-02-21 15:31:52.820203 gzspidertools-0.0.9/gzspidertools/scraper/pipelines/download/file.py
+-rw-r--r--   0        0        0     2259 2024-02-21 15:31:53.582235 gzspidertools-0.0.9/gzspidertools/scraper/pipelines/es/__init__.py
+-rw-r--r--   0        0        0     2927 2024-02-21 15:31:52.913204 gzspidertools-0.0.9/gzspidertools/scraper/pipelines/es/asynced.py
+-rw-r--r--   0        0        0      149 2024-02-21 15:31:52.956207 gzspidertools-0.0.9/gzspidertools/scraper/pipelines/es/fantasy.py
+-rw-r--r--   0        0        0        0 2024-02-21 08:35:30.104882 gzspidertools-0.0.9/gzspidertools/scraper/pipelines/mongo/__init__.py
+-rw-r--r--   0        0        0     1620 2024-02-21 15:31:54.271204 gzspidertools-0.0.9/gzspidertools/scraper/pipelines/mongo/asynced.py
+-rw-r--r--   0        0        0     1498 2024-02-21 15:31:53.961203 gzspidertools-0.0.9/gzspidertools/scraper/pipelines/mongo/fantasy.py
+-rw-r--r--   0        0        0      910 2024-02-21 15:31:53.416207 gzspidertools-0.0.9/gzspidertools/scraper/pipelines/mongo/twisted.py
+-rw-r--r--   0        0        0      150 2024-02-21 08:35:30.107884 gzspidertools-0.0.9/gzspidertools/scraper/pipelines/msgproducer/__init__.py
+-rw-r--r--   0        0        0     3130 2024-02-21 15:31:53.313205 gzspidertools-0.0.9/gzspidertools/scraper/pipelines/msgproducer/kafkapub.py
+-rw-r--r--   0        0        0     2092 2024-02-21 15:31:54.249208 gzspidertools-0.0.9/gzspidertools/scraper/pipelines/msgproducer/mqpub.py
+-rw-r--r--   0        0        0     2645 2024-02-21 15:31:53.427205 gzspidertools-0.0.9/gzspidertools/scraper/pipelines/mysql/__init__.py
+-rw-r--r--   0        0        0     2319 2024-02-21 15:31:53.481203 gzspidertools-0.0.9/gzspidertools/scraper/pipelines/mysql/asynced.py
+-rw-r--r--   0        0        0      164 2024-02-21 15:31:54.181209 gzspidertools-0.0.9/gzspidertools/scraper/pipelines/mysql/fantasy.py
+-rw-r--r--   0        0        0     7055 2024-02-21 15:31:52.624209 gzspidertools-0.0.9/gzspidertools/scraper/pipelines/mysql/stats.py
+-rw-r--r--   0        0        0     2376 2024-02-21 15:31:53.635233 gzspidertools-0.0.9/gzspidertools/scraper/pipelines/mysql/turbo.py
+-rw-r--r--   0        0        0     3096 2024-02-21 15:31:53.341217 gzspidertools-0.0.9/gzspidertools/scraper/pipelines/mysql/twisted.py
+-rw-r--r--   0        0        0     1402 2024-02-21 15:31:53.981205 gzspidertools-0.0.9/gzspidertools/scraper/pipelines/oracle/__init__.py
+-rw-r--r--   0        0        0      169 2024-02-21 15:31:53.831210 gzspidertools-0.0.9/gzspidertools/scraper/pipelines/oracle/fantasy.py
+-rw-r--r--   0        0        0     2229 2024-02-21 15:31:54.202257 gzspidertools-0.0.9/gzspidertools/scraper/pipelines/oracle/twisted.py
+-rw-r--r--   0        0        0        0 2024-02-21 08:35:30.114883 gzspidertools-0.0.9/gzspidertools/scraper/pipelines/oss/__init__.py
+-rw-r--r--   0        0        0     2760 2024-02-21 15:31:52.637205 gzspidertools-0.0.9/gzspidertools/scraper/pipelines/oss/ali.py
+-rw-r--r--   0        0        0     2140 2024-02-21 15:31:53.360206 gzspidertools-0.0.9/gzspidertools/scraper/pipelines/postgres/__init__.py
+-rw-r--r--   0        0        0     1995 2024-02-21 15:31:53.241209 gzspidertools-0.0.9/gzspidertools/scraper/pipelines/postgres/asynced.py
+-rw-r--r--   0        0        0      179 2024-02-21 15:31:54.087210 gzspidertools-0.0.9/gzspidertools/scraper/pipelines/postgres/fantasy.py
+-rw-r--r--   0        0        0     2874 2024-02-21 15:31:52.892208 gzspidertools-0.0.9/gzspidertools/scraper/pipelines/postgres/twisted.py
+-rw-r--r--   0        0        0     6164 2024-02-21 15:31:54.194203 gzspidertools-0.0.9/gzspidertools/scraper/spiders/__init__.py
+-rw-r--r--   0        0        0      333 2024-02-21 15:31:53.179206 gzspidertools-0.0.9/gzspidertools/scraper/spiders/crawl.py
+-rw-r--r--   0        0        0      176 2024-02-21 15:31:53.797234 gzspidertools-0.0.9/gzspidertools/spiders.py
+-rw-r--r--   0        0        0        0 2024-02-21 08:35:30.120856 gzspidertools-0.0.9/gzspidertools/templates/project/module/__init__.py
+-rw-r--r--   0        0        0      282 2024-02-21 08:35:30.121883 gzspidertools-0.0.9/gzspidertools/templates/project/module/items.py.tmpl
+-rw-r--r--   0        0        0     3765 2024-02-21 08:35:30.121883 gzspidertools-0.0.9/gzspidertools/templates/project/module/middlewares.py.tmpl
+-rw-r--r--   0        0        0      381 2024-02-21 08:35:30.122883 gzspidertools-0.0.9/gzspidertools/templates/project/module/pipelines.py.tmpl
+-rw-r--r--   0        0        0       87 2024-02-21 08:35:30.122883 gzspidertools-0.0.9/gzspidertools/templates/project/module/run.py.tmpl
+-rw-r--r--   0        0        0      164 2024-02-21 08:35:30.123882 gzspidertools-0.0.9/gzspidertools/templates/project/module/run.sh.tmpl
+-rw-r--r--   0        0        0     1113 2024-02-21 08:35:30.123882 gzspidertools-0.0.9/gzspidertools/templates/project/module/settings.py.tmpl
+-rw-r--r--   0        0        0      165 2024-02-21 08:35:30.124883 gzspidertools-0.0.9/gzspidertools/templates/project/module/spiders/__init__.py
+-rw-r--r--   0        0        0     5519 2024-02-21 15:48:10.747624 gzspidertools-0.0.9/gzspidertools/templates/project/module/VIT/.conf
+-rw-r--r--   0        0        0       67 2024-02-21 08:35:30.125880 gzspidertools-0.0.9/gzspidertools/templates/project/pyproject.toml
+-rw-r--r--   0        0        0      133 2024-02-23 03:11:20.437318 gzspidertools-0.0.9/gzspidertools/templates/project/README.md
+-rw-r--r--   0        0        0        0 2024-02-21 08:35:30.193490 gzspidertools-0.0.9/gzspidertools/templates/project/requirements.txt
+-rw-r--r--   0        0        0      284 2024-02-21 08:35:30.194484 gzspidertools-0.0.9/gzspidertools/templates/project/scrapy.cfg
+-rw-r--r--   0        0        0    18012 2024-02-22 14:23:01.132000 gzspidertools-0.0.9/gzspidertools/templates/project/scrapy_redis-0.7.3-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     1391 2024-02-21 15:48:11.117622 gzspidertools-0.0.9/gzspidertools/templates/spiders/async.tmpl
+-rw-r--r--   0        0        0     4371 2024-02-22 06:08:00.756821 gzspidertools-0.0.9/gzspidertools/templates/spiders/basic.tmpl
+-rw-r--r--   0        0        0     1255 2024-02-21 15:48:10.911623 gzspidertools-0.0.9/gzspidertools/templates/spiders/crawl.tmpl
+-rw-r--r--   0        0        0      565 2024-02-21 08:35:30.197483 gzspidertools-0.0.9/gzspidertools/templates/spiders/csvfeed.tmpl
+-rw-r--r--   0        0        0     5482 2024-02-23 04:03:45.136692 gzspidertools-0.0.9/gzspidertools/templates/spiders/sr.tmpl
+-rw-r--r--   0        0        0      559 2024-02-21 08:35:30.197483 gzspidertools-0.0.9/gzspidertools/templates/spiders/xmlfeed.tmpl
+-rw-r--r--   0        0        0        0 2024-02-21 08:35:30.198483 gzspidertools-0.0.9/gzspidertools/utils/__init__.py
+-rw-r--r--   0        0        0     6024 2024-02-22 06:29:33.478836 gzspidertools-0.0.9/gzspidertools/utils/cmdline.py
+-rw-r--r--   0        0        0     3077 2024-02-22 06:56:49.258000 gzspidertools-0.0.9/gzspidertools/utils/text_verification.py
+-rw-r--r--   0        0        0     1091 2024-02-21 08:35:30.069878 gzspidertools-0.0.9/LICENSE
+-rw-r--r--   0        0        0     4503 2024-02-23 04:06:56.434923 gzspidertools-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1284 2024-02-23 04:02:23.775262 gzspidertools-0.0.9/README.md
+-rw-r--r--   0        0        0     3749 1970-01-01 00:00:00.000000 gzspidertools-0.0.9/PKG-INFO
```

### Comparing `gzspidertools-0.0.8/gzspidertools/commands/startproject.py` & `gzspidertools-0.0.9/gzspidertools/commands/startproject.py`

 * *Files identical despite different names*

### Comparing `gzspidertools-0.0.8/gzspidertools/common/encryption.py` & `gzspidertools-0.0.9/gzspidertools/common/encryption.py`

 * *Files identical despite different names*

### Comparing `gzspidertools-0.0.8/gzspidertools/common/expend.py` & `gzspidertools-0.0.9/gzspidertools/common/expend.py`

 * *Files identical despite different names*

### Comparing `gzspidertools-0.0.8/gzspidertools/common/mongodbpipe.py` & `gzspidertools-0.0.9/gzspidertools/common/mongodbpipe.py`

 * *Files identical despite different names*

### Comparing `gzspidertools-0.0.8/gzspidertools/common/multiplexing.py` & `gzspidertools-0.0.9/gzspidertools/common/multiplexing.py`

 * *Files identical despite different names*

### Comparing `gzspidertools-0.0.8/gzspidertools/common/mysqlerrhandle.py` & `gzspidertools-0.0.9/gzspidertools/common/mysqlerrhandle.py`

 * *Files identical despite different names*

### Comparing `gzspidertools-0.0.8/gzspidertools/common/params.py` & `gzspidertools-0.0.9/gzspidertools/common/params.py`

 * *Files identical despite different names*

### Comparing `gzspidertools-0.0.8/gzspidertools/common/postgreserrhandle.py` & `gzspidertools-0.0.9/gzspidertools/common/postgreserrhandle.py`

 * *Files identical despite different names*

### Comparing `gzspidertools-0.0.8/gzspidertools/common/spiderconf.py` & `gzspidertools-0.0.9/gzspidertools/common/spiderconf.py`

 * *Files identical despite different names*

### Comparing `gzspidertools-0.0.8/gzspidertools/common/sqlformat.py` & `gzspidertools-0.0.9/gzspidertools/common/sqlformat.py`

 * *Files identical despite different names*

### Comparing `gzspidertools-0.0.8/gzspidertools/common/typevars.py` & `gzspidertools-0.0.9/gzspidertools/common/typevars.py`

 * *Files identical despite different names*

### Comparing `gzspidertools-0.0.8/gzspidertools/common/utils.py` & `gzspidertools-0.0.9/gzspidertools/common/utils.py`

 * *Files identical despite different names*

### Comparing `gzspidertools-0.0.8/gzspidertools/extras/cvnpil.py` & `gzspidertools-0.0.9/gzspidertools/extras/cvnpil.py`

 * *Files identical despite different names*

### Comparing `gzspidertools-0.0.8/gzspidertools/extras/ext.py` & `gzspidertools-0.0.9/gzspidertools/extras/ext.py`

 * *Files identical despite different names*

### Comparing `gzspidertools-0.0.8/gzspidertools/extras/oss.py` & `gzspidertools-0.0.9/gzspidertools/extras/oss.py`

 * *Files identical despite different names*

### Comparing `gzspidertools-0.0.8/gzspidertools/formatdata.py` & `gzspidertools-0.0.9/gzspidertools/formatdata.py`

 * *Files identical despite different names*

### Comparing `gzspidertools-0.0.8/gzspidertools/items.py` & `gzspidertools-0.0.9/gzspidertools/items.py`

 * *Files identical despite different names*

### Comparing `gzspidertools-0.0.8/gzspidertools/middlewares.py` & `gzspidertools-0.0.9/gzspidertools/middlewares.py`

 * *Files identical despite different names*

### Comparing `gzspidertools-0.0.8/gzspidertools/mongoclient.py` & `gzspidertools-0.0.9/gzspidertools/mongoclient.py`

 * *Files identical despite different names*

### Comparing `gzspidertools-0.0.8/gzspidertools/mysqlclient.py` & `gzspidertools-0.0.9/gzspidertools/mysqlclient.py`

 * *Files identical despite different names*

### Comparing `gzspidertools-0.0.8/gzspidertools/pipelines.py` & `gzspidertools-0.0.9/gzspidertools/pipelines.py`

 * *Files identical despite different names*

### Comparing `gzspidertools-0.0.8/gzspidertools/scraper/http/request/__init__.py` & `gzspidertools-0.0.9/gzspidertools/scraper/http/request/__init__.py`

 * *Files identical despite different names*

### Comparing `gzspidertools-0.0.8/gzspidertools/scraper/http/request/form.py` & `gzspidertools-0.0.9/gzspidertools/scraper/http/request/form.py`

 * *Files identical despite different names*

### Comparing `gzspidertools-0.0.8/gzspidertools/scraper/middlewares/__init__.py` & `gzspidertools-0.0.9/gzspidertools/scraper/middlewares/__init__.py`

 * *Files identical despite different names*

### Comparing `gzspidertools-0.0.8/gzspidertools/scraper/middlewares/headers/ua.py` & `gzspidertools-0.0.9/gzspidertools/scraper/middlewares/headers/ua.py`

 * *Files identical despite different names*

### Comparing `gzspidertools-0.0.8/gzspidertools/scraper/middlewares/netlib/aiohttplib.py` & `gzspidertools-0.0.9/gzspidertools/scraper/middlewares/netlib/aiohttplib.py`

 * *Files identical despite different names*

### Comparing `gzspidertools-0.0.8/gzspidertools/scraper/middlewares/proxy/dynamic.py` & `gzspidertools-0.0.9/gzspidertools/scraper/middlewares/proxy/dynamic.py`

 * *Files identical despite different names*

### Comparing `gzspidertools-0.0.8/gzspidertools/scraper/middlewares/proxy/exclusive.py` & `gzspidertools-0.0.9/gzspidertools/scraper/middlewares/proxy/exclusive.py`

 * *Files identical despite different names*

### Comparing `gzspidertools-0.0.8/gzspidertools/scraper/pipelines/__init__.py` & `gzspidertools-0.0.9/gzspidertools/scraper/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `gzspidertools-0.0.8/gzspidertools/scraper/pipelines/download/file.py` & `gzspidertools-0.0.9/gzspidertools/scraper/pipelines/download/file.py`

 * *Files identical despite different names*

### Comparing `gzspidertools-0.0.8/gzspidertools/scraper/pipelines/es/__init__.py` & `gzspidertools-0.0.9/gzspidertools/scraper/pipelines/es/__init__.py`

 * *Files identical despite different names*

### Comparing `gzspidertools-0.0.8/gzspidertools/scraper/pipelines/es/asynced.py` & `gzspidertools-0.0.9/gzspidertools/scraper/pipelines/es/asynced.py`

 * *Files identical despite different names*

### Comparing `gzspidertools-0.0.8/gzspidertools/scraper/pipelines/mongo/asynced.py` & `gzspidertools-0.0.9/gzspidertools/scraper/pipelines/mongo/asynced.py`

 * *Files identical despite different names*

### Comparing `gzspidertools-0.0.8/gzspidertools/scraper/pipelines/mongo/fantasy.py` & `gzspidertools-0.0.9/gzspidertools/scraper/pipelines/mongo/fantasy.py`

 * *Files identical despite different names*

### Comparing `gzspidertools-0.0.8/gzspidertools/scraper/pipelines/mongo/twisted.py` & `gzspidertools-0.0.9/gzspidertools/scraper/pipelines/mongo/twisted.py`

 * *Files identical despite different names*

### Comparing `gzspidertools-0.0.8/gzspidertools/scraper/pipelines/msgproducer/kafkapub.py` & `gzspidertools-0.0.9/gzspidertools/scraper/pipelines/msgproducer/kafkapub.py`

 * *Files identical despite different names*

### Comparing `gzspidertools-0.0.8/gzspidertools/scraper/pipelines/msgproducer/mqpub.py` & `gzspidertools-0.0.9/gzspidertools/scraper/pipelines/msgproducer/mqpub.py`

 * *Files identical despite different names*

### Comparing `gzspidertools-0.0.8/gzspidertools/scraper/pipelines/mysql/__init__.py` & `gzspidertools-0.0.9/gzspidertools/scraper/pipelines/mysql/__init__.py`

 * *Files identical despite different names*

### Comparing `gzspidertools-0.0.8/gzspidertools/scraper/pipelines/mysql/asynced.py` & `gzspidertools-0.0.9/gzspidertools/scraper/pipelines/mysql/asynced.py`

 * *Files identical despite different names*

### Comparing `gzspidertools-0.0.8/gzspidertools/scraper/pipelines/mysql/stats.py` & `gzspidertools-0.0.9/gzspidertools/scraper/pipelines/mysql/stats.py`

 * *Files identical despite different names*

### Comparing `gzspidertools-0.0.8/gzspidertools/scraper/pipelines/mysql/turbo.py` & `gzspidertools-0.0.9/gzspidertools/scraper/pipelines/mysql/turbo.py`

 * *Files identical despite different names*

### Comparing `gzspidertools-0.0.8/gzspidertools/scraper/pipelines/mysql/twisted.py` & `gzspidertools-0.0.9/gzspidertools/scraper/pipelines/mysql/twisted.py`

 * *Files identical despite different names*

### Comparing `gzspidertools-0.0.8/gzspidertools/scraper/pipelines/oracle/__init__.py` & `gzspidertools-0.0.9/gzspidertools/scraper/pipelines/oracle/__init__.py`

 * *Files identical despite different names*

### Comparing `gzspidertools-0.0.8/gzspidertools/scraper/pipelines/oracle/twisted.py` & `gzspidertools-0.0.9/gzspidertools/scraper/pipelines/oracle/twisted.py`

 * *Files identical despite different names*

### Comparing `gzspidertools-0.0.8/gzspidertools/scraper/pipelines/oss/ali.py` & `gzspidertools-0.0.9/gzspidertools/scraper/pipelines/oss/ali.py`

 * *Files identical despite different names*

### Comparing `gzspidertools-0.0.8/gzspidertools/scraper/pipelines/postgres/__init__.py` & `gzspidertools-0.0.9/gzspidertools/scraper/pipelines/postgres/__init__.py`

 * *Files identical despite different names*

### Comparing `gzspidertools-0.0.8/gzspidertools/scraper/pipelines/postgres/asynced.py` & `gzspidertools-0.0.9/gzspidertools/scraper/pipelines/postgres/asynced.py`

 * *Files identical despite different names*

### Comparing `gzspidertools-0.0.8/gzspidertools/scraper/pipelines/postgres/twisted.py` & `gzspidertools-0.0.9/gzspidertools/scraper/pipelines/postgres/twisted.py`

 * *Files identical despite different names*

### Comparing `gzspidertools-0.0.8/gzspidertools/scraper/spiders/__init__.py` & `gzspidertools-0.0.9/gzspidertools/scraper/spiders/__init__.py`

 * *Files identical despite different names*

### Comparing `gzspidertools-0.0.8/gzspidertools/templates/project/module/middlewares.py.tmpl` & `gzspidertools-0.0.9/gzspidertools/templates/project/module/middlewares.py.tmpl`

 * *Files identical despite different names*

### Comparing `gzspidertools-0.0.8/gzspidertools/templates/project/module/settings.py.tmpl` & `gzspidertools-0.0.9/gzspidertools/templates/project/module/settings.py.tmpl`

 * *Files identical despite different names*

### Comparing `gzspidertools-0.0.8/gzspidertools/templates/project/module/VIT/.conf` & `gzspidertools-0.0.9/gzspidertools/templates/project/module/VIT/.conf`

 * *Files identical despite different names*

### Comparing `gzspidertools-0.0.8/gzspidertools/templates/project/scrapy_redis-0.7.3-py2.py3-none-any.whl` & `gzspidertools-0.0.9/gzspidertools/templates/project/scrapy_redis-0.7.3-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `gzspidertools-0.0.8/gzspidertools/templates/spiders/async.tmpl` & `gzspidertools-0.0.9/gzspidertools/templates/spiders/async.tmpl`

 * *Files identical despite different names*

### Comparing `gzspidertools-0.0.8/gzspidertools/templates/spiders/basic.tmpl` & `gzspidertools-0.0.9/gzspidertools/templates/spiders/basic.tmpl`

 * *Files identical despite different names*

### Comparing `gzspidertools-0.0.8/gzspidertools/templates/spiders/crawl.tmpl` & `gzspidertools-0.0.9/gzspidertools/templates/spiders/crawl.tmpl`

 * *Files identical despite different names*

### Comparing `gzspidertools-0.0.8/gzspidertools/templates/spiders/csvfeed.tmpl` & `gzspidertools-0.0.9/gzspidertools/templates/spiders/csvfeed.tmpl`

 * *Files identical despite different names*

### Comparing `gzspidertools-0.0.8/gzspidertools/templates/spiders/sr.tmpl` & `gzspidertools-0.0.9/gzspidertools/templates/spiders/sr.tmpl`

 * *Files 0% similar despite different names*

```diff
@@ -120,9 +120,9 @@
                     yield article_item
             else:
                 yield article_item
 
 
 if __name__ == '__main__':
     process = CrawlerProcess(get_project_settings())
-    process.crawl($classname.$name)
+    process.crawl($classname.name)
     process.start()
```

### Comparing `gzspidertools-0.0.8/gzspidertools/templates/spiders/xmlfeed.tmpl` & `gzspidertools-0.0.9/gzspidertools/templates/spiders/xmlfeed.tmpl`

 * *Files identical despite different names*

### Comparing `gzspidertools-0.0.8/gzspidertools/utils/cmdline.py` & `gzspidertools-0.0.9/gzspidertools/utils/cmdline.py`

 * *Files identical despite different names*

### Comparing `gzspidertools-0.0.8/gzspidertools/utils/text_verification.py` & `gzspidertools-0.0.9/gzspidertools/utils/text_verification.py`

 * *Files identical despite different names*

### Comparing `gzspidertools-0.0.8/LICENSE` & `gzspidertools-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gzspidertools-0.0.8/pyproject.toml` & `gzspidertools-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gzspidertools"
-version = "0.0.8"
+version = "0.0.9"
 description = "魔改使用工具库"
 authors = ["George <persistencehoo@gmail.com>"]
 maintainers = ["George <persistencehoo@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "gzspidertools" }]
 repository = "https://github.com/georgeJzzz/gzspidertools"
 keywords = ["crawler", "scraping", "aiohttp", "asyncio", "scrapy"]
```

### Comparing `gzspidertools-0.0.8/README.md` & `gzspidertools-0.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,14 @@
 # 这里是为了演示方便，正常情况是直接在 VIT 中的 .conf 文件填上你需要的配置即可
 cp /root/mytemp/.conf DemoSpider/VIT/.conf
 
 # 生成爬虫脚本
 gzcmd genspider <spider_name> <example.com>
 
 # 生成 scrapy-redis 爬虫脚本   pip install scrapy_redis-0.7.3-py2.py3-none-any.whl
-gzcmd genspider <spider_name> <example.com>
+gzcmd genspider -t=sr <spider_name> <example.com>
 
 # 运行脚本
 scrapy crawl <spider_name>
 # 注：也可以使用 gzcmd crawl <spider_name>
 ```
```

### Comparing `gzspidertools-0.0.8/PKG-INFO` & `gzspidertools-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gzspidertools
-Version: 0.0.8
+Version: 0.0.9
 Summary: 魔改使用工具库
 Home-page: https://github.com/georgeJzzz/gzspidertools
 Keywords: crawler,scraping,aiohttp,asyncio,scrapy
 Author: George
 Author-email: persistencehoo@gmail.com
 Maintainer: George
 Maintainer-email: persistencehoo@gmail.com
@@ -91,15 +91,15 @@
 # 这里是为了演示方便，正常情况是直接在 VIT 中的 .conf 文件填上你需要的配置即可
 cp /root/mytemp/.conf DemoSpider/VIT/.conf
 
 # 生成爬虫脚本
 gzcmd genspider <spider_name> <example.com>
 
 # 生成 scrapy-redis 爬虫脚本   pip install scrapy_redis-0.7.3-py2.py3-none-any.whl
-gzcmd genspider <spider_name> <example.com>
+gzcmd genspider -t=sr <spider_name> <example.com>
 
 # 运行脚本
 scrapy crawl <spider_name>
 # 注：也可以使用 gzcmd crawl <spider_name>
 ```
```

