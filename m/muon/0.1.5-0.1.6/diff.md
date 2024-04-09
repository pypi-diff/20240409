# Comparing `tmp/muon-0.1.5.tar.gz` & `tmp/muon-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "muon-0.1.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "muon-0.1.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `muon-0.1.5.tar` & `muon-0.1.6.tar`

### file list

```diff
@@ -1,772 +1,772 @@
--rw-r--r--   0        0        0     4937 2023-06-07 09:07:57.080380 muon-0.1.5/README.md
--rw-r--r--   0        0        0      343 2023-06-09 01:08:06.568554 muon-0.1.5/muon/__init__.py
--rw-r--r--   0        0        0       97 2023-02-20 20:04:01.127617 muon-0.1.5/muon/_atac/__init__.py
--rw-r--r--   0        0        0      296 2023-02-20 20:04:01.127870 muon-0.1.5/muon/_atac/_ref/jaspar/MA0002.2.pfm
--rw-r--r--   0        0        0      384 2023-02-20 20:04:01.128008 muon-0.1.5/muon/_atac/_ref/jaspar/MA0003.4.pfm
--rw-r--r--   0        0        0      149 2023-02-20 20:04:01.128199 muon-0.1.5/muon/_atac/_ref/jaspar/MA0004.1.pfm
--rw-r--r--   0        0        0      149 2023-02-20 20:04:01.128343 muon-0.1.5/muon/_atac/_ref/jaspar/MA0006.1.pfm
--rw-r--r--   0        0        0      466 2023-02-20 20:04:01.128493 muon-0.1.5/muon/_atac/_ref/jaspar/MA0007.3.pfm
--rw-r--r--   0        0        0      435 2023-02-20 20:04:01.128651 muon-0.1.5/muon/_atac/_ref/jaspar/MA0009.2.pfm
--rw-r--r--   0        0        0      324 2023-02-20 20:04:01.128808 muon-0.1.5/muon/_atac/_ref/jaspar/MA0014.3.pfm
--rw-r--r--   0        0        0      357 2023-02-20 20:04:01.129002 muon-0.1.5/muon/_atac/_ref/jaspar/MA0017.2.pfm
--rw-r--r--   0        0        0      360 2023-02-20 20:04:01.129214 muon-0.1.5/muon/_atac/_ref/jaspar/MA0018.4.pfm
--rw-r--r--   0        0        0      318 2023-02-20 20:04:01.129440 muon-0.1.5/muon/_atac/_ref/jaspar/MA0019.1.pfm
--rw-r--r--   0        0        0      323 2023-02-20 20:04:01.129703 muon-0.1.5/muon/_atac/_ref/jaspar/MA0024.3.pfm
--rw-r--r--   0        0        0      356 2023-02-20 20:04:01.129915 muon-0.1.5/muon/_atac/_ref/jaspar/MA0025.2.pfm
--rw-r--r--   0        0        0      213 2023-02-20 20:04:01.130046 muon-0.1.5/muon/_atac/_ref/jaspar/MA0027.2.pfm
--rw-r--r--   0        0        0      274 2023-02-20 20:04:01.130202 muon-0.1.5/muon/_atac/_ref/jaspar/MA0028.2.pfm
--rw-r--r--   0        0        0      373 2023-02-20 20:04:01.130334 muon-0.1.5/muon/_atac/_ref/jaspar/MA0029.1.pfm
--rw-r--r--   0        0        0      373 2023-02-20 20:04:01.130461 muon-0.1.5/muon/_atac/_ref/jaspar/MA0030.1.pfm
--rw-r--r--   0        0        0      205 2023-02-20 20:04:01.130575 muon-0.1.5/muon/_atac/_ref/jaspar/MA0031.1.pfm
--rw-r--r--   0        0        0      299 2023-02-20 20:04:01.130696 muon-0.1.5/muon/_atac/_ref/jaspar/MA0032.2.pfm
--rw-r--r--   0        0        0      185 2023-02-20 20:04:01.130824 muon-0.1.5/muon/_atac/_ref/jaspar/MA0033.2.pfm
--rw-r--r--   0        0        0      304 2023-02-20 20:04:01.131076 muon-0.1.5/muon/_atac/_ref/jaspar/MA0035.4.pfm
--rw-r--r--   0        0        0      300 2023-02-20 20:04:01.131237 muon-0.1.5/muon/_atac/_ref/jaspar/MA0036.3.pfm
--rw-r--r--   0        0        0      210 2023-02-20 20:04:01.131379 muon-0.1.5/muon/_atac/_ref/jaspar/MA0037.3.pfm
--rw-r--r--   0        0        0      329 2023-02-20 20:04:01.131524 muon-0.1.5/muon/_atac/_ref/jaspar/MA0038.2.pfm
--rw-r--r--   0        0        0      332 2023-02-20 20:04:01.131656 muon-0.1.5/muon/_atac/_ref/jaspar/MA0039.4.pfm
--rw-r--r--   0        0        0      288 2023-02-20 20:04:01.131787 muon-0.1.5/muon/_atac/_ref/jaspar/MA0040.1.pfm
--rw-r--r--   0        0        0      318 2023-02-20 20:04:01.131919 muon-0.1.5/muon/_atac/_ref/jaspar/MA0041.1.pfm
--rw-r--r--   0        0        0      182 2023-02-20 20:04:01.132055 muon-0.1.5/muon/_atac/_ref/jaspar/MA0042.2.pfm
--rw-r--r--   0        0        0      384 2023-02-20 20:04:01.132205 muon-0.1.5/muon/_atac/_ref/jaspar/MA0043.3.pfm
--rw-r--r--   0        0        0      412 2023-02-20 20:04:01.132361 muon-0.1.5/muon/_atac/_ref/jaspar/MA0046.2.pfm
--rw-r--r--   0        0        0      305 2023-02-20 20:04:01.132497 muon-0.1.5/muon/_atac/_ref/jaspar/MA0047.3.pfm
--rw-r--r--   0        0        0      269 2023-02-20 20:04:01.132642 muon-0.1.5/muon/_atac/_ref/jaspar/MA0048.2.pfm
--rw-r--r--   0        0        0      576 2023-02-20 20:04:01.132775 muon-0.1.5/muon/_atac/_ref/jaspar/MA0050.2.pfm
--rw-r--r--   0        0        0      484 2023-02-20 20:04:01.132908 muon-0.1.5/muon/_atac/_ref/jaspar/MA0051.1.pfm
--rw-r--r--   0        0        0      412 2023-02-20 20:04:01.133039 muon-0.1.5/muon/_atac/_ref/jaspar/MA0052.4.pfm
--rw-r--r--   0        0        0      356 2023-02-20 20:04:01.133170 muon-0.1.5/muon/_atac/_ref/jaspar/MA0056.2.pfm
--rw-r--r--   0        0        0      260 2023-02-20 20:04:01.133293 muon-0.1.5/muon/_atac/_ref/jaspar/MA0057.1.pfm
--rw-r--r--   0        0        0      271 2023-02-20 20:04:01.133546 muon-0.1.5/muon/_atac/_ref/jaspar/MA0058.3.pfm
--rw-r--r--   0        0        0      288 2023-02-20 20:04:01.133717 muon-0.1.5/muon/_atac/_ref/jaspar/MA0059.1.pfm
--rw-r--r--   0        0        0      298 2023-02-20 20:04:01.133873 muon-0.1.5/muon/_atac/_ref/jaspar/MA0060.3.pfm
--rw-r--r--   0        0        0      388 2023-02-20 20:04:01.134025 muon-0.1.5/muon/_atac/_ref/jaspar/MA0062.3.pfm
--rw-r--r--   0        0        0      300 2023-02-20 20:04:01.134166 muon-0.1.5/muon/_atac/_ref/jaspar/MA0063.2.pfm
--rw-r--r--   0        0        0      407 2023-02-20 20:04:01.134332 muon-0.1.5/muon/_atac/_ref/jaspar/MA0065.2.pfm
--rw-r--r--   0        0        0      541 2023-02-20 20:04:01.134684 muon-0.1.5/muon/_atac/_ref/jaspar/MA0066.1.pfm
--rw-r--r--   0        0        0      205 2023-02-20 20:04:01.134941 muon-0.1.5/muon/_atac/_ref/jaspar/MA0067.1.pfm
--rw-r--r--   0        0        0      210 2023-02-20 20:04:01.135150 muon-0.1.5/muon/_atac/_ref/jaspar/MA0068.2.pfm
--rw-r--r--   0        0        0      373 2023-02-20 20:04:01.135352 muon-0.1.5/muon/_atac/_ref/jaspar/MA0069.1.pfm
--rw-r--r--   0        0        0      316 2023-02-20 20:04:01.135495 muon-0.1.5/muon/_atac/_ref/jaspar/MA0070.1.pfm
--rw-r--r--   0        0        0      261 2023-02-20 20:04:01.135630 muon-0.1.5/muon/_atac/_ref/jaspar/MA0071.1.pfm
--rw-r--r--   0        0        0      373 2023-02-20 20:04:01.135784 muon-0.1.5/muon/_atac/_ref/jaspar/MA0072.1.pfm
--rw-r--r--   0        0        0      540 2023-02-20 20:04:01.135917 muon-0.1.5/muon/_atac/_ref/jaspar/MA0073.1.pfm
--rw-r--r--   0        0        0      400 2023-02-20 20:04:01.136054 muon-0.1.5/muon/_atac/_ref/jaspar/MA0074.1.pfm
--rw-r--r--   0        0        0      215 2023-02-20 20:04:01.136186 muon-0.1.5/muon/_atac/_ref/jaspar/MA0075.3.pfm
--rw-r--r--   0        0        0      297 2023-02-20 20:04:01.136308 muon-0.1.5/muon/_atac/_ref/jaspar/MA0076.2.pfm
--rw-r--r--   0        0        0      233 2023-02-20 20:04:01.136474 muon-0.1.5/muon/_atac/_ref/jaspar/MA0077.1.pfm
--rw-r--r--   0        0        0      232 2023-02-20 20:04:01.136632 muon-0.1.5/muon/_atac/_ref/jaspar/MA0078.1.pfm
--rw-r--r--   0        0        0      414 2023-02-20 20:04:01.136781 muon-0.1.5/muon/_atac/_ref/jaspar/MA0079.4.pfm
--rw-r--r--   0        0        0      556 2023-02-20 20:04:01.136915 muon-0.1.5/muon/_atac/_ref/jaspar/MA0080.5.pfm
--rw-r--r--   0        0        0      441 2023-02-20 20:04:01.137065 muon-0.1.5/muon/_atac/_ref/jaspar/MA0081.2.pfm
--rw-r--r--   0        0        0      436 2023-02-20 20:04:01.137219 muon-0.1.5/muon/_atac/_ref/jaspar/MA0083.3.pfm
--rw-r--r--   0        0        0      233 2023-02-20 20:04:01.137344 muon-0.1.5/muon/_atac/_ref/jaspar/MA0084.1.pfm
--rw-r--r--   0        0        0      177 2023-02-20 20:04:01.137576 muon-0.1.5/muon/_atac/_ref/jaspar/MA0087.1.pfm
--rw-r--r--   0        0        0      436 2023-02-20 20:04:01.137761 muon-0.1.5/muon/_atac/_ref/jaspar/MA0088.2.pfm
--rw-r--r--   0        0        0      437 2023-02-20 20:04:01.137906 muon-0.1.5/muon/_atac/_ref/jaspar/MA0089.2.pfm
--rw-r--r--   0        0        0      360 2023-02-20 20:04:01.138046 muon-0.1.5/muon/_atac/_ref/jaspar/MA0090.3.pfm
--rw-r--r--   0        0        0      318 2023-02-20 20:04:01.138183 muon-0.1.5/muon/_atac/_ref/jaspar/MA0091.1.pfm
--rw-r--r--   0        0        0      261 2023-02-20 20:04:01.138326 muon-0.1.5/muon/_atac/_ref/jaspar/MA0092.1.pfm
--rw-r--r--   0        0        0      388 2023-02-20 20:04:01.138469 muon-0.1.5/muon/_atac/_ref/jaspar/MA0093.3.pfm
--rw-r--r--   0        0        0      326 2023-02-20 20:04:01.138600 muon-0.1.5/muon/_atac/_ref/jaspar/MA0095.2.pfm
--rw-r--r--   0        0        0      269 2023-02-20 20:04:01.138839 muon-0.1.5/muon/_atac/_ref/jaspar/MA0098.3.pfm
--rw-r--r--   0        0        0      267 2023-02-20 20:04:01.138997 muon-0.1.5/muon/_atac/_ref/jaspar/MA0099.3.pfm
--rw-r--r--   0        0        0      268 2023-02-20 20:04:01.139184 muon-0.1.5/muon/_atac/_ref/jaspar/MA0100.3.pfm
--rw-r--r--   0        0        0      260 2023-02-20 20:04:01.139338 muon-0.1.5/muon/_atac/_ref/jaspar/MA0101.1.pfm
--rw-r--r--   0        0        0      388 2023-02-20 20:04:01.139523 muon-0.1.5/muon/_atac/_ref/jaspar/MA0102.4.pfm
--rw-r--r--   0        0        0      300 2023-02-20 20:04:01.139819 muon-0.1.5/muon/_atac/_ref/jaspar/MA0103.3.pfm
--rw-r--r--   0        0        0      328 2023-02-20 20:04:01.140063 muon-0.1.5/muon/_atac/_ref/jaspar/MA0104.4.pfm
--rw-r--r--   0        0        0      354 2023-02-20 20:04:01.140242 muon-0.1.5/muon/_atac/_ref/jaspar/MA0105.4.pfm
--rw-r--r--   0        0        0      496 2023-02-20 20:04:01.140644 muon-0.1.5/muon/_atac/_ref/jaspar/MA0106.3.pfm
--rw-r--r--   0        0        0      261 2023-02-20 20:04:01.141075 muon-0.1.5/muon/_atac/_ref/jaspar/MA0107.1.pfm
--rw-r--r--   0        0        0      406 2023-02-20 20:04:01.141327 muon-0.1.5/muon/_atac/_ref/jaspar/MA0108.2.pfm
--rw-r--r--   0        0        0      264 2023-02-20 20:04:01.141518 muon-0.1.5/muon/_atac/_ref/jaspar/MA0109.1.pfm
--rw-r--r--   0        0        0      288 2023-02-20 20:04:01.141706 muon-0.1.5/muon/_atac/_ref/jaspar/MA0111.1.pfm
--rw-r--r--   0        0        0      462 2023-02-20 20:04:01.142064 muon-0.1.5/muon/_atac/_ref/jaspar/MA0112.3.pfm
--rw-r--r--   0        0        0      468 2023-02-20 20:04:01.142282 muon-0.1.5/muon/_atac/_ref/jaspar/MA0113.3.pfm
--rw-r--r--   0        0        0      359 2023-02-20 20:04:01.142434 muon-0.1.5/muon/_atac/_ref/jaspar/MA0114.4.pfm
--rw-r--r--   0        0        0      457 2023-02-20 20:04:01.142706 muon-0.1.5/muon/_atac/_ref/jaspar/MA0115.1.pfm
--rw-r--r--   0        0        0      401 2023-02-20 20:04:01.143015 muon-0.1.5/muon/_atac/_ref/jaspar/MA0116.1.pfm
--rw-r--r--   0        0        0      325 2023-02-20 20:04:01.143269 muon-0.1.5/muon/_atac/_ref/jaspar/MA0117.2.pfm
--rw-r--r--   0        0        0      373 2023-02-20 20:04:01.143565 muon-0.1.5/muon/_atac/_ref/jaspar/MA0119.1.pfm
--rw-r--r--   0        0        0      356 2023-02-20 20:04:01.143773 muon-0.1.5/muon/_atac/_ref/jaspar/MA0122.3.pfm
--rw-r--r--   0        0        0      242 2023-02-20 20:04:01.144054 muon-0.1.5/muon/_atac/_ref/jaspar/MA0124.2.pfm
--rw-r--r--   0        0        0      205 2023-02-20 20:04:01.144340 muon-0.1.5/muon/_atac/_ref/jaspar/MA0125.1.pfm
--rw-r--r--   0        0        0      148 2023-02-20 20:04:01.144556 muon-0.1.5/muon/_atac/_ref/jaspar/MA0130.1.pfm
--rw-r--r--   0        0        0      323 2023-02-20 20:04:01.144775 muon-0.1.5/muon/_atac/_ref/jaspar/MA0131.2.pfm
--rw-r--r--   0        0        0      215 2023-02-20 20:04:01.144986 muon-0.1.5/muon/_atac/_ref/jaspar/MA0132.2.pfm
--rw-r--r--   0        0        0      344 2023-02-20 20:04:01.145188 muon-0.1.5/muon/_atac/_ref/jaspar/MA0135.1.pfm
--rw-r--r--   0        0        0      297 2023-02-20 20:04:01.145402 muon-0.1.5/muon/_atac/_ref/jaspar/MA0136.2.pfm
--rw-r--r--   0        0        0      297 2023-02-20 20:04:01.145697 muon-0.1.5/muon/_atac/_ref/jaspar/MA0137.3.pfm
--rw-r--r--   0        0        0      576 2023-02-20 20:04:01.145894 muon-0.1.5/muon/_atac/_ref/jaspar/MA0138.2.pfm
--rw-r--r--   0        0        0      518 2023-02-20 20:04:01.146162 muon-0.1.5/muon/_atac/_ref/jaspar/MA0139.1.pfm
--rw-r--r--   0        0        0      494 2023-02-20 20:04:01.146437 muon-0.1.5/muon/_atac/_ref/jaspar/MA0140.2.pfm
--rw-r--r--   0        0        0      296 2023-02-20 20:04:01.146654 muon-0.1.5/muon/_atac/_ref/jaspar/MA0141.3.pfm
--rw-r--r--   0        0        0      406 2023-02-20 20:04:01.146921 muon-0.1.5/muon/_atac/_ref/jaspar/MA0142.1.pfm
--rw-r--r--   0        0        0      304 2023-02-20 20:04:01.147096 muon-0.1.5/muon/_atac/_ref/jaspar/MA0143.4.pfm
--rw-r--r--   0        0        0      300 2023-02-20 20:04:01.147245 muon-0.1.5/muon/_atac/_ref/jaspar/MA0144.2.pfm
--rw-r--r--   0        0        0      266 2023-02-20 20:04:01.147379 muon-0.1.5/muon/_atac/_ref/jaspar/MA0145.3.pfm
--rw-r--r--   0        0        0      378 2023-02-20 20:04:01.147531 muon-0.1.5/muon/_atac/_ref/jaspar/MA0146.2.pfm
--rw-r--r--   0        0        0      327 2023-02-20 20:04:01.147676 muon-0.1.5/muon/_atac/_ref/jaspar/MA0147.3.pfm
--rw-r--r--   0        0        0      333 2023-02-20 20:04:01.147806 muon-0.1.5/muon/_atac/_ref/jaspar/MA0148.4.pfm
--rw-r--r--   0        0        0      486 2023-02-20 20:04:01.147960 muon-0.1.5/muon/_atac/_ref/jaspar/MA0149.1.pfm
--rw-r--r--   0        0        0      408 2023-02-20 20:04:01.148257 muon-0.1.5/muon/_atac/_ref/jaspar/MA0150.2.pfm
--rw-r--r--   0        0        0      149 2023-02-20 20:04:01.148412 muon-0.1.5/muon/_atac/_ref/jaspar/MA0151.1.pfm
--rw-r--r--   0        0        0      177 2023-02-20 20:04:01.148598 muon-0.1.5/muon/_atac/_ref/jaspar/MA0152.1.pfm
--rw-r--r--   0        0        0      357 2023-02-20 20:04:01.148839 muon-0.1.5/muon/_atac/_ref/jaspar/MA0153.2.pfm
--rw-r--r--   0        0        0      415 2023-02-20 20:04:01.149056 muon-0.1.5/muon/_atac/_ref/jaspar/MA0154.4.pfm
--rw-r--r--   0        0        0      317 2023-02-20 20:04:01.149246 muon-0.1.5/muon/_atac/_ref/jaspar/MA0155.1.pfm
--rw-r--r--   0        0        0      271 2023-02-20 20:04:01.149377 muon-0.1.5/muon/_atac/_ref/jaspar/MA0156.2.pfm
--rw-r--r--   0        0        0      207 2023-02-20 20:04:01.149513 muon-0.1.5/muon/_atac/_ref/jaspar/MA0157.2.pfm
--rw-r--r--   0        0        0      213 2023-02-20 20:04:01.149648 muon-0.1.5/muon/_atac/_ref/jaspar/MA0158.2.pfm
--rw-r--r--   0        0        0      458 2023-02-20 20:04:01.149783 muon-0.1.5/muon/_atac/_ref/jaspar/MA0159.1.pfm
--rw-r--r--   0        0        0      204 2023-02-20 20:04:01.149967 muon-0.1.5/muon/_atac/_ref/jaspar/MA0160.1.pfm
--rw-r--r--   0        0        0      300 2023-02-20 20:04:01.150213 muon-0.1.5/muon/_atac/_ref/jaspar/MA0161.2.pfm
--rw-r--r--   0        0        0      385 2023-02-20 20:04:01.150429 muon-0.1.5/muon/_atac/_ref/jaspar/MA0162.4.pfm
--rw-r--r--   0        0        0      373 2023-02-20 20:04:01.150577 muon-0.1.5/muon/_atac/_ref/jaspar/MA0163.1.pfm
--rw-r--r--   0        0        0      177 2023-02-20 20:04:01.150710 muon-0.1.5/muon/_atac/_ref/jaspar/MA0164.1.pfm
--rw-r--r--   0        0        0      409 2023-02-20 20:04:01.150852 muon-0.1.5/muon/_atac/_ref/jaspar/MA0258.2.pfm
--rw-r--r--   0        0        0      207 2023-02-20 20:04:01.151007 muon-0.1.5/muon/_atac/_ref/jaspar/MA0259.1.pfm
--rw-r--r--   0        0        0      296 2023-02-20 20:04:01.151132 muon-0.1.5/muon/_atac/_ref/jaspar/MA0442.2.pfm
--rw-r--r--   0        0        0      267 2023-02-20 20:04:01.151252 muon-0.1.5/muon/_atac/_ref/jaspar/MA0461.2.pfm
--rw-r--r--   0        0        0      302 2023-02-20 20:04:01.151446 muon-0.1.5/muon/_atac/_ref/jaspar/MA0462.2.pfm
--rw-r--r--   0        0        0      440 2023-02-20 20:04:01.151583 muon-0.1.5/muon/_atac/_ref/jaspar/MA0463.2.pfm
--rw-r--r--   0        0        0      272 2023-02-20 20:04:01.151712 muon-0.1.5/muon/_atac/_ref/jaspar/MA0464.2.pfm
--rw-r--r--   0        0        0      329 2023-02-20 20:04:01.151832 muon-0.1.5/muon/_atac/_ref/jaspar/MA0465.2.pfm
--rw-r--r--   0        0        0      272 2023-02-20 20:04:01.151948 muon-0.1.5/muon/_atac/_ref/jaspar/MA0466.2.pfm
--rw-r--r--   0        0        0      297 2023-02-20 20:04:01.152062 muon-0.1.5/muon/_atac/_ref/jaspar/MA0467.1.pfm
--rw-r--r--   0        0        0      300 2023-02-20 20:04:01.152175 muon-0.1.5/muon/_atac/_ref/jaspar/MA0468.1.pfm
--rw-r--r--   0        0        0      441 2023-02-20 20:04:01.152287 muon-0.1.5/muon/_atac/_ref/jaspar/MA0469.3.pfm
--rw-r--r--   0        0        0      384 2023-02-20 20:04:01.152401 muon-0.1.5/muon/_atac/_ref/jaspar/MA0470.2.pfm
--rw-r--r--   0        0        0      357 2023-02-20 20:04:01.152672 muon-0.1.5/muon/_atac/_ref/jaspar/MA0471.2.pfm
--rw-r--r--   0        0        0      296 2023-02-20 20:04:01.152867 muon-0.1.5/muon/_atac/_ref/jaspar/MA0472.2.pfm
--rw-r--r--   0        0        0      386 2023-02-20 20:04:01.153007 muon-0.1.5/muon/_atac/_ref/jaspar/MA0473.3.pfm
--rw-r--r--   0        0        0      269 2023-02-20 20:04:01.153137 muon-0.1.5/muon/_atac/_ref/jaspar/MA0474.2.pfm
--rw-r--r--   0        0        0      273 2023-02-20 20:04:01.153257 muon-0.1.5/muon/_atac/_ref/jaspar/MA0475.2.pfm
--rw-r--r--   0        0        0      300 2023-02-20 20:04:01.153372 muon-0.1.5/muon/_atac/_ref/jaspar/MA0476.1.pfm
--rw-r--r--   0        0        0      360 2023-02-20 20:04:01.153488 muon-0.1.5/muon/_atac/_ref/jaspar/MA0477.2.pfm
--rw-r--r--   0        0        0      298 2023-02-20 20:04:01.153639 muon-0.1.5/muon/_atac/_ref/jaspar/MA0478.1.pfm
--rw-r--r--   0        0        0      299 2023-02-20 20:04:01.153938 muon-0.1.5/muon/_atac/_ref/jaspar/MA0479.1.pfm
--rw-r--r--   0        0        0      297 2023-02-20 20:04:01.154153 muon-0.1.5/muon/_atac/_ref/jaspar/MA0480.1.pfm
--rw-r--r--   0        0        0      304 2023-02-20 20:04:01.154318 muon-0.1.5/muon/_atac/_ref/jaspar/MA0481.3.pfm
--rw-r--r--   0        0        0      332 2023-02-20 20:04:01.154488 muon-0.1.5/muon/_atac/_ref/jaspar/MA0482.2.pfm
--rw-r--r--   0        0        0      296 2023-02-20 20:04:01.154636 muon-0.1.5/muon/_atac/_ref/jaspar/MA0483.1.pfm
--rw-r--r--   0        0        0      356 2023-02-20 20:04:01.154780 muon-0.1.5/muon/_atac/_ref/jaspar/MA0484.2.pfm
--rw-r--r--   0        0        0      270 2023-02-20 20:04:01.154902 muon-0.1.5/muon/_atac/_ref/jaspar/MA0485.2.pfm
--rw-r--r--   0        0        0      350 2023-02-20 20:04:01.155021 muon-0.1.5/muon/_atac/_ref/jaspar/MA0486.2.pfm
--rw-r--r--   0        0        0      356 2023-02-20 20:04:01.155249 muon-0.1.5/muon/_atac/_ref/jaspar/MA0488.1.pfm
--rw-r--r--   0        0        0      384 2023-02-20 20:04:01.155454 muon-0.1.5/muon/_atac/_ref/jaspar/MA0489.1.pfm
--rw-r--r--   0        0        0      360 2023-02-20 20:04:01.155691 muon-0.1.5/muon/_atac/_ref/jaspar/MA0490.2.pfm
--rw-r--r--   0        0        0      360 2023-02-20 20:04:01.155911 muon-0.1.5/muon/_atac/_ref/jaspar/MA0491.2.pfm
--rw-r--r--   0        0        0      413 2023-02-20 20:04:01.156132 muon-0.1.5/muon/_atac/_ref/jaspar/MA0492.1.pfm
--rw-r--r--   0        0        0      294 2023-02-20 20:04:01.156332 muon-0.1.5/muon/_atac/_ref/jaspar/MA0493.1.pfm
--rw-r--r--   0        0        0      517 2023-02-20 20:04:01.156652 muon-0.1.5/muon/_atac/_ref/jaspar/MA0494.1.pfm
--rw-r--r--   0        0        0      442 2023-02-20 20:04:01.157021 muon-0.1.5/muon/_atac/_ref/jaspar/MA0495.3.pfm
--rw-r--r--   0        0        0      415 2023-02-20 20:04:01.157261 muon-0.1.5/muon/_atac/_ref/jaspar/MA0496.3.pfm
--rw-r--r--   0        0        0      408 2023-02-20 20:04:01.157480 muon-0.1.5/muon/_atac/_ref/jaspar/MA0497.1.pfm
--rw-r--r--   0        0        0      191 2023-02-20 20:04:01.157826 muon-0.1.5/muon/_atac/_ref/jaspar/MA0498.2.pfm
--rw-r--r--   0        0        0      357 2023-02-20 20:04:01.158061 muon-0.1.5/muon/_atac/_ref/jaspar/MA0499.2.pfm
--rw-r--r--   0        0        0      328 2023-02-20 20:04:01.158305 muon-0.1.5/muon/_atac/_ref/jaspar/MA0500.2.pfm
--rw-r--r--   0        0        0      405 2023-02-20 20:04:01.158537 muon-0.1.5/muon/_atac/_ref/jaspar/MA0501.1.pfm
--rw-r--r--   0        0        0      327 2023-02-20 20:04:01.158753 muon-0.1.5/muon/_atac/_ref/jaspar/MA0502.2.pfm
--rw-r--r--   0        0        0      297 2023-02-20 20:04:01.158959 muon-0.1.5/muon/_atac/_ref/jaspar/MA0503.1.pfm
--rw-r--r--   0        0        0      406 2023-02-20 20:04:01.159150 muon-0.1.5/muon/_atac/_ref/jaspar/MA0504.1.pfm
--rw-r--r--   0        0        0      408 2023-02-20 20:04:01.159288 muon-0.1.5/muon/_atac/_ref/jaspar/MA0505.1.pfm
--rw-r--r--   0        0        0      295 2023-02-20 20:04:01.159411 muon-0.1.5/muon/_atac/_ref/jaspar/MA0506.1.pfm
--rw-r--r--   0        0        0      352 2023-02-20 20:04:01.159538 muon-0.1.5/muon/_atac/_ref/jaspar/MA0507.1.pfm
--rw-r--r--   0        0        0      302 2023-02-20 20:04:01.159738 muon-0.1.5/muon/_atac/_ref/jaspar/MA0508.3.pfm
--rw-r--r--   0        0        0      384 2023-02-20 20:04:01.159929 muon-0.1.5/muon/_atac/_ref/jaspar/MA0509.2.pfm
--rw-r--r--   0        0        0      437 2023-02-20 20:04:01.160149 muon-0.1.5/muon/_atac/_ref/jaspar/MA0510.2.pfm
--rw-r--r--   0        0        0      243 2023-02-20 20:04:01.160350 muon-0.1.5/muon/_atac/_ref/jaspar/MA0511.2.pfm
--rw-r--r--   0        0        0      386 2023-02-20 20:04:01.160507 muon-0.1.5/muon/_atac/_ref/jaspar/MA0512.2.pfm
--rw-r--r--   0        0        0      352 2023-02-20 20:04:01.160645 muon-0.1.5/muon/_atac/_ref/jaspar/MA0513.1.pfm
--rw-r--r--   0        0        0      267 2023-02-20 20:04:01.160795 muon-0.1.5/muon/_atac/_ref/jaspar/MA0514.1.pfm
--rw-r--r--   0        0        0      264 2023-02-20 20:04:01.160932 muon-0.1.5/muon/_atac/_ref/jaspar/MA0515.1.pfm
--rw-r--r--   0        0        0      464 2023-02-20 20:04:01.161140 muon-0.1.5/muon/_atac/_ref/jaspar/MA0516.2.pfm
--rw-r--r--   0        0        0      405 2023-02-20 20:04:01.161317 muon-0.1.5/muon/_atac/_ref/jaspar/MA0517.1.pfm
--rw-r--r--   0        0        0      382 2023-02-20 20:04:01.161453 muon-0.1.5/muon/_atac/_ref/jaspar/MA0518.1.pfm
--rw-r--r--   0        0        0      300 2023-02-20 20:04:01.161623 muon-0.1.5/muon/_atac/_ref/jaspar/MA0519.1.pfm
--rw-r--r--   0        0        0      408 2023-02-20 20:04:01.161755 muon-0.1.5/muon/_atac/_ref/jaspar/MA0520.1.pfm
--rw-r--r--   0        0        0      298 2023-02-20 20:04:01.161909 muon-0.1.5/muon/_atac/_ref/jaspar/MA0521.1.pfm
--rw-r--r--   0        0        0      301 2023-02-20 20:04:01.162094 muon-0.1.5/muon/_atac/_ref/jaspar/MA0522.3.pfm
--rw-r--r--   0        0        0      382 2023-02-20 20:04:01.162248 muon-0.1.5/muon/_atac/_ref/jaspar/MA0523.1.pfm
--rw-r--r--   0        0        0      327 2023-02-20 20:04:01.162382 muon-0.1.5/muon/_atac/_ref/jaspar/MA0524.2.pfm
--rw-r--r--   0        0        0      492 2023-02-20 20:04:01.162529 muon-0.1.5/muon/_atac/_ref/jaspar/MA0525.2.pfm
--rw-r--r--   0        0        0      385 2023-02-20 20:04:01.162664 muon-0.1.5/muon/_atac/_ref/jaspar/MA0526.3.pfm
--rw-r--r--   0        0        0      407 2023-02-20 20:04:01.162838 muon-0.1.5/muon/_atac/_ref/jaspar/MA0527.1.pfm
--rw-r--r--   0        0        0      331 2023-02-20 20:04:01.162976 muon-0.1.5/muon/_atac/_ref/jaspar/MA0528.2.pfm
--rw-r--r--   0        0        0      404 2023-02-20 20:04:01.163165 muon-0.1.5/muon/_atac/_ref/jaspar/MA0591.1.pfm
--rw-r--r--   0        0        0      356 2023-02-20 20:04:01.163301 muon-0.1.5/muon/_atac/_ref/jaspar/MA0592.3.pfm
--rw-r--r--   0        0        0      296 2023-02-20 20:04:01.163417 muon-0.1.5/muon/_atac/_ref/jaspar/MA0593.1.pfm
--rw-r--r--   0        0        0      267 2023-02-20 20:04:01.163561 muon-0.1.5/muon/_atac/_ref/jaspar/MA0594.2.pfm
--rw-r--r--   0        0        0      263 2023-02-20 20:04:01.163688 muon-0.1.5/muon/_atac/_ref/jaspar/MA0595.1.pfm
--rw-r--r--   0        0        0      262 2023-02-20 20:04:01.163825 muon-0.1.5/muon/_atac/_ref/jaspar/MA0596.1.pfm
--rw-r--r--   0        0        0      236 2023-02-20 20:04:01.163954 muon-0.1.5/muon/_atac/_ref/jaspar/MA0597.1.pfm
--rw-r--r--   0        0        0      412 2023-02-20 20:04:01.164202 muon-0.1.5/muon/_atac/_ref/jaspar/MA0598.3.pfm
--rw-r--r--   0        0        0      272 2023-02-20 20:04:01.164422 muon-0.1.5/muon/_atac/_ref/jaspar/MA0599.1.pfm
--rw-r--r--   0        0        0      440 2023-02-20 20:04:01.164636 muon-0.1.5/muon/_atac/_ref/jaspar/MA0600.2.pfm
--rw-r--r--   0        0        0      296 2023-02-20 20:04:01.164777 muon-0.1.5/muon/_atac/_ref/jaspar/MA0601.1.pfm
--rw-r--r--   0        0        0      376 2023-02-20 20:04:01.164899 muon-0.1.5/muon/_atac/_ref/jaspar/MA0602.1.pfm
--rw-r--r--   0        0        0      268 2023-02-20 20:04:01.165015 muon-0.1.5/muon/_atac/_ref/jaspar/MA0603.1.pfm
--rw-r--r--   0        0        0      210 2023-02-20 20:04:01.165128 muon-0.1.5/muon/_atac/_ref/jaspar/MA0604.1.pfm
--rw-r--r--   0        0        0      329 2023-02-20 20:04:01.165239 muon-0.1.5/muon/_atac/_ref/jaspar/MA0605.2.pfm
--rw-r--r--   0        0        0      268 2023-02-20 20:04:01.165380 muon-0.1.5/muon/_atac/_ref/jaspar/MA0606.1.pfm
--rw-r--r--   0        0        0      210 2023-02-20 20:04:01.165573 muon-0.1.5/muon/_atac/_ref/jaspar/MA0607.1.pfm
--rw-r--r--   0        0        0      236 2023-02-20 20:04:01.165690 muon-0.1.5/muon/_atac/_ref/jaspar/MA0608.1.pfm
--rw-r--r--   0        0        0      440 2023-02-20 20:04:01.165810 muon-0.1.5/muon/_atac/_ref/jaspar/MA0609.2.pfm
--rw-r--r--   0        0        0      296 2023-02-20 20:04:01.165928 muon-0.1.5/muon/_atac/_ref/jaspar/MA0610.1.pfm
--rw-r--r--   0        0        0      212 2023-02-20 20:04:01.166161 muon-0.1.5/muon/_atac/_ref/jaspar/MA0611.1.pfm
--rw-r--r--   0        0        0      216 2023-02-20 20:04:01.166333 muon-0.1.5/muon/_atac/_ref/jaspar/MA0612.2.pfm
--rw-r--r--   0        0        0      208 2023-02-20 20:04:01.166588 muon-0.1.5/muon/_atac/_ref/jaspar/MA0613.1.pfm
--rw-r--r--   0        0        0      208 2023-02-20 20:04:01.166762 muon-0.1.5/muon/_atac/_ref/jaspar/MA0614.1.pfm
--rw-r--r--   0        0        0      460 2023-02-20 20:04:01.166996 muon-0.1.5/muon/_atac/_ref/jaspar/MA0615.1.pfm
--rw-r--r--   0        0        0      270 2023-02-20 20:04:01.167151 muon-0.1.5/muon/_atac/_ref/jaspar/MA0616.2.pfm
--rw-r--r--   0        0        0      212 2023-02-20 20:04:01.167289 muon-0.1.5/muon/_atac/_ref/jaspar/MA0618.1.pfm
--rw-r--r--   0        0        0      239 2023-02-20 20:04:01.167427 muon-0.1.5/muon/_atac/_ref/jaspar/MA0619.1.pfm
--rw-r--r--   0        0        0      500 2023-02-20 20:04:01.167646 muon-0.1.5/muon/_atac/_ref/jaspar/MA0620.3.pfm
--rw-r--r--   0        0        0      296 2023-02-20 20:04:01.167866 muon-0.1.5/muon/_atac/_ref/jaspar/MA0621.1.pfm
--rw-r--r--   0        0        0      211 2023-02-20 20:04:01.168043 muon-0.1.5/muon/_atac/_ref/jaspar/MA0622.1.pfm
--rw-r--r--   0        0        0      269 2023-02-20 20:04:01.168207 muon-0.1.5/muon/_atac/_ref/jaspar/MA0623.2.pfm
--rw-r--r--   0        0        0      268 2023-02-20 20:04:01.168456 muon-0.1.5/muon/_atac/_ref/jaspar/MA0624.1.pfm
--rw-r--r--   0        0        0      267 2023-02-20 20:04:01.168661 muon-0.1.5/muon/_atac/_ref/jaspar/MA0625.1.pfm
--rw-r--r--   0        0        0      268 2023-02-20 20:04:01.168872 muon-0.1.5/muon/_atac/_ref/jaspar/MA0626.1.pfm
--rw-r--r--   0        0        0      360 2023-02-20 20:04:01.169038 muon-0.1.5/muon/_atac/_ref/jaspar/MA0627.2.pfm
--rw-r--r--   0        0        0      267 2023-02-20 20:04:01.169194 muon-0.1.5/muon/_atac/_ref/jaspar/MA0628.1.pfm
--rw-r--r--   0        0        0      460 2023-02-20 20:04:01.169321 muon-0.1.5/muon/_atac/_ref/jaspar/MA0629.1.pfm
--rw-r--r--   0        0        0      212 2023-02-20 20:04:01.169451 muon-0.1.5/muon/_atac/_ref/jaspar/MA0630.1.pfm
--rw-r--r--   0        0        0      459 2023-02-20 20:04:01.169598 muon-0.1.5/muon/_atac/_ref/jaspar/MA0631.1.pfm
--rw-r--r--   0        0        0      275 2023-02-20 20:04:01.169737 muon-0.1.5/muon/_atac/_ref/jaspar/MA0632.2.pfm
--rw-r--r--   0        0        0      268 2023-02-20 20:04:01.169869 muon-0.1.5/muon/_atac/_ref/jaspar/MA0633.1.pfm
--rw-r--r--   0        0        0      272 2023-02-20 20:04:01.170033 muon-0.1.5/muon/_atac/_ref/jaspar/MA0634.1.pfm
--rw-r--r--   0        0        0      272 2023-02-20 20:04:01.170169 muon-0.1.5/muon/_atac/_ref/jaspar/MA0635.1.pfm
--rw-r--r--   0        0        0      270 2023-02-20 20:04:01.170404 muon-0.1.5/muon/_atac/_ref/jaspar/MA0636.1.pfm
--rw-r--r--   0        0        0      407 2023-02-20 20:04:01.170543 muon-0.1.5/muon/_atac/_ref/jaspar/MA0637.1.pfm
--rw-r--r--   0        0        0      377 2023-02-20 20:04:01.170680 muon-0.1.5/muon/_atac/_ref/jaspar/MA0638.1.pfm
--rw-r--r--   0        0        0      328 2023-02-20 20:04:01.170835 muon-0.1.5/muon/_atac/_ref/jaspar/MA0639.1.pfm
--rw-r--r--   0        0        0      388 2023-02-20 20:04:01.170962 muon-0.1.5/muon/_atac/_ref/jaspar/MA0640.2.pfm
--rw-r--r--   0        0        0      324 2023-02-20 20:04:01.171090 muon-0.1.5/muon/_atac/_ref/jaspar/MA0641.1.pfm
--rw-r--r--   0        0        0      268 2023-02-20 20:04:01.171220 muon-0.1.5/muon/_atac/_ref/jaspar/MA0642.1.pfm
--rw-r--r--   0        0        0      273 2023-02-20 20:04:01.171496 muon-0.1.5/muon/_atac/_ref/jaspar/MA0643.1.pfm
--rw-r--r--   0        0        0      273 2023-02-20 20:04:01.171673 muon-0.1.5/muon/_atac/_ref/jaspar/MA0644.1.pfm
--rw-r--r--   0        0        0      272 2023-02-20 20:04:01.171821 muon-0.1.5/muon/_atac/_ref/jaspar/MA0645.1.pfm
--rw-r--r--   0        0        0      300 2023-02-20 20:04:01.171958 muon-0.1.5/muon/_atac/_ref/jaspar/MA0646.1.pfm
--rw-r--r--   0        0        0      325 2023-02-20 20:04:01.172098 muon-0.1.5/muon/_atac/_ref/jaspar/MA0647.1.pfm
--rw-r--r--   0        0        0      271 2023-02-20 20:04:01.172232 muon-0.1.5/muon/_atac/_ref/jaspar/MA0648.1.pfm
--rw-r--r--   0        0        0      268 2023-02-20 20:04:01.172364 muon-0.1.5/muon/_atac/_ref/jaspar/MA0649.1.pfm
--rw-r--r--   0        0        0      295 2023-02-20 20:04:01.172489 muon-0.1.5/muon/_atac/_ref/jaspar/MA0650.2.pfm
--rw-r--r--   0        0        0      297 2023-02-20 20:04:01.172628 muon-0.1.5/muon/_atac/_ref/jaspar/MA0651.1.pfm
--rw-r--r--   0        0        0      383 2023-02-20 20:04:01.172839 muon-0.1.5/muon/_atac/_ref/jaspar/MA0652.1.pfm
--rw-r--r--   0        0        0      407 2023-02-20 20:04:01.172988 muon-0.1.5/muon/_atac/_ref/jaspar/MA0653.1.pfm
--rw-r--r--   0        0        0      212 2023-02-20 20:04:01.173125 muon-0.1.5/muon/_atac/_ref/jaspar/MA0654.1.pfm
--rw-r--r--   0        0        0      238 2023-02-20 20:04:01.173267 muon-0.1.5/muon/_atac/_ref/jaspar/MA0655.1.pfm
--rw-r--r--   0        0        0      329 2023-02-20 20:04:01.173418 muon-0.1.5/muon/_atac/_ref/jaspar/MA0656.1.pfm
--rw-r--r--   0        0        0      493 2023-02-20 20:04:01.173560 muon-0.1.5/muon/_atac/_ref/jaspar/MA0657.1.pfm
--rw-r--r--   0        0        0      270 2023-02-20 20:04:01.173804 muon-0.1.5/muon/_atac/_ref/jaspar/MA0658.1.pfm
--rw-r--r--   0        0        0      412 2023-02-20 20:04:01.173966 muon-0.1.5/muon/_atac/_ref/jaspar/MA0659.2.pfm
--rw-r--r--   0        0        0      325 2023-02-20 20:04:01.174124 muon-0.1.5/muon/_atac/_ref/jaspar/MA0660.1.pfm
--rw-r--r--   0        0        0      268 2023-02-20 20:04:01.174260 muon-0.1.5/muon/_atac/_ref/jaspar/MA0661.1.pfm
--rw-r--r--   0        0        0      272 2023-02-20 20:04:01.174396 muon-0.1.5/muon/_atac/_ref/jaspar/MA0662.1.pfm
--rw-r--r--   0        0        0      265 2023-02-20 20:04:01.174604 muon-0.1.5/muon/_atac/_ref/jaspar/MA0663.1.pfm
--rw-r--r--   0        0        0      267 2023-02-20 20:04:01.174781 muon-0.1.5/muon/_atac/_ref/jaspar/MA0664.1.pfm
--rw-r--r--   0        0        0      262 2023-02-20 20:04:01.174955 muon-0.1.5/muon/_atac/_ref/jaspar/MA0665.1.pfm
--rw-r--r--   0        0        0      213 2023-02-20 20:04:01.175095 muon-0.1.5/muon/_atac/_ref/jaspar/MA0666.1.pfm
--rw-r--r--   0        0        0      264 2023-02-20 20:04:01.175229 muon-0.1.5/muon/_atac/_ref/jaspar/MA0667.1.pfm
--rw-r--r--   0        0        0      267 2023-02-20 20:04:01.175401 muon-0.1.5/muon/_atac/_ref/jaspar/MA0668.1.pfm
--rw-r--r--   0        0        0      264 2023-02-20 20:04:01.175571 muon-0.1.5/muon/_atac/_ref/jaspar/MA0669.1.pfm
--rw-r--r--   0        0        0      276 2023-02-20 20:04:01.175727 muon-0.1.5/muon/_atac/_ref/jaspar/MA0670.1.pfm
--rw-r--r--   0        0        0      244 2023-02-20 20:04:01.175867 muon-0.1.5/muon/_atac/_ref/jaspar/MA0671.1.pfm
--rw-r--r--   0        0        0      272 2023-02-20 20:04:01.175993 muon-0.1.5/muon/_atac/_ref/jaspar/MA0672.1.pfm
--rw-r--r--   0        0        0      243 2023-02-20 20:04:01.176116 muon-0.1.5/muon/_atac/_ref/jaspar/MA0673.1.pfm
--rw-r--r--   0        0        0      212 2023-02-20 20:04:01.176250 muon-0.1.5/muon/_atac/_ref/jaspar/MA0674.1.pfm
--rw-r--r--   0        0        0      216 2023-02-20 20:04:01.176388 muon-0.1.5/muon/_atac/_ref/jaspar/MA0675.1.pfm
--rw-r--r--   0        0        0      241 2023-02-20 20:04:01.176522 muon-0.1.5/muon/_atac/_ref/jaspar/MA0676.1.pfm
--rw-r--r--   0        0        0      378 2023-02-20 20:04:01.176722 muon-0.1.5/muon/_atac/_ref/jaspar/MA0677.1.pfm
--rw-r--r--   0        0        0      268 2023-02-20 20:04:01.176948 muon-0.1.5/muon/_atac/_ref/jaspar/MA0678.1.pfm
--rw-r--r--   0        0        0      444 2023-02-20 20:04:01.177157 muon-0.1.5/muon/_atac/_ref/jaspar/MA0679.2.pfm
--rw-r--r--   0        0        0      267 2023-02-20 20:04:01.177358 muon-0.1.5/muon/_atac/_ref/jaspar/MA0680.1.pfm
--rw-r--r--   0        0        0      442 2023-02-20 20:04:01.177563 muon-0.1.5/muon/_atac/_ref/jaspar/MA0681.2.pfm
--rw-r--r--   0        0        0      216 2023-02-20 20:04:01.177763 muon-0.1.5/muon/_atac/_ref/jaspar/MA0682.2.pfm
--rw-r--r--   0        0        0      437 2023-02-20 20:04:01.177896 muon-0.1.5/muon/_atac/_ref/jaspar/MA0683.1.pfm
--rw-r--r--   0        0        0      328 2023-02-20 20:04:01.178029 muon-0.1.5/muon/_atac/_ref/jaspar/MA0684.2.pfm
--rw-r--r--   0        0        0      466 2023-02-20 20:04:01.178213 muon-0.1.5/muon/_atac/_ref/jaspar/MA0685.1.pfm
--rw-r--r--   0        0        0      297 2023-02-20 20:04:01.178389 muon-0.1.5/muon/_atac/_ref/jaspar/MA0686.1.pfm
--rw-r--r--   0        0        0      377 2023-02-20 20:04:01.178534 muon-0.1.5/muon/_atac/_ref/jaspar/MA0687.1.pfm
--rw-r--r--   0        0        0      297 2023-02-20 20:04:01.178676 muon-0.1.5/muon/_atac/_ref/jaspar/MA0688.1.pfm
--rw-r--r--   0        0        0      294 2023-02-20 20:04:01.178813 muon-0.1.5/muon/_atac/_ref/jaspar/MA0689.1.pfm
--rw-r--r--   0        0        0      269 2023-02-20 20:04:01.179025 muon-0.1.5/muon/_atac/_ref/jaspar/MA0690.1.pfm
--rw-r--r--   0        0        0      269 2023-02-20 20:04:01.179242 muon-0.1.5/muon/_atac/_ref/jaspar/MA0691.1.pfm
--rw-r--r--   0        0        0      271 2023-02-20 20:04:01.179437 muon-0.1.5/muon/_atac/_ref/jaspar/MA0692.1.pfm
--rw-r--r--   0        0        0      211 2023-02-20 20:04:01.179612 muon-0.1.5/muon/_atac/_ref/jaspar/MA0693.2.pfm
--rw-r--r--   0        0        0      324 2023-02-20 20:04:01.179747 muon-0.1.5/muon/_atac/_ref/jaspar/MA0694.1.pfm
--rw-r--r--   0        0        0      324 2023-02-20 20:04:01.179892 muon-0.1.5/muon/_atac/_ref/jaspar/MA0695.1.pfm
--rw-r--r--   0        0        0      385 2023-02-20 20:04:01.180043 muon-0.1.5/muon/_atac/_ref/jaspar/MA0696.1.pfm
--rw-r--r--   0        0        0      405 2023-02-20 20:04:01.180186 muon-0.1.5/muon/_atac/_ref/jaspar/MA0697.1.pfm
--rw-r--r--   0        0        0      356 2023-02-20 20:04:01.180340 muon-0.1.5/muon/_atac/_ref/jaspar/MA0698.1.pfm
--rw-r--r--   0        0        0      268 2023-02-20 20:04:01.180559 muon-0.1.5/muon/_atac/_ref/jaspar/MA0699.1.pfm
--rw-r--r--   0        0        0      299 2023-02-20 20:04:01.180728 muon-0.1.5/muon/_atac/_ref/jaspar/MA0700.2.pfm
--rw-r--r--   0        0        0      215 2023-02-20 20:04:01.180873 muon-0.1.5/muon/_atac/_ref/jaspar/MA0701.2.pfm
--rw-r--r--   0        0        0      213 2023-02-20 20:04:01.181019 muon-0.1.5/muon/_atac/_ref/jaspar/MA0702.2.pfm
--rw-r--r--   0        0        0      297 2023-02-20 20:04:01.181138 muon-0.1.5/muon/_atac/_ref/jaspar/MA0703.2.pfm
--rw-r--r--   0        0        0      213 2023-02-20 20:04:01.181257 muon-0.1.5/muon/_atac/_ref/jaspar/MA0704.1.pfm
--rw-r--r--   0        0        0      214 2023-02-20 20:04:01.181388 muon-0.1.5/muon/_atac/_ref/jaspar/MA0705.1.pfm
--rw-r--r--   0        0        0      272 2023-02-20 20:04:01.181560 muon-0.1.5/muon/_atac/_ref/jaspar/MA0706.1.pfm
--rw-r--r--   0        0        0      267 2023-02-20 20:04:01.181849 muon-0.1.5/muon/_atac/_ref/jaspar/MA0707.1.pfm
--rw-r--r--   0        0        0      213 2023-02-20 20:04:01.182009 muon-0.1.5/muon/_atac/_ref/jaspar/MA0708.1.pfm
--rw-r--r--   0        0        0      216 2023-02-20 20:04:01.182143 muon-0.1.5/muon/_atac/_ref/jaspar/MA0709.1.pfm
--rw-r--r--   0        0        0      272 2023-02-20 20:04:01.182287 muon-0.1.5/muon/_atac/_ref/jaspar/MA0710.1.pfm
--rw-r--r--   0        0        0      216 2023-02-20 20:04:01.182426 muon-0.1.5/muon/_atac/_ref/jaspar/MA0711.1.pfm
--rw-r--r--   0        0        0      332 2023-02-20 20:04:01.182570 muon-0.1.5/muon/_atac/_ref/jaspar/MA0712.2.pfm
--rw-r--r--   0        0        0      300 2023-02-20 20:04:01.182694 muon-0.1.5/muon/_atac/_ref/jaspar/MA0713.1.pfm
--rw-r--r--   0        0        0      244 2023-02-20 20:04:01.182807 muon-0.1.5/muon/_atac/_ref/jaspar/MA0714.1.pfm
--rw-r--r--   0        0        0      293 2023-02-20 20:04:01.183050 muon-0.1.5/muon/_atac/_ref/jaspar/MA0715.1.pfm
--rw-r--r--   0        0        0      216 2023-02-20 20:04:01.183230 muon-0.1.5/muon/_atac/_ref/jaspar/MA0716.1.pfm
--rw-r--r--   0        0        0      218 2023-02-20 20:04:01.183378 muon-0.1.5/muon/_atac/_ref/jaspar/MA0717.1.pfm
--rw-r--r--   0        0        0      268 2023-02-20 20:04:01.183511 muon-0.1.5/muon/_atac/_ref/jaspar/MA0718.1.pfm
--rw-r--r--   0        0        0      216 2023-02-20 20:04:01.183644 muon-0.1.5/muon/_atac/_ref/jaspar/MA0719.1.pfm
--rw-r--r--   0        0        0      216 2023-02-20 20:04:01.183773 muon-0.1.5/muon/_atac/_ref/jaspar/MA0720.1.pfm
--rw-r--r--   0        0        0      218 2023-02-20 20:04:01.183902 muon-0.1.5/muon/_atac/_ref/jaspar/MA0721.1.pfm
--rw-r--r--   0        0        0      214 2023-02-20 20:04:01.184028 muon-0.1.5/muon/_atac/_ref/jaspar/MA0722.1.pfm
--rw-r--r--   0        0        0      215 2023-02-20 20:04:01.184155 muon-0.1.5/muon/_atac/_ref/jaspar/MA0723.1.pfm
--rw-r--r--   0        0        0      244 2023-02-20 20:04:01.184338 muon-0.1.5/muon/_atac/_ref/jaspar/MA0724.1.pfm
--rw-r--r--   0        0        0      214 2023-02-20 20:04:01.184494 muon-0.1.5/muon/_atac/_ref/jaspar/MA0725.1.pfm
--rw-r--r--   0        0        0      214 2023-02-20 20:04:01.184645 muon-0.1.5/muon/_atac/_ref/jaspar/MA0726.1.pfm
--rw-r--r--   0        0        0      470 2023-02-20 20:04:01.184809 muon-0.1.5/muon/_atac/_ref/jaspar/MA0727.1.pfm
--rw-r--r--   0        0        0      405 2023-02-20 20:04:01.184970 muon-0.1.5/muon/_atac/_ref/jaspar/MA0728.1.pfm
--rw-r--r--   0        0        0      488 2023-02-20 20:04:01.185132 muon-0.1.5/muon/_atac/_ref/jaspar/MA0729.1.pfm
--rw-r--r--   0        0        0      462 2023-02-20 20:04:01.185282 muon-0.1.5/muon/_atac/_ref/jaspar/MA0730.1.pfm
--rw-r--r--   0        0        0      459 2023-02-20 20:04:01.185439 muon-0.1.5/muon/_atac/_ref/jaspar/MA0731.1.pfm
--rw-r--r--   0        0        0      408 2023-02-20 20:04:01.185635 muon-0.1.5/muon/_atac/_ref/jaspar/MA0732.1.pfm
--rw-r--r--   0        0        0      440 2023-02-20 20:04:01.185940 muon-0.1.5/muon/_atac/_ref/jaspar/MA0733.1.pfm
--rw-r--r--   0        0        0      412 2023-02-20 20:04:01.186130 muon-0.1.5/muon/_atac/_ref/jaspar/MA0734.2.pfm
--rw-r--r--   0        0        0      438 2023-02-20 20:04:01.186280 muon-0.1.5/muon/_atac/_ref/jaspar/MA0735.1.pfm
--rw-r--r--   0        0        0      379 2023-02-20 20:04:01.186418 muon-0.1.5/muon/_atac/_ref/jaspar/MA0736.1.pfm
--rw-r--r--   0        0        0      377 2023-02-20 20:04:01.186550 muon-0.1.5/muon/_atac/_ref/jaspar/MA0737.1.pfm
--rw-r--r--   0        0        0      242 2023-02-20 20:04:01.186682 muon-0.1.5/muon/_atac/_ref/jaspar/MA0738.1.pfm
--rw-r--r--   0        0        0      242 2023-02-20 20:04:01.186814 muon-0.1.5/muon/_atac/_ref/jaspar/MA0739.1.pfm
--rw-r--r--   0        0        0      380 2023-02-20 20:04:01.186995 muon-0.1.5/muon/_atac/_ref/jaspar/MA0740.1.pfm
--rw-r--r--   0        0        0      297 2023-02-20 20:04:01.187203 muon-0.1.5/muon/_atac/_ref/jaspar/MA0741.1.pfm
--rw-r--r--   0        0        0      408 2023-02-20 20:04:01.187364 muon-0.1.5/muon/_atac/_ref/jaspar/MA0742.1.pfm
--rw-r--r--   0        0        0      444 2023-02-20 20:04:01.187578 muon-0.1.5/muon/_atac/_ref/jaspar/MA0743.2.pfm
--rw-r--r--   0        0        0      444 2023-02-20 20:04:01.187879 muon-0.1.5/muon/_atac/_ref/jaspar/MA0744.2.pfm
--rw-r--r--   0        0        0      359 2023-02-20 20:04:01.188048 muon-0.1.5/muon/_atac/_ref/jaspar/MA0745.2.pfm
--rw-r--r--   0        0        0      356 2023-02-20 20:04:01.188200 muon-0.1.5/muon/_atac/_ref/jaspar/MA0746.2.pfm
--rw-r--r--   0        0        0      320 2023-02-20 20:04:01.188338 muon-0.1.5/muon/_atac/_ref/jaspar/MA0747.1.pfm
--rw-r--r--   0        0        0      300 2023-02-20 20:04:01.188589 muon-0.1.5/muon/_atac/_ref/jaspar/MA0748.2.pfm
--rw-r--r--   0        0        0      354 2023-02-20 20:04:01.188780 muon-0.1.5/muon/_atac/_ref/jaspar/MA0749.1.pfm
--rw-r--r--   0        0        0      356 2023-02-20 20:04:01.188999 muon-0.1.5/muon/_atac/_ref/jaspar/MA0750.2.pfm
--rw-r--r--   0        0        0      410 2023-02-20 20:04:01.189286 muon-0.1.5/muon/_atac/_ref/jaspar/MA0751.1.pfm
--rw-r--r--   0        0        0      465 2023-02-20 20:04:01.189565 muon-0.1.5/muon/_atac/_ref/jaspar/MA0752.1.pfm
--rw-r--r--   0        0        0      352 2023-02-20 20:04:01.189744 muon-0.1.5/muon/_atac/_ref/jaspar/MA0753.2.pfm
--rw-r--r--   0        0        0      273 2023-02-20 20:04:01.189886 muon-0.1.5/muon/_atac/_ref/jaspar/MA0754.1.pfm
--rw-r--r--   0        0        0      273 2023-02-20 20:04:01.190120 muon-0.1.5/muon/_atac/_ref/jaspar/MA0755.1.pfm
--rw-r--r--   0        0        0      381 2023-02-20 20:04:01.190364 muon-0.1.5/muon/_atac/_ref/jaspar/MA0756.1.pfm
--rw-r--r--   0        0        0      383 2023-02-20 20:04:01.190526 muon-0.1.5/muon/_atac/_ref/jaspar/MA0757.1.pfm
--rw-r--r--   0        0        0      379 2023-02-20 20:04:01.190700 muon-0.1.5/muon/_atac/_ref/jaspar/MA0758.1.pfm
--rw-r--r--   0        0        0      269 2023-02-20 20:04:01.190886 muon-0.1.5/muon/_atac/_ref/jaspar/MA0759.1.pfm
--rw-r--r--   0        0        0      263 2023-02-20 20:04:01.191053 muon-0.1.5/muon/_atac/_ref/jaspar/MA0760.1.pfm
--rw-r--r--   0        0        0      385 2023-02-20 20:04:01.191190 muon-0.1.5/muon/_atac/_ref/jaspar/MA0761.2.pfm
--rw-r--r--   0        0        0      297 2023-02-20 20:04:01.191323 muon-0.1.5/muon/_atac/_ref/jaspar/MA0762.1.pfm
--rw-r--r--   0        0        0      265 2023-02-20 20:04:01.191469 muon-0.1.5/muon/_atac/_ref/jaspar/MA0763.1.pfm
--rw-r--r--   0        0        0      272 2023-02-20 20:04:01.191616 muon-0.1.5/muon/_atac/_ref/jaspar/MA0764.2.pfm
--rw-r--r--   0        0        0      300 2023-02-20 20:04:01.191801 muon-0.1.5/muon/_atac/_ref/jaspar/MA0765.2.pfm
--rw-r--r--   0        0        0      272 2023-02-20 20:04:01.191945 muon-0.1.5/muon/_atac/_ref/jaspar/MA0766.2.pfm
--rw-r--r--   0        0        0      268 2023-02-20 20:04:01.192072 muon-0.1.5/muon/_atac/_ref/jaspar/MA0767.1.pfm
--rw-r--r--   0        0        0      408 2023-02-20 20:04:01.192259 muon-0.1.5/muon/_atac/_ref/jaspar/MA0768.1.pfm
--rw-r--r--   0        0        0      300 2023-02-20 20:04:01.192520 muon-0.1.5/muon/_atac/_ref/jaspar/MA0769.2.pfm
--rw-r--r--   0        0        0      351 2023-02-20 20:04:01.192696 muon-0.1.5/muon/_atac/_ref/jaspar/MA0770.1.pfm
--rw-r--r--   0        0        0      357 2023-02-20 20:04:01.192838 muon-0.1.5/muon/_atac/_ref/jaspar/MA0771.1.pfm
--rw-r--r--   0        0        0      379 2023-02-20 20:04:01.192976 muon-0.1.5/muon/_atac/_ref/jaspar/MA0772.1.pfm
--rw-r--r--   0        0        0      327 2023-02-20 20:04:01.193108 muon-0.1.5/muon/_atac/_ref/jaspar/MA0773.1.pfm
--rw-r--r--   0        0        0      213 2023-02-20 20:04:01.193240 muon-0.1.5/muon/_atac/_ref/jaspar/MA0774.1.pfm
--rw-r--r--   0        0        0      214 2023-02-20 20:04:01.193384 muon-0.1.5/muon/_atac/_ref/jaspar/MA0775.1.pfm
--rw-r--r--   0        0        0      324 2023-02-20 20:04:01.193580 muon-0.1.5/muon/_atac/_ref/jaspar/MA0776.1.pfm
--rw-r--r--   0        0        0      406 2023-02-20 20:04:01.193801 muon-0.1.5/muon/_atac/_ref/jaspar/MA0777.1.pfm
--rw-r--r--   0        0        0      356 2023-02-20 20:04:01.193956 muon-0.1.5/muon/_atac/_ref/jaspar/MA0778.1.pfm
--rw-r--r--   0        0        0      466 2023-02-20 20:04:01.194172 muon-0.1.5/muon/_atac/_ref/jaspar/MA0779.1.pfm
--rw-r--r--   0        0        0      270 2023-02-20 20:04:01.194405 muon-0.1.5/muon/_atac/_ref/jaspar/MA0780.1.pfm
--rw-r--r--   0        0        0      466 2023-02-20 20:04:01.194678 muon-0.1.5/muon/_atac/_ref/jaspar/MA0781.1.pfm
--rw-r--r--   0        0        0      413 2023-02-20 20:04:01.194916 muon-0.1.5/muon/_atac/_ref/jaspar/MA0782.2.pfm
--rw-r--r--   0        0        0      320 2023-02-20 20:04:01.195134 muon-0.1.5/muon/_atac/_ref/jaspar/MA0783.1.pfm
--rw-r--r--   0        0        0      381 2023-02-20 20:04:01.195299 muon-0.1.5/muon/_atac/_ref/jaspar/MA0784.1.pfm
--rw-r--r--   0        0        0      328 2023-02-20 20:04:01.195543 muon-0.1.5/muon/_atac/_ref/jaspar/MA0785.1.pfm
--rw-r--r--   0        0        0      326 2023-02-20 20:04:01.195767 muon-0.1.5/muon/_atac/_ref/jaspar/MA0786.1.pfm
--rw-r--r--   0        0        0      323 2023-02-20 20:04:01.195998 muon-0.1.5/muon/_atac/_ref/jaspar/MA0787.1.pfm
--rw-r--r--   0        0        0      351 2023-02-20 20:04:01.196179 muon-0.1.5/muon/_atac/_ref/jaspar/MA0788.1.pfm
--rw-r--r--   0        0        0      242 2023-02-20 20:04:01.196372 muon-0.1.5/muon/_atac/_ref/jaspar/MA0789.1.pfm
--rw-r--r--   0        0        0      383 2023-02-20 20:04:01.196577 muon-0.1.5/muon/_atac/_ref/jaspar/MA0790.1.pfm
--rw-r--r--   0        0        0      437 2023-02-20 20:04:01.196760 muon-0.1.5/muon/_atac/_ref/jaspar/MA0791.1.pfm
--rw-r--r--   0        0        0      243 2023-02-20 20:04:01.196917 muon-0.1.5/muon/_atac/_ref/jaspar/MA0792.1.pfm
--rw-r--r--   0        0        0      269 2023-02-20 20:04:01.197158 muon-0.1.5/muon/_atac/_ref/jaspar/MA0793.1.pfm
--rw-r--r--   0        0        0      326 2023-02-20 20:04:01.197360 muon-0.1.5/muon/_atac/_ref/jaspar/MA0794.1.pfm
--rw-r--r--   0        0        0      269 2023-02-20 20:04:01.197516 muon-0.1.5/muon/_atac/_ref/jaspar/MA0795.1.pfm
--rw-r--r--   0        0        0      322 2023-02-20 20:04:01.197664 muon-0.1.5/muon/_atac/_ref/jaspar/MA0796.1.pfm
--rw-r--r--   0        0        0      326 2023-02-20 20:04:01.197825 muon-0.1.5/muon/_atac/_ref/jaspar/MA0797.1.pfm
--rw-r--r--   0        0        0      382 2023-02-20 20:04:01.197963 muon-0.1.5/muon/_atac/_ref/jaspar/MA0798.2.pfm
--rw-r--r--   0        0        0      440 2023-02-20 20:04:01.198125 muon-0.1.5/muon/_atac/_ref/jaspar/MA0799.1.pfm
--rw-r--r--   0        0        0      355 2023-02-20 20:04:01.198260 muon-0.1.5/muon/_atac/_ref/jaspar/MA0800.1.pfm
--rw-r--r--   0        0        0      217 2023-02-20 20:04:01.198393 muon-0.1.5/muon/_atac/_ref/jaspar/MA0801.1.pfm
--rw-r--r--   0        0        0      272 2023-02-20 20:04:01.198518 muon-0.1.5/muon/_atac/_ref/jaspar/MA0802.1.pfm
--rw-r--r--   0        0        0      213 2023-02-20 20:04:01.198633 muon-0.1.5/muon/_atac/_ref/jaspar/MA0803.1.pfm
--rw-r--r--   0        0        0      554 2023-02-20 20:04:01.198752 muon-0.1.5/muon/_atac/_ref/jaspar/MA0804.1.pfm
--rw-r--r--   0        0        0      215 2023-02-20 20:04:01.198875 muon-0.1.5/muon/_atac/_ref/jaspar/MA0805.1.pfm
--rw-r--r--   0        0        0      216 2023-02-20 20:04:01.199006 muon-0.1.5/muon/_atac/_ref/jaspar/MA0806.1.pfm
--rw-r--r--   0        0        0      212 2023-02-20 20:04:01.199144 muon-0.1.5/muon/_atac/_ref/jaspar/MA0807.1.pfm
--rw-r--r--   0        0        0      215 2023-02-20 20:04:01.199276 muon-0.1.5/muon/_atac/_ref/jaspar/MA0808.1.pfm
--rw-r--r--   0        0        0      332 2023-02-20 20:04:01.199401 muon-0.1.5/muon/_atac/_ref/jaspar/MA0809.2.pfm
--rw-r--r--   0        0        0      326 2023-02-20 20:04:01.199557 muon-0.1.5/muon/_atac/_ref/jaspar/MA0810.1.pfm
--rw-r--r--   0        0        0      325 2023-02-20 20:04:01.199782 muon-0.1.5/muon/_atac/_ref/jaspar/MA0811.1.pfm
--rw-r--r--   0        0        0      299 2023-02-20 20:04:01.199922 muon-0.1.5/muon/_atac/_ref/jaspar/MA0812.1.pfm
--rw-r--r--   0        0        0      351 2023-02-20 20:04:01.200054 muon-0.1.5/muon/_atac/_ref/jaspar/MA0813.1.pfm
--rw-r--r--   0        0        0      388 2023-02-20 20:04:01.200175 muon-0.1.5/muon/_atac/_ref/jaspar/MA0814.2.pfm
--rw-r--r--   0        0        0      353 2023-02-20 20:04:01.200304 muon-0.1.5/muon/_atac/_ref/jaspar/MA0815.1.pfm
--rw-r--r--   0        0        0      265 2023-02-20 20:04:01.200435 muon-0.1.5/muon/_atac/_ref/jaspar/MA0816.1.pfm
--rw-r--r--   0        0        0      325 2023-02-20 20:04:01.200560 muon-0.1.5/muon/_atac/_ref/jaspar/MA0817.1.pfm
--rw-r--r--   0        0        0      266 2023-02-20 20:04:01.200687 muon-0.1.5/muon/_atac/_ref/jaspar/MA0818.1.pfm
--rw-r--r--   0        0        0      265 2023-02-20 20:04:01.200836 muon-0.1.5/muon/_atac/_ref/jaspar/MA0819.1.pfm
--rw-r--r--   0        0        0      268 2023-02-20 20:04:01.200962 muon-0.1.5/muon/_atac/_ref/jaspar/MA0820.1.pfm
--rw-r--r--   0        0        0      323 2023-02-20 20:04:01.201086 muon-0.1.5/muon/_atac/_ref/jaspar/MA0821.1.pfm
--rw-r--r--   0        0        0      323 2023-02-20 20:04:01.201218 muon-0.1.5/muon/_atac/_ref/jaspar/MA0822.1.pfm
--rw-r--r--   0        0        0      269 2023-02-20 20:04:01.201352 muon-0.1.5/muon/_atac/_ref/jaspar/MA0823.1.pfm
--rw-r--r--   0        0        0      268 2023-02-20 20:04:01.201480 muon-0.1.5/muon/_atac/_ref/jaspar/MA0825.1.pfm
--rw-r--r--   0        0        0      271 2023-02-20 20:04:01.201600 muon-0.1.5/muon/_atac/_ref/jaspar/MA0826.1.pfm
--rw-r--r--   0        0        0      269 2023-02-20 20:04:01.201715 muon-0.1.5/muon/_atac/_ref/jaspar/MA0827.1.pfm
--rw-r--r--   0        0        0      269 2023-02-20 20:04:01.201847 muon-0.1.5/muon/_atac/_ref/jaspar/MA0828.1.pfm
--rw-r--r--   0        0        0      384 2023-02-20 20:04:01.202022 muon-0.1.5/muon/_atac/_ref/jaspar/MA0829.2.pfm
--rw-r--r--   0        0        0      357 2023-02-20 20:04:01.202193 muon-0.1.5/muon/_atac/_ref/jaspar/MA0830.2.pfm
--rw-r--r--   0        0        0      206 2023-02-20 20:04:01.202358 muon-0.1.5/muon/_atac/_ref/jaspar/MA0831.2.pfm
--rw-r--r--   0        0        0      376 2023-02-20 20:04:01.202531 muon-0.1.5/muon/_atac/_ref/jaspar/MA0832.1.pfm
--rw-r--r--   0        0        0      385 2023-02-20 20:04:01.202702 muon-0.1.5/muon/_atac/_ref/jaspar/MA0833.2.pfm
--rw-r--r--   0        0        0      384 2023-02-20 20:04:01.202870 muon-0.1.5/muon/_atac/_ref/jaspar/MA0834.1.pfm
--rw-r--r--   0        0        0      300 2023-02-20 20:04:01.203039 muon-0.1.5/muon/_atac/_ref/jaspar/MA0835.2.pfm
--rw-r--r--   0        0        0      356 2023-02-20 20:04:01.203207 muon-0.1.5/muon/_atac/_ref/jaspar/MA0836.2.pfm
--rw-r--r--   0        0        0      270 2023-02-20 20:04:01.203380 muon-0.1.5/muon/_atac/_ref/jaspar/MA0837.1.pfm
--rw-r--r--   0        0        0      272 2023-02-20 20:04:01.203533 muon-0.1.5/muon/_atac/_ref/jaspar/MA0838.1.pfm
--rw-r--r--   0        0        0      380 2023-02-20 20:04:01.203650 muon-0.1.5/muon/_atac/_ref/jaspar/MA0839.1.pfm
--rw-r--r--   0        0        0      326 2023-02-20 20:04:01.203772 muon-0.1.5/muon/_atac/_ref/jaspar/MA0840.1.pfm
--rw-r--r--   0        0        0      299 2023-02-20 20:04:01.203894 muon-0.1.5/muon/_atac/_ref/jaspar/MA0841.1.pfm
--rw-r--r--   0        0        0      357 2023-02-20 20:04:01.204023 muon-0.1.5/muon/_atac/_ref/jaspar/MA0842.2.pfm
--rw-r--r--   0        0        0      326 2023-02-20 20:04:01.204152 muon-0.1.5/muon/_atac/_ref/jaspar/MA0843.1.pfm
--rw-r--r--   0        0        0      382 2023-02-20 20:04:01.204282 muon-0.1.5/muon/_atac/_ref/jaspar/MA0844.1.pfm
--rw-r--r--   0        0        0      298 2023-02-20 20:04:01.204431 muon-0.1.5/muon/_atac/_ref/jaspar/MA0845.1.pfm
--rw-r--r--   0        0        0      328 2023-02-20 20:04:01.204569 muon-0.1.5/muon/_atac/_ref/jaspar/MA0846.1.pfm
--rw-r--r--   0        0        0      355 2023-02-20 20:04:01.204779 muon-0.1.5/muon/_atac/_ref/jaspar/MA0847.2.pfm
--rw-r--r--   0        0        0      183 2023-02-20 20:04:01.204926 muon-0.1.5/muon/_atac/_ref/jaspar/MA0848.1.pfm
--rw-r--r--   0        0        0      182 2023-02-20 20:04:01.205058 muon-0.1.5/muon/_atac/_ref/jaspar/MA0849.1.pfm
--rw-r--r--   0        0        0      179 2023-02-20 20:04:01.205175 muon-0.1.5/muon/_atac/_ref/jaspar/MA0850.1.pfm
--rw-r--r--   0        0        0      460 2023-02-20 20:04:01.205376 muon-0.1.5/muon/_atac/_ref/jaspar/MA0851.1.pfm
--rw-r--r--   0        0        0      380 2023-02-20 20:04:01.205566 muon-0.1.5/muon/_atac/_ref/jaspar/MA0852.2.pfm
--rw-r--r--   0        0        0      460 2023-02-20 20:04:01.205714 muon-0.1.5/muon/_atac/_ref/jaspar/MA0853.1.pfm
--rw-r--r--   0        0        0      460 2023-02-20 20:04:01.205917 muon-0.1.5/muon/_atac/_ref/jaspar/MA0854.1.pfm
--rw-r--r--   0        0        0      382 2023-02-20 20:04:01.206068 muon-0.1.5/muon/_atac/_ref/jaspar/MA0855.1.pfm
--rw-r--r--   0        0        0      385 2023-02-20 20:04:01.206209 muon-0.1.5/muon/_atac/_ref/jaspar/MA0856.1.pfm
--rw-r--r--   0        0        0      437 2023-02-20 20:04:01.206385 muon-0.1.5/muon/_atac/_ref/jaspar/MA0857.1.pfm
--rw-r--r--   0        0        0      459 2023-02-20 20:04:01.206619 muon-0.1.5/muon/_atac/_ref/jaspar/MA0858.1.pfm
--rw-r--r--   0        0        0      442 2023-02-20 20:04:01.206756 muon-0.1.5/muon/_atac/_ref/jaspar/MA0859.1.pfm
--rw-r--r--   0        0        0      463 2023-02-20 20:04:01.206883 muon-0.1.5/muon/_atac/_ref/jaspar/MA0860.1.pfm
--rw-r--r--   0        0        0      495 2023-02-20 20:04:01.207013 muon-0.1.5/muon/_atac/_ref/jaspar/MA0861.1.pfm
--rw-r--r--   0        0        0      210 2023-02-20 20:04:01.207146 muon-0.1.5/muon/_atac/_ref/jaspar/MA0862.1.pfm
--rw-r--r--   0        0        0      373 2023-02-20 20:04:01.207344 muon-0.1.5/muon/_atac/_ref/jaspar/MA0863.1.pfm
--rw-r--r--   0        0        0      438 2023-02-20 20:04:01.207504 muon-0.1.5/muon/_atac/_ref/jaspar/MA0864.2.pfm
--rw-r--r--   0        0        0      317 2023-02-20 20:04:01.207654 muon-0.1.5/muon/_atac/_ref/jaspar/MA0865.1.pfm
--rw-r--r--   0        0        0      409 2023-02-20 20:04:01.207796 muon-0.1.5/muon/_atac/_ref/jaspar/MA0866.1.pfm
--rw-r--r--   0        0        0      272 2023-02-20 20:04:01.207934 muon-0.1.5/muon/_atac/_ref/jaspar/MA0867.2.pfm
--rw-r--r--   0        0        0      270 2023-02-20 20:04:01.208203 muon-0.1.5/muon/_atac/_ref/jaspar/MA0868.2.pfm
--rw-r--r--   0        0        0      402 2023-02-20 20:04:01.208350 muon-0.1.5/muon/_atac/_ref/jaspar/MA0869.1.pfm
--rw-r--r--   0        0        0      409 2023-02-20 20:04:01.208496 muon-0.1.5/muon/_atac/_ref/jaspar/MA0870.1.pfm
--rw-r--r--   0        0        0      300 2023-02-20 20:04:01.208721 muon-0.1.5/muon/_atac/_ref/jaspar/MA0871.2.pfm
--rw-r--r--   0        0        0      352 2023-02-20 20:04:01.208953 muon-0.1.5/muon/_atac/_ref/jaspar/MA0872.1.pfm
--rw-r--r--   0        0        0      295 2023-02-20 20:04:01.209114 muon-0.1.5/muon/_atac/_ref/jaspar/MA0873.1.pfm
--rw-r--r--   0        0        0      460 2023-02-20 20:04:01.209250 muon-0.1.5/muon/_atac/_ref/jaspar/MA0874.1.pfm
--rw-r--r--   0        0        0      215 2023-02-20 20:04:01.209379 muon-0.1.5/muon/_atac/_ref/jaspar/MA0875.1.pfm
--rw-r--r--   0        0        0      216 2023-02-20 20:04:01.209507 muon-0.1.5/muon/_atac/_ref/jaspar/MA0876.1.pfm
--rw-r--r--   0        0        0      214 2023-02-20 20:04:01.209634 muon-0.1.5/muon/_atac/_ref/jaspar/MA0877.2.pfm
--rw-r--r--   0        0        0      300 2023-02-20 20:04:01.209751 muon-0.1.5/muon/_atac/_ref/jaspar/MA0878.2.pfm
--rw-r--r--   0        0        0      272 2023-02-20 20:04:01.209865 muon-0.1.5/muon/_atac/_ref/jaspar/MA0879.1.pfm
--rw-r--r--   0        0        0      216 2023-02-20 20:04:01.210067 muon-0.1.5/muon/_atac/_ref/jaspar/MA0880.1.pfm
--rw-r--r--   0        0        0      216 2023-02-20 20:04:01.210218 muon-0.1.5/muon/_atac/_ref/jaspar/MA0881.1.pfm
--rw-r--r--   0        0        0      212 2023-02-20 20:04:01.210410 muon-0.1.5/muon/_atac/_ref/jaspar/MA0882.1.pfm
--rw-r--r--   0        0        0      460 2023-02-20 20:04:01.210677 muon-0.1.5/muon/_atac/_ref/jaspar/MA0883.1.pfm
--rw-r--r--   0        0        0      352 2023-02-20 20:04:01.210956 muon-0.1.5/muon/_atac/_ref/jaspar/MA0884.1.pfm
--rw-r--r--   0        0        0      216 2023-02-20 20:04:01.211122 muon-0.1.5/muon/_atac/_ref/jaspar/MA0885.1.pfm
--rw-r--r--   0        0        0      274 2023-02-20 20:04:01.211264 muon-0.1.5/muon/_atac/_ref/jaspar/MA0886.1.pfm
--rw-r--r--   0        0        0      272 2023-02-20 20:04:01.211396 muon-0.1.5/muon/_atac/_ref/jaspar/MA0887.1.pfm
--rw-r--r--   0        0        0      272 2023-02-20 20:04:01.211536 muon-0.1.5/muon/_atac/_ref/jaspar/MA0888.1.pfm
--rw-r--r--   0        0        0      273 2023-02-20 20:04:01.211664 muon-0.1.5/muon/_atac/_ref/jaspar/MA0889.1.pfm
--rw-r--r--   0        0        0      273 2023-02-20 20:04:01.211820 muon-0.1.5/muon/_atac/_ref/jaspar/MA0890.1.pfm
--rw-r--r--   0        0        0      268 2023-02-20 20:04:01.212028 muon-0.1.5/muon/_atac/_ref/jaspar/MA0891.1.pfm
--rw-r--r--   0        0        0      268 2023-02-20 20:04:01.212192 muon-0.1.5/muon/_atac/_ref/jaspar/MA0892.1.pfm
--rw-r--r--   0        0        0      212 2023-02-20 20:04:01.212329 muon-0.1.5/muon/_atac/_ref/jaspar/MA0893.2.pfm
--rw-r--r--   0        0        0      269 2023-02-20 20:04:01.212465 muon-0.1.5/muon/_atac/_ref/jaspar/MA0894.1.pfm
--rw-r--r--   0        0        0      268 2023-02-20 20:04:01.212652 muon-0.1.5/muon/_atac/_ref/jaspar/MA0895.1.pfm
--rw-r--r--   0        0        0      460 2023-02-20 20:04:01.212802 muon-0.1.5/muon/_atac/_ref/jaspar/MA0896.1.pfm
--rw-r--r--   0        0        0      459 2023-02-20 20:04:01.212929 muon-0.1.5/muon/_atac/_ref/jaspar/MA0897.1.pfm
--rw-r--r--   0        0        0      459 2023-02-20 20:04:01.213056 muon-0.1.5/muon/_atac/_ref/jaspar/MA0898.1.pfm
--rw-r--r--   0        0        0      300 2023-02-20 20:04:01.213295 muon-0.1.5/muon/_atac/_ref/jaspar/MA0899.1.pfm
--rw-r--r--   0        0        0      218 2023-02-20 20:04:01.213460 muon-0.1.5/muon/_atac/_ref/jaspar/MA0900.2.pfm
--rw-r--r--   0        0        0      388 2023-02-20 20:04:01.213605 muon-0.1.5/muon/_atac/_ref/jaspar/MA0901.2.pfm
--rw-r--r--   0        0        0      215 2023-02-20 20:04:01.213738 muon-0.1.5/muon/_atac/_ref/jaspar/MA0902.2.pfm
--rw-r--r--   0        0        0      272 2023-02-20 20:04:01.213872 muon-0.1.5/muon/_atac/_ref/jaspar/MA0903.1.pfm
--rw-r--r--   0        0        0      214 2023-02-20 20:04:01.214007 muon-0.1.5/muon/_atac/_ref/jaspar/MA0904.2.pfm
--rw-r--r--   0        0        0      270 2023-02-20 20:04:01.214172 muon-0.1.5/muon/_atac/_ref/jaspar/MA0905.1.pfm
--rw-r--r--   0        0        0      298 2023-02-20 20:04:01.214294 muon-0.1.5/muon/_atac/_ref/jaspar/MA0906.1.pfm
--rw-r--r--   0        0        0      296 2023-02-20 20:04:01.214412 muon-0.1.5/muon/_atac/_ref/jaspar/MA0907.1.pfm
--rw-r--r--   0        0        0      265 2023-02-20 20:04:01.214617 muon-0.1.5/muon/_atac/_ref/jaspar/MA0908.1.pfm
--rw-r--r--   0        0        0      294 2023-02-20 20:04:01.214761 muon-0.1.5/muon/_atac/_ref/jaspar/MA0909.2.pfm
--rw-r--r--   0        0        0      213 2023-02-20 20:04:01.214894 muon-0.1.5/muon/_atac/_ref/jaspar/MA0910.2.pfm
--rw-r--r--   0        0        0      324 2023-02-20 20:04:01.215021 muon-0.1.5/muon/_atac/_ref/jaspar/MA0911.1.pfm
--rw-r--r--   0        0        0      215 2023-02-20 20:04:01.215149 muon-0.1.5/muon/_atac/_ref/jaspar/MA0912.2.pfm
--rw-r--r--   0        0        0      271 2023-02-20 20:04:01.215277 muon-0.1.5/muon/_atac/_ref/jaspar/MA0913.2.pfm
--rw-r--r--   0        0        0      216 2023-02-20 20:04:01.215401 muon-0.1.5/muon/_atac/_ref/jaspar/MA0914.1.pfm
--rw-r--r--   0        0        0      273 2023-02-20 20:04:01.215528 muon-0.1.5/muon/_atac/_ref/jaspar/MA1099.2.pfm
--rw-r--r--   0        0        0      270 2023-02-20 20:04:01.215690 muon-0.1.5/muon/_atac/_ref/jaspar/MA1100.2.pfm
--rw-r--r--   0        0        0      528 2023-02-20 20:04:01.215823 muon-0.1.5/muon/_atac/_ref/jaspar/MA1101.2.pfm
--rw-r--r--   0        0        0      328 2023-02-20 20:04:01.215949 muon-0.1.5/muon/_atac/_ref/jaspar/MA1102.2.pfm
--rw-r--r--   0        0        0      300 2023-02-20 20:04:01.216081 muon-0.1.5/muon/_atac/_ref/jaspar/MA1103.2.pfm
--rw-r--r--   0        0        0      360 2023-02-20 20:04:01.216217 muon-0.1.5/muon/_atac/_ref/jaspar/MA1104.2.pfm
--rw-r--r--   0        0        0      329 2023-02-20 20:04:01.216357 muon-0.1.5/muon/_atac/_ref/jaspar/MA1105.2.pfm
--rw-r--r--   0        0        0      268 2023-02-20 20:04:01.216486 muon-0.1.5/muon/_atac/_ref/jaspar/MA1106.1.pfm
--rw-r--r--   0        0        0      441 2023-02-20 20:04:01.216613 muon-0.1.5/muon/_atac/_ref/jaspar/MA1107.2.pfm
--rw-r--r--   0        0        0      272 2023-02-20 20:04:01.216804 muon-0.1.5/muon/_atac/_ref/jaspar/MA1108.2.pfm
--rw-r--r--   0        0        0      352 2023-02-20 20:04:01.216975 muon-0.1.5/muon/_atac/_ref/jaspar/MA1109.1.pfm
--rw-r--r--   0        0        0      294 2023-02-20 20:04:01.217115 muon-0.1.5/muon/_atac/_ref/jaspar/MA1110.1.pfm
--rw-r--r--   0        0        0      296 2023-02-20 20:04:01.217242 muon-0.1.5/muon/_atac/_ref/jaspar/MA1111.1.pfm
--rw-r--r--   0        0        0      328 2023-02-20 20:04:01.217369 muon-0.1.5/muon/_atac/_ref/jaspar/MA1112.2.pfm
--rw-r--r--   0        0        0      356 2023-02-20 20:04:01.217501 muon-0.1.5/muon/_atac/_ref/jaspar/MA1113.2.pfm
--rw-r--r--   0        0        0      468 2023-02-20 20:04:01.217631 muon-0.1.5/muon/_atac/_ref/jaspar/MA1114.1.pfm
--rw-r--r--   0        0        0      300 2023-02-20 20:04:01.217853 muon-0.1.5/muon/_atac/_ref/jaspar/MA1115.1.pfm
--rw-r--r--   0        0        0      268 2023-02-20 20:04:01.217997 muon-0.1.5/muon/_atac/_ref/jaspar/MA1116.1.pfm
--rw-r--r--   0        0        0      297 2023-02-20 20:04:01.218147 muon-0.1.5/muon/_atac/_ref/jaspar/MA1117.1.pfm
--rw-r--r--   0        0        0      294 2023-02-20 20:04:01.218277 muon-0.1.5/muon/_atac/_ref/jaspar/MA1118.1.pfm
--rw-r--r--   0        0        0      440 2023-02-20 20:04:01.218405 muon-0.1.5/muon/_atac/_ref/jaspar/MA1119.1.pfm
--rw-r--r--   0        0        0      298 2023-02-20 20:04:01.218539 muon-0.1.5/muon/_atac/_ref/jaspar/MA1120.1.pfm
--rw-r--r--   0        0        0      352 2023-02-20 20:04:01.218658 muon-0.1.5/muon/_atac/_ref/jaspar/MA1121.1.pfm
--rw-r--r--   0        0        0      296 2023-02-20 20:04:01.218775 muon-0.1.5/muon/_atac/_ref/jaspar/MA1122.1.pfm
--rw-r--r--   0        0        0      356 2023-02-20 20:04:01.218901 muon-0.1.5/muon/_atac/_ref/jaspar/MA1123.2.pfm
--rw-r--r--   0        0        0      357 2023-02-20 20:04:01.219029 muon-0.1.5/muon/_atac/_ref/jaspar/MA1124.1.pfm
--rw-r--r--   0        0        0      329 2023-02-20 20:04:01.219161 muon-0.1.5/muon/_atac/_ref/jaspar/MA1125.1.pfm
--rw-r--r--   0        0        0      435 2023-02-20 20:04:01.219353 muon-0.1.5/muon/_atac/_ref/jaspar/MA1126.1.pfm
--rw-r--r--   0        0        0      295 2023-02-20 20:04:01.219496 muon-0.1.5/muon/_atac/_ref/jaspar/MA1127.1.pfm
--rw-r--r--   0        0        0      352 2023-02-20 20:04:01.219632 muon-0.1.5/muon/_atac/_ref/jaspar/MA1128.1.pfm
--rw-r--r--   0        0        0      266 2023-02-20 20:04:01.219764 muon-0.1.5/muon/_atac/_ref/jaspar/MA1129.1.pfm
--rw-r--r--   0        0        0      324 2023-02-20 20:04:01.219895 muon-0.1.5/muon/_atac/_ref/jaspar/MA1130.1.pfm
--rw-r--r--   0        0        0      295 2023-02-20 20:04:01.220027 muon-0.1.5/muon/_atac/_ref/jaspar/MA1131.1.pfm
--rw-r--r--   0        0        0      268 2023-02-20 20:04:01.220140 muon-0.1.5/muon/_atac/_ref/jaspar/MA1132.1.pfm
--rw-r--r--   0        0        0      323 2023-02-20 20:04:01.220312 muon-0.1.5/muon/_atac/_ref/jaspar/MA1133.1.pfm
--rw-r--r--   0        0        0      324 2023-02-20 20:04:01.220567 muon-0.1.5/muon/_atac/_ref/jaspar/MA1134.1.pfm
--rw-r--r--   0        0        0      268 2023-02-20 20:04:01.220715 muon-0.1.5/muon/_atac/_ref/jaspar/MA1135.1.pfm
--rw-r--r--   0        0        0      266 2023-02-20 20:04:01.220955 muon-0.1.5/muon/_atac/_ref/jaspar/MA1136.1.pfm
--rw-r--r--   0        0        0      352 2023-02-20 20:04:01.221115 muon-0.1.5/muon/_atac/_ref/jaspar/MA1137.1.pfm
--rw-r--r--   0        0        0      268 2023-02-20 20:04:01.221324 muon-0.1.5/muon/_atac/_ref/jaspar/MA1138.1.pfm
--rw-r--r--   0        0        0      324 2023-02-20 20:04:01.221579 muon-0.1.5/muon/_atac/_ref/jaspar/MA1139.1.pfm
--rw-r--r--   0        0        0      321 2023-02-20 20:04:01.221785 muon-0.1.5/muon/_atac/_ref/jaspar/MA1140.2.pfm
--rw-r--r--   0        0        0      352 2023-02-20 20:04:01.221952 muon-0.1.5/muon/_atac/_ref/jaspar/MA1141.1.pfm
--rw-r--r--   0        0        0      268 2023-02-20 20:04:01.222102 muon-0.1.5/muon/_atac/_ref/jaspar/MA1142.1.pfm
--rw-r--r--   0        0        0      266 2023-02-20 20:04:01.222248 muon-0.1.5/muon/_atac/_ref/jaspar/MA1143.1.pfm
--rw-r--r--   0        0        0      268 2023-02-20 20:04:01.222406 muon-0.1.5/muon/_atac/_ref/jaspar/MA1144.1.pfm
--rw-r--r--   0        0        0      408 2023-02-20 20:04:01.222597 muon-0.1.5/muon/_atac/_ref/jaspar/MA1145.1.pfm
--rw-r--r--   0        0        0      408 2023-02-20 20:04:01.222733 muon-0.1.5/muon/_atac/_ref/jaspar/MA1146.1.pfm
--rw-r--r--   0        0        0      408 2023-02-20 20:04:01.223033 muon-0.1.5/muon/_atac/_ref/jaspar/MA1147.1.pfm
--rw-r--r--   0        0        0      492 2023-02-20 20:04:01.223217 muon-0.1.5/muon/_atac/_ref/jaspar/MA1148.1.pfm
--rw-r--r--   0        0        0      492 2023-02-20 20:04:01.223509 muon-0.1.5/muon/_atac/_ref/jaspar/MA1149.1.pfm
--rw-r--r--   0        0        0      294 2023-02-20 20:04:01.223666 muon-0.1.5/muon/_atac/_ref/jaspar/MA1150.1.pfm
--rw-r--r--   0        0        0      324 2023-02-20 20:04:01.223804 muon-0.1.5/muon/_atac/_ref/jaspar/MA1151.1.pfm
--rw-r--r--   0        0        0      267 2023-02-20 20:04:01.223945 muon-0.1.5/muon/_atac/_ref/jaspar/MA1152.1.pfm
--rw-r--r--   0        0        0      210 2023-02-20 20:04:01.224175 muon-0.1.5/muon/_atac/_ref/jaspar/MA1153.1.pfm
--rw-r--r--   0        0        0      461 2023-02-20 20:04:01.224372 muon-0.1.5/muon/_atac/_ref/jaspar/MA1154.1.pfm
--rw-r--r--   0        0        0      409 2023-02-20 20:04:01.224519 muon-0.1.5/muon/_atac/_ref/jaspar/MA1155.1.pfm
--rw-r--r--   0        0        0      580 2023-02-20 20:04:01.224658 muon-0.1.5/muon/_atac/_ref/jaspar/MA1418.1.pfm
--rw-r--r--   0        0        0      415 2023-02-20 20:04:01.224792 muon-0.1.5/muon/_atac/_ref/jaspar/MA1419.1.pfm
--rw-r--r--   0        0        0      377 2023-02-20 20:04:01.224911 muon-0.1.5/muon/_atac/_ref/jaspar/MA1420.1.pfm
--rw-r--r--   0        0        0      320 2023-02-20 20:04:01.225024 muon-0.1.5/muon/_atac/_ref/jaspar/MA1421.1.pfm
--rw-r--r--   0        0        0      272 2023-02-20 20:04:01.225135 muon-0.1.5/muon/_atac/_ref/jaspar/MA1463.1.pfm
--rw-r--r--   0        0        0      274 2023-02-20 20:04:01.225280 muon-0.1.5/muon/_atac/_ref/jaspar/MA1464.1.pfm
--rw-r--r--   0        0        0      379 2023-02-20 20:04:01.225410 muon-0.1.5/muon/_atac/_ref/jaspar/MA1466.1.pfm
--rw-r--r--   0        0        0      267 2023-02-20 20:04:01.225535 muon-0.1.5/muon/_atac/_ref/jaspar/MA1467.1.pfm
--rw-r--r--   0        0        0      266 2023-02-20 20:04:01.225663 muon-0.1.5/muon/_atac/_ref/jaspar/MA1468.1.pfm
--rw-r--r--   0        0        0      545 2023-02-20 20:04:01.225797 muon-0.1.5/muon/_atac/_ref/jaspar/MA1470.1.pfm
--rw-r--r--   0        0        0      328 2023-02-20 20:04:01.225931 muon-0.1.5/muon/_atac/_ref/jaspar/MA1471.1.pfm
--rw-r--r--   0        0        0      268 2023-02-20 20:04:01.226062 muon-0.1.5/muon/_atac/_ref/jaspar/MA1472.1.pfm
--rw-r--r--   0        0        0      301 2023-02-20 20:04:01.226195 muon-0.1.5/muon/_atac/_ref/jaspar/MA1473.1.pfm
--rw-r--r--   0        0        0      326 2023-02-20 20:04:01.226324 muon-0.1.5/muon/_atac/_ref/jaspar/MA1474.1.pfm
--rw-r--r--   0        0        0      324 2023-02-20 20:04:01.226454 muon-0.1.5/muon/_atac/_ref/jaspar/MA1475.1.pfm
--rw-r--r--   0        0        0      216 2023-02-20 20:04:01.226575 muon-0.1.5/muon/_atac/_ref/jaspar/MA1476.1.pfm
--rw-r--r--   0        0        0      324 2023-02-20 20:04:01.226692 muon-0.1.5/muon/_atac/_ref/jaspar/MA1478.1.pfm
--rw-r--r--   0        0        0      323 2023-02-20 20:04:01.226818 muon-0.1.5/muon/_atac/_ref/jaspar/MA1479.1.pfm
--rw-r--r--   0        0        0      271 2023-02-20 20:04:01.226943 muon-0.1.5/muon/_atac/_ref/jaspar/MA1480.1.pfm
--rw-r--r--   0        0        0      216 2023-02-20 20:04:01.227067 muon-0.1.5/muon/_atac/_ref/jaspar/MA1481.1.pfm
--rw-r--r--   0        0        0      328 2023-02-20 20:04:01.227192 muon-0.1.5/muon/_atac/_ref/jaspar/MA1483.1.pfm
--rw-r--r--   0        0        0      272 2023-02-20 20:04:01.227321 muon-0.1.5/muon/_atac/_ref/jaspar/MA1484.1.pfm
--rw-r--r--   0        0        0      382 2023-02-20 20:04:01.227465 muon-0.1.5/muon/_atac/_ref/jaspar/MA1485.1.pfm
--rw-r--r--   0        0        0      407 2023-02-20 20:04:01.227621 muon-0.1.5/muon/_atac/_ref/jaspar/MA1487.1.pfm
--rw-r--r--   0        0        0      206 2023-02-20 20:04:01.227747 muon-0.1.5/muon/_atac/_ref/jaspar/MA1489.1.pfm
--rw-r--r--   0        0        0      412 2023-02-20 20:04:01.227875 muon-0.1.5/muon/_atac/_ref/jaspar/MA1491.1.pfm
--rw-r--r--   0        0        0      265 2023-02-20 20:04:01.227992 muon-0.1.5/muon/_atac/_ref/jaspar/MA1493.1.pfm
--rw-r--r--   0        0        0      406 2023-02-20 20:04:01.228102 muon-0.1.5/muon/_atac/_ref/jaspar/MA1494.1.pfm
--rw-r--r--   0        0        0      216 2023-02-20 20:04:01.228234 muon-0.1.5/muon/_atac/_ref/jaspar/MA1495.1.pfm
--rw-r--r--   0        0        0      213 2023-02-20 20:04:01.228360 muon-0.1.5/muon/_atac/_ref/jaspar/MA1496.1.pfm
--rw-r--r--   0        0        0      272 2023-02-20 20:04:01.228484 muon-0.1.5/muon/_atac/_ref/jaspar/MA1497.1.pfm
--rw-r--r--   0        0        0      213 2023-02-20 20:04:01.228626 muon-0.1.5/muon/_atac/_ref/jaspar/MA1498.1.pfm
--rw-r--r--   0        0        0      216 2023-02-20 20:04:01.228743 muon-0.1.5/muon/_atac/_ref/jaspar/MA1499.1.pfm
--rw-r--r--   0        0        0      216 2023-02-20 20:04:01.228869 muon-0.1.5/muon/_atac/_ref/jaspar/MA1500.1.pfm
--rw-r--r--   0        0        0      268 2023-02-20 20:04:01.228988 muon-0.1.5/muon/_atac/_ref/jaspar/MA1501.1.pfm
--rw-r--r--   0        0        0      213 2023-02-20 20:04:01.229112 muon-0.1.5/muon/_atac/_ref/jaspar/MA1502.1.pfm
--rw-r--r--   0        0        0      267 2023-02-20 20:04:01.229232 muon-0.1.5/muon/_atac/_ref/jaspar/MA1503.1.pfm
--rw-r--r--   0        0        0      216 2023-02-20 20:04:01.229356 muon-0.1.5/muon/_atac/_ref/jaspar/MA1504.1.pfm
--rw-r--r--   0        0        0      216 2023-02-20 20:04:01.229479 muon-0.1.5/muon/_atac/_ref/jaspar/MA1505.1.pfm
--rw-r--r--   0        0        0      298 2023-02-20 20:04:01.229615 muon-0.1.5/muon/_atac/_ref/jaspar/MA1506.1.pfm
--rw-r--r--   0        0        0      214 2023-02-20 20:04:01.229793 muon-0.1.5/muon/_atac/_ref/jaspar/MA1507.1.pfm
--rw-r--r--   0        0        0      328 2023-02-20 20:04:01.229937 muon-0.1.5/muon/_atac/_ref/jaspar/MA1508.1.pfm
--rw-r--r--   0        0        0      240 2023-02-20 20:04:01.230073 muon-0.1.5/muon/_atac/_ref/jaspar/MA1509.1.pfm
--rw-r--r--   0        0        0      301 2023-02-20 20:04:01.230206 muon-0.1.5/muon/_atac/_ref/jaspar/MA1511.1.pfm
--rw-r--r--   0        0        0      300 2023-02-20 20:04:01.230346 muon-0.1.5/muon/_atac/_ref/jaspar/MA1512.1.pfm
--rw-r--r--   0        0        0      300 2023-02-20 20:04:01.230489 muon-0.1.5/muon/_atac/_ref/jaspar/MA1513.1.pfm
--rw-r--r--   0        0        0      413 2023-02-20 20:04:01.230629 muon-0.1.5/muon/_atac/_ref/jaspar/MA1514.1.pfm
--rw-r--r--   0        0        0      299 2023-02-20 20:04:01.230765 muon-0.1.5/muon/_atac/_ref/jaspar/MA1515.1.pfm
--rw-r--r--   0        0        0      301 2023-02-20 20:04:01.231009 muon-0.1.5/muon/_atac/_ref/jaspar/MA1516.1.pfm
--rw-r--r--   0        0        0      296 2023-02-20 20:04:01.231155 muon-0.1.5/muon/_atac/_ref/jaspar/MA1517.1.pfm
--rw-r--r--   0        0        0      216 2023-02-20 20:04:01.231338 muon-0.1.5/muon/_atac/_ref/jaspar/MA1518.1.pfm
--rw-r--r--   0        0        0      215 2023-02-20 20:04:01.231554 muon-0.1.5/muon/_atac/_ref/jaspar/MA1519.1.pfm
--rw-r--r--   0        0        0      408 2023-02-20 20:04:01.231783 muon-0.1.5/muon/_atac/_ref/jaspar/MA1520.1.pfm
--rw-r--r--   0        0        0      412 2023-02-20 20:04:01.231988 muon-0.1.5/muon/_atac/_ref/jaspar/MA1521.1.pfm
--rw-r--r--   0        0        0      300 2023-02-20 20:04:01.232242 muon-0.1.5/muon/_atac/_ref/jaspar/MA1522.1.pfm
--rw-r--r--   0        0        0      267 2023-02-20 20:04:01.232450 muon-0.1.5/muon/_atac/_ref/jaspar/MA1523.1.pfm
--rw-r--r--   0        0        0      328 2023-02-20 20:04:01.232609 muon-0.1.5/muon/_atac/_ref/jaspar/MA1524.1.pfm
--rw-r--r--   0        0        0      269 2023-02-20 20:04:01.232836 muon-0.1.5/muon/_atac/_ref/jaspar/MA1525.1.pfm
--rw-r--r--   0        0        0      464 2023-02-20 20:04:01.233044 muon-0.1.5/muon/_atac/_ref/jaspar/MA1527.1.pfm
--rw-r--r--   0        0        0      468 2023-02-20 20:04:01.233216 muon-0.1.5/muon/_atac/_ref/jaspar/MA1528.1.pfm
--rw-r--r--   0        0        0      496 2023-02-20 20:04:01.233390 muon-0.1.5/muon/_atac/_ref/jaspar/MA1529.1.pfm
--rw-r--r--   0        0        0      242 2023-02-20 20:04:01.233547 muon-0.1.5/muon/_atac/_ref/jaspar/MA1530.1.pfm
--rw-r--r--   0        0        0      409 2023-02-20 20:04:01.233681 muon-0.1.5/muon/_atac/_ref/jaspar/MA1531.1.pfm
--rw-r--r--   0        0        0      407 2023-02-20 20:04:01.233825 muon-0.1.5/muon/_atac/_ref/jaspar/MA1532.1.pfm
--rw-r--r--   0        0        0      460 2023-02-20 20:04:01.233948 muon-0.1.5/muon/_atac/_ref/jaspar/MA1533.1.pfm
--rw-r--r--   0        0        0      246 2023-02-20 20:04:01.234116 muon-0.1.5/muon/_atac/_ref/jaspar/MA1534.1.pfm
--rw-r--r--   0        0        0      244 2023-02-20 20:04:01.234297 muon-0.1.5/muon/_atac/_ref/jaspar/MA1535.1.pfm
--rw-r--r--   0        0        0      216 2023-02-20 20:04:01.234459 muon-0.1.5/muon/_atac/_ref/jaspar/MA1536.1.pfm
--rw-r--r--   0        0        0      414 2023-02-20 20:04:01.234596 muon-0.1.5/muon/_atac/_ref/jaspar/MA1537.1.pfm
--rw-r--r--   0        0        0      410 2023-02-20 20:04:01.234729 muon-0.1.5/muon/_atac/_ref/jaspar/MA1538.1.pfm
--rw-r--r--   0        0        0      410 2023-02-20 20:04:01.234866 muon-0.1.5/muon/_atac/_ref/jaspar/MA1539.1.pfm
--rw-r--r--   0        0        0      298 2023-02-20 20:04:01.235136 muon-0.1.5/muon/_atac/_ref/jaspar/MA1540.1.pfm
--rw-r--r--   0        0        0      464 2023-02-20 20:04:01.235358 muon-0.1.5/muon/_atac/_ref/jaspar/MA1541.1.pfm
--rw-r--r--   0        0        0      271 2023-02-20 20:04:01.235515 muon-0.1.5/muon/_atac/_ref/jaspar/MA1542.1.pfm
--rw-r--r--   0        0        0      384 2023-02-20 20:04:01.235678 muon-0.1.5/muon/_atac/_ref/jaspar/MA1544.1.pfm
--rw-r--r--   0        0        0      356 2023-02-20 20:04:01.235820 muon-0.1.5/muon/_atac/_ref/jaspar/MA1545.1.pfm
--rw-r--r--   0        0        0      436 2023-02-20 20:04:01.235994 muon-0.1.5/muon/_atac/_ref/jaspar/MA1546.1.pfm
--rw-r--r--   0        0        0      216 2023-02-20 20:04:01.236132 muon-0.1.5/muon/_atac/_ref/jaspar/MA1547.1.pfm
--rw-r--r--   0        0        0      268 2023-02-20 20:04:01.236257 muon-0.1.5/muon/_atac/_ref/jaspar/MA1548.1.pfm
--rw-r--r--   0        0        0      271 2023-02-20 20:04:01.236385 muon-0.1.5/muon/_atac/_ref/jaspar/MA1549.1.pfm
--rw-r--r--   0        0        0      440 2023-02-20 20:04:01.236513 muon-0.1.5/muon/_atac/_ref/jaspar/MA1550.1.pfm
--rw-r--r--   0        0        0      378 2023-02-20 20:04:01.236638 muon-0.1.5/muon/_atac/_ref/jaspar/MA1552.1.pfm
--rw-r--r--   0        0        0      381 2023-02-20 20:04:01.236755 muon-0.1.5/muon/_atac/_ref/jaspar/MA1553.1.pfm
--rw-r--r--   0        0        0      236 2023-02-20 20:04:01.236870 muon-0.1.5/muon/_atac/_ref/jaspar/MA1554.1.pfm
--rw-r--r--   0        0        0      380 2023-02-20 20:04:01.237080 muon-0.1.5/muon/_atac/_ref/jaspar/MA1555.1.pfm
--rw-r--r--   0        0        0      380 2023-02-20 20:04:01.237253 muon-0.1.5/muon/_atac/_ref/jaspar/MA1556.1.pfm
--rw-r--r--   0        0        0      270 2023-02-20 20:04:01.237399 muon-0.1.5/muon/_atac/_ref/jaspar/MA1557.1.pfm
--rw-r--r--   0        0        0      272 2023-02-20 20:04:01.237536 muon-0.1.5/muon/_atac/_ref/jaspar/MA1558.1.pfm
--rw-r--r--   0        0        0      271 2023-02-20 20:04:01.237661 muon-0.1.5/muon/_atac/_ref/jaspar/MA1559.1.pfm
--rw-r--r--   0        0        0      268 2023-02-20 20:04:01.237789 muon-0.1.5/muon/_atac/_ref/jaspar/MA1560.1.pfm
--rw-r--r--   0        0        0      296 2023-02-20 20:04:01.237910 muon-0.1.5/muon/_atac/_ref/jaspar/MA1561.1.pfm
--rw-r--r--   0        0        0      268 2023-02-20 20:04:01.238061 muon-0.1.5/muon/_atac/_ref/jaspar/MA1562.1.pfm
--rw-r--r--   0        0        0      211 2023-02-20 20:04:01.238263 muon-0.1.5/muon/_atac/_ref/jaspar/MA1563.1.pfm
--rw-r--r--   0        0        0      324 2023-02-20 20:04:01.238458 muon-0.1.5/muon/_atac/_ref/jaspar/MA1564.1.pfm
--rw-r--r--   0        0        0      323 2023-02-20 20:04:01.238592 muon-0.1.5/muon/_atac/_ref/jaspar/MA1565.1.pfm
--rw-r--r--   0        0        0      269 2023-02-20 20:04:01.238716 muon-0.1.5/muon/_atac/_ref/jaspar/MA1566.1.pfm
--rw-r--r--   0        0        0      272 2023-02-20 20:04:01.238852 muon-0.1.5/muon/_atac/_ref/jaspar/MA1567.1.pfm
--rw-r--r--   0        0        0      324 2023-02-20 20:04:01.239087 muon-0.1.5/muon/_atac/_ref/jaspar/MA1568.1.pfm
--rw-r--r--   0        0        0      300 2023-02-20 20:04:01.239229 muon-0.1.5/muon/_atac/_ref/jaspar/MA1569.1.pfm
--rw-r--r--   0        0        0      267 2023-02-20 20:04:01.239364 muon-0.1.5/muon/_atac/_ref/jaspar/MA1570.1.pfm
--rw-r--r--   0        0        0      325 2023-02-20 20:04:01.239603 muon-0.1.5/muon/_atac/_ref/jaspar/MA1571.1.pfm
--rw-r--r--   0        0        0      325 2023-02-20 20:04:01.239846 muon-0.1.5/muon/_atac/_ref/jaspar/MA1572.1.pfm
--rw-r--r--   0        0        0      518 2023-02-20 20:04:01.240037 muon-0.1.5/muon/_atac/_ref/jaspar/MA1573.1.pfm
--rw-r--r--   0        0        0      412 2023-02-20 20:04:01.240254 muon-0.1.5/muon/_atac/_ref/jaspar/MA1574.1.pfm
--rw-r--r--   0        0        0      522 2023-02-20 20:04:01.240427 muon-0.1.5/muon/_atac/_ref/jaspar/MA1575.1.pfm
--rw-r--r--   0        0        0      518 2023-02-20 20:04:01.240572 muon-0.1.5/muon/_atac/_ref/jaspar/MA1576.1.pfm
--rw-r--r--   0        0        0      215 2023-02-20 20:04:01.240712 muon-0.1.5/muon/_atac/_ref/jaspar/MA1577.1.pfm
--rw-r--r--   0        0        0      265 2023-02-20 20:04:01.240996 muon-0.1.5/muon/_atac/_ref/jaspar/MA1578.1.pfm
--rw-r--r--   0        0        0      408 2023-02-20 20:04:01.241200 muon-0.1.5/muon/_atac/_ref/jaspar/MA1579.1.pfm
--rw-r--r--   0        0        0      268 2023-02-20 20:04:01.241367 muon-0.1.5/muon/_atac/_ref/jaspar/MA1580.1.pfm
--rw-r--r--   0        0        0      352 2023-02-20 20:04:01.241515 muon-0.1.5/muon/_atac/_ref/jaspar/MA1581.1.pfm
--rw-r--r--   0        0        0      356 2023-02-20 20:04:01.241650 muon-0.1.5/muon/_atac/_ref/jaspar/MA1583.1.pfm
--rw-r--r--   0        0        0      440 2023-02-20 20:04:01.241783 muon-0.1.5/muon/_atac/_ref/jaspar/MA1584.1.pfm
--rw-r--r--   0        0        0      269 2023-02-20 20:04:01.241906 muon-0.1.5/muon/_atac/_ref/jaspar/MA1585.1.pfm
--rw-r--r--   0        0        0      379 2023-02-20 20:04:01.242022 muon-0.1.5/muon/_atac/_ref/jaspar/MA1587.1.pfm
--rw-r--r--   0        0        0      410 2023-02-20 20:04:01.242148 muon-0.1.5/muon/_atac/_ref/jaspar/MA1588.1.pfm
--rw-r--r--   0        0        0      576 2023-02-20 20:04:01.242272 muon-0.1.5/muon/_atac/_ref/jaspar/MA1589.1.pfm
--rw-r--r--   0        0        0      440 2023-02-20 20:04:01.242475 muon-0.1.5/muon/_atac/_ref/jaspar/MA1592.1.pfm
--rw-r--r--   0        0        0      328 2023-02-20 20:04:01.242638 muon-0.1.5/muon/_atac/_ref/jaspar/MA1593.1.pfm
--rw-r--r--   0        0        0      661 2023-02-20 20:04:01.242800 muon-0.1.5/muon/_atac/_ref/jaspar/MA1594.1.pfm
--rw-r--r--   0        0        0      436 2023-02-20 20:04:01.242947 muon-0.1.5/muon/_atac/_ref/jaspar/MA1596.1.pfm
--rw-r--r--   0        0        0      461 2023-02-20 20:04:01.243086 muon-0.1.5/muon/_atac/_ref/jaspar/MA1597.1.pfm
--rw-r--r--   0        0        0      436 2023-02-20 20:04:01.243217 muon-0.1.5/muon/_atac/_ref/jaspar/MA1599.1.pfm
--rw-r--r--   0        0        0      492 2023-02-20 20:04:01.243339 muon-0.1.5/muon/_atac/_ref/jaspar/MA1600.1.pfm
--rw-r--r--   0        0        0      272 2023-02-20 20:04:01.243472 muon-0.1.5/muon/_atac/_ref/jaspar/MA1601.1.pfm
--rw-r--r--   0        0        0      323 2023-02-20 20:04:01.243708 muon-0.1.5/muon/_atac/_ref/jaspar/MA1602.1.pfm
--rw-r--r--   0        0        0      357 2023-02-20 20:04:01.243925 muon-0.1.5/muon/_atac/_ref/jaspar/MA1603.1.pfm
--rw-r--r--   0        0        0      356 2023-02-20 20:04:01.244186 muon-0.1.5/muon/_atac/_ref/jaspar/MA1604.1.pfm
--rw-r--r--   0        0        0      304 2023-02-20 20:04:01.244357 muon-0.1.5/muon/_atac/_ref/jaspar/MA1606.1.pfm
--rw-r--r--   0        0        0      384 2023-02-20 20:04:01.244526 muon-0.1.5/muon/_atac/_ref/jaspar/MA1607.1.pfm
--rw-r--r--   0        0        0      300 2023-02-20 20:04:01.244667 muon-0.1.5/muon/_atac/_ref/jaspar/MA1608.1.pfm
--rw-r--r--   0        0        0      356 2023-02-20 20:04:01.244842 muon-0.1.5/muon/_atac/_ref/jaspar/MA1615.1.pfm
--rw-r--r--   0        0        0      408 2023-02-20 20:04:01.244965 muon-0.1.5/muon/_atac/_ref/jaspar/MA1616.1.pfm
--rw-r--r--   0        0        0      356 2023-02-20 20:04:01.245084 muon-0.1.5/muon/_atac/_ref/jaspar/MA1618.1.pfm
--rw-r--r--   0        0        0      328 2023-02-20 20:04:01.245273 muon-0.1.5/muon/_atac/_ref/jaspar/MA1619.1.pfm
--rw-r--r--   0        0        0      328 2023-02-20 20:04:01.245445 muon-0.1.5/muon/_atac/_ref/jaspar/MA1620.1.pfm
--rw-r--r--   0        0        0      384 2023-02-20 20:04:01.245588 muon-0.1.5/muon/_atac/_ref/jaspar/MA1621.1.pfm
--rw-r--r--   0        0        0      384 2023-02-20 20:04:01.245721 muon-0.1.5/muon/_atac/_ref/jaspar/MA1622.1.pfm
--rw-r--r--   0        0        0      354 2023-02-20 20:04:01.245872 muon-0.1.5/muon/_atac/_ref/jaspar/MA1623.1.pfm
--rw-r--r--   0        0        0      327 2023-02-20 20:04:01.246015 muon-0.1.5/muon/_atac/_ref/jaspar/MA1624.1.pfm
--rw-r--r--   0        0        0      408 2023-02-20 20:04:01.246178 muon-0.1.5/muon/_atac/_ref/jaspar/MA1625.1.pfm
--rw-r--r--   0        0        0      382 2023-02-20 20:04:01.246312 muon-0.1.5/muon/_atac/_ref/jaspar/MA1627.1.pfm
--rw-r--r--   0        0        0      299 2023-02-20 20:04:01.246446 muon-0.1.5/muon/_atac/_ref/jaspar/MA1628.1.pfm
--rw-r--r--   0        0        0      384 2023-02-20 20:04:01.246617 muon-0.1.5/muon/_atac/_ref/jaspar/MA1629.1.pfm
--rw-r--r--   0        0        0      298 2023-02-20 20:04:01.246764 muon-0.1.5/muon/_atac/_ref/jaspar/MA1630.1.pfm
--rw-r--r--   0        0        0      357 2023-02-20 20:04:01.246905 muon-0.1.5/muon/_atac/_ref/jaspar/MA1631.1.pfm
--rw-r--r--   0        0        0      360 2023-02-20 20:04:01.247037 muon-0.1.5/muon/_atac/_ref/jaspar/MA1632.1.pfm
--rw-r--r--   0        0        0      356 2023-02-20 20:04:01.247164 muon-0.1.5/muon/_atac/_ref/jaspar/MA1633.1.pfm
--rw-r--r--   0        0        0      303 2023-02-20 20:04:01.247296 muon-0.1.5/muon/_atac/_ref/jaspar/MA1634.1.pfm
--rw-r--r--   0        0        0      272 2023-02-20 20:04:01.247424 muon-0.1.5/muon/_atac/_ref/jaspar/MA1635.1.pfm
--rw-r--r--   0        0        0      413 2023-02-20 20:04:01.247568 muon-0.1.5/muon/_atac/_ref/jaspar/MA1636.1.pfm
--rw-r--r--   0        0        0      356 2023-02-20 20:04:01.247736 muon-0.1.5/muon/_atac/_ref/jaspar/MA1637.1.pfm
--rw-r--r--   0        0        0      273 2023-02-20 20:04:01.247900 muon-0.1.5/muon/_atac/_ref/jaspar/MA1638.1.pfm
--rw-r--r--   0        0        0      356 2023-02-20 20:04:01.248024 muon-0.1.5/muon/_atac/_ref/jaspar/MA1639.1.pfm
--rw-r--r--   0        0        0      412 2023-02-20 20:04:01.248141 muon-0.1.5/muon/_atac/_ref/jaspar/MA1640.1.pfm
--rw-r--r--   0        0        0      328 2023-02-20 20:04:01.248265 muon-0.1.5/muon/_atac/_ref/jaspar/MA1641.1.pfm
--rw-r--r--   0        0        0      357 2023-02-20 20:04:01.248405 muon-0.1.5/muon/_atac/_ref/jaspar/MA1642.1.pfm
--rw-r--r--   0        0        0      579 2023-02-20 20:04:01.248541 muon-0.1.5/muon/_atac/_ref/jaspar/MA1643.1.pfm
--rw-r--r--   0        0        0      300 2023-02-20 20:04:01.248668 muon-0.1.5/muon/_atac/_ref/jaspar/MA1644.1.pfm
--rw-r--r--   0        0        0      384 2023-02-20 20:04:01.248889 muon-0.1.5/muon/_atac/_ref/jaspar/MA1645.1.pfm
--rw-r--r--   0        0        0      328 2023-02-20 20:04:01.249094 muon-0.1.5/muon/_atac/_ref/jaspar/MA1646.1.pfm
--rw-r--r--   0        0        0      300 2023-02-20 20:04:01.249275 muon-0.1.5/muon/_atac/_ref/jaspar/MA1647.1.pfm
--rw-r--r--   0        0        0      304 2023-02-20 20:04:01.249453 muon-0.1.5/muon/_atac/_ref/jaspar/MA1648.1.pfm
--rw-r--r--   0        0        0      299 2023-02-20 20:04:01.249627 muon-0.1.5/muon/_atac/_ref/jaspar/MA1649.1.pfm
--rw-r--r--   0        0        0      326 2023-02-20 20:04:01.249800 muon-0.1.5/muon/_atac/_ref/jaspar/MA1650.1.pfm
--rw-r--r--   0        0        0      576 2023-02-20 20:04:01.249944 muon-0.1.5/muon/_atac/_ref/jaspar/MA1651.1.pfm
--rw-r--r--   0        0        0      381 2023-02-20 20:04:01.250073 muon-0.1.5/muon/_atac/_ref/jaspar/MA1652.1.pfm
--rw-r--r--   0        0        0      328 2023-02-20 20:04:01.250202 muon-0.1.5/muon/_atac/_ref/jaspar/MA1653.1.pfm
--rw-r--r--   0        0        0      629 2023-02-20 20:04:01.250397 muon-0.1.5/muon/_atac/_ref/jaspar/MA1654.1.pfm
--rw-r--r--   0        0        0      328 2023-02-20 20:04:01.250597 muon-0.1.5/muon/_atac/_ref/jaspar/MA1655.1.pfm
--rw-r--r--   0        0        0      384 2023-02-20 20:04:01.250745 muon-0.1.5/muon/_atac/_ref/jaspar/MA1656.1.pfm
--rw-r--r--   0        0        0      328 2023-02-20 20:04:01.250891 muon-0.1.5/muon/_atac/_ref/jaspar/MA1657.1.pfm
--rw-r--r--   0        0        0      302 2023-02-20 20:04:01.251035 muon-0.1.5/muon/_atac/_ref/jaspar/MA1683.1.pfm
--rw-r--r--   0        0        0    11673 2023-02-20 20:04:01.251258 muon-0.1.5/muon/_atac/_ref/jaspar/motif_to_gene.txt
--rw-r--r--   0        0        0     4491 2023-02-20 20:04:01.251460 muon-0.1.5/muon/_atac/io.py
--rw-r--r--   0        0        0    12779 2023-06-08 08:49:54.375686 muon-0.1.5/muon/_atac/plot.py
--rw-r--r--   0        0        0     7133 2023-02-20 20:04:01.251976 muon-0.1.5/muon/_atac/preproc.py
--rw-r--r--   0        0        0    44213 2023-06-07 09:07:57.087492 muon-0.1.5/muon/_atac/tools.py
--rw-r--r--   0        0        0      316 2023-06-07 09:07:57.088441 muon-0.1.5/muon/_atac/utils.py
--rw-r--r--   0        0        0        0 2023-02-20 20:04:01.252851 muon-0.1.5/muon/_core/__init__.py
--rw-r--r--   0        0        0     2032 2023-02-20 20:04:01.252993 muon-0.1.5/muon/_core/config.py
--rw-r--r--   0        0        0     3135 2023-02-20 20:04:41.107395 muon-0.1.5/muon/_core/io.py
--rw-r--r--   0        0        0    16833 2023-06-08 08:49:54.376617 muon-0.1.5/muon/_core/plot.py
--rw-r--r--   0        0        0    35383 2023-06-07 09:07:57.090694 muon-0.1.5/muon/_core/preproc.py
--rw-r--r--   0        0        0    52375 2023-06-08 08:49:54.378345 muon-0.1.5/muon/_core/tools.py
--rw-r--r--   0        0        0     8448 2023-02-20 20:04:01.254933 muon-0.1.5/muon/_core/utils.py
--rw-r--r--   0        0        0       46 2023-02-20 20:04:01.255165 muon-0.1.5/muon/_prot/__init__.py
--rw-r--r--   0        0        0      723 2023-02-20 20:04:01.255299 muon-0.1.5/muon/_prot/io.py
--rw-r--r--   0        0        0    10314 2023-06-07 09:07:57.092293 muon-0.1.5/muon/_prot/preproc.py
--rw-r--r--   0        0        0        0 2023-02-20 20:04:01.255631 muon-0.1.5/muon/_rna/__init__.py
--rw-r--r--   0        0        0     1270 2023-02-20 20:04:01.255794 muon-0.1.5/muon/_rna/utils.py
--rw-r--r--   0        0        0       21 2023-02-20 20:04:01.255949 muon-0.1.5/muon/atac.py
--rw-r--r--   0        0        0       21 2023-02-20 20:04:01.256101 muon-0.1.5/muon/prot.py
--rw-r--r--   0        0        0       20 2023-02-20 20:04:01.256224 muon-0.1.5/muon/rna.py
--rw-r--r--   0        0        0     1242 2023-06-07 09:07:57.092944 muon-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     6313 1970-01-01 00:00:00.000000 muon-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     5701 2024-04-09 08:19:07.551543 muon-0.1.6/README.md
+-rw-r--r--   0        0        0      343 2024-04-09 08:48:27.099734 muon-0.1.6/muon/__init__.py
+-rw-r--r--   0        0        0       97 2024-04-09 08:19:07.575346 muon-0.1.6/muon/_atac/__init__.py
+-rw-r--r--   0        0        0      296 2024-04-09 08:19:07.575914 muon-0.1.6/muon/_atac/_ref/jaspar/MA0002.2.pfm
+-rw-r--r--   0        0        0      384 2024-04-09 08:19:07.576321 muon-0.1.6/muon/_atac/_ref/jaspar/MA0003.4.pfm
+-rw-r--r--   0        0        0      149 2024-04-09 08:19:07.576479 muon-0.1.6/muon/_atac/_ref/jaspar/MA0004.1.pfm
+-rw-r--r--   0        0        0      149 2024-04-09 08:19:07.576633 muon-0.1.6/muon/_atac/_ref/jaspar/MA0006.1.pfm
+-rw-r--r--   0        0        0      466 2024-04-09 08:19:07.576918 muon-0.1.6/muon/_atac/_ref/jaspar/MA0007.3.pfm
+-rw-r--r--   0        0        0      435 2024-04-09 08:19:07.577292 muon-0.1.6/muon/_atac/_ref/jaspar/MA0009.2.pfm
+-rw-r--r--   0        0        0      324 2024-04-09 08:19:07.577578 muon-0.1.6/muon/_atac/_ref/jaspar/MA0014.3.pfm
+-rw-r--r--   0        0        0      357 2024-04-09 08:19:07.577961 muon-0.1.6/muon/_atac/_ref/jaspar/MA0017.2.pfm
+-rw-r--r--   0        0        0      360 2024-04-09 08:19:07.578295 muon-0.1.6/muon/_atac/_ref/jaspar/MA0018.4.pfm
+-rw-r--r--   0        0        0      318 2024-04-09 08:19:07.578732 muon-0.1.6/muon/_atac/_ref/jaspar/MA0019.1.pfm
+-rw-r--r--   0        0        0      323 2024-04-09 08:19:07.578978 muon-0.1.6/muon/_atac/_ref/jaspar/MA0024.3.pfm
+-rw-r--r--   0        0        0      356 2024-04-09 08:19:07.579166 muon-0.1.6/muon/_atac/_ref/jaspar/MA0025.2.pfm
+-rw-r--r--   0        0        0      213 2024-04-09 08:19:07.579346 muon-0.1.6/muon/_atac/_ref/jaspar/MA0027.2.pfm
+-rw-r--r--   0        0        0      274 2024-04-09 08:19:07.579668 muon-0.1.6/muon/_atac/_ref/jaspar/MA0028.2.pfm
+-rw-r--r--   0        0        0      373 2024-04-09 08:19:07.579974 muon-0.1.6/muon/_atac/_ref/jaspar/MA0029.1.pfm
+-rw-r--r--   0        0        0      373 2024-04-09 08:19:07.580326 muon-0.1.6/muon/_atac/_ref/jaspar/MA0030.1.pfm
+-rw-r--r--   0        0        0      205 2024-04-09 08:19:07.580506 muon-0.1.6/muon/_atac/_ref/jaspar/MA0031.1.pfm
+-rw-r--r--   0        0        0      299 2024-04-09 08:19:07.580799 muon-0.1.6/muon/_atac/_ref/jaspar/MA0032.2.pfm
+-rw-r--r--   0        0        0      185 2024-04-09 08:19:07.581038 muon-0.1.6/muon/_atac/_ref/jaspar/MA0033.2.pfm
+-rw-r--r--   0        0        0      304 2024-04-09 08:19:07.581251 muon-0.1.6/muon/_atac/_ref/jaspar/MA0035.4.pfm
+-rw-r--r--   0        0        0      300 2024-04-09 08:19:07.581636 muon-0.1.6/muon/_atac/_ref/jaspar/MA0036.3.pfm
+-rw-r--r--   0        0        0      210 2024-04-09 08:19:07.583289 muon-0.1.6/muon/_atac/_ref/jaspar/MA0037.3.pfm
+-rw-r--r--   0        0        0      329 2024-04-09 08:19:07.583613 muon-0.1.6/muon/_atac/_ref/jaspar/MA0038.2.pfm
+-rw-r--r--   0        0        0      332 2024-04-09 08:19:07.583862 muon-0.1.6/muon/_atac/_ref/jaspar/MA0039.4.pfm
+-rw-r--r--   0        0        0      288 2024-04-09 08:19:07.584040 muon-0.1.6/muon/_atac/_ref/jaspar/MA0040.1.pfm
+-rw-r--r--   0        0        0      318 2024-04-09 08:19:07.584254 muon-0.1.6/muon/_atac/_ref/jaspar/MA0041.1.pfm
+-rw-r--r--   0        0        0      182 2024-04-09 08:19:07.584543 muon-0.1.6/muon/_atac/_ref/jaspar/MA0042.2.pfm
+-rw-r--r--   0        0        0      384 2024-04-09 08:19:07.584761 muon-0.1.6/muon/_atac/_ref/jaspar/MA0043.3.pfm
+-rw-r--r--   0        0        0      412 2024-04-09 08:19:07.585074 muon-0.1.6/muon/_atac/_ref/jaspar/MA0046.2.pfm
+-rw-r--r--   0        0        0      305 2024-04-09 08:19:07.585271 muon-0.1.6/muon/_atac/_ref/jaspar/MA0047.3.pfm
+-rw-r--r--   0        0        0      269 2024-04-09 08:19:07.585424 muon-0.1.6/muon/_atac/_ref/jaspar/MA0048.2.pfm
+-rw-r--r--   0        0        0      576 2024-04-09 08:19:07.585725 muon-0.1.6/muon/_atac/_ref/jaspar/MA0050.2.pfm
+-rw-r--r--   0        0        0      484 2024-04-09 08:19:07.586032 muon-0.1.6/muon/_atac/_ref/jaspar/MA0051.1.pfm
+-rw-r--r--   0        0        0      412 2024-04-09 08:19:07.586247 muon-0.1.6/muon/_atac/_ref/jaspar/MA0052.4.pfm
+-rw-r--r--   0        0        0      356 2024-04-09 08:19:07.586449 muon-0.1.6/muon/_atac/_ref/jaspar/MA0056.2.pfm
+-rw-r--r--   0        0        0      260 2024-04-09 08:19:07.586713 muon-0.1.6/muon/_atac/_ref/jaspar/MA0057.1.pfm
+-rw-r--r--   0        0        0      271 2024-04-09 08:19:07.587099 muon-0.1.6/muon/_atac/_ref/jaspar/MA0058.3.pfm
+-rw-r--r--   0        0        0      288 2024-04-09 08:19:07.587418 muon-0.1.6/muon/_atac/_ref/jaspar/MA0059.1.pfm
+-rw-r--r--   0        0        0      298 2024-04-09 08:19:07.588692 muon-0.1.6/muon/_atac/_ref/jaspar/MA0060.3.pfm
+-rw-r--r--   0        0        0      388 2024-04-09 08:19:07.588908 muon-0.1.6/muon/_atac/_ref/jaspar/MA0062.3.pfm
+-rw-r--r--   0        0        0      300 2024-04-09 08:19:07.590119 muon-0.1.6/muon/_atac/_ref/jaspar/MA0063.2.pfm
+-rw-r--r--   0        0        0      407 2024-04-09 08:19:07.591055 muon-0.1.6/muon/_atac/_ref/jaspar/MA0065.2.pfm
+-rw-r--r--   0        0        0      541 2024-04-09 08:19:07.591251 muon-0.1.6/muon/_atac/_ref/jaspar/MA0066.1.pfm
+-rw-r--r--   0        0        0      205 2024-04-09 08:19:07.591402 muon-0.1.6/muon/_atac/_ref/jaspar/MA0067.1.pfm
+-rw-r--r--   0        0        0      210 2024-04-09 08:19:07.591561 muon-0.1.6/muon/_atac/_ref/jaspar/MA0068.2.pfm
+-rw-r--r--   0        0        0      373 2024-04-09 08:19:07.591740 muon-0.1.6/muon/_atac/_ref/jaspar/MA0069.1.pfm
+-rw-r--r--   0        0        0      316 2024-04-09 08:19:07.592997 muon-0.1.6/muon/_atac/_ref/jaspar/MA0070.1.pfm
+-rw-r--r--   0        0        0      261 2024-04-09 08:19:07.593236 muon-0.1.6/muon/_atac/_ref/jaspar/MA0071.1.pfm
+-rw-r--r--   0        0        0      373 2024-04-09 08:19:07.593397 muon-0.1.6/muon/_atac/_ref/jaspar/MA0072.1.pfm
+-rw-r--r--   0        0        0      540 2024-04-09 08:19:07.593579 muon-0.1.6/muon/_atac/_ref/jaspar/MA0073.1.pfm
+-rw-r--r--   0        0        0      400 2024-04-09 08:19:07.593747 muon-0.1.6/muon/_atac/_ref/jaspar/MA0074.1.pfm
+-rw-r--r--   0        0        0      215 2024-04-09 08:19:07.594226 muon-0.1.6/muon/_atac/_ref/jaspar/MA0075.3.pfm
+-rw-r--r--   0        0        0      297 2024-04-09 08:19:07.594520 muon-0.1.6/muon/_atac/_ref/jaspar/MA0076.2.pfm
+-rw-r--r--   0        0        0      233 2024-04-09 08:19:07.594771 muon-0.1.6/muon/_atac/_ref/jaspar/MA0077.1.pfm
+-rw-r--r--   0        0        0      232 2024-04-09 08:19:07.594982 muon-0.1.6/muon/_atac/_ref/jaspar/MA0078.1.pfm
+-rw-r--r--   0        0        0      414 2024-04-09 08:19:07.595204 muon-0.1.6/muon/_atac/_ref/jaspar/MA0079.4.pfm
+-rw-r--r--   0        0        0      556 2024-04-09 08:19:07.595430 muon-0.1.6/muon/_atac/_ref/jaspar/MA0080.5.pfm
+-rw-r--r--   0        0        0      441 2024-04-09 08:19:07.595600 muon-0.1.6/muon/_atac/_ref/jaspar/MA0081.2.pfm
+-rw-r--r--   0        0        0      436 2024-04-09 08:19:07.595778 muon-0.1.6/muon/_atac/_ref/jaspar/MA0083.3.pfm
+-rw-r--r--   0        0        0      233 2024-04-09 08:19:07.596061 muon-0.1.6/muon/_atac/_ref/jaspar/MA0084.1.pfm
+-rw-r--r--   0        0        0      177 2024-04-09 08:19:07.596407 muon-0.1.6/muon/_atac/_ref/jaspar/MA0087.1.pfm
+-rw-r--r--   0        0        0      436 2024-04-09 08:19:07.596725 muon-0.1.6/muon/_atac/_ref/jaspar/MA0088.2.pfm
+-rw-r--r--   0        0        0      437 2024-04-09 08:19:07.596908 muon-0.1.6/muon/_atac/_ref/jaspar/MA0089.2.pfm
+-rw-r--r--   0        0        0      360 2024-04-09 08:19:07.597071 muon-0.1.6/muon/_atac/_ref/jaspar/MA0090.3.pfm
+-rw-r--r--   0        0        0      318 2024-04-09 08:19:07.597267 muon-0.1.6/muon/_atac/_ref/jaspar/MA0091.1.pfm
+-rw-r--r--   0        0        0      261 2024-04-09 08:19:07.597535 muon-0.1.6/muon/_atac/_ref/jaspar/MA0092.1.pfm
+-rw-r--r--   0        0        0      388 2024-04-09 08:19:07.597987 muon-0.1.6/muon/_atac/_ref/jaspar/MA0093.3.pfm
+-rw-r--r--   0        0        0      326 2024-04-09 08:19:07.598162 muon-0.1.6/muon/_atac/_ref/jaspar/MA0095.2.pfm
+-rw-r--r--   0        0        0      269 2024-04-09 08:19:07.598313 muon-0.1.6/muon/_atac/_ref/jaspar/MA0098.3.pfm
+-rw-r--r--   0        0        0      267 2024-04-09 08:19:07.598453 muon-0.1.6/muon/_atac/_ref/jaspar/MA0099.3.pfm
+-rw-r--r--   0        0        0      268 2024-04-09 08:19:07.598588 muon-0.1.6/muon/_atac/_ref/jaspar/MA0100.3.pfm
+-rw-r--r--   0        0        0      260 2024-04-09 08:19:07.598971 muon-0.1.6/muon/_atac/_ref/jaspar/MA0101.1.pfm
+-rw-r--r--   0        0        0      388 2024-04-09 08:19:07.599188 muon-0.1.6/muon/_atac/_ref/jaspar/MA0102.4.pfm
+-rw-r--r--   0        0        0      300 2024-04-09 08:19:07.599394 muon-0.1.6/muon/_atac/_ref/jaspar/MA0103.3.pfm
+-rw-r--r--   0        0        0      328 2024-04-09 08:19:07.599583 muon-0.1.6/muon/_atac/_ref/jaspar/MA0104.4.pfm
+-rw-r--r--   0        0        0      354 2024-04-09 08:19:07.599832 muon-0.1.6/muon/_atac/_ref/jaspar/MA0105.4.pfm
+-rw-r--r--   0        0        0      496 2024-04-09 08:19:07.600015 muon-0.1.6/muon/_atac/_ref/jaspar/MA0106.3.pfm
+-rw-r--r--   0        0        0      261 2024-04-09 08:19:07.601210 muon-0.1.6/muon/_atac/_ref/jaspar/MA0107.1.pfm
+-rw-r--r--   0        0        0      406 2024-04-09 08:19:07.601401 muon-0.1.6/muon/_atac/_ref/jaspar/MA0108.2.pfm
+-rw-r--r--   0        0        0      264 2024-04-09 08:19:07.601599 muon-0.1.6/muon/_atac/_ref/jaspar/MA0109.1.pfm
+-rw-r--r--   0        0        0      288 2024-04-09 08:19:07.601876 muon-0.1.6/muon/_atac/_ref/jaspar/MA0111.1.pfm
+-rw-r--r--   0        0        0      462 2024-04-09 08:19:07.603275 muon-0.1.6/muon/_atac/_ref/jaspar/MA0112.3.pfm
+-rw-r--r--   0        0        0      468 2024-04-09 08:19:07.603502 muon-0.1.6/muon/_atac/_ref/jaspar/MA0113.3.pfm
+-rw-r--r--   0        0        0      359 2024-04-09 08:19:07.610755 muon-0.1.6/muon/_atac/_ref/jaspar/MA0114.4.pfm
+-rw-r--r--   0        0        0      457 2024-04-09 08:19:07.611345 muon-0.1.6/muon/_atac/_ref/jaspar/MA0115.1.pfm
+-rw-r--r--   0        0        0      401 2024-04-09 08:19:07.612428 muon-0.1.6/muon/_atac/_ref/jaspar/MA0116.1.pfm
+-rw-r--r--   0        0        0      325 2024-04-09 08:19:07.612724 muon-0.1.6/muon/_atac/_ref/jaspar/MA0117.2.pfm
+-rw-r--r--   0        0        0      373 2024-04-09 08:19:07.613023 muon-0.1.6/muon/_atac/_ref/jaspar/MA0119.1.pfm
+-rw-r--r--   0        0        0      356 2024-04-09 08:19:07.613982 muon-0.1.6/muon/_atac/_ref/jaspar/MA0122.3.pfm
+-rw-r--r--   0        0        0      242 2024-04-09 08:19:07.614192 muon-0.1.6/muon/_atac/_ref/jaspar/MA0124.2.pfm
+-rw-r--r--   0        0        0      205 2024-04-09 08:19:07.614339 muon-0.1.6/muon/_atac/_ref/jaspar/MA0125.1.pfm
+-rw-r--r--   0        0        0      148 2024-04-09 08:19:07.645143 muon-0.1.6/muon/_atac/_ref/jaspar/MA0130.1.pfm
+-rw-r--r--   0        0        0      323 2024-04-09 08:19:07.645348 muon-0.1.6/muon/_atac/_ref/jaspar/MA0131.2.pfm
+-rw-r--r--   0        0        0      215 2024-04-09 08:19:07.645523 muon-0.1.6/muon/_atac/_ref/jaspar/MA0132.2.pfm
+-rw-r--r--   0        0        0      344 2024-04-09 08:19:07.648056 muon-0.1.6/muon/_atac/_ref/jaspar/MA0135.1.pfm
+-rw-r--r--   0        0        0      297 2024-04-09 08:19:07.648384 muon-0.1.6/muon/_atac/_ref/jaspar/MA0136.2.pfm
+-rw-r--r--   0        0        0      297 2024-04-09 08:19:07.648620 muon-0.1.6/muon/_atac/_ref/jaspar/MA0137.3.pfm
+-rw-r--r--   0        0        0      576 2024-04-09 08:19:07.648784 muon-0.1.6/muon/_atac/_ref/jaspar/MA0138.2.pfm
+-rw-r--r--   0        0        0      518 2024-04-09 08:19:07.648975 muon-0.1.6/muon/_atac/_ref/jaspar/MA0139.1.pfm
+-rw-r--r--   0        0        0      494 2024-04-09 08:19:07.649212 muon-0.1.6/muon/_atac/_ref/jaspar/MA0140.2.pfm
+-rw-r--r--   0        0        0      296 2024-04-09 08:19:07.649557 muon-0.1.6/muon/_atac/_ref/jaspar/MA0141.3.pfm
+-rw-r--r--   0        0        0      406 2024-04-09 08:19:07.649723 muon-0.1.6/muon/_atac/_ref/jaspar/MA0142.1.pfm
+-rw-r--r--   0        0        0      304 2024-04-09 08:19:07.649865 muon-0.1.6/muon/_atac/_ref/jaspar/MA0143.4.pfm
+-rw-r--r--   0        0        0      300 2024-04-09 08:19:07.650257 muon-0.1.6/muon/_atac/_ref/jaspar/MA0144.2.pfm
+-rw-r--r--   0        0        0      266 2024-04-09 08:19:07.650510 muon-0.1.6/muon/_atac/_ref/jaspar/MA0145.3.pfm
+-rw-r--r--   0        0        0      378 2024-04-09 08:19:07.650689 muon-0.1.6/muon/_atac/_ref/jaspar/MA0146.2.pfm
+-rw-r--r--   0        0        0      327 2024-04-09 08:19:07.651075 muon-0.1.6/muon/_atac/_ref/jaspar/MA0147.3.pfm
+-rw-r--r--   0        0        0      333 2024-04-09 08:19:07.651513 muon-0.1.6/muon/_atac/_ref/jaspar/MA0148.4.pfm
+-rw-r--r--   0        0        0      486 2024-04-09 08:19:07.651697 muon-0.1.6/muon/_atac/_ref/jaspar/MA0149.1.pfm
+-rw-r--r--   0        0        0      408 2024-04-09 08:19:07.652025 muon-0.1.6/muon/_atac/_ref/jaspar/MA0150.2.pfm
+-rw-r--r--   0        0        0      149 2024-04-09 08:19:07.652253 muon-0.1.6/muon/_atac/_ref/jaspar/MA0151.1.pfm
+-rw-r--r--   0        0        0      177 2024-04-09 08:19:07.652584 muon-0.1.6/muon/_atac/_ref/jaspar/MA0152.1.pfm
+-rw-r--r--   0        0        0      357 2024-04-09 08:19:07.652800 muon-0.1.6/muon/_atac/_ref/jaspar/MA0153.2.pfm
+-rw-r--r--   0        0        0      415 2024-04-09 08:19:07.653418 muon-0.1.6/muon/_atac/_ref/jaspar/MA0154.4.pfm
+-rw-r--r--   0        0        0      317 2024-04-09 08:19:07.654173 muon-0.1.6/muon/_atac/_ref/jaspar/MA0155.1.pfm
+-rw-r--r--   0        0        0      271 2024-04-09 08:19:07.654971 muon-0.1.6/muon/_atac/_ref/jaspar/MA0156.2.pfm
+-rw-r--r--   0        0        0      207 2024-04-09 08:19:07.656152 muon-0.1.6/muon/_atac/_ref/jaspar/MA0157.2.pfm
+-rw-r--r--   0        0        0      213 2024-04-09 08:19:07.657856 muon-0.1.6/muon/_atac/_ref/jaspar/MA0158.2.pfm
+-rw-r--r--   0        0        0      458 2024-04-09 08:19:07.659190 muon-0.1.6/muon/_atac/_ref/jaspar/MA0159.1.pfm
+-rw-r--r--   0        0        0      204 2024-04-09 08:19:07.659671 muon-0.1.6/muon/_atac/_ref/jaspar/MA0160.1.pfm
+-rw-r--r--   0        0        0      300 2024-04-09 08:19:07.659997 muon-0.1.6/muon/_atac/_ref/jaspar/MA0161.2.pfm
+-rw-r--r--   0        0        0      385 2024-04-09 08:19:07.660406 muon-0.1.6/muon/_atac/_ref/jaspar/MA0162.4.pfm
+-rw-r--r--   0        0        0      373 2024-04-09 08:19:07.660696 muon-0.1.6/muon/_atac/_ref/jaspar/MA0163.1.pfm
+-rw-r--r--   0        0        0      177 2024-04-09 08:19:07.661840 muon-0.1.6/muon/_atac/_ref/jaspar/MA0164.1.pfm
+-rw-r--r--   0        0        0      409 2024-04-09 08:19:07.662212 muon-0.1.6/muon/_atac/_ref/jaspar/MA0258.2.pfm
+-rw-r--r--   0        0        0      207 2024-04-09 08:19:07.662616 muon-0.1.6/muon/_atac/_ref/jaspar/MA0259.1.pfm
+-rw-r--r--   0        0        0      296 2024-04-09 08:19:07.663022 muon-0.1.6/muon/_atac/_ref/jaspar/MA0442.2.pfm
+-rw-r--r--   0        0        0      267 2024-04-09 08:19:07.663317 muon-0.1.6/muon/_atac/_ref/jaspar/MA0461.2.pfm
+-rw-r--r--   0        0        0      302 2024-04-09 08:19:07.663771 muon-0.1.6/muon/_atac/_ref/jaspar/MA0462.2.pfm
+-rw-r--r--   0        0        0      440 2024-04-09 08:19:07.664189 muon-0.1.6/muon/_atac/_ref/jaspar/MA0463.2.pfm
+-rw-r--r--   0        0        0      272 2024-04-09 08:19:07.664471 muon-0.1.6/muon/_atac/_ref/jaspar/MA0464.2.pfm
+-rw-r--r--   0        0        0      329 2024-04-09 08:19:07.664677 muon-0.1.6/muon/_atac/_ref/jaspar/MA0465.2.pfm
+-rw-r--r--   0        0        0      272 2024-04-09 08:19:07.665134 muon-0.1.6/muon/_atac/_ref/jaspar/MA0466.2.pfm
+-rw-r--r--   0        0        0      297 2024-04-09 08:19:07.665798 muon-0.1.6/muon/_atac/_ref/jaspar/MA0467.1.pfm
+-rw-r--r--   0        0        0      300 2024-04-09 08:19:07.666102 muon-0.1.6/muon/_atac/_ref/jaspar/MA0468.1.pfm
+-rw-r--r--   0        0        0      441 2024-04-09 08:19:07.666296 muon-0.1.6/muon/_atac/_ref/jaspar/MA0469.3.pfm
+-rw-r--r--   0        0        0      384 2024-04-09 08:19:07.666474 muon-0.1.6/muon/_atac/_ref/jaspar/MA0470.2.pfm
+-rw-r--r--   0        0        0      357 2024-04-09 08:19:07.666632 muon-0.1.6/muon/_atac/_ref/jaspar/MA0471.2.pfm
+-rw-r--r--   0        0        0      296 2024-04-09 08:19:07.666780 muon-0.1.6/muon/_atac/_ref/jaspar/MA0472.2.pfm
+-rw-r--r--   0        0        0      386 2024-04-09 08:19:07.667003 muon-0.1.6/muon/_atac/_ref/jaspar/MA0473.3.pfm
+-rw-r--r--   0        0        0      269 2024-04-09 08:19:07.667209 muon-0.1.6/muon/_atac/_ref/jaspar/MA0474.2.pfm
+-rw-r--r--   0        0        0      273 2024-04-09 08:19:07.667658 muon-0.1.6/muon/_atac/_ref/jaspar/MA0475.2.pfm
+-rw-r--r--   0        0        0      300 2024-04-09 08:19:07.667982 muon-0.1.6/muon/_atac/_ref/jaspar/MA0476.1.pfm
+-rw-r--r--   0        0        0      360 2024-04-09 08:19:07.668211 muon-0.1.6/muon/_atac/_ref/jaspar/MA0477.2.pfm
+-rw-r--r--   0        0        0      298 2024-04-09 08:19:07.668392 muon-0.1.6/muon/_atac/_ref/jaspar/MA0478.1.pfm
+-rw-r--r--   0        0        0      299 2024-04-09 08:19:07.668862 muon-0.1.6/muon/_atac/_ref/jaspar/MA0479.1.pfm
+-rw-r--r--   0        0        0      297 2024-04-09 08:19:07.669094 muon-0.1.6/muon/_atac/_ref/jaspar/MA0480.1.pfm
+-rw-r--r--   0        0        0      304 2024-04-09 08:19:07.669309 muon-0.1.6/muon/_atac/_ref/jaspar/MA0481.3.pfm
+-rw-r--r--   0        0        0      332 2024-04-09 08:19:07.669917 muon-0.1.6/muon/_atac/_ref/jaspar/MA0482.2.pfm
+-rw-r--r--   0        0        0      296 2024-04-09 08:19:07.670442 muon-0.1.6/muon/_atac/_ref/jaspar/MA0483.1.pfm
+-rw-r--r--   0        0        0      356 2024-04-09 08:19:07.670685 muon-0.1.6/muon/_atac/_ref/jaspar/MA0484.2.pfm
+-rw-r--r--   0        0        0      270 2024-04-09 08:19:07.671220 muon-0.1.6/muon/_atac/_ref/jaspar/MA0485.2.pfm
+-rw-r--r--   0        0        0      350 2024-04-09 08:19:07.671511 muon-0.1.6/muon/_atac/_ref/jaspar/MA0486.2.pfm
+-rw-r--r--   0        0        0      356 2024-04-09 08:19:07.671800 muon-0.1.6/muon/_atac/_ref/jaspar/MA0488.1.pfm
+-rw-r--r--   0        0        0      384 2024-04-09 08:19:07.672000 muon-0.1.6/muon/_atac/_ref/jaspar/MA0489.1.pfm
+-rw-r--r--   0        0        0      360 2024-04-09 08:19:07.672190 muon-0.1.6/muon/_atac/_ref/jaspar/MA0490.2.pfm
+-rw-r--r--   0        0        0      360 2024-04-09 08:19:07.672462 muon-0.1.6/muon/_atac/_ref/jaspar/MA0491.2.pfm
+-rw-r--r--   0        0        0      413 2024-04-09 08:19:07.672652 muon-0.1.6/muon/_atac/_ref/jaspar/MA0492.1.pfm
+-rw-r--r--   0        0        0      294 2024-04-09 08:19:07.672801 muon-0.1.6/muon/_atac/_ref/jaspar/MA0493.1.pfm
+-rw-r--r--   0        0        0      517 2024-04-09 08:19:07.673028 muon-0.1.6/muon/_atac/_ref/jaspar/MA0494.1.pfm
+-rw-r--r--   0        0        0      442 2024-04-09 08:19:07.673255 muon-0.1.6/muon/_atac/_ref/jaspar/MA0495.3.pfm
+-rw-r--r--   0        0        0      415 2024-04-09 08:19:07.673437 muon-0.1.6/muon/_atac/_ref/jaspar/MA0496.3.pfm
+-rw-r--r--   0        0        0      408 2024-04-09 08:19:07.673887 muon-0.1.6/muon/_atac/_ref/jaspar/MA0497.1.pfm
+-rw-r--r--   0        0        0      191 2024-04-09 08:19:07.674084 muon-0.1.6/muon/_atac/_ref/jaspar/MA0498.2.pfm
+-rw-r--r--   0        0        0      357 2024-04-09 08:19:07.674364 muon-0.1.6/muon/_atac/_ref/jaspar/MA0499.2.pfm
+-rw-r--r--   0        0        0      328 2024-04-09 08:19:07.674578 muon-0.1.6/muon/_atac/_ref/jaspar/MA0500.2.pfm
+-rw-r--r--   0        0        0      405 2024-04-09 08:19:07.674835 muon-0.1.6/muon/_atac/_ref/jaspar/MA0501.1.pfm
+-rw-r--r--   0        0        0      327 2024-04-09 08:19:07.675085 muon-0.1.6/muon/_atac/_ref/jaspar/MA0502.2.pfm
+-rw-r--r--   0        0        0      297 2024-04-09 08:19:07.675323 muon-0.1.6/muon/_atac/_ref/jaspar/MA0503.1.pfm
+-rw-r--r--   0        0        0      406 2024-04-09 08:19:07.675555 muon-0.1.6/muon/_atac/_ref/jaspar/MA0504.1.pfm
+-rw-r--r--   0        0        0      408 2024-04-09 08:19:07.676080 muon-0.1.6/muon/_atac/_ref/jaspar/MA0505.1.pfm
+-rw-r--r--   0        0        0      295 2024-04-09 08:19:07.676463 muon-0.1.6/muon/_atac/_ref/jaspar/MA0506.1.pfm
+-rw-r--r--   0        0        0      352 2024-04-09 08:19:07.676723 muon-0.1.6/muon/_atac/_ref/jaspar/MA0507.1.pfm
+-rw-r--r--   0        0        0      302 2024-04-09 08:19:07.677040 muon-0.1.6/muon/_atac/_ref/jaspar/MA0508.3.pfm
+-rw-r--r--   0        0        0      384 2024-04-09 08:19:07.677286 muon-0.1.6/muon/_atac/_ref/jaspar/MA0509.2.pfm
+-rw-r--r--   0        0        0      437 2024-04-09 08:19:07.677468 muon-0.1.6/muon/_atac/_ref/jaspar/MA0510.2.pfm
+-rw-r--r--   0        0        0      243 2024-04-09 08:19:07.677733 muon-0.1.6/muon/_atac/_ref/jaspar/MA0511.2.pfm
+-rw-r--r--   0        0        0      386 2024-04-09 08:19:07.678238 muon-0.1.6/muon/_atac/_ref/jaspar/MA0512.2.pfm
+-rw-r--r--   0        0        0      352 2024-04-09 08:19:07.678606 muon-0.1.6/muon/_atac/_ref/jaspar/MA0513.1.pfm
+-rw-r--r--   0        0        0      267 2024-04-09 08:19:07.680092 muon-0.1.6/muon/_atac/_ref/jaspar/MA0514.1.pfm
+-rw-r--r--   0        0        0      264 2024-04-09 08:19:07.680588 muon-0.1.6/muon/_atac/_ref/jaspar/MA0515.1.pfm
+-rw-r--r--   0        0        0      464 2024-04-09 08:19:07.680868 muon-0.1.6/muon/_atac/_ref/jaspar/MA0516.2.pfm
+-rw-r--r--   0        0        0      405 2024-04-09 08:19:07.681337 muon-0.1.6/muon/_atac/_ref/jaspar/MA0517.1.pfm
+-rw-r--r--   0        0        0      382 2024-04-09 08:19:07.681544 muon-0.1.6/muon/_atac/_ref/jaspar/MA0518.1.pfm
+-rw-r--r--   0        0        0      300 2024-04-09 08:19:07.681717 muon-0.1.6/muon/_atac/_ref/jaspar/MA0519.1.pfm
+-rw-r--r--   0        0        0      408 2024-04-09 08:19:07.681934 muon-0.1.6/muon/_atac/_ref/jaspar/MA0520.1.pfm
+-rw-r--r--   0        0        0      298 2024-04-09 08:19:07.682275 muon-0.1.6/muon/_atac/_ref/jaspar/MA0521.1.pfm
+-rw-r--r--   0        0        0      301 2024-04-09 08:19:07.682471 muon-0.1.6/muon/_atac/_ref/jaspar/MA0522.3.pfm
+-rw-r--r--   0        0        0      382 2024-04-09 08:19:07.682883 muon-0.1.6/muon/_atac/_ref/jaspar/MA0523.1.pfm
+-rw-r--r--   0        0        0      327 2024-04-09 08:19:07.683071 muon-0.1.6/muon/_atac/_ref/jaspar/MA0524.2.pfm
+-rw-r--r--   0        0        0      492 2024-04-09 08:19:07.683224 muon-0.1.6/muon/_atac/_ref/jaspar/MA0525.2.pfm
+-rw-r--r--   0        0        0      385 2024-04-09 08:19:07.683725 muon-0.1.6/muon/_atac/_ref/jaspar/MA0526.3.pfm
+-rw-r--r--   0        0        0      407 2024-04-09 08:19:07.684114 muon-0.1.6/muon/_atac/_ref/jaspar/MA0527.1.pfm
+-rw-r--r--   0        0        0      331 2024-04-09 08:19:07.685401 muon-0.1.6/muon/_atac/_ref/jaspar/MA0528.2.pfm
+-rw-r--r--   0        0        0      404 2024-04-09 08:19:07.685719 muon-0.1.6/muon/_atac/_ref/jaspar/MA0591.1.pfm
+-rw-r--r--   0        0        0      356 2024-04-09 08:19:07.685978 muon-0.1.6/muon/_atac/_ref/jaspar/MA0592.3.pfm
+-rw-r--r--   0        0        0      296 2024-04-09 08:19:07.686414 muon-0.1.6/muon/_atac/_ref/jaspar/MA0593.1.pfm
+-rw-r--r--   0        0        0      267 2024-04-09 08:19:07.686667 muon-0.1.6/muon/_atac/_ref/jaspar/MA0594.2.pfm
+-rw-r--r--   0        0        0      263 2024-04-09 08:19:07.687137 muon-0.1.6/muon/_atac/_ref/jaspar/MA0595.1.pfm
+-rw-r--r--   0        0        0      262 2024-04-09 08:19:07.687472 muon-0.1.6/muon/_atac/_ref/jaspar/MA0596.1.pfm
+-rw-r--r--   0        0        0      236 2024-04-09 08:19:07.687740 muon-0.1.6/muon/_atac/_ref/jaspar/MA0597.1.pfm
+-rw-r--r--   0        0        0      412 2024-04-09 08:19:07.687979 muon-0.1.6/muon/_atac/_ref/jaspar/MA0598.3.pfm
+-rw-r--r--   0        0        0      272 2024-04-09 08:19:07.688215 muon-0.1.6/muon/_atac/_ref/jaspar/MA0599.1.pfm
+-rw-r--r--   0        0        0      440 2024-04-09 08:19:07.688380 muon-0.1.6/muon/_atac/_ref/jaspar/MA0600.2.pfm
+-rw-r--r--   0        0        0      296 2024-04-09 08:19:07.688923 muon-0.1.6/muon/_atac/_ref/jaspar/MA0601.1.pfm
+-rw-r--r--   0        0        0      376 2024-04-09 08:19:07.690814 muon-0.1.6/muon/_atac/_ref/jaspar/MA0602.1.pfm
+-rw-r--r--   0        0        0      268 2024-04-09 08:19:07.691929 muon-0.1.6/muon/_atac/_ref/jaspar/MA0603.1.pfm
+-rw-r--r--   0        0        0      210 2024-04-09 08:19:07.692553 muon-0.1.6/muon/_atac/_ref/jaspar/MA0604.1.pfm
+-rw-r--r--   0        0        0      329 2024-04-09 08:19:07.693259 muon-0.1.6/muon/_atac/_ref/jaspar/MA0605.2.pfm
+-rw-r--r--   0        0        0      268 2024-04-09 08:19:07.693894 muon-0.1.6/muon/_atac/_ref/jaspar/MA0606.1.pfm
+-rw-r--r--   0        0        0      210 2024-04-09 08:19:07.694636 muon-0.1.6/muon/_atac/_ref/jaspar/MA0607.1.pfm
+-rw-r--r--   0        0        0      236 2024-04-09 08:19:07.695006 muon-0.1.6/muon/_atac/_ref/jaspar/MA0608.1.pfm
+-rw-r--r--   0        0        0      440 2024-04-09 08:19:07.695477 muon-0.1.6/muon/_atac/_ref/jaspar/MA0609.2.pfm
+-rw-r--r--   0        0        0      296 2024-04-09 08:19:07.695927 muon-0.1.6/muon/_atac/_ref/jaspar/MA0610.1.pfm
+-rw-r--r--   0        0        0      212 2024-04-09 08:19:07.696380 muon-0.1.6/muon/_atac/_ref/jaspar/MA0611.1.pfm
+-rw-r--r--   0        0        0      216 2024-04-09 08:19:07.696884 muon-0.1.6/muon/_atac/_ref/jaspar/MA0612.2.pfm
+-rw-r--r--   0        0        0      208 2024-04-09 08:19:07.697595 muon-0.1.6/muon/_atac/_ref/jaspar/MA0613.1.pfm
+-rw-r--r--   0        0        0      208 2024-04-09 08:19:07.698142 muon-0.1.6/muon/_atac/_ref/jaspar/MA0614.1.pfm
+-rw-r--r--   0        0        0      460 2024-04-09 08:19:07.698708 muon-0.1.6/muon/_atac/_ref/jaspar/MA0615.1.pfm
+-rw-r--r--   0        0        0      270 2024-04-09 08:19:07.699368 muon-0.1.6/muon/_atac/_ref/jaspar/MA0616.2.pfm
+-rw-r--r--   0        0        0      212 2024-04-09 08:19:07.699718 muon-0.1.6/muon/_atac/_ref/jaspar/MA0618.1.pfm
+-rw-r--r--   0        0        0      239 2024-04-09 08:19:07.699974 muon-0.1.6/muon/_atac/_ref/jaspar/MA0619.1.pfm
+-rw-r--r--   0        0        0      500 2024-04-09 08:19:07.700251 muon-0.1.6/muon/_atac/_ref/jaspar/MA0620.3.pfm
+-rw-r--r--   0        0        0      296 2024-04-09 08:19:07.700824 muon-0.1.6/muon/_atac/_ref/jaspar/MA0621.1.pfm
+-rw-r--r--   0        0        0      211 2024-04-09 08:19:07.702181 muon-0.1.6/muon/_atac/_ref/jaspar/MA0622.1.pfm
+-rw-r--r--   0        0        0      269 2024-04-09 08:19:07.702937 muon-0.1.6/muon/_atac/_ref/jaspar/MA0623.2.pfm
+-rw-r--r--   0        0        0      268 2024-04-09 08:19:07.703902 muon-0.1.6/muon/_atac/_ref/jaspar/MA0624.1.pfm
+-rw-r--r--   0        0        0      267 2024-04-09 08:19:07.704761 muon-0.1.6/muon/_atac/_ref/jaspar/MA0625.1.pfm
+-rw-r--r--   0        0        0      268 2024-04-09 08:19:07.705265 muon-0.1.6/muon/_atac/_ref/jaspar/MA0626.1.pfm
+-rw-r--r--   0        0        0      360 2024-04-09 08:19:07.705776 muon-0.1.6/muon/_atac/_ref/jaspar/MA0627.2.pfm
+-rw-r--r--   0        0        0      267 2024-04-09 08:19:07.706014 muon-0.1.6/muon/_atac/_ref/jaspar/MA0628.1.pfm
+-rw-r--r--   0        0        0      460 2024-04-09 08:19:07.706395 muon-0.1.6/muon/_atac/_ref/jaspar/MA0629.1.pfm
+-rw-r--r--   0        0        0      212 2024-04-09 08:19:07.706856 muon-0.1.6/muon/_atac/_ref/jaspar/MA0630.1.pfm
+-rw-r--r--   0        0        0      459 2024-04-09 08:19:07.707054 muon-0.1.6/muon/_atac/_ref/jaspar/MA0631.1.pfm
+-rw-r--r--   0        0        0      275 2024-04-09 08:19:07.707422 muon-0.1.6/muon/_atac/_ref/jaspar/MA0632.2.pfm
+-rw-r--r--   0        0        0      268 2024-04-09 08:19:07.707753 muon-0.1.6/muon/_atac/_ref/jaspar/MA0633.1.pfm
+-rw-r--r--   0        0        0      272 2024-04-09 08:19:07.709496 muon-0.1.6/muon/_atac/_ref/jaspar/MA0634.1.pfm
+-rw-r--r--   0        0        0      272 2024-04-09 08:19:07.709988 muon-0.1.6/muon/_atac/_ref/jaspar/MA0635.1.pfm
+-rw-r--r--   0        0        0      270 2024-04-09 08:19:07.710427 muon-0.1.6/muon/_atac/_ref/jaspar/MA0636.1.pfm
+-rw-r--r--   0        0        0      407 2024-04-09 08:19:07.710651 muon-0.1.6/muon/_atac/_ref/jaspar/MA0637.1.pfm
+-rw-r--r--   0        0        0      377 2024-04-09 08:19:07.711010 muon-0.1.6/muon/_atac/_ref/jaspar/MA0638.1.pfm
+-rw-r--r--   0        0        0      328 2024-04-09 08:19:07.711463 muon-0.1.6/muon/_atac/_ref/jaspar/MA0639.1.pfm
+-rw-r--r--   0        0        0      388 2024-04-09 08:19:07.711971 muon-0.1.6/muon/_atac/_ref/jaspar/MA0640.2.pfm
+-rw-r--r--   0        0        0      324 2024-04-09 08:19:07.712880 muon-0.1.6/muon/_atac/_ref/jaspar/MA0641.1.pfm
+-rw-r--r--   0        0        0      268 2024-04-09 08:19:07.713201 muon-0.1.6/muon/_atac/_ref/jaspar/MA0642.1.pfm
+-rw-r--r--   0        0        0      273 2024-04-09 08:19:07.713541 muon-0.1.6/muon/_atac/_ref/jaspar/MA0643.1.pfm
+-rw-r--r--   0        0        0      273 2024-04-09 08:19:07.713826 muon-0.1.6/muon/_atac/_ref/jaspar/MA0644.1.pfm
+-rw-r--r--   0        0        0      272 2024-04-09 08:19:07.714187 muon-0.1.6/muon/_atac/_ref/jaspar/MA0645.1.pfm
+-rw-r--r--   0        0        0      300 2024-04-09 08:19:07.714416 muon-0.1.6/muon/_atac/_ref/jaspar/MA0646.1.pfm
+-rw-r--r--   0        0        0      325 2024-04-09 08:19:07.714667 muon-0.1.6/muon/_atac/_ref/jaspar/MA0647.1.pfm
+-rw-r--r--   0        0        0      271 2024-04-09 08:19:07.714918 muon-0.1.6/muon/_atac/_ref/jaspar/MA0648.1.pfm
+-rw-r--r--   0        0        0      268 2024-04-09 08:19:07.715415 muon-0.1.6/muon/_atac/_ref/jaspar/MA0649.1.pfm
+-rw-r--r--   0        0        0      295 2024-04-09 08:19:07.715977 muon-0.1.6/muon/_atac/_ref/jaspar/MA0650.2.pfm
+-rw-r--r--   0        0        0      297 2024-04-09 08:19:07.716883 muon-0.1.6/muon/_atac/_ref/jaspar/MA0651.1.pfm
+-rw-r--r--   0        0        0      383 2024-04-09 08:19:07.717590 muon-0.1.6/muon/_atac/_ref/jaspar/MA0652.1.pfm
+-rw-r--r--   0        0        0      407 2024-04-09 08:19:07.718037 muon-0.1.6/muon/_atac/_ref/jaspar/MA0653.1.pfm
+-rw-r--r--   0        0        0      212 2024-04-09 08:19:07.718777 muon-0.1.6/muon/_atac/_ref/jaspar/MA0654.1.pfm
+-rw-r--r--   0        0        0      238 2024-04-09 08:19:07.720133 muon-0.1.6/muon/_atac/_ref/jaspar/MA0655.1.pfm
+-rw-r--r--   0        0        0      329 2024-04-09 08:19:07.720828 muon-0.1.6/muon/_atac/_ref/jaspar/MA0656.1.pfm
+-rw-r--r--   0        0        0      493 2024-04-09 08:19:07.721489 muon-0.1.6/muon/_atac/_ref/jaspar/MA0657.1.pfm
+-rw-r--r--   0        0        0      270 2024-04-09 08:19:07.721811 muon-0.1.6/muon/_atac/_ref/jaspar/MA0658.1.pfm
+-rw-r--r--   0        0        0      412 2024-04-09 08:19:07.722028 muon-0.1.6/muon/_atac/_ref/jaspar/MA0659.2.pfm
+-rw-r--r--   0        0        0      325 2024-04-09 08:19:07.722192 muon-0.1.6/muon/_atac/_ref/jaspar/MA0660.1.pfm
+-rw-r--r--   0        0        0      268 2024-04-09 08:19:07.722365 muon-0.1.6/muon/_atac/_ref/jaspar/MA0661.1.pfm
+-rw-r--r--   0        0        0      272 2024-04-09 08:19:07.722631 muon-0.1.6/muon/_atac/_ref/jaspar/MA0662.1.pfm
+-rw-r--r--   0        0        0      265 2024-04-09 08:19:07.722853 muon-0.1.6/muon/_atac/_ref/jaspar/MA0663.1.pfm
+-rw-r--r--   0        0        0      267 2024-04-09 08:19:07.723082 muon-0.1.6/muon/_atac/_ref/jaspar/MA0664.1.pfm
+-rw-r--r--   0        0        0      262 2024-04-09 08:19:07.723581 muon-0.1.6/muon/_atac/_ref/jaspar/MA0665.1.pfm
+-rw-r--r--   0        0        0      213 2024-04-09 08:19:07.724452 muon-0.1.6/muon/_atac/_ref/jaspar/MA0666.1.pfm
+-rw-r--r--   0        0        0      264 2024-04-09 08:19:07.724700 muon-0.1.6/muon/_atac/_ref/jaspar/MA0667.1.pfm
+-rw-r--r--   0        0        0      267 2024-04-09 08:19:07.725036 muon-0.1.6/muon/_atac/_ref/jaspar/MA0668.1.pfm
+-rw-r--r--   0        0        0      264 2024-04-09 08:19:07.725272 muon-0.1.6/muon/_atac/_ref/jaspar/MA0669.1.pfm
+-rw-r--r--   0        0        0      276 2024-04-09 08:19:07.726064 muon-0.1.6/muon/_atac/_ref/jaspar/MA0670.1.pfm
+-rw-r--r--   0        0        0      244 2024-04-09 08:19:07.726950 muon-0.1.6/muon/_atac/_ref/jaspar/MA0671.1.pfm
+-rw-r--r--   0        0        0      272 2024-04-09 08:19:07.727967 muon-0.1.6/muon/_atac/_ref/jaspar/MA0672.1.pfm
+-rw-r--r--   0        0        0      243 2024-04-09 08:19:07.728825 muon-0.1.6/muon/_atac/_ref/jaspar/MA0673.1.pfm
+-rw-r--r--   0        0        0      212 2024-04-09 08:19:07.729385 muon-0.1.6/muon/_atac/_ref/jaspar/MA0674.1.pfm
+-rw-r--r--   0        0        0      216 2024-04-09 08:19:07.729924 muon-0.1.6/muon/_atac/_ref/jaspar/MA0675.1.pfm
+-rw-r--r--   0        0        0      241 2024-04-09 08:19:07.730432 muon-0.1.6/muon/_atac/_ref/jaspar/MA0676.1.pfm
+-rw-r--r--   0        0        0      378 2024-04-09 08:19:07.731310 muon-0.1.6/muon/_atac/_ref/jaspar/MA0677.1.pfm
+-rw-r--r--   0        0        0      268 2024-04-09 08:19:07.732064 muon-0.1.6/muon/_atac/_ref/jaspar/MA0678.1.pfm
+-rw-r--r--   0        0        0      444 2024-04-09 08:19:07.733617 muon-0.1.6/muon/_atac/_ref/jaspar/MA0679.2.pfm
+-rw-r--r--   0        0        0      267 2024-04-09 08:19:07.734694 muon-0.1.6/muon/_atac/_ref/jaspar/MA0680.1.pfm
+-rw-r--r--   0        0        0      442 2024-04-09 08:19:07.735348 muon-0.1.6/muon/_atac/_ref/jaspar/MA0681.2.pfm
+-rw-r--r--   0        0        0      216 2024-04-09 08:19:07.735941 muon-0.1.6/muon/_atac/_ref/jaspar/MA0682.2.pfm
+-rw-r--r--   0        0        0      437 2024-04-09 08:19:07.737731 muon-0.1.6/muon/_atac/_ref/jaspar/MA0683.1.pfm
+-rw-r--r--   0        0        0      328 2024-04-09 08:19:07.738327 muon-0.1.6/muon/_atac/_ref/jaspar/MA0684.2.pfm
+-rw-r--r--   0        0        0      466 2024-04-09 08:19:07.739087 muon-0.1.6/muon/_atac/_ref/jaspar/MA0685.1.pfm
+-rw-r--r--   0        0        0      297 2024-04-09 08:19:07.739661 muon-0.1.6/muon/_atac/_ref/jaspar/MA0686.1.pfm
+-rw-r--r--   0        0        0      377 2024-04-09 08:19:07.740146 muon-0.1.6/muon/_atac/_ref/jaspar/MA0687.1.pfm
+-rw-r--r--   0        0        0      297 2024-04-09 08:19:07.740624 muon-0.1.6/muon/_atac/_ref/jaspar/MA0688.1.pfm
+-rw-r--r--   0        0        0      294 2024-04-09 08:19:07.741381 muon-0.1.6/muon/_atac/_ref/jaspar/MA0689.1.pfm
+-rw-r--r--   0        0        0      269 2024-04-09 08:19:07.741982 muon-0.1.6/muon/_atac/_ref/jaspar/MA0690.1.pfm
+-rw-r--r--   0        0        0      269 2024-04-09 08:19:07.742660 muon-0.1.6/muon/_atac/_ref/jaspar/MA0691.1.pfm
+-rw-r--r--   0        0        0      271 2024-04-09 08:19:07.743240 muon-0.1.6/muon/_atac/_ref/jaspar/MA0692.1.pfm
+-rw-r--r--   0        0        0      211 2024-04-09 08:19:07.743766 muon-0.1.6/muon/_atac/_ref/jaspar/MA0693.2.pfm
+-rw-r--r--   0        0        0      324 2024-04-09 08:19:07.744316 muon-0.1.6/muon/_atac/_ref/jaspar/MA0694.1.pfm
+-rw-r--r--   0        0        0      324 2024-04-09 08:19:07.745140 muon-0.1.6/muon/_atac/_ref/jaspar/MA0695.1.pfm
+-rw-r--r--   0        0        0      385 2024-04-09 08:19:07.745699 muon-0.1.6/muon/_atac/_ref/jaspar/MA0696.1.pfm
+-rw-r--r--   0        0        0      405 2024-04-09 08:19:07.746454 muon-0.1.6/muon/_atac/_ref/jaspar/MA0697.1.pfm
+-rw-r--r--   0        0        0      356 2024-04-09 08:19:07.747386 muon-0.1.6/muon/_atac/_ref/jaspar/MA0698.1.pfm
+-rw-r--r--   0        0        0      268 2024-04-09 08:19:07.748367 muon-0.1.6/muon/_atac/_ref/jaspar/MA0699.1.pfm
+-rw-r--r--   0        0        0      299 2024-04-09 08:19:07.749323 muon-0.1.6/muon/_atac/_ref/jaspar/MA0700.2.pfm
+-rw-r--r--   0        0        0      215 2024-04-09 08:19:07.749882 muon-0.1.6/muon/_atac/_ref/jaspar/MA0701.2.pfm
+-rw-r--r--   0        0        0      213 2024-04-09 08:19:07.750752 muon-0.1.6/muon/_atac/_ref/jaspar/MA0702.2.pfm
+-rw-r--r--   0        0        0      297 2024-04-09 08:19:07.751319 muon-0.1.6/muon/_atac/_ref/jaspar/MA0703.2.pfm
+-rw-r--r--   0        0        0      213 2024-04-09 08:19:07.751967 muon-0.1.6/muon/_atac/_ref/jaspar/MA0704.1.pfm
+-rw-r--r--   0        0        0      214 2024-04-09 08:19:07.752887 muon-0.1.6/muon/_atac/_ref/jaspar/MA0705.1.pfm
+-rw-r--r--   0        0        0      272 2024-04-09 08:19:07.753711 muon-0.1.6/muon/_atac/_ref/jaspar/MA0706.1.pfm
+-rw-r--r--   0        0        0      267 2024-04-09 08:19:07.754252 muon-0.1.6/muon/_atac/_ref/jaspar/MA0707.1.pfm
+-rw-r--r--   0        0        0      213 2024-04-09 08:19:07.754824 muon-0.1.6/muon/_atac/_ref/jaspar/MA0708.1.pfm
+-rw-r--r--   0        0        0      216 2024-04-09 08:19:07.755336 muon-0.1.6/muon/_atac/_ref/jaspar/MA0709.1.pfm
+-rw-r--r--   0        0        0      272 2024-04-09 08:19:07.757394 muon-0.1.6/muon/_atac/_ref/jaspar/MA0710.1.pfm
+-rw-r--r--   0        0        0      216 2024-04-09 08:19:07.757988 muon-0.1.6/muon/_atac/_ref/jaspar/MA0711.1.pfm
+-rw-r--r--   0        0        0      332 2024-04-09 08:19:07.759340 muon-0.1.6/muon/_atac/_ref/jaspar/MA0712.2.pfm
+-rw-r--r--   0        0        0      300 2024-04-09 08:19:07.760225 muon-0.1.6/muon/_atac/_ref/jaspar/MA0713.1.pfm
+-rw-r--r--   0        0        0      244 2024-04-09 08:19:07.761097 muon-0.1.6/muon/_atac/_ref/jaspar/MA0714.1.pfm
+-rw-r--r--   0        0        0      293 2024-04-09 08:19:07.761645 muon-0.1.6/muon/_atac/_ref/jaspar/MA0715.1.pfm
+-rw-r--r--   0        0        0      216 2024-04-09 08:19:07.763846 muon-0.1.6/muon/_atac/_ref/jaspar/MA0716.1.pfm
+-rw-r--r--   0        0        0      218 2024-04-09 08:19:07.764592 muon-0.1.6/muon/_atac/_ref/jaspar/MA0717.1.pfm
+-rw-r--r--   0        0        0      268 2024-04-09 08:19:07.765117 muon-0.1.6/muon/_atac/_ref/jaspar/MA0718.1.pfm
+-rw-r--r--   0        0        0      216 2024-04-09 08:19:07.765774 muon-0.1.6/muon/_atac/_ref/jaspar/MA0719.1.pfm
+-rw-r--r--   0        0        0      216 2024-04-09 08:19:07.766485 muon-0.1.6/muon/_atac/_ref/jaspar/MA0720.1.pfm
+-rw-r--r--   0        0        0      218 2024-04-09 08:19:07.767289 muon-0.1.6/muon/_atac/_ref/jaspar/MA0721.1.pfm
+-rw-r--r--   0        0        0      214 2024-04-09 08:19:07.767987 muon-0.1.6/muon/_atac/_ref/jaspar/MA0722.1.pfm
+-rw-r--r--   0        0        0      215 2024-04-09 08:19:07.768756 muon-0.1.6/muon/_atac/_ref/jaspar/MA0723.1.pfm
+-rw-r--r--   0        0        0      244 2024-04-09 08:19:07.769484 muon-0.1.6/muon/_atac/_ref/jaspar/MA0724.1.pfm
+-rw-r--r--   0        0        0      214 2024-04-09 08:19:07.770782 muon-0.1.6/muon/_atac/_ref/jaspar/MA0725.1.pfm
+-rw-r--r--   0        0        0      214 2024-04-09 08:19:07.771388 muon-0.1.6/muon/_atac/_ref/jaspar/MA0726.1.pfm
+-rw-r--r--   0        0        0      470 2024-04-09 08:19:07.772010 muon-0.1.6/muon/_atac/_ref/jaspar/MA0727.1.pfm
+-rw-r--r--   0        0        0      405 2024-04-09 08:19:07.772532 muon-0.1.6/muon/_atac/_ref/jaspar/MA0728.1.pfm
+-rw-r--r--   0        0        0      488 2024-04-09 08:19:07.773031 muon-0.1.6/muon/_atac/_ref/jaspar/MA0729.1.pfm
+-rw-r--r--   0        0        0      462 2024-04-09 08:19:07.773557 muon-0.1.6/muon/_atac/_ref/jaspar/MA0730.1.pfm
+-rw-r--r--   0        0        0      459 2024-04-09 08:19:07.774064 muon-0.1.6/muon/_atac/_ref/jaspar/MA0731.1.pfm
+-rw-r--r--   0        0        0      408 2024-04-09 08:19:07.774546 muon-0.1.6/muon/_atac/_ref/jaspar/MA0732.1.pfm
+-rw-r--r--   0        0        0      440 2024-04-09 08:19:07.775350 muon-0.1.6/muon/_atac/_ref/jaspar/MA0733.1.pfm
+-rw-r--r--   0        0        0      412 2024-04-09 08:19:07.775989 muon-0.1.6/muon/_atac/_ref/jaspar/MA0734.2.pfm
+-rw-r--r--   0        0        0      438 2024-04-09 08:19:07.777959 muon-0.1.6/muon/_atac/_ref/jaspar/MA0735.1.pfm
+-rw-r--r--   0        0        0      379 2024-04-09 08:19:07.779204 muon-0.1.6/muon/_atac/_ref/jaspar/MA0736.1.pfm
+-rw-r--r--   0        0        0      377 2024-04-09 08:19:07.781302 muon-0.1.6/muon/_atac/_ref/jaspar/MA0737.1.pfm
+-rw-r--r--   0        0        0      242 2024-04-09 08:19:07.782071 muon-0.1.6/muon/_atac/_ref/jaspar/MA0738.1.pfm
+-rw-r--r--   0        0        0      242 2024-04-09 08:19:07.783679 muon-0.1.6/muon/_atac/_ref/jaspar/MA0739.1.pfm
+-rw-r--r--   0        0        0      380 2024-04-09 08:19:07.785076 muon-0.1.6/muon/_atac/_ref/jaspar/MA0740.1.pfm
+-rw-r--r--   0        0        0      297 2024-04-09 08:19:07.785621 muon-0.1.6/muon/_atac/_ref/jaspar/MA0741.1.pfm
+-rw-r--r--   0        0        0      408 2024-04-09 08:19:07.786229 muon-0.1.6/muon/_atac/_ref/jaspar/MA0742.1.pfm
+-rw-r--r--   0        0        0      444 2024-04-09 08:19:07.786728 muon-0.1.6/muon/_atac/_ref/jaspar/MA0743.2.pfm
+-rw-r--r--   0        0        0      444 2024-04-09 08:19:07.787565 muon-0.1.6/muon/_atac/_ref/jaspar/MA0744.2.pfm
+-rw-r--r--   0        0        0      359 2024-04-09 08:19:07.788145 muon-0.1.6/muon/_atac/_ref/jaspar/MA0745.2.pfm
+-rw-r--r--   0        0        0      356 2024-04-09 08:19:07.789142 muon-0.1.6/muon/_atac/_ref/jaspar/MA0746.2.pfm
+-rw-r--r--   0        0        0      320 2024-04-09 08:19:07.790367 muon-0.1.6/muon/_atac/_ref/jaspar/MA0747.1.pfm
+-rw-r--r--   0        0        0      300 2024-04-09 08:19:07.790902 muon-0.1.6/muon/_atac/_ref/jaspar/MA0748.2.pfm
+-rw-r--r--   0        0        0      354 2024-04-09 08:19:07.791394 muon-0.1.6/muon/_atac/_ref/jaspar/MA0749.1.pfm
+-rw-r--r--   0        0        0      356 2024-04-09 08:19:07.791923 muon-0.1.6/muon/_atac/_ref/jaspar/MA0750.2.pfm
+-rw-r--r--   0        0        0      410 2024-04-09 08:19:07.792429 muon-0.1.6/muon/_atac/_ref/jaspar/MA0751.1.pfm
+-rw-r--r--   0        0        0      465 2024-04-09 08:19:07.800706 muon-0.1.6/muon/_atac/_ref/jaspar/MA0752.1.pfm
+-rw-r--r--   0        0        0      352 2024-04-09 08:19:07.801380 muon-0.1.6/muon/_atac/_ref/jaspar/MA0753.2.pfm
+-rw-r--r--   0        0        0      273 2024-04-09 08:19:07.801935 muon-0.1.6/muon/_atac/_ref/jaspar/MA0754.1.pfm
+-rw-r--r--   0        0        0      273 2024-04-09 08:19:07.808975 muon-0.1.6/muon/_atac/_ref/jaspar/MA0755.1.pfm
+-rw-r--r--   0        0        0      381 2024-04-09 08:19:07.809834 muon-0.1.6/muon/_atac/_ref/jaspar/MA0756.1.pfm
+-rw-r--r--   0        0        0      383 2024-04-09 08:19:07.810398 muon-0.1.6/muon/_atac/_ref/jaspar/MA0757.1.pfm
+-rw-r--r--   0        0        0      379 2024-04-09 08:19:07.811004 muon-0.1.6/muon/_atac/_ref/jaspar/MA0758.1.pfm
+-rw-r--r--   0        0        0      269 2024-04-09 08:19:07.818632 muon-0.1.6/muon/_atac/_ref/jaspar/MA0759.1.pfm
+-rw-r--r--   0        0        0      263 2024-04-09 08:19:07.821786 muon-0.1.6/muon/_atac/_ref/jaspar/MA0760.1.pfm
+-rw-r--r--   0        0        0      385 2024-04-09 08:19:07.822599 muon-0.1.6/muon/_atac/_ref/jaspar/MA0761.2.pfm
+-rw-r--r--   0        0        0      297 2024-04-09 08:19:07.823418 muon-0.1.6/muon/_atac/_ref/jaspar/MA0762.1.pfm
+-rw-r--r--   0        0        0      265 2024-04-09 08:19:07.824214 muon-0.1.6/muon/_atac/_ref/jaspar/MA0763.1.pfm
+-rw-r--r--   0        0        0      272 2024-04-09 08:19:07.824735 muon-0.1.6/muon/_atac/_ref/jaspar/MA0764.2.pfm
+-rw-r--r--   0        0        0      300 2024-04-09 08:19:07.825284 muon-0.1.6/muon/_atac/_ref/jaspar/MA0765.2.pfm
+-rw-r--r--   0        0        0      272 2024-04-09 08:19:07.826508 muon-0.1.6/muon/_atac/_ref/jaspar/MA0766.2.pfm
+-rw-r--r--   0        0        0      268 2024-04-09 08:19:07.827242 muon-0.1.6/muon/_atac/_ref/jaspar/MA0767.1.pfm
+-rw-r--r--   0        0        0      408 2024-04-09 08:19:07.828093 muon-0.1.6/muon/_atac/_ref/jaspar/MA0768.1.pfm
+-rw-r--r--   0        0        0      300 2024-04-09 08:19:07.828697 muon-0.1.6/muon/_atac/_ref/jaspar/MA0769.2.pfm
+-rw-r--r--   0        0        0      351 2024-04-09 08:19:07.829439 muon-0.1.6/muon/_atac/_ref/jaspar/MA0770.1.pfm
+-rw-r--r--   0        0        0      357 2024-04-09 08:19:07.831817 muon-0.1.6/muon/_atac/_ref/jaspar/MA0771.1.pfm
+-rw-r--r--   0        0        0      379 2024-04-09 08:19:07.836688 muon-0.1.6/muon/_atac/_ref/jaspar/MA0772.1.pfm
+-rw-r--r--   0        0        0      327 2024-04-09 08:19:07.838545 muon-0.1.6/muon/_atac/_ref/jaspar/MA0773.1.pfm
+-rw-r--r--   0        0        0      213 2024-04-09 08:19:07.839347 muon-0.1.6/muon/_atac/_ref/jaspar/MA0774.1.pfm
+-rw-r--r--   0        0        0      214 2024-04-09 08:19:07.840276 muon-0.1.6/muon/_atac/_ref/jaspar/MA0775.1.pfm
+-rw-r--r--   0        0        0      324 2024-04-09 08:19:07.842275 muon-0.1.6/muon/_atac/_ref/jaspar/MA0776.1.pfm
+-rw-r--r--   0        0        0      406 2024-04-09 08:19:07.843086 muon-0.1.6/muon/_atac/_ref/jaspar/MA0777.1.pfm
+-rw-r--r--   0        0        0      356 2024-04-09 08:19:07.843808 muon-0.1.6/muon/_atac/_ref/jaspar/MA0778.1.pfm
+-rw-r--r--   0        0        0      466 2024-04-09 08:19:07.844586 muon-0.1.6/muon/_atac/_ref/jaspar/MA0779.1.pfm
+-rw-r--r--   0        0        0      270 2024-04-09 08:19:07.845315 muon-0.1.6/muon/_atac/_ref/jaspar/MA0780.1.pfm
+-rw-r--r--   0        0        0      466 2024-04-09 08:19:07.845793 muon-0.1.6/muon/_atac/_ref/jaspar/MA0781.1.pfm
+-rw-r--r--   0        0        0      413 2024-04-09 08:19:07.846364 muon-0.1.6/muon/_atac/_ref/jaspar/MA0782.2.pfm
+-rw-r--r--   0        0        0      320 2024-04-09 08:19:07.847040 muon-0.1.6/muon/_atac/_ref/jaspar/MA0783.1.pfm
+-rw-r--r--   0        0        0      381 2024-04-09 08:19:07.848296 muon-0.1.6/muon/_atac/_ref/jaspar/MA0784.1.pfm
+-rw-r--r--   0        0        0      328 2024-04-09 08:19:07.849020 muon-0.1.6/muon/_atac/_ref/jaspar/MA0785.1.pfm
+-rw-r--r--   0        0        0      326 2024-04-09 08:19:07.849634 muon-0.1.6/muon/_atac/_ref/jaspar/MA0786.1.pfm
+-rw-r--r--   0        0        0      323 2024-04-09 08:19:07.850290 muon-0.1.6/muon/_atac/_ref/jaspar/MA0787.1.pfm
+-rw-r--r--   0        0        0      351 2024-04-09 08:19:07.851004 muon-0.1.6/muon/_atac/_ref/jaspar/MA0788.1.pfm
+-rw-r--r--   0        0        0      242 2024-04-09 08:19:07.851899 muon-0.1.6/muon/_atac/_ref/jaspar/MA0789.1.pfm
+-rw-r--r--   0        0        0      383 2024-04-09 08:19:07.852783 muon-0.1.6/muon/_atac/_ref/jaspar/MA0790.1.pfm
+-rw-r--r--   0        0        0      437 2024-04-09 08:19:07.853556 muon-0.1.6/muon/_atac/_ref/jaspar/MA0791.1.pfm
+-rw-r--r--   0        0        0      243 2024-04-09 08:19:07.854264 muon-0.1.6/muon/_atac/_ref/jaspar/MA0792.1.pfm
+-rw-r--r--   0        0        0      269 2024-04-09 08:19:07.855045 muon-0.1.6/muon/_atac/_ref/jaspar/MA0793.1.pfm
+-rw-r--r--   0        0        0      326 2024-04-09 08:19:07.855787 muon-0.1.6/muon/_atac/_ref/jaspar/MA0794.1.pfm
+-rw-r--r--   0        0        0      269 2024-04-09 08:19:07.856731 muon-0.1.6/muon/_atac/_ref/jaspar/MA0795.1.pfm
+-rw-r--r--   0        0        0      322 2024-04-09 08:19:07.857601 muon-0.1.6/muon/_atac/_ref/jaspar/MA0796.1.pfm
+-rw-r--r--   0        0        0      326 2024-04-09 08:19:07.858105 muon-0.1.6/muon/_atac/_ref/jaspar/MA0797.1.pfm
+-rw-r--r--   0        0        0      382 2024-04-09 08:19:07.858874 muon-0.1.6/muon/_atac/_ref/jaspar/MA0798.2.pfm
+-rw-r--r--   0        0        0      440 2024-04-09 08:19:07.859383 muon-0.1.6/muon/_atac/_ref/jaspar/MA0799.1.pfm
+-rw-r--r--   0        0        0      355 2024-04-09 08:19:07.859839 muon-0.1.6/muon/_atac/_ref/jaspar/MA0800.1.pfm
+-rw-r--r--   0        0        0      217 2024-04-09 08:19:07.860308 muon-0.1.6/muon/_atac/_ref/jaspar/MA0801.1.pfm
+-rw-r--r--   0        0        0      272 2024-04-09 08:19:07.860863 muon-0.1.6/muon/_atac/_ref/jaspar/MA0802.1.pfm
+-rw-r--r--   0        0        0      213 2024-04-09 08:19:07.861382 muon-0.1.6/muon/_atac/_ref/jaspar/MA0803.1.pfm
+-rw-r--r--   0        0        0      554 2024-04-09 08:19:07.861881 muon-0.1.6/muon/_atac/_ref/jaspar/MA0804.1.pfm
+-rw-r--r--   0        0        0      215 2024-04-09 08:19:07.862367 muon-0.1.6/muon/_atac/_ref/jaspar/MA0805.1.pfm
+-rw-r--r--   0        0        0      216 2024-04-09 08:19:07.862861 muon-0.1.6/muon/_atac/_ref/jaspar/MA0806.1.pfm
+-rw-r--r--   0        0        0      212 2024-04-09 08:19:07.863407 muon-0.1.6/muon/_atac/_ref/jaspar/MA0807.1.pfm
+-rw-r--r--   0        0        0      215 2024-04-09 08:19:07.864169 muon-0.1.6/muon/_atac/_ref/jaspar/MA0808.1.pfm
+-rw-r--r--   0        0        0      332 2024-04-09 08:19:07.864653 muon-0.1.6/muon/_atac/_ref/jaspar/MA0809.2.pfm
+-rw-r--r--   0        0        0      326 2024-04-09 08:19:07.865258 muon-0.1.6/muon/_atac/_ref/jaspar/MA0810.1.pfm
+-rw-r--r--   0        0        0      325 2024-04-09 08:19:07.865973 muon-0.1.6/muon/_atac/_ref/jaspar/MA0811.1.pfm
+-rw-r--r--   0        0        0      299 2024-04-09 08:19:07.866458 muon-0.1.6/muon/_atac/_ref/jaspar/MA0812.1.pfm
+-rw-r--r--   0        0        0      351 2024-04-09 08:19:07.866946 muon-0.1.6/muon/_atac/_ref/jaspar/MA0813.1.pfm
+-rw-r--r--   0        0        0      388 2024-04-09 08:19:07.867742 muon-0.1.6/muon/_atac/_ref/jaspar/MA0814.2.pfm
+-rw-r--r--   0        0        0      353 2024-04-09 08:19:07.868588 muon-0.1.6/muon/_atac/_ref/jaspar/MA0815.1.pfm
+-rw-r--r--   0        0        0      265 2024-04-09 08:19:07.869116 muon-0.1.6/muon/_atac/_ref/jaspar/MA0816.1.pfm
+-rw-r--r--   0        0        0      325 2024-04-09 08:19:07.869615 muon-0.1.6/muon/_atac/_ref/jaspar/MA0817.1.pfm
+-rw-r--r--   0        0        0      266 2024-04-09 08:19:07.870130 muon-0.1.6/muon/_atac/_ref/jaspar/MA0818.1.pfm
+-rw-r--r--   0        0        0      265 2024-04-09 08:19:07.870606 muon-0.1.6/muon/_atac/_ref/jaspar/MA0819.1.pfm
+-rw-r--r--   0        0        0      268 2024-04-09 08:19:07.871135 muon-0.1.6/muon/_atac/_ref/jaspar/MA0820.1.pfm
+-rw-r--r--   0        0        0      323 2024-04-09 08:19:07.871890 muon-0.1.6/muon/_atac/_ref/jaspar/MA0821.1.pfm
+-rw-r--r--   0        0        0      323 2024-04-09 08:19:07.872651 muon-0.1.6/muon/_atac/_ref/jaspar/MA0822.1.pfm
+-rw-r--r--   0        0        0      269 2024-04-09 08:19:07.873256 muon-0.1.6/muon/_atac/_ref/jaspar/MA0823.1.pfm
+-rw-r--r--   0        0        0      268 2024-04-09 08:19:07.873886 muon-0.1.6/muon/_atac/_ref/jaspar/MA0825.1.pfm
+-rw-r--r--   0        0        0      271 2024-04-09 08:19:07.874519 muon-0.1.6/muon/_atac/_ref/jaspar/MA0826.1.pfm
+-rw-r--r--   0        0        0      269 2024-04-09 08:19:07.875152 muon-0.1.6/muon/_atac/_ref/jaspar/MA0827.1.pfm
+-rw-r--r--   0        0        0      269 2024-04-09 08:19:07.875683 muon-0.1.6/muon/_atac/_ref/jaspar/MA0828.1.pfm
+-rw-r--r--   0        0        0      384 2024-04-09 08:19:07.876152 muon-0.1.6/muon/_atac/_ref/jaspar/MA0829.2.pfm
+-rw-r--r--   0        0        0      357 2024-04-09 08:19:07.876866 muon-0.1.6/muon/_atac/_ref/jaspar/MA0830.2.pfm
+-rw-r--r--   0        0        0      206 2024-04-09 08:19:07.877396 muon-0.1.6/muon/_atac/_ref/jaspar/MA0831.2.pfm
+-rw-r--r--   0        0        0      376 2024-04-09 08:19:07.877951 muon-0.1.6/muon/_atac/_ref/jaspar/MA0832.1.pfm
+-rw-r--r--   0        0        0      385 2024-04-09 08:19:07.878672 muon-0.1.6/muon/_atac/_ref/jaspar/MA0833.2.pfm
+-rw-r--r--   0        0        0      384 2024-04-09 08:19:07.879168 muon-0.1.6/muon/_atac/_ref/jaspar/MA0834.1.pfm
+-rw-r--r--   0        0        0      300 2024-04-09 08:19:07.879910 muon-0.1.6/muon/_atac/_ref/jaspar/MA0835.2.pfm
+-rw-r--r--   0        0        0      356 2024-04-09 08:19:07.880645 muon-0.1.6/muon/_atac/_ref/jaspar/MA0836.2.pfm
+-rw-r--r--   0        0        0      270 2024-04-09 08:19:07.881130 muon-0.1.6/muon/_atac/_ref/jaspar/MA0837.1.pfm
+-rw-r--r--   0        0        0      272 2024-04-09 08:19:07.881833 muon-0.1.6/muon/_atac/_ref/jaspar/MA0838.1.pfm
+-rw-r--r--   0        0        0      380 2024-04-09 08:19:07.882315 muon-0.1.6/muon/_atac/_ref/jaspar/MA0839.1.pfm
+-rw-r--r--   0        0        0      326 2024-04-09 08:19:07.883753 muon-0.1.6/muon/_atac/_ref/jaspar/MA0840.1.pfm
+-rw-r--r--   0        0        0      299 2024-04-09 08:19:07.884229 muon-0.1.6/muon/_atac/_ref/jaspar/MA0841.1.pfm
+-rw-r--r--   0        0        0      357 2024-04-09 08:19:07.884697 muon-0.1.6/muon/_atac/_ref/jaspar/MA0842.2.pfm
+-rw-r--r--   0        0        0      326 2024-04-09 08:19:07.885177 muon-0.1.6/muon/_atac/_ref/jaspar/MA0843.1.pfm
+-rw-r--r--   0        0        0      382 2024-04-09 08:19:07.885650 muon-0.1.6/muon/_atac/_ref/jaspar/MA0844.1.pfm
+-rw-r--r--   0        0        0      298 2024-04-09 08:19:07.886563 muon-0.1.6/muon/_atac/_ref/jaspar/MA0845.1.pfm
+-rw-r--r--   0        0        0      328 2024-04-09 08:19:07.887158 muon-0.1.6/muon/_atac/_ref/jaspar/MA0846.1.pfm
+-rw-r--r--   0        0        0      355 2024-04-09 08:19:07.888869 muon-0.1.6/muon/_atac/_ref/jaspar/MA0847.2.pfm
+-rw-r--r--   0        0        0      183 2024-04-09 08:19:07.890323 muon-0.1.6/muon/_atac/_ref/jaspar/MA0848.1.pfm
+-rw-r--r--   0        0        0      182 2024-04-09 08:19:07.890855 muon-0.1.6/muon/_atac/_ref/jaspar/MA0849.1.pfm
+-rw-r--r--   0        0        0      179 2024-04-09 08:19:07.892847 muon-0.1.6/muon/_atac/_ref/jaspar/MA0850.1.pfm
+-rw-r--r--   0        0        0      460 2024-04-09 08:19:07.893659 muon-0.1.6/muon/_atac/_ref/jaspar/MA0851.1.pfm
+-rw-r--r--   0        0        0      380 2024-04-09 08:19:07.894660 muon-0.1.6/muon/_atac/_ref/jaspar/MA0852.2.pfm
+-rw-r--r--   0        0        0      460 2024-04-09 08:19:07.895574 muon-0.1.6/muon/_atac/_ref/jaspar/MA0853.1.pfm
+-rw-r--r--   0        0        0      460 2024-04-09 08:19:07.896961 muon-0.1.6/muon/_atac/_ref/jaspar/MA0854.1.pfm
+-rw-r--r--   0        0        0      382 2024-04-09 08:19:07.898554 muon-0.1.6/muon/_atac/_ref/jaspar/MA0855.1.pfm
+-rw-r--r--   0        0        0      385 2024-04-09 08:19:07.900081 muon-0.1.6/muon/_atac/_ref/jaspar/MA0856.1.pfm
+-rw-r--r--   0        0        0      437 2024-04-09 08:19:07.900853 muon-0.1.6/muon/_atac/_ref/jaspar/MA0857.1.pfm
+-rw-r--r--   0        0        0      459 2024-04-09 08:19:07.902406 muon-0.1.6/muon/_atac/_ref/jaspar/MA0858.1.pfm
+-rw-r--r--   0        0        0      442 2024-04-09 08:19:07.903793 muon-0.1.6/muon/_atac/_ref/jaspar/MA0859.1.pfm
+-rw-r--r--   0        0        0      463 2024-04-09 08:19:07.904494 muon-0.1.6/muon/_atac/_ref/jaspar/MA0860.1.pfm
+-rw-r--r--   0        0        0      495 2024-04-09 08:19:07.906051 muon-0.1.6/muon/_atac/_ref/jaspar/MA0861.1.pfm
+-rw-r--r--   0        0        0      210 2024-04-09 08:19:07.906730 muon-0.1.6/muon/_atac/_ref/jaspar/MA0862.1.pfm
+-rw-r--r--   0        0        0      373 2024-04-09 08:19:07.907721 muon-0.1.6/muon/_atac/_ref/jaspar/MA0863.1.pfm
+-rw-r--r--   0        0        0      438 2024-04-09 08:19:07.908392 muon-0.1.6/muon/_atac/_ref/jaspar/MA0864.2.pfm
+-rw-r--r--   0        0        0      317 2024-04-09 08:19:07.909270 muon-0.1.6/muon/_atac/_ref/jaspar/MA0865.1.pfm
+-rw-r--r--   0        0        0      409 2024-04-09 08:19:07.910006 muon-0.1.6/muon/_atac/_ref/jaspar/MA0866.1.pfm
+-rw-r--r--   0        0        0      272 2024-04-09 08:19:07.910715 muon-0.1.6/muon/_atac/_ref/jaspar/MA0867.2.pfm
+-rw-r--r--   0        0        0      270 2024-04-09 08:19:07.911403 muon-0.1.6/muon/_atac/_ref/jaspar/MA0868.2.pfm
+-rw-r--r--   0        0        0      402 2024-04-09 08:19:07.912005 muon-0.1.6/muon/_atac/_ref/jaspar/MA0869.1.pfm
+-rw-r--r--   0        0        0      409 2024-04-09 08:19:07.912865 muon-0.1.6/muon/_atac/_ref/jaspar/MA0870.1.pfm
+-rw-r--r--   0        0        0      300 2024-04-09 08:19:07.913426 muon-0.1.6/muon/_atac/_ref/jaspar/MA0871.2.pfm
+-rw-r--r--   0        0        0      352 2024-04-09 08:19:07.914102 muon-0.1.6/muon/_atac/_ref/jaspar/MA0872.1.pfm
+-rw-r--r--   0        0        0      295 2024-04-09 08:19:07.916026 muon-0.1.6/muon/_atac/_ref/jaspar/MA0873.1.pfm
+-rw-r--r--   0        0        0      460 2024-04-09 08:19:07.916738 muon-0.1.6/muon/_atac/_ref/jaspar/MA0874.1.pfm
+-rw-r--r--   0        0        0      215 2024-04-09 08:19:07.917522 muon-0.1.6/muon/_atac/_ref/jaspar/MA0875.1.pfm
+-rw-r--r--   0        0        0      216 2024-04-09 08:19:07.918248 muon-0.1.6/muon/_atac/_ref/jaspar/MA0876.1.pfm
+-rw-r--r--   0        0        0      214 2024-04-09 08:19:07.919117 muon-0.1.6/muon/_atac/_ref/jaspar/MA0877.2.pfm
+-rw-r--r--   0        0        0      300 2024-04-09 08:19:07.919916 muon-0.1.6/muon/_atac/_ref/jaspar/MA0878.2.pfm
+-rw-r--r--   0        0        0      272 2024-04-09 08:19:07.920384 muon-0.1.6/muon/_atac/_ref/jaspar/MA0879.1.pfm
+-rw-r--r--   0        0        0      216 2024-04-09 08:19:07.920826 muon-0.1.6/muon/_atac/_ref/jaspar/MA0880.1.pfm
+-rw-r--r--   0        0        0      216 2024-04-09 08:19:07.921473 muon-0.1.6/muon/_atac/_ref/jaspar/MA0881.1.pfm
+-rw-r--r--   0        0        0      212 2024-04-09 08:19:07.921985 muon-0.1.6/muon/_atac/_ref/jaspar/MA0882.1.pfm
+-rw-r--r--   0        0        0      460 2024-04-09 08:19:07.922806 muon-0.1.6/muon/_atac/_ref/jaspar/MA0883.1.pfm
+-rw-r--r--   0        0        0      352 2024-04-09 08:19:07.923646 muon-0.1.6/muon/_atac/_ref/jaspar/MA0884.1.pfm
+-rw-r--r--   0        0        0      216 2024-04-09 08:19:07.924388 muon-0.1.6/muon/_atac/_ref/jaspar/MA0885.1.pfm
+-rw-r--r--   0        0        0      274 2024-04-09 08:19:07.925140 muon-0.1.6/muon/_atac/_ref/jaspar/MA0886.1.pfm
+-rw-r--r--   0        0        0      272 2024-04-09 08:19:07.925770 muon-0.1.6/muon/_atac/_ref/jaspar/MA0887.1.pfm
+-rw-r--r--   0        0        0      272 2024-04-09 08:19:07.926451 muon-0.1.6/muon/_atac/_ref/jaspar/MA0888.1.pfm
+-rw-r--r--   0        0        0      273 2024-04-09 08:19:07.927263 muon-0.1.6/muon/_atac/_ref/jaspar/MA0889.1.pfm
+-rw-r--r--   0        0        0      273 2024-04-09 08:19:07.927737 muon-0.1.6/muon/_atac/_ref/jaspar/MA0890.1.pfm
+-rw-r--r--   0        0        0      268 2024-04-09 08:19:07.928410 muon-0.1.6/muon/_atac/_ref/jaspar/MA0891.1.pfm
+-rw-r--r--   0        0        0      268 2024-04-09 08:19:07.928855 muon-0.1.6/muon/_atac/_ref/jaspar/MA0892.1.pfm
+-rw-r--r--   0        0        0      212 2024-04-09 08:19:07.929298 muon-0.1.6/muon/_atac/_ref/jaspar/MA0893.2.pfm
+-rw-r--r--   0        0        0      269 2024-04-09 08:19:07.929739 muon-0.1.6/muon/_atac/_ref/jaspar/MA0894.1.pfm
+-rw-r--r--   0        0        0      268 2024-04-09 08:19:07.931047 muon-0.1.6/muon/_atac/_ref/jaspar/MA0895.1.pfm
+-rw-r--r--   0        0        0      460 2024-04-09 08:19:07.931504 muon-0.1.6/muon/_atac/_ref/jaspar/MA0896.1.pfm
+-rw-r--r--   0        0        0      459 2024-04-09 08:19:07.933054 muon-0.1.6/muon/_atac/_ref/jaspar/MA0897.1.pfm
+-rw-r--r--   0        0        0      459 2024-04-09 08:19:07.933575 muon-0.1.6/muon/_atac/_ref/jaspar/MA0898.1.pfm
+-rw-r--r--   0        0        0      300 2024-04-09 08:19:07.934527 muon-0.1.6/muon/_atac/_ref/jaspar/MA0899.1.pfm
+-rw-r--r--   0        0        0      218 2024-04-09 08:19:07.935163 muon-0.1.6/muon/_atac/_ref/jaspar/MA0900.2.pfm
+-rw-r--r--   0        0        0      388 2024-04-09 08:19:07.935690 muon-0.1.6/muon/_atac/_ref/jaspar/MA0901.2.pfm
+-rw-r--r--   0        0        0      215 2024-04-09 08:19:07.936430 muon-0.1.6/muon/_atac/_ref/jaspar/MA0902.2.pfm
+-rw-r--r--   0        0        0      272 2024-04-09 08:19:07.938862 muon-0.1.6/muon/_atac/_ref/jaspar/MA0903.1.pfm
+-rw-r--r--   0        0        0      214 2024-04-09 08:19:07.939947 muon-0.1.6/muon/_atac/_ref/jaspar/MA0904.2.pfm
+-rw-r--r--   0        0        0      270 2024-04-09 08:19:07.940460 muon-0.1.6/muon/_atac/_ref/jaspar/MA0905.1.pfm
+-rw-r--r--   0        0        0      298 2024-04-09 08:19:07.941087 muon-0.1.6/muon/_atac/_ref/jaspar/MA0906.1.pfm
+-rw-r--r--   0        0        0      296 2024-04-09 08:19:07.941792 muon-0.1.6/muon/_atac/_ref/jaspar/MA0907.1.pfm
+-rw-r--r--   0        0        0      265 2024-04-09 08:19:07.942927 muon-0.1.6/muon/_atac/_ref/jaspar/MA0908.1.pfm
+-rw-r--r--   0        0        0      294 2024-04-09 08:19:07.943704 muon-0.1.6/muon/_atac/_ref/jaspar/MA0909.2.pfm
+-rw-r--r--   0        0        0      213 2024-04-09 08:19:07.945745 muon-0.1.6/muon/_atac/_ref/jaspar/MA0910.2.pfm
+-rw-r--r--   0        0        0      324 2024-04-09 08:19:07.946298 muon-0.1.6/muon/_atac/_ref/jaspar/MA0911.1.pfm
+-rw-r--r--   0        0        0      215 2024-04-09 08:19:07.947067 muon-0.1.6/muon/_atac/_ref/jaspar/MA0912.2.pfm
+-rw-r--r--   0        0        0      271 2024-04-09 08:19:07.948078 muon-0.1.6/muon/_atac/_ref/jaspar/MA0913.2.pfm
+-rw-r--r--   0        0        0      216 2024-04-09 08:19:07.950332 muon-0.1.6/muon/_atac/_ref/jaspar/MA0914.1.pfm
+-rw-r--r--   0        0        0      273 2024-04-09 08:19:07.951074 muon-0.1.6/muon/_atac/_ref/jaspar/MA1099.2.pfm
+-rw-r--r--   0        0        0      270 2024-04-09 08:19:07.951837 muon-0.1.6/muon/_atac/_ref/jaspar/MA1100.2.pfm
+-rw-r--r--   0        0        0      528 2024-04-09 08:19:07.953459 muon-0.1.6/muon/_atac/_ref/jaspar/MA1101.2.pfm
+-rw-r--r--   0        0        0      328 2024-04-09 08:19:07.954049 muon-0.1.6/muon/_atac/_ref/jaspar/MA1102.2.pfm
+-rw-r--r--   0        0        0      300 2024-04-09 08:19:07.954645 muon-0.1.6/muon/_atac/_ref/jaspar/MA1103.2.pfm
+-rw-r--r--   0        0        0      360 2024-04-09 08:19:07.956441 muon-0.1.6/muon/_atac/_ref/jaspar/MA1104.2.pfm
+-rw-r--r--   0        0        0      329 2024-04-09 08:19:07.957714 muon-0.1.6/muon/_atac/_ref/jaspar/MA1105.2.pfm
+-rw-r--r--   0        0        0      268 2024-04-09 08:19:07.958283 muon-0.1.6/muon/_atac/_ref/jaspar/MA1106.1.pfm
+-rw-r--r--   0        0        0      441 2024-04-09 08:19:07.959104 muon-0.1.6/muon/_atac/_ref/jaspar/MA1107.2.pfm
+-rw-r--r--   0        0        0      272 2024-04-09 08:19:07.959622 muon-0.1.6/muon/_atac/_ref/jaspar/MA1108.2.pfm
+-rw-r--r--   0        0        0      352 2024-04-09 08:19:07.960176 muon-0.1.6/muon/_atac/_ref/jaspar/MA1109.1.pfm
+-rw-r--r--   0        0        0      294 2024-04-09 08:19:07.960676 muon-0.1.6/muon/_atac/_ref/jaspar/MA1110.1.pfm
+-rw-r--r--   0        0        0      296 2024-04-09 08:19:07.961417 muon-0.1.6/muon/_atac/_ref/jaspar/MA1111.1.pfm
+-rw-r--r--   0        0        0      328 2024-04-09 08:19:07.961928 muon-0.1.6/muon/_atac/_ref/jaspar/MA1112.2.pfm
+-rw-r--r--   0        0        0      356 2024-04-09 08:19:07.962394 muon-0.1.6/muon/_atac/_ref/jaspar/MA1113.2.pfm
+-rw-r--r--   0        0        0      468 2024-04-09 08:19:07.962905 muon-0.1.6/muon/_atac/_ref/jaspar/MA1114.1.pfm
+-rw-r--r--   0        0        0      300 2024-04-09 08:19:07.963404 muon-0.1.6/muon/_atac/_ref/jaspar/MA1115.1.pfm
+-rw-r--r--   0        0        0      268 2024-04-09 08:19:07.964196 muon-0.1.6/muon/_atac/_ref/jaspar/MA1116.1.pfm
+-rw-r--r--   0        0        0      297 2024-04-09 08:19:07.964712 muon-0.1.6/muon/_atac/_ref/jaspar/MA1117.1.pfm
+-rw-r--r--   0        0        0      294 2024-04-09 08:19:07.966678 muon-0.1.6/muon/_atac/_ref/jaspar/MA1118.1.pfm
+-rw-r--r--   0        0        0      440 2024-04-09 08:19:07.967415 muon-0.1.6/muon/_atac/_ref/jaspar/MA1119.1.pfm
+-rw-r--r--   0        0        0      298 2024-04-09 08:19:07.968532 muon-0.1.6/muon/_atac/_ref/jaspar/MA1120.1.pfm
+-rw-r--r--   0        0        0      352 2024-04-09 08:19:07.969759 muon-0.1.6/muon/_atac/_ref/jaspar/MA1121.1.pfm
+-rw-r--r--   0        0        0      296 2024-04-09 08:19:07.970410 muon-0.1.6/muon/_atac/_ref/jaspar/MA1122.1.pfm
+-rw-r--r--   0        0        0      356 2024-04-09 08:19:07.971804 muon-0.1.6/muon/_atac/_ref/jaspar/MA1123.2.pfm
+-rw-r--r--   0        0        0      357 2024-04-09 08:19:07.972571 muon-0.1.6/muon/_atac/_ref/jaspar/MA1124.1.pfm
+-rw-r--r--   0        0        0      329 2024-04-09 08:19:07.974276 muon-0.1.6/muon/_atac/_ref/jaspar/MA1125.1.pfm
+-rw-r--r--   0        0        0      435 2024-04-09 08:19:07.975262 muon-0.1.6/muon/_atac/_ref/jaspar/MA1126.1.pfm
+-rw-r--r--   0        0        0      295 2024-04-09 08:19:07.975872 muon-0.1.6/muon/_atac/_ref/jaspar/MA1127.1.pfm
+-rw-r--r--   0        0        0      352 2024-04-09 08:19:07.976930 muon-0.1.6/muon/_atac/_ref/jaspar/MA1128.1.pfm
+-rw-r--r--   0        0        0      266 2024-04-09 08:19:07.977841 muon-0.1.6/muon/_atac/_ref/jaspar/MA1129.1.pfm
+-rw-r--r--   0        0        0      324 2024-04-09 08:19:07.978520 muon-0.1.6/muon/_atac/_ref/jaspar/MA1130.1.pfm
+-rw-r--r--   0        0        0      295 2024-04-09 08:19:07.979311 muon-0.1.6/muon/_atac/_ref/jaspar/MA1131.1.pfm
+-rw-r--r--   0        0        0      268 2024-04-09 08:19:07.980476 muon-0.1.6/muon/_atac/_ref/jaspar/MA1132.1.pfm
+-rw-r--r--   0        0        0      323 2024-04-09 08:19:07.981377 muon-0.1.6/muon/_atac/_ref/jaspar/MA1133.1.pfm
+-rw-r--r--   0        0        0      324 2024-04-09 08:19:07.982116 muon-0.1.6/muon/_atac/_ref/jaspar/MA1134.1.pfm
+-rw-r--r--   0        0        0      268 2024-04-09 08:19:07.982837 muon-0.1.6/muon/_atac/_ref/jaspar/MA1135.1.pfm
+-rw-r--r--   0        0        0      266 2024-04-09 08:19:07.983439 muon-0.1.6/muon/_atac/_ref/jaspar/MA1136.1.pfm
+-rw-r--r--   0        0        0      352 2024-04-09 08:19:07.984138 muon-0.1.6/muon/_atac/_ref/jaspar/MA1137.1.pfm
+-rw-r--r--   0        0        0      268 2024-04-09 08:19:07.984969 muon-0.1.6/muon/_atac/_ref/jaspar/MA1138.1.pfm
+-rw-r--r--   0        0        0      324 2024-04-09 08:19:07.985968 muon-0.1.6/muon/_atac/_ref/jaspar/MA1139.1.pfm
+-rw-r--r--   0        0        0      321 2024-04-09 08:19:07.988057 muon-0.1.6/muon/_atac/_ref/jaspar/MA1140.2.pfm
+-rw-r--r--   0        0        0      352 2024-04-09 08:19:07.989428 muon-0.1.6/muon/_atac/_ref/jaspar/MA1141.1.pfm
+-rw-r--r--   0        0        0      268 2024-04-09 08:19:07.989984 muon-0.1.6/muon/_atac/_ref/jaspar/MA1142.1.pfm
+-rw-r--r--   0        0        0      266 2024-04-09 08:19:07.990738 muon-0.1.6/muon/_atac/_ref/jaspar/MA1143.1.pfm
+-rw-r--r--   0        0        0      268 2024-04-09 08:19:07.991322 muon-0.1.6/muon/_atac/_ref/jaspar/MA1144.1.pfm
+-rw-r--r--   0        0        0      408 2024-04-09 08:19:07.992707 muon-0.1.6/muon/_atac/_ref/jaspar/MA1145.1.pfm
+-rw-r--r--   0        0        0      408 2024-04-09 08:19:07.993214 muon-0.1.6/muon/_atac/_ref/jaspar/MA1146.1.pfm
+-rw-r--r--   0        0        0      408 2024-04-09 08:19:07.993726 muon-0.1.6/muon/_atac/_ref/jaspar/MA1147.1.pfm
+-rw-r--r--   0        0        0      492 2024-04-09 08:19:07.994325 muon-0.1.6/muon/_atac/_ref/jaspar/MA1148.1.pfm
+-rw-r--r--   0        0        0      492 2024-04-09 08:19:07.996814 muon-0.1.6/muon/_atac/_ref/jaspar/MA1149.1.pfm
+-rw-r--r--   0        0        0      294 2024-04-09 08:19:07.997350 muon-0.1.6/muon/_atac/_ref/jaspar/MA1150.1.pfm
+-rw-r--r--   0        0        0      324 2024-04-09 08:19:07.998209 muon-0.1.6/muon/_atac/_ref/jaspar/MA1151.1.pfm
+-rw-r--r--   0        0        0      267 2024-04-09 08:19:07.998827 muon-0.1.6/muon/_atac/_ref/jaspar/MA1152.1.pfm
+-rw-r--r--   0        0        0      210 2024-04-09 08:19:07.999332 muon-0.1.6/muon/_atac/_ref/jaspar/MA1153.1.pfm
+-rw-r--r--   0        0        0      461 2024-04-09 08:19:07.999824 muon-0.1.6/muon/_atac/_ref/jaspar/MA1154.1.pfm
+-rw-r--r--   0        0        0      409 2024-04-09 08:19:08.000347 muon-0.1.6/muon/_atac/_ref/jaspar/MA1155.1.pfm
+-rw-r--r--   0        0        0      580 2024-04-09 08:19:08.000878 muon-0.1.6/muon/_atac/_ref/jaspar/MA1418.1.pfm
+-rw-r--r--   0        0        0      415 2024-04-09 08:19:08.001445 muon-0.1.6/muon/_atac/_ref/jaspar/MA1419.1.pfm
+-rw-r--r--   0        0        0      377 2024-04-09 08:19:08.001972 muon-0.1.6/muon/_atac/_ref/jaspar/MA1420.1.pfm
+-rw-r--r--   0        0        0      320 2024-04-09 08:19:08.002681 muon-0.1.6/muon/_atac/_ref/jaspar/MA1421.1.pfm
+-rw-r--r--   0        0        0      272 2024-04-09 08:19:08.003226 muon-0.1.6/muon/_atac/_ref/jaspar/MA1463.1.pfm
+-rw-r--r--   0        0        0      274 2024-04-09 08:19:08.003749 muon-0.1.6/muon/_atac/_ref/jaspar/MA1464.1.pfm
+-rw-r--r--   0        0        0      379 2024-04-09 08:19:08.005212 muon-0.1.6/muon/_atac/_ref/jaspar/MA1466.1.pfm
+-rw-r--r--   0        0        0      267 2024-04-09 08:19:08.005895 muon-0.1.6/muon/_atac/_ref/jaspar/MA1467.1.pfm
+-rw-r--r--   0        0        0      266 2024-04-09 08:19:08.006621 muon-0.1.6/muon/_atac/_ref/jaspar/MA1468.1.pfm
+-rw-r--r--   0        0        0      545 2024-04-09 08:19:08.008387 muon-0.1.6/muon/_atac/_ref/jaspar/MA1470.1.pfm
+-rw-r--r--   0        0        0      328 2024-04-09 08:19:08.009303 muon-0.1.6/muon/_atac/_ref/jaspar/MA1471.1.pfm
+-rw-r--r--   0        0        0      268 2024-04-09 08:19:08.011013 muon-0.1.6/muon/_atac/_ref/jaspar/MA1472.1.pfm
+-rw-r--r--   0        0        0      301 2024-04-09 08:19:08.012410 muon-0.1.6/muon/_atac/_ref/jaspar/MA1473.1.pfm
+-rw-r--r--   0        0        0      326 2024-04-09 08:19:08.012979 muon-0.1.6/muon/_atac/_ref/jaspar/MA1474.1.pfm
+-rw-r--r--   0        0        0      324 2024-04-09 08:19:08.013553 muon-0.1.6/muon/_atac/_ref/jaspar/MA1475.1.pfm
+-rw-r--r--   0        0        0      216 2024-04-09 08:19:08.014057 muon-0.1.6/muon/_atac/_ref/jaspar/MA1476.1.pfm
+-rw-r--r--   0        0        0      324 2024-04-09 08:19:08.014524 muon-0.1.6/muon/_atac/_ref/jaspar/MA1478.1.pfm
+-rw-r--r--   0        0        0      323 2024-04-09 08:19:08.015069 muon-0.1.6/muon/_atac/_ref/jaspar/MA1479.1.pfm
+-rw-r--r--   0        0        0      271 2024-04-09 08:19:08.016222 muon-0.1.6/muon/_atac/_ref/jaspar/MA1480.1.pfm
+-rw-r--r--   0        0        0      216 2024-04-09 08:19:08.016788 muon-0.1.6/muon/_atac/_ref/jaspar/MA1481.1.pfm
+-rw-r--r--   0        0        0      328 2024-04-09 08:19:08.018003 muon-0.1.6/muon/_atac/_ref/jaspar/MA1483.1.pfm
+-rw-r--r--   0        0        0      272 2024-04-09 08:19:08.018790 muon-0.1.6/muon/_atac/_ref/jaspar/MA1484.1.pfm
+-rw-r--r--   0        0        0      382 2024-04-09 08:19:08.020305 muon-0.1.6/muon/_atac/_ref/jaspar/MA1485.1.pfm
+-rw-r--r--   0        0        0      407 2024-04-09 08:19:08.020810 muon-0.1.6/muon/_atac/_ref/jaspar/MA1487.1.pfm
+-rw-r--r--   0        0        0      206 2024-04-09 08:19:08.021508 muon-0.1.6/muon/_atac/_ref/jaspar/MA1489.1.pfm
+-rw-r--r--   0        0        0      412 2024-04-09 08:19:08.022029 muon-0.1.6/muon/_atac/_ref/jaspar/MA1491.1.pfm
+-rw-r--r--   0        0        0      265 2024-04-09 08:19:08.022655 muon-0.1.6/muon/_atac/_ref/jaspar/MA1493.1.pfm
+-rw-r--r--   0        0        0      406 2024-04-09 08:19:08.023148 muon-0.1.6/muon/_atac/_ref/jaspar/MA1494.1.pfm
+-rw-r--r--   0        0        0      216 2024-04-09 08:19:08.024429 muon-0.1.6/muon/_atac/_ref/jaspar/MA1495.1.pfm
+-rw-r--r--   0        0        0      213 2024-04-09 08:19:08.025212 muon-0.1.6/muon/_atac/_ref/jaspar/MA1496.1.pfm
+-rw-r--r--   0        0        0      272 2024-04-09 08:19:08.026162 muon-0.1.6/muon/_atac/_ref/jaspar/MA1497.1.pfm
+-rw-r--r--   0        0        0      213 2024-04-09 08:19:08.026996 muon-0.1.6/muon/_atac/_ref/jaspar/MA1498.1.pfm
+-rw-r--r--   0        0        0      216 2024-04-09 08:19:08.027808 muon-0.1.6/muon/_atac/_ref/jaspar/MA1499.1.pfm
+-rw-r--r--   0        0        0      216 2024-04-09 08:19:08.028599 muon-0.1.6/muon/_atac/_ref/jaspar/MA1500.1.pfm
+-rw-r--r--   0        0        0      268 2024-04-09 08:19:08.029124 muon-0.1.6/muon/_atac/_ref/jaspar/MA1501.1.pfm
+-rw-r--r--   0        0        0      213 2024-04-09 08:19:08.029725 muon-0.1.6/muon/_atac/_ref/jaspar/MA1502.1.pfm
+-rw-r--r--   0        0        0      267 2024-04-09 08:19:08.030297 muon-0.1.6/muon/_atac/_ref/jaspar/MA1503.1.pfm
+-rw-r--r--   0        0        0      216 2024-04-09 08:19:08.032167 muon-0.1.6/muon/_atac/_ref/jaspar/MA1504.1.pfm
+-rw-r--r--   0        0        0      216 2024-04-09 08:19:08.032687 muon-0.1.6/muon/_atac/_ref/jaspar/MA1505.1.pfm
+-rw-r--r--   0        0        0      298 2024-04-09 08:19:08.034236 muon-0.1.6/muon/_atac/_ref/jaspar/MA1506.1.pfm
+-rw-r--r--   0        0        0      214 2024-04-09 08:19:08.035024 muon-0.1.6/muon/_atac/_ref/jaspar/MA1507.1.pfm
+-rw-r--r--   0        0        0      328 2024-04-09 08:19:08.035747 muon-0.1.6/muon/_atac/_ref/jaspar/MA1508.1.pfm
+-rw-r--r--   0        0        0      240 2024-04-09 08:19:09.843526 muon-0.1.6/muon/_atac/_ref/jaspar/MA1509.1.pfm
+-rw-r--r--   0        0        0      301 2024-04-09 08:19:09.852300 muon-0.1.6/muon/_atac/_ref/jaspar/MA1511.1.pfm
+-rw-r--r--   0        0        0      300 2024-04-09 08:19:09.852782 muon-0.1.6/muon/_atac/_ref/jaspar/MA1512.1.pfm
+-rw-r--r--   0        0        0      300 2024-04-09 08:19:09.853062 muon-0.1.6/muon/_atac/_ref/jaspar/MA1513.1.pfm
+-rw-r--r--   0        0        0      413 2024-04-09 08:19:09.853560 muon-0.1.6/muon/_atac/_ref/jaspar/MA1514.1.pfm
+-rw-r--r--   0        0        0      299 2024-04-09 08:19:09.874791 muon-0.1.6/muon/_atac/_ref/jaspar/MA1515.1.pfm
+-rw-r--r--   0        0        0      301 2024-04-09 08:19:09.875255 muon-0.1.6/muon/_atac/_ref/jaspar/MA1516.1.pfm
+-rw-r--r--   0        0        0      296 2024-04-09 08:19:09.875558 muon-0.1.6/muon/_atac/_ref/jaspar/MA1517.1.pfm
+-rw-r--r--   0        0        0      216 2024-04-09 08:19:09.899634 muon-0.1.6/muon/_atac/_ref/jaspar/MA1518.1.pfm
+-rw-r--r--   0        0        0      215 2024-04-09 08:19:09.900152 muon-0.1.6/muon/_atac/_ref/jaspar/MA1519.1.pfm
+-rw-r--r--   0        0        0      408 2024-04-09 08:19:09.900535 muon-0.1.6/muon/_atac/_ref/jaspar/MA1520.1.pfm
+-rw-r--r--   0        0        0      412 2024-04-09 08:19:09.900865 muon-0.1.6/muon/_atac/_ref/jaspar/MA1521.1.pfm
+-rw-r--r--   0        0        0      300 2024-04-09 08:19:09.901120 muon-0.1.6/muon/_atac/_ref/jaspar/MA1522.1.pfm
+-rw-r--r--   0        0        0      267 2024-04-09 08:19:09.901391 muon-0.1.6/muon/_atac/_ref/jaspar/MA1523.1.pfm
+-rw-r--r--   0        0        0      328 2024-04-09 08:19:09.901710 muon-0.1.6/muon/_atac/_ref/jaspar/MA1524.1.pfm
+-rw-r--r--   0        0        0      269 2024-04-09 08:19:09.902043 muon-0.1.6/muon/_atac/_ref/jaspar/MA1525.1.pfm
+-rw-r--r--   0        0        0      464 2024-04-09 08:19:09.902405 muon-0.1.6/muon/_atac/_ref/jaspar/MA1527.1.pfm
+-rw-r--r--   0        0        0      468 2024-04-09 08:19:09.902894 muon-0.1.6/muon/_atac/_ref/jaspar/MA1528.1.pfm
+-rw-r--r--   0        0        0      496 2024-04-09 08:19:09.903213 muon-0.1.6/muon/_atac/_ref/jaspar/MA1529.1.pfm
+-rw-r--r--   0        0        0      242 2024-04-09 08:19:09.903531 muon-0.1.6/muon/_atac/_ref/jaspar/MA1530.1.pfm
+-rw-r--r--   0        0        0      409 2024-04-09 08:19:09.903791 muon-0.1.6/muon/_atac/_ref/jaspar/MA1531.1.pfm
+-rw-r--r--   0        0        0      407 2024-04-09 08:19:09.904101 muon-0.1.6/muon/_atac/_ref/jaspar/MA1532.1.pfm
+-rw-r--r--   0        0        0      460 2024-04-09 08:19:09.904369 muon-0.1.6/muon/_atac/_ref/jaspar/MA1533.1.pfm
+-rw-r--r--   0        0        0      246 2024-04-09 08:19:09.904767 muon-0.1.6/muon/_atac/_ref/jaspar/MA1534.1.pfm
+-rw-r--r--   0        0        0      244 2024-04-09 08:19:09.905065 muon-0.1.6/muon/_atac/_ref/jaspar/MA1535.1.pfm
+-rw-r--r--   0        0        0      216 2024-04-09 08:19:09.905371 muon-0.1.6/muon/_atac/_ref/jaspar/MA1536.1.pfm
+-rw-r--r--   0        0        0      414 2024-04-09 08:19:09.905656 muon-0.1.6/muon/_atac/_ref/jaspar/MA1537.1.pfm
+-rw-r--r--   0        0        0      410 2024-04-09 08:19:09.905909 muon-0.1.6/muon/_atac/_ref/jaspar/MA1538.1.pfm
+-rw-r--r--   0        0        0      410 2024-04-09 08:19:09.906150 muon-0.1.6/muon/_atac/_ref/jaspar/MA1539.1.pfm
+-rw-r--r--   0        0        0      298 2024-04-09 08:19:09.906426 muon-0.1.6/muon/_atac/_ref/jaspar/MA1540.1.pfm
+-rw-r--r--   0        0        0      464 2024-04-09 08:19:09.906679 muon-0.1.6/muon/_atac/_ref/jaspar/MA1541.1.pfm
+-rw-r--r--   0        0        0      271 2024-04-09 08:19:09.906953 muon-0.1.6/muon/_atac/_ref/jaspar/MA1542.1.pfm
+-rw-r--r--   0        0        0      384 2024-04-09 08:19:09.907180 muon-0.1.6/muon/_atac/_ref/jaspar/MA1544.1.pfm
+-rw-r--r--   0        0        0      356 2024-04-09 08:19:09.907435 muon-0.1.6/muon/_atac/_ref/jaspar/MA1545.1.pfm
+-rw-r--r--   0        0        0      436 2024-04-09 08:19:09.907701 muon-0.1.6/muon/_atac/_ref/jaspar/MA1546.1.pfm
+-rw-r--r--   0        0        0      216 2024-04-09 08:19:09.907928 muon-0.1.6/muon/_atac/_ref/jaspar/MA1547.1.pfm
+-rw-r--r--   0        0        0      268 2024-04-09 08:19:09.908196 muon-0.1.6/muon/_atac/_ref/jaspar/MA1548.1.pfm
+-rw-r--r--   0        0        0      271 2024-04-09 08:19:09.953457 muon-0.1.6/muon/_atac/_ref/jaspar/MA1549.1.pfm
+-rw-r--r--   0        0        0      440 2024-04-09 08:19:09.953908 muon-0.1.6/muon/_atac/_ref/jaspar/MA1550.1.pfm
+-rw-r--r--   0        0        0      378 2024-04-09 08:19:09.954203 muon-0.1.6/muon/_atac/_ref/jaspar/MA1552.1.pfm
+-rw-r--r--   0        0        0      381 2024-04-09 08:19:09.954445 muon-0.1.6/muon/_atac/_ref/jaspar/MA1553.1.pfm
+-rw-r--r--   0        0        0      236 2024-04-09 08:19:09.954709 muon-0.1.6/muon/_atac/_ref/jaspar/MA1554.1.pfm
+-rw-r--r--   0        0        0      380 2024-04-09 08:19:09.954977 muon-0.1.6/muon/_atac/_ref/jaspar/MA1555.1.pfm
+-rw-r--r--   0        0        0      380 2024-04-09 08:19:09.955280 muon-0.1.6/muon/_atac/_ref/jaspar/MA1556.1.pfm
+-rw-r--r--   0        0        0      270 2024-04-09 08:19:09.955967 muon-0.1.6/muon/_atac/_ref/jaspar/MA1557.1.pfm
+-rw-r--r--   0        0        0      272 2024-04-09 08:19:09.961179 muon-0.1.6/muon/_atac/_ref/jaspar/MA1558.1.pfm
+-rw-r--r--   0        0        0      271 2024-04-09 08:19:09.961763 muon-0.1.6/muon/_atac/_ref/jaspar/MA1559.1.pfm
+-rw-r--r--   0        0        0      268 2024-04-09 08:19:09.962035 muon-0.1.6/muon/_atac/_ref/jaspar/MA1560.1.pfm
+-rw-r--r--   0        0        0      296 2024-04-09 08:19:09.963076 muon-0.1.6/muon/_atac/_ref/jaspar/MA1561.1.pfm
+-rw-r--r--   0        0        0      268 2024-04-09 08:19:09.963497 muon-0.1.6/muon/_atac/_ref/jaspar/MA1562.1.pfm
+-rw-r--r--   0        0        0      211 2024-04-09 08:19:09.963745 muon-0.1.6/muon/_atac/_ref/jaspar/MA1563.1.pfm
+-rw-r--r--   0        0        0      324 2024-04-09 08:19:09.963986 muon-0.1.6/muon/_atac/_ref/jaspar/MA1564.1.pfm
+-rw-r--r--   0        0        0      323 2024-04-09 08:19:09.964211 muon-0.1.6/muon/_atac/_ref/jaspar/MA1565.1.pfm
+-rw-r--r--   0        0        0      269 2024-04-09 08:19:09.964448 muon-0.1.6/muon/_atac/_ref/jaspar/MA1566.1.pfm
+-rw-r--r--   0        0        0      272 2024-04-09 08:19:09.964747 muon-0.1.6/muon/_atac/_ref/jaspar/MA1567.1.pfm
+-rw-r--r--   0        0        0      324 2024-04-09 08:19:09.964963 muon-0.1.6/muon/_atac/_ref/jaspar/MA1568.1.pfm
+-rw-r--r--   0        0        0      300 2024-04-09 08:19:09.965276 muon-0.1.6/muon/_atac/_ref/jaspar/MA1569.1.pfm
+-rw-r--r--   0        0        0      267 2024-04-09 08:19:09.965607 muon-0.1.6/muon/_atac/_ref/jaspar/MA1570.1.pfm
+-rw-r--r--   0        0        0      325 2024-04-09 08:19:09.965877 muon-0.1.6/muon/_atac/_ref/jaspar/MA1571.1.pfm
+-rw-r--r--   0        0        0      325 2024-04-09 08:19:09.966394 muon-0.1.6/muon/_atac/_ref/jaspar/MA1572.1.pfm
+-rw-r--r--   0        0        0      518 2024-04-09 08:19:09.966662 muon-0.1.6/muon/_atac/_ref/jaspar/MA1573.1.pfm
+-rw-r--r--   0        0        0      412 2024-04-09 08:19:09.966920 muon-0.1.6/muon/_atac/_ref/jaspar/MA1574.1.pfm
+-rw-r--r--   0        0        0      522 2024-04-09 08:19:09.967254 muon-0.1.6/muon/_atac/_ref/jaspar/MA1575.1.pfm
+-rw-r--r--   0        0        0      518 2024-04-09 08:19:09.967483 muon-0.1.6/muon/_atac/_ref/jaspar/MA1576.1.pfm
+-rw-r--r--   0        0        0      215 2024-04-09 08:19:09.967975 muon-0.1.6/muon/_atac/_ref/jaspar/MA1577.1.pfm
+-rw-r--r--   0        0        0      265 2024-04-09 08:19:09.968291 muon-0.1.6/muon/_atac/_ref/jaspar/MA1578.1.pfm
+-rw-r--r--   0        0        0      408 2024-04-09 08:19:09.968533 muon-0.1.6/muon/_atac/_ref/jaspar/MA1579.1.pfm
+-rw-r--r--   0        0        0      268 2024-04-09 08:19:09.968765 muon-0.1.6/muon/_atac/_ref/jaspar/MA1580.1.pfm
+-rw-r--r--   0        0        0      352 2024-04-09 08:19:09.969117 muon-0.1.6/muon/_atac/_ref/jaspar/MA1581.1.pfm
+-rw-r--r--   0        0        0      356 2024-04-09 08:19:09.969445 muon-0.1.6/muon/_atac/_ref/jaspar/MA1583.1.pfm
+-rw-r--r--   0        0        0      440 2024-04-09 08:19:09.970132 muon-0.1.6/muon/_atac/_ref/jaspar/MA1584.1.pfm
+-rw-r--r--   0        0        0      269 2024-04-09 08:19:09.970418 muon-0.1.6/muon/_atac/_ref/jaspar/MA1585.1.pfm
+-rw-r--r--   0        0        0      379 2024-04-09 08:19:09.970674 muon-0.1.6/muon/_atac/_ref/jaspar/MA1587.1.pfm
+-rw-r--r--   0        0        0      410 2024-04-09 08:19:09.970940 muon-0.1.6/muon/_atac/_ref/jaspar/MA1588.1.pfm
+-rw-r--r--   0        0        0      576 2024-04-09 08:19:09.971182 muon-0.1.6/muon/_atac/_ref/jaspar/MA1589.1.pfm
+-rw-r--r--   0        0        0      440 2024-04-09 08:19:09.972606 muon-0.1.6/muon/_atac/_ref/jaspar/MA1592.1.pfm
+-rw-r--r--   0        0        0      328 2024-04-09 08:19:09.972890 muon-0.1.6/muon/_atac/_ref/jaspar/MA1593.1.pfm
+-rw-r--r--   0        0        0      661 2024-04-09 08:19:09.973115 muon-0.1.6/muon/_atac/_ref/jaspar/MA1594.1.pfm
+-rw-r--r--   0        0        0      436 2024-04-09 08:19:09.973458 muon-0.1.6/muon/_atac/_ref/jaspar/MA1596.1.pfm
+-rw-r--r--   0        0        0      461 2024-04-09 08:19:09.973741 muon-0.1.6/muon/_atac/_ref/jaspar/MA1597.1.pfm
+-rw-r--r--   0        0        0      436 2024-04-09 08:19:09.973982 muon-0.1.6/muon/_atac/_ref/jaspar/MA1599.1.pfm
+-rw-r--r--   0        0        0      492 2024-04-09 08:19:09.974244 muon-0.1.6/muon/_atac/_ref/jaspar/MA1600.1.pfm
+-rw-r--r--   0        0        0      272 2024-04-09 08:19:09.974537 muon-0.1.6/muon/_atac/_ref/jaspar/MA1601.1.pfm
+-rw-r--r--   0        0        0      323 2024-04-09 08:19:09.974874 muon-0.1.6/muon/_atac/_ref/jaspar/MA1602.1.pfm
+-rw-r--r--   0        0        0      357 2024-04-09 08:19:09.975151 muon-0.1.6/muon/_atac/_ref/jaspar/MA1603.1.pfm
+-rw-r--r--   0        0        0      356 2024-04-09 08:19:09.975403 muon-0.1.6/muon/_atac/_ref/jaspar/MA1604.1.pfm
+-rw-r--r--   0        0        0      304 2024-04-09 08:19:09.975743 muon-0.1.6/muon/_atac/_ref/jaspar/MA1606.1.pfm
+-rw-r--r--   0        0        0      384 2024-04-09 08:19:09.976112 muon-0.1.6/muon/_atac/_ref/jaspar/MA1607.1.pfm
+-rw-r--r--   0        0        0      300 2024-04-09 08:19:09.976411 muon-0.1.6/muon/_atac/_ref/jaspar/MA1608.1.pfm
+-rw-r--r--   0        0        0      356 2024-04-09 08:19:09.976657 muon-0.1.6/muon/_atac/_ref/jaspar/MA1615.1.pfm
+-rw-r--r--   0        0        0      408 2024-04-09 08:19:09.976920 muon-0.1.6/muon/_atac/_ref/jaspar/MA1616.1.pfm
+-rw-r--r--   0        0        0      356 2024-04-09 08:19:09.977221 muon-0.1.6/muon/_atac/_ref/jaspar/MA1618.1.pfm
+-rw-r--r--   0        0        0      328 2024-04-09 08:19:09.977567 muon-0.1.6/muon/_atac/_ref/jaspar/MA1619.1.pfm
+-rw-r--r--   0        0        0      328 2024-04-09 08:19:09.977844 muon-0.1.6/muon/_atac/_ref/jaspar/MA1620.1.pfm
+-rw-r--r--   0        0        0      384 2024-04-09 08:19:09.978134 muon-0.1.6/muon/_atac/_ref/jaspar/MA1621.1.pfm
+-rw-r--r--   0        0        0      384 2024-04-09 08:19:09.978484 muon-0.1.6/muon/_atac/_ref/jaspar/MA1622.1.pfm
+-rw-r--r--   0        0        0      354 2024-04-09 08:19:09.978771 muon-0.1.6/muon/_atac/_ref/jaspar/MA1623.1.pfm
+-rw-r--r--   0        0        0      327 2024-04-09 08:19:09.979039 muon-0.1.6/muon/_atac/_ref/jaspar/MA1624.1.pfm
+-rw-r--r--   0        0        0      408 2024-04-09 08:19:09.979325 muon-0.1.6/muon/_atac/_ref/jaspar/MA1625.1.pfm
+-rw-r--r--   0        0        0      382 2024-04-09 08:19:09.979619 muon-0.1.6/muon/_atac/_ref/jaspar/MA1627.1.pfm
+-rw-r--r--   0        0        0      299 2024-04-09 08:19:09.980138 muon-0.1.6/muon/_atac/_ref/jaspar/MA1628.1.pfm
+-rw-r--r--   0        0        0      384 2024-04-09 08:19:09.980452 muon-0.1.6/muon/_atac/_ref/jaspar/MA1629.1.pfm
+-rw-r--r--   0        0        0      298 2024-04-09 08:19:09.980775 muon-0.1.6/muon/_atac/_ref/jaspar/MA1630.1.pfm
+-rw-r--r--   0        0        0      357 2024-04-09 08:19:09.981275 muon-0.1.6/muon/_atac/_ref/jaspar/MA1631.1.pfm
+-rw-r--r--   0        0        0      360 2024-04-09 08:19:09.981810 muon-0.1.6/muon/_atac/_ref/jaspar/MA1632.1.pfm
+-rw-r--r--   0        0        0      356 2024-04-09 08:19:09.982123 muon-0.1.6/muon/_atac/_ref/jaspar/MA1633.1.pfm
+-rw-r--r--   0        0        0      303 2024-04-09 08:19:09.982387 muon-0.1.6/muon/_atac/_ref/jaspar/MA1634.1.pfm
+-rw-r--r--   0        0        0      272 2024-04-09 08:19:09.982644 muon-0.1.6/muon/_atac/_ref/jaspar/MA1635.1.pfm
+-rw-r--r--   0        0        0      413 2024-04-09 08:19:09.982934 muon-0.1.6/muon/_atac/_ref/jaspar/MA1636.1.pfm
+-rw-r--r--   0        0        0      356 2024-04-09 08:19:10.010679 muon-0.1.6/muon/_atac/_ref/jaspar/MA1637.1.pfm
+-rw-r--r--   0        0        0      273 2024-04-09 08:19:10.011125 muon-0.1.6/muon/_atac/_ref/jaspar/MA1638.1.pfm
+-rw-r--r--   0        0        0      356 2024-04-09 08:19:10.011656 muon-0.1.6/muon/_atac/_ref/jaspar/MA1639.1.pfm
+-rw-r--r--   0        0        0      412 2024-04-09 08:19:10.012369 muon-0.1.6/muon/_atac/_ref/jaspar/MA1640.1.pfm
+-rw-r--r--   0        0        0      328 2024-04-09 08:19:10.012726 muon-0.1.6/muon/_atac/_ref/jaspar/MA1641.1.pfm
+-rw-r--r--   0        0        0      357 2024-04-09 08:19:10.012944 muon-0.1.6/muon/_atac/_ref/jaspar/MA1642.1.pfm
+-rw-r--r--   0        0        0      579 2024-04-09 08:19:10.013119 muon-0.1.6/muon/_atac/_ref/jaspar/MA1643.1.pfm
+-rw-r--r--   0        0        0      300 2024-04-09 08:19:10.013388 muon-0.1.6/muon/_atac/_ref/jaspar/MA1644.1.pfm
+-rw-r--r--   0        0        0      384 2024-04-09 08:19:10.013680 muon-0.1.6/muon/_atac/_ref/jaspar/MA1645.1.pfm
+-rw-r--r--   0        0        0      328 2024-04-09 08:19:10.014034 muon-0.1.6/muon/_atac/_ref/jaspar/MA1646.1.pfm
+-rw-r--r--   0        0        0      300 2024-04-09 08:19:10.014322 muon-0.1.6/muon/_atac/_ref/jaspar/MA1647.1.pfm
+-rw-r--r--   0        0        0      304 2024-04-09 08:19:10.014642 muon-0.1.6/muon/_atac/_ref/jaspar/MA1648.1.pfm
+-rw-r--r--   0        0        0      299 2024-04-09 08:19:10.015046 muon-0.1.6/muon/_atac/_ref/jaspar/MA1649.1.pfm
+-rw-r--r--   0        0        0      326 2024-04-09 08:19:10.015255 muon-0.1.6/muon/_atac/_ref/jaspar/MA1650.1.pfm
+-rw-r--r--   0        0        0      576 2024-04-09 08:19:10.015501 muon-0.1.6/muon/_atac/_ref/jaspar/MA1651.1.pfm
+-rw-r--r--   0        0        0      381 2024-04-09 08:19:10.015650 muon-0.1.6/muon/_atac/_ref/jaspar/MA1652.1.pfm
+-rw-r--r--   0        0        0      328 2024-04-09 08:19:10.015897 muon-0.1.6/muon/_atac/_ref/jaspar/MA1653.1.pfm
+-rw-r--r--   0        0        0      629 2024-04-09 08:19:10.016316 muon-0.1.6/muon/_atac/_ref/jaspar/MA1654.1.pfm
+-rw-r--r--   0        0        0      328 2024-04-09 08:19:10.016744 muon-0.1.6/muon/_atac/_ref/jaspar/MA1655.1.pfm
+-rw-r--r--   0        0        0      384 2024-04-09 08:19:10.017126 muon-0.1.6/muon/_atac/_ref/jaspar/MA1656.1.pfm
+-rw-r--r--   0        0        0      328 2024-04-09 08:19:10.017359 muon-0.1.6/muon/_atac/_ref/jaspar/MA1657.1.pfm
+-rw-r--r--   0        0        0      302 2024-04-09 08:19:10.017532 muon-0.1.6/muon/_atac/_ref/jaspar/MA1683.1.pfm
+-rw-r--r--   0        0        0    11673 2024-04-09 08:19:10.017837 muon-0.1.6/muon/_atac/_ref/jaspar/motif_to_gene.txt
+-rw-r--r--   0        0        0     4491 2024-04-09 08:19:10.020727 muon-0.1.6/muon/_atac/io.py
+-rw-r--r--   0        0        0    12779 2024-04-09 08:19:10.034840 muon-0.1.6/muon/_atac/plot.py
+-rw-r--r--   0        0        0     7133 2024-04-09 08:19:10.035301 muon-0.1.6/muon/_atac/preproc.py
+-rw-r--r--   0        0        0    44213 2024-04-09 08:19:10.035983 muon-0.1.6/muon/_atac/tools.py
+-rw-r--r--   0        0        0      316 2024-04-09 08:19:10.036196 muon-0.1.6/muon/_atac/utils.py
+-rw-r--r--   0        0        0        0 2024-04-09 08:19:10.036356 muon-0.1.6/muon/_core/__init__.py
+-rw-r--r--   0        0        0     2032 2024-04-09 08:19:10.036615 muon-0.1.6/muon/_core/config.py
+-rw-r--r--   0        0        0     3135 2024-04-09 08:19:10.036793 muon-0.1.6/muon/_core/io.py
+-rw-r--r--   0        0        0    16833 2024-04-09 08:19:10.039492 muon-0.1.6/muon/_core/plot.py
+-rw-r--r--   0        0        0    36039 2024-04-09 08:48:27.100732 muon-0.1.6/muon/_core/preproc.py
+-rw-r--r--   0        0        0    52403 2024-04-09 08:48:27.102055 muon-0.1.6/muon/_core/tools.py
+-rw-r--r--   0        0        0     8448 2024-04-09 08:19:10.047583 muon-0.1.6/muon/_core/utils.py
+-rw-r--r--   0        0        0       46 2024-04-09 08:19:10.047850 muon-0.1.6/muon/_prot/__init__.py
+-rw-r--r--   0        0        0      723 2024-04-09 08:19:10.048000 muon-0.1.6/muon/_prot/io.py
+-rw-r--r--   0        0        0    10314 2024-04-09 08:19:10.048224 muon-0.1.6/muon/_prot/preproc.py
+-rw-r--r--   0        0        0        0 2024-04-09 08:19:10.048388 muon-0.1.6/muon/_rna/__init__.py
+-rw-r--r--   0        0        0     1270 2024-04-09 08:19:10.048558 muon-0.1.6/muon/_rna/utils.py
+-rw-r--r--   0        0        0       21 2024-04-09 08:19:10.048758 muon-0.1.6/muon/atac.py
+-rw-r--r--   0        0        0       21 2024-04-09 08:19:10.049031 muon-0.1.6/muon/prot.py
+-rw-r--r--   0        0        0       20 2024-04-09 08:19:10.049360 muon-0.1.6/muon/rna.py
+-rw-r--r--   0        0        0     1281 2024-04-09 08:48:27.102506 muon-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     7178 1970-01-01 00:00:00.000000 muon-0.1.6/PKG-INFO
```

### Comparing `muon-0.1.5/README.md` & `muon-0.1.6/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 `muon` is a multimodal omics Python framework. 
 
 [Documentation](https://muon.readthedocs.io/) | [Tutorials](https://muon-tutorials.readthedocs.io/) | [Publication](https://genomebiology.biomedcentral.com/articles/10.1186/s13059-021-02577-8)
 
 [![Documentation Status](https://readthedocs.org/projects/muon/badge/?version=latest)](http://muon.readthedocs.io/?badge=latest)
 [![PyPi version](https://img.shields.io/pypi/v/muon)](https://pypi.org/project/muon)
+[![Powered by NumFOCUS](https://img.shields.io/badge/powered%20by-NumFOCUS-orange.svg?style=flat&colorA=E1523D&colorB=007D8A)](https://numfocus.org)
 
 ## Data structure
 
 `muon` is designed around `MuData` (multimodal data) objects — in the same vein as [scanpy](https://github.com/theislab/scanpy) and [AnnData](https://github.com/theislab/anndata) are designed to work primarily with scRNA-seq data in Python. Individual modalities in `MuData` are naturally represented with `AnnData` objects.
 
 `MuData` class and `.h5mu` files I/O operations are part of [the standalone mudata library](https://github.com/scverse/mudata).
 
@@ -115,8 +116,22 @@
 
 You can cite the scverse publication as follows:
 
 > **The scverse project provides a computational ecosystem for single-cell omics data analysis**
 >
 > Isaac Virshup, Danila Bredikhin, Lukas Heumos, Giovanni Palla, Gregor Sturm, Adam Gayoso, Ilia Kats, Mikaela Koutrouli, Scverse Community, Bonnie Berger, Dana Pe’er, Aviv Regev, Sarah A. Teichmann, Francesca Finotello, F. Alexander Wolf, Nir Yosef, Oliver Stegle & Fabian J. Theis
 >
-> _Nat Biotechnol._ 2022 Apr 10. doi: [10.1038/s41587-023-01733-8](https://doi.org/10.1038/s41587-023-01733-8).
+> _Nat Biotechnol._ 2023 Apr 10. doi: [10.1038/s41587-023-01733-8](https://doi.org/10.1038/s41587-023-01733-8).
+
+
+[//]: # "numfocus-fiscal-sponsor-attribution"
+
+`muon` is part of the scverse project ([website](https://scverse.org), [governance](https://scverse.org/about/roles)) and is fiscally sponsored by [NumFOCUS](https://numfocus.org/).
+Please consider making a tax-deductible [donation](https://numfocus.org/donate-to-scverse) to help the project pay for developer time, professional services, travel, workshops, and a variety of other needs.
+
+<a href="https://numfocus.org/project/scverse">
+  <img
+    src="https://raw.githubusercontent.com/numfocus/templates/master/images/numfocus-logo.png"
+    width="200"
+  >
+</a>
+
```

### Comparing `muon-0.1.5/muon/_atac/_ref/jaspar/MA0050.2.pfm` & `muon-0.1.6/muon/_atac/_ref/jaspar/MA0050.2.pfm`

 * *Files identical despite different names*

### Comparing `muon-0.1.5/muon/_atac/_ref/jaspar/MA0066.1.pfm` & `muon-0.1.6/muon/_atac/_ref/jaspar/MA0066.1.pfm`

 * *Files identical despite different names*

### Comparing `muon-0.1.5/muon/_atac/_ref/jaspar/MA0073.1.pfm` & `muon-0.1.6/muon/_atac/_ref/jaspar/MA0073.1.pfm`

 * *Files identical despite different names*

### Comparing `muon-0.1.5/muon/_atac/_ref/jaspar/MA0080.5.pfm` & `muon-0.1.6/muon/_atac/_ref/jaspar/MA0080.5.pfm`

 * *Files identical despite different names*

### Comparing `muon-0.1.5/muon/_atac/_ref/jaspar/MA0138.2.pfm` & `muon-0.1.6/muon/_atac/_ref/jaspar/MA0138.2.pfm`

 * *Files identical despite different names*

### Comparing `muon-0.1.5/muon/_atac/_ref/jaspar/MA0139.1.pfm` & `muon-0.1.6/muon/_atac/_ref/jaspar/MA0139.1.pfm`

 * *Files identical despite different names*

### Comparing `muon-0.1.5/muon/_atac/_ref/jaspar/MA0494.1.pfm` & `muon-0.1.6/muon/_atac/_ref/jaspar/MA0494.1.pfm`

 * *Files identical despite different names*

### Comparing `muon-0.1.5/muon/_atac/_ref/jaspar/MA0804.1.pfm` & `muon-0.1.6/muon/_atac/_ref/jaspar/MA0804.1.pfm`

 * *Files identical despite different names*

### Comparing `muon-0.1.5/muon/_atac/_ref/jaspar/MA1101.2.pfm` & `muon-0.1.6/muon/_atac/_ref/jaspar/MA1101.2.pfm`

 * *Files identical despite different names*

### Comparing `muon-0.1.5/muon/_atac/_ref/jaspar/MA1418.1.pfm` & `muon-0.1.6/muon/_atac/_ref/jaspar/MA1418.1.pfm`

 * *Files identical despite different names*

### Comparing `muon-0.1.5/muon/_atac/_ref/jaspar/MA1470.1.pfm` & `muon-0.1.6/muon/_atac/_ref/jaspar/MA1470.1.pfm`

 * *Files identical despite different names*

### Comparing `muon-0.1.5/muon/_atac/_ref/jaspar/MA1573.1.pfm` & `muon-0.1.6/muon/_atac/_ref/jaspar/MA1573.1.pfm`

 * *Files identical despite different names*

### Comparing `muon-0.1.5/muon/_atac/_ref/jaspar/MA1575.1.pfm` & `muon-0.1.6/muon/_atac/_ref/jaspar/MA1575.1.pfm`

 * *Files identical despite different names*

### Comparing `muon-0.1.5/muon/_atac/_ref/jaspar/MA1576.1.pfm` & `muon-0.1.6/muon/_atac/_ref/jaspar/MA1576.1.pfm`

 * *Files identical despite different names*

### Comparing `muon-0.1.5/muon/_atac/_ref/jaspar/MA1589.1.pfm` & `muon-0.1.6/muon/_atac/_ref/jaspar/MA1589.1.pfm`

 * *Files identical despite different names*

### Comparing `muon-0.1.5/muon/_atac/_ref/jaspar/MA1594.1.pfm` & `muon-0.1.6/muon/_atac/_ref/jaspar/MA1594.1.pfm`

 * *Files identical despite different names*

### Comparing `muon-0.1.5/muon/_atac/_ref/jaspar/MA1643.1.pfm` & `muon-0.1.6/muon/_atac/_ref/jaspar/MA1643.1.pfm`

 * *Files identical despite different names*

### Comparing `muon-0.1.5/muon/_atac/_ref/jaspar/MA1651.1.pfm` & `muon-0.1.6/muon/_atac/_ref/jaspar/MA1651.1.pfm`

 * *Files identical despite different names*

### Comparing `muon-0.1.5/muon/_atac/_ref/jaspar/MA1654.1.pfm` & `muon-0.1.6/muon/_atac/_ref/jaspar/MA1654.1.pfm`

 * *Files identical despite different names*

### Comparing `muon-0.1.5/muon/_atac/_ref/jaspar/motif_to_gene.txt` & `muon-0.1.6/muon/_atac/_ref/jaspar/motif_to_gene.txt`

 * *Files identical despite different names*

### Comparing `muon-0.1.5/muon/_atac/io.py` & `muon-0.1.6/muon/_atac/io.py`

 * *Files identical despite different names*

### Comparing `muon-0.1.5/muon/_atac/plot.py` & `muon-0.1.6/muon/_atac/plot.py`

 * *Files identical despite different names*

### Comparing `muon-0.1.5/muon/_atac/preproc.py` & `muon-0.1.6/muon/_atac/preproc.py`

 * *Files identical despite different names*

### Comparing `muon-0.1.5/muon/_atac/tools.py` & `muon-0.1.6/muon/_atac/tools.py`

 * *Files identical despite different names*

### Comparing `muon-0.1.5/muon/_core/config.py` & `muon-0.1.6/muon/_core/config.py`

 * *Files identical despite different names*

### Comparing `muon-0.1.5/muon/_core/io.py` & `muon-0.1.6/muon/_core/io.py`

 * *Files identical despite different names*

### Comparing `muon-0.1.5/muon/_core/plot.py` & `muon-0.1.6/muon/_core/plot.py`

 * *Files identical despite different names*

### Comparing `muon-0.1.5/muon/_core/preproc.py` & `muon-0.1.6/muon/_core/preproc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,42 @@
 from typing import Union, Callable, Optional, Sequence, Dict, Iterable, Literal
 from functools import reduce
 import warnings
 from itertools import repeat
 
 import numpy as np
-from scipy.sparse import csr_matrix, issparse, SparseEfficiencyWarning
+from scipy.sparse import (
+    csr_matrix,
+    issparse,
+    SparseEfficiencyWarning,
+    linalg,
+    isspmatrix_csc,
+    isspmatrix_csr,
+    isspmatrix_coo,
+)
 from scipy.spatial.distance import cdist
 from scipy.special import softmax
 from sklearn.utils import check_random_state
 
 from anndata import AnnData
+import scanpy
 from scanpy import logging
 from scanpy.tools._utils import _choose_representation
-from scanpy.neighbors import _compute_connectivities_umap
 from umap.distances import euclidean
 from umap.sparse import sparse_euclidean, sparse_jaccard
 from umap.umap_ import nearest_neighbors
 from numba import njit, prange
 
+from packaging.version import Version
+
+if Version(scanpy.__version__) < Version("1.10"):
+    from scanpy.neighbors import _compute_connectivities_umap
+else:
+    from scanpy.neighbors._connectivity import umap as _compute_connectivities_umap
+
 from mudata import MuData
 
 # Computational methods for preprocessing
 
 _euclidean = njit(euclidean.py_func, inline="always", fastmath=True)
 _sparse_euclidean = njit(sparse_euclidean.py_func, inline="always")
 _sparse_jaccard = njit(sparse_jaccard.py_func, inline="always")
@@ -150,19 +165,30 @@
             allstops.append((stop,))
     return np.concatenate(allstarts), np.concatenate(allstops)
 
 
 def _l2norm(
     adata: AnnData, rep: Optional[Union[Iterable[str], str]] = None, n_pcs: Optional[int] = 0
 ):
-    X = _choose_representation(adata, rep, n_pcs)
-    norm = X / np.linalg.norm(X, ord=2, axis=1, keepdims=True)
-    norm[~np.isfinite(norm)] = 0
+    X = _choose_representation(adata=adata, use_rep=rep, n_pcs=n_pcs)
+    sparse_X = issparse(X)
+    if sparse_X:
+        X_norm = linalg.norm(X, ord=2, axis=1)
+        norm = X / np.expand_dims(X_norm, axis=1)
+        if not issparse(norm):
+            norm = csr_matrix(norm)
+        norm.data[~np.isfinite(norm.data)] = 0
+    else:
+        norm = X / np.linalg.norm(X, ord=2, axis=1, keepdims=True)
+        norm[~np.isfinite(norm)] = 0
     X.astype(norm.dtype, copy=False)
-    X[:] = norm
+    if sparse_X and (isspmatrix_csc(X) or isspmatrix_csr(X) or isspmatrix_coo(X)):
+        X.data[:] = norm.data[:]
+    else:
+        X[:] = norm
 
 
 def l2norm(
     mdata: Union[MuData, AnnData],
     mod: Optional[Union[Iterable[str], str]] = None,
     rep: Optional[Union[Iterable[str], str]] = None,
     n_pcs: Optional[Union[Iterable[int], int]] = 0,
@@ -188,24 +214,24 @@
     """
     if isinstance(mdata, AnnData):
         if rep is not None and not isinstance(rep, str):
             it = iter(rep)
             rep = next(it)
             try:
                 next(it)
-            except StopIteration as e:
+            except StopIteration:
                 pass
             else:
                 raise RuntimeError("If 'rep' is an Iterable, it must have length 1")
         if n_pcs is not None and isinstance(n_pcs, Iterable):
             it = iter(n_pcs)
             n_pcs = next(it)
             try:
                 next(it)
-            except StopIteration as e:
+            except StopIteration:
                 pass
             else:
                 raise RuntimeError("If 'n_pcs' is an Iterable, it must have length 1")
         if copy:
             mdata = mdata.copy()
         _l2norm(mdata, rep, n_pcs)
     else:
@@ -335,15 +361,15 @@
             )
 
         use_rep = nparams["params"].get("use_rep", None)
         n_pcs = nparams["params"].get("n_pcs", None)
         mod_neighbors[i] = nparams["params"].get("n_neighbors", 0)
 
         neighbors_params[mod] = nparams
-        reps[mod] = _choose_representation(mdata.mod[mod], use_rep, n_pcs)
+        reps[mod] = _choose_representation(adata=mdata.mod[mod], use_rep=use_rep, n_pcs=n_pcs)
         mod_reps[mod] = (
             use_rep if use_rep is not None else -1
         )  # otherwise this is not saved to h5mu
         mod_n_pcs[mod] = n_pcs if n_pcs is not None else -1
 
     if n_neighbors is None:
         mod_neighbors = mod_neighbors[mod_neighbors > 0]
@@ -562,30 +588,30 @@
                 np.exp(neighdist(cell, nz) / csigmas[cell]).squeeze() * weights[cell, i]
             )
     neighbordistances.data = np.sqrt(0.5 * (1 - neighbordistances.data))
 
     neighbordistances = _sparse_csr_fast_knn(neighbordistances, n_neighbors + 1)
 
     logging.info("Calculating connectivities...")
-    _, connectivities = _compute_connectivities_umap(
+    connectivities = _compute_connectivities_umap(
         knn_indices=neighbordistances.indices.reshape(
             (neighbordistances.shape[0], n_neighbors + 1)
         ),
         knn_dists=neighbordistances.data.reshape((neighbordistances.shape[0], n_neighbors + 1)),
         n_obs=neighbordistances.shape[0],
         n_neighbors=n_neighbors + 1,
     )
 
     if key_added is None:
         key_added = "neighbors"
         conns_key = "connectivities"
         dists_key = "distances"
     else:
-        conns_key = key_added + "_connectivities"
-        dists_key = key_added + "_distances"
+        conns_key = f"{key_added}_connectivities"
+        dists_key = f"{key_added}_distances"
     neighbors_dict = {"connectivities_key": conns_key, "distances_key": dists_key}
     neighbors_dict["params"] = {
         "n_neighbors": n_neighbors,
         "n_multineighbors": n_multineighbors,
         "metric": metric,
         "eps": eps,
         "random_state": random_state,
@@ -688,15 +714,15 @@
     else:
         if func is None:
             if np.array(var).dtype == bool:
                 obs_subset = np.array(var)
             else:
                 obs_subset = data.obs_names.isin(var)
         else:
-            raise ValueError(f"When providing obs_names directly, func has to be None.")
+            raise ValueError("When providing obs_names directly, func has to be None.")
 
     # Subset .obs
     data._obs = data.obs[obs_subset]
     data._n_obs = data.obs.shape[0]
 
     # Subset .obsm
     for k, v in data.obsm.items():
@@ -796,20 +822,17 @@
             var_subset = func(data.X[:, np.where(data.obs_names == var)[0]].reshape(-1))
         else:
             raise ValueError(
                 f"Column name from .var or one of the obs_names was expected but got {var}."
             )
     else:
         if func is None:
-            if np.array(var).dtype == bool:
-                var_subset = var
-            else:
-                var_subset = data.var_names.isin(var)
+            var_subset = var if np.array(var).dtype == bool else data.var_names.isin(var)
         else:
-            raise ValueError(f"When providing var_names directly, func has to be None.")
+            raise ValueError("When providing var_names directly, func has to be None.")
 
     # Subset .var
     data._var = data.var[var_subset]
     data._n_vars = data.var.shape[0]
 
     # Subset .varm
     for k, v in data.varm.items():
```

### Comparing `muon-0.1.5/muon/_core/tools.py` & `muon-0.1.6/muon/_core/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 import h5py
 from natsort import natsorted
 from anndata import AnnData
 from mudata import MuData
 
 from scanpy import logging
 from scanpy.tools._utils import _choose_representation
-from scanpy.neighbors import _compute_connectivities_umap
+
+# from scanpy.neighbors import _compute_connectivities_umap
 
 from typing import Union, Optional, List, Iterable, Mapping, Sequence, Type, Any, Dict, Literal
 from types import MappingProxyType
 
 from .preproc import _sparse_csr_fast_knn
 
 try:
@@ -431,19 +432,17 @@
         mdata = data
     else:
         raise TypeError("Expected an MuData object")
 
     if outfile is None:
         outfile = os.path.join("/tmp", "mofa_{}.hdf5".format(strftime("%Y%m%d-%H%M%S")))
 
-    if use_var:
-        if use_var not in data.var.columns:
-            warn(f"There is no column {use_var} in the provided object")
-            use_var = None
-
+    if use_var and use_var not in data.var.columns:
+        warn(f"There is no column {use_var} in the provided object")
+        use_var = None
     if isinstance(data, MuData):
         common_obs = reduce(np.intersect1d, [v.obs_names.values for k, v in mdata.mod.items()])
         if len(common_obs) != mdata.n_obs:
             if not use_obs:
                 raise IndexError(
                     "Not all the observations are the same across modalities. Please run `mdata.intersect_obs()` to subset the data or devise a strategy with `use_obs` ('union' or 'intersection')"
                 )
@@ -453,17 +452,16 @@
                 )
         else:
             use_obs = None
 
     ent = entry_point()
 
     lik = likelihoods
-    if lik is not None:
-        if isinstance(lik, str) and isinstance(lik, Iterable):
-            lik = [lik for _ in range(len(mdata.mod))]
+    if lik is not None and (isinstance(lik, str) and isinstance(lik, Iterable)):
+        lik = [lik for _ in range(len(mdata.mod))]
 
     ent.set_data_options(
         scale_views=scale_views,
         scale_groups=scale_groups,
         center_groups=center_groups,
         use_float32=use_float32,
     )
@@ -635,15 +633,15 @@
         w = np.concatenate([expectations_w[m][:, :] for m in data.mod], axis=1).T
     else:
         w = expectations_w["data"][:, :].T
 
     if use_var:
         # Set the weights of features that were not used to zero
         data.varm["LFs"] = np.zeros(shape=(data.n_vars, w.shape[1]))
-        data.varm["LFs"][data.var[use_var]] = w
+        data.varm["LFs"][data.var[use_var].astype(bool)] = w
     else:
         data.varm["LFs"] = w
 
     # Aligned times
     if smooth_covariate is not None and smooth_warping:
         for c in range(ent.dimensionalities["C"]):
             cnm = ent.smooth_opts["covariates_names"][c] + "_warped"
@@ -783,15 +781,15 @@
             )
 
         use_rep = nparams["params"].get("use_rep", None)
         n_pcs = nparams["params"].get("n_pcs", None)
         mod_neighbors[i] = nparams["params"].get("n_neighbors", 0)
 
         neighbors_params[mod] = nparams
-        reps[mod] = _choose_representation(mdata.mod[mod], use_rep, n_pcs)
+        reps[mod] = _choose_representation(adata=mdata.mod[mod], use_rep=use_rep, n_pcs=n_pcs)
         mod_reps[mod] = (
             use_rep if use_rep is not None else -1
         )  # otherwise this is not saved to h5mu
         mod_n_pcs[mod] = n_pcs if n_pcs is not None else -1
 
     def _affinity_matrix(dist, k, sigma):
         """
@@ -851,15 +849,15 @@
         np.fill_diagonal(x, 0.5)
         x = (x + x.T) / 2
         return x
 
     def _dominateset(x, k=20):
         def _zero(arr):
             if k >= len(arr):
-                raise ValueError(f"'n_neighbors' seems to be too high.")
+                raise ValueError("'n_neighbors' seems to be too high.")
             arr = arr.copy()
             arr[np.argsort(arr)[: (len(arr) - k)]] = 0
             return arr
 
         x = np.apply_along_axis(_zero, 0, x)
         return x / x.sum(axis=1)
 
@@ -1315,15 +1313,15 @@
     reps = {}
     nfeatures = 0
     nparams = neighbors["params"]
     use_rep = {k: (v if v != -1 else None) for k, v in nparams["use_rep"].items()}
     n_pcs = {k: (v if v != -1 else None) for k, v in nparams["n_pcs"].items()}
     observations = mdata.obs.index
     for mod, rep in use_rep.items():
-        rep = _choose_representation(mdata.mod[mod], rep, n_pcs[mod])
+        rep = _choose_representation(adata=mdata.mod[mod], use_rep=rep, n_pcs=n_pcs[mod])
         nfeatures += rep.shape[1]
         reps[mod] = rep
     rep = np.empty((len(observations), nfeatures), np.float32)
     nfeatures = 0
     for mod, crep in reps.items():
         cnfeatures = nfeatures + crep.shape[1]
         idx = observations.isin(mdata.mod[mod].obs.index)
```

### Comparing `muon-0.1.5/muon/_core/utils.py` & `muon-0.1.6/muon/_core/utils.py`

 * *Files identical despite different names*

### Comparing `muon-0.1.5/muon/_prot/io.py` & `muon-0.1.6/muon/_prot/io.py`

 * *Files identical despite different names*

### Comparing `muon-0.1.5/muon/_prot/preproc.py` & `muon-0.1.6/muon/_prot/preproc.py`

 * *Files identical despite different names*

### Comparing `muon-0.1.5/muon/_rna/utils.py` & `muon-0.1.6/muon/_rna/utils.py`

 * *Files identical despite different names*

### Comparing `muon-0.1.5/pyproject.toml` & `muon-0.1.6/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -42,14 +42,18 @@
     "nbsphinx",
     "sphinx_automodapi"
 ]
 atac = [
     "pybedtools",
     "pysam"
 ]
+test = [
+    "pytest",
+    "flake8",
+]
 
 [tool.flit.metadata.urls]
 Documentation = "https://muon.readthedocs.io/en/latest/"
 
 [tool.flit.sdist]
 exclude = [".github", "docs/build"]
```

### Comparing `muon-0.1.5/PKG-INFO` & `muon-0.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muon
-Version: 0.1.5
+Version: 0.1.6
 Summary: Multimodal omics analysis framework
 Home-page: https://github.com/scverse/muon
 Author: Danila Bredikhin
 Author-email: danila.bredikhin@embl.de
 Requires-Python: >= 3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
@@ -30,26 +30,30 @@
 Requires-Dist: pysam ; extra == "atac"
 Requires-Dist: sphinx >= 4.0 ; extra == "docs"
 Requires-Dist: pydata-sphinx-theme==0.8.1 ; extra == "docs"
 Requires-Dist: sphinx-book-theme==0.3.3 ; extra == "docs"
 Requires-Dist: readthedocs-sphinx-search ; extra == "docs"
 Requires-Dist: nbsphinx ; extra == "docs"
 Requires-Dist: sphinx_automodapi ; extra == "docs"
+Requires-Dist: pytest ; extra == "test"
+Requires-Dist: flake8 ; extra == "test"
 Project-URL: Documentation, https://muon.readthedocs.io/en/latest/
 Provides-Extra: atac
 Provides-Extra: docs
+Provides-Extra: test
 
 <img src="./docs/img/muon_header.png" data-canonical-src="./docs/img/muon_header.png" width="700"/>
 
 `muon` is a multimodal omics Python framework. 
 
 [Documentation](https://muon.readthedocs.io/) | [Tutorials](https://muon-tutorials.readthedocs.io/) | [Publication](https://genomebiology.biomedcentral.com/articles/10.1186/s13059-021-02577-8)
 
 [![Documentation Status](https://readthedocs.org/projects/muon/badge/?version=latest)](http://muon.readthedocs.io/?badge=latest)
 [![PyPi version](https://img.shields.io/pypi/v/muon)](https://pypi.org/project/muon)
+[![Powered by NumFOCUS](https://img.shields.io/badge/powered%20by-NumFOCUS-orange.svg?style=flat&colorA=E1523D&colorB=007D8A)](https://numfocus.org)
 
 ## Data structure
 
 `muon` is designed around `MuData` (multimodal data) objects — in the same vein as [scanpy](https://github.com/theislab/scanpy) and [AnnData](https://github.com/theislab/anndata) are designed to work primarily with scRNA-seq data in Python. Individual modalities in `MuData` are naturally represented with `AnnData` objects.
 
 `MuData` class and `.h5mu` files I/O operations are part of [the standalone mudata library](https://github.com/scverse/mudata).
 
@@ -155,9 +159,23 @@
 
 You can cite the scverse publication as follows:
 
 > **The scverse project provides a computational ecosystem for single-cell omics data analysis**
 >
 > Isaac Virshup, Danila Bredikhin, Lukas Heumos, Giovanni Palla, Gregor Sturm, Adam Gayoso, Ilia Kats, Mikaela Koutrouli, Scverse Community, Bonnie Berger, Dana Pe’er, Aviv Regev, Sarah A. Teichmann, Francesca Finotello, F. Alexander Wolf, Nir Yosef, Oliver Stegle & Fabian J. Theis
 >
-> _Nat Biotechnol._ 2022 Apr 10. doi: [10.1038/s41587-023-01733-8](https://doi.org/10.1038/s41587-023-01733-8).
+> _Nat Biotechnol._ 2023 Apr 10. doi: [10.1038/s41587-023-01733-8](https://doi.org/10.1038/s41587-023-01733-8).
+
+
+[//]: # "numfocus-fiscal-sponsor-attribution"
+
+`muon` is part of the scverse project ([website](https://scverse.org), [governance](https://scverse.org/about/roles)) and is fiscally sponsored by [NumFOCUS](https://numfocus.org/).
+Please consider making a tax-deductible [donation](https://numfocus.org/donate-to-scverse) to help the project pay for developer time, professional services, travel, workshops, and a variety of other needs.
+
+<a href="https://numfocus.org/project/scverse">
+  <img
+    src="https://raw.githubusercontent.com/numfocus/templates/master/images/numfocus-logo.png"
+    width="200"
+  >
+</a>
+
```

