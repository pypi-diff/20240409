# Comparing `tmp/faststream-0.5.0rc0.tar.gz` & `tmp/faststream-0.5.0rc1.tar.gz`

## Comparing `faststream-0.5.0rc0.tar` & `faststream-0.5.0rc1.tar`

### file list

```diff
@@ -1,322 +1,323 @@
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/.codespell-whitelist.txt
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     3860 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/.secrets.baseline
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/.semgrepignore
--rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/CITATION.cff
--rw-r--r--   0        0        0     5480 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     2630 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/CONTRIBUTING.md
--rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/SECURITY.md
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/.github/dependabot.yml
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/.github/workflows/check-broken-links-in-docs.yaml
--rw-r--r--   0        0        0     3520 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/.github/workflows/codeql.yml
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/.github/workflows/dependency-review.yaml
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/.github/workflows/deploy-docs.yaml
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/.github/workflows/publish_coverage.yml
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/.github/workflows/publish_pypi.yml
--rw-r--r--   0        0        0    16460 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/.github/workflows/test.yaml
--rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/.github/workflows/update_release_notes.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/__init__.py
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/e01_basic_consume.py
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/e02_1_basic_publisher.py
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/e02_2_basic_publisher.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/e02_3_basic_publisher.py
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/e03_miltiple_pubsub.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/e04_msg_filter.py
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/e05_rpc_request.py
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/e06_manual_ack.py
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/e07_ack_immediately.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/e08_testing.py
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/e09_testing_mocks.py
--rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/e10_middlewares.py
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/e11_settings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/fastapi_integration/__init__.py
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/fastapi_integration/app.py
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/fastapi_integration/testing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/howto/__init__.py
--rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/howto/structlogs.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/kafka/__init__.py
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/kafka/ack_after_process.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/kafka/batch_consume.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/kafka/batch_publish_1.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/kafka/batch_publish_2.py
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/kafka/batch_publish_3.py
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/kafka/testing.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/nats/__init__.py
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/nats/e01_basic.py
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/nats/e02_basic_rpc.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/nats/e03_publisher.py
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/nats/e04_js_basic.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/nats/e05_basic_and_js.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/nats/e06_key_value.py
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/nats/e07_object_storage.py
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/nats/e08_wildcards.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/nats/e09_pull_sub.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/rabbit/__init__.py
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/rabbit/direct.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/rabbit/fanout.py
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/rabbit/header.py
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/rabbit/stream.py
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/rabbit/topic.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/redis/__init__.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/redis/channel_sub.py
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/redis/channel_sub_pattern.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/redis/list_sub.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/redis/list_sub_batch.py
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/redis/rpc.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/redis/stream_sub.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/redis/stream_sub_batch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/router/__init__.py
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/router/basic_consume.py
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/router/basic_publish.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/router/delay_registration.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/serialization/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/serialization/avro/__init__.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/serialization/avro/avro.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/serialization/avro/person.avsc
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/serialization/avro/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/serialization/msgpack/__init__.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/serialization/msgpack/pack.py
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/serialization/msgpack/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/serialization/protobuf/__init__.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/serialization/protobuf/message.proto
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/serialization/protobuf/protobuf.py
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/examples/serialization/protobuf/requirements.txt
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/__about__.py
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/__init__.py
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/__main__.py
--rw-r--r--   0        0        0     5740 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/_compat.py
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/annotations.py
--rw-r--r--   0        0        0     6908 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/app.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/constants.py
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/py.typed
--rw-r--r--   0        0        0     9620 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/security.py
--rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/types.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/asyncapi/__init__.py
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/asyncapi/abc.py
--rw-r--r--   0        0        0     5733 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/asyncapi/generate.py
--rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/asyncapi/message.py
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/asyncapi/proto.py
--rw-r--r--   0        0        0     4802 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/asyncapi/site.py
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/asyncapi/utils.py
--rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/asyncapi/schema/__init__.py
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/asyncapi/schema/channels.py
--rw-r--r--   0        0        0     5067 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/asyncapi/schema/info.py
--rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/asyncapi/schema/main.py
--rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/asyncapi/schema/message.py
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/asyncapi/schema/operations.py
--rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/asyncapi/schema/security.py
--rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/asyncapi/schema/servers.py
--rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/asyncapi/schema/utils.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/asyncapi/schema/bindings/__init__.py
--rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/asyncapi/schema/bindings/amqp.py
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/asyncapi/schema/bindings/kafka.py
--rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/asyncapi/schema/bindings/main.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/asyncapi/schema/bindings/nats.py
--rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/asyncapi/schema/bindings/redis.py
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/asyncapi/schema/bindings/sqs.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/broker/__init__.py
--rw-r--r--   0        0        0     5908 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/broker/acknowledgement_watcher.py
--rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/broker/message.py
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/broker/proto.py
--rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/broker/router.py
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/broker/schemas.py
--rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/broker/types.py
--rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/broker/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/broker/core/__init__.py
--rw-r--r--   0        0        0     3424 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/broker/core/abc.py
--rw-r--r--   0        0        0     2646 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/broker/core/logging.py
--rw-r--r--   0        0        0    10480 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/broker/core/usecase.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/broker/fastapi/__init__.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/broker/fastapi/context.py
--rw-r--r--   0        0        0     4259 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/broker/fastapi/get_dependant.py
--rw-r--r--   0        0        0     9565 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/broker/fastapi/route.py
--rw-r--r--   0        0        0    17621 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/broker/fastapi/router.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/broker/middlewares/__init__.py
--rw-r--r--   0        0        0     3039 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/broker/middlewares/base.py
--rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/broker/middlewares/logging.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/broker/publisher/__init__.py
--rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/broker/publisher/fake.py
--rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/broker/publisher/proto.py
--rw-r--r--   0        0        0     4872 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/broker/publisher/usecase.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/broker/subscriber/__init__.py
--rw-r--r--   0        0        0     5314 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/broker/subscriber/call_item.py
--rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/broker/subscriber/proto.py
--rw-r--r--   0        0        0    13286 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/broker/subscriber/usecase.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/broker/wrapper/__init__.py
--rw-r--r--   0        0        0     5791 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/broker/wrapper/call.py
--rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/broker/wrapper/proto.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/cli/__init__.py
--rw-r--r--   0        0        0     7047 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/cli/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/cli/docs/__init__.py
--rw-r--r--   0        0        0     5035 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/cli/docs/app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/cli/supervisors/__init__.py
--rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/cli/supervisors/basereload.py
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/cli/supervisors/multiprocess.py
--rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/cli/supervisors/utils.py
--rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/cli/supervisors/watchfiles.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/cli/utils/__init__.py
--rw-r--r--   0        0        0     4539 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/cli/utils/imports.py
--rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/cli/utils/logs.py
--rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/cli/utils/parser.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/confluent/__init__.py
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/confluent/annotations.py
--rw-r--r--   0        0        0    14880 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/confluent/client.py
--rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/confluent/message.py
--rw-r--r--   0        0        0     3301 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/confluent/parser.py
--rw-r--r--   0        0        0    11465 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/confluent/router.py
--rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/confluent/security.py
--rw-r--r--   0        0        0     7896 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/confluent/testing.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/confluent/broker/__init__.py
--rw-r--r--   0        0        0    19248 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/confluent/broker/broker.py
--rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/confluent/broker/logging.py
--rw-r--r--   0        0        0    18762 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/confluent/broker/registrator.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/confluent/fastapi/__init__.py
--rw-r--r--   0        0        0    26173 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/confluent/fastapi/fastapi.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/confluent/publisher/__init__.py
--rw-r--r--   0        0        0     5353 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/confluent/publisher/asyncapi.py
--rw-r--r--   0        0        0     3279 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/confluent/publisher/producer.py
--rw-r--r--   0        0        0     6062 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/confluent/publisher/usecase.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/confluent/schemas/__init__.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/confluent/schemas/params.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/confluent/subscriber/__init__.py
--rw-r--r--   0        0        0     6019 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/confluent/subscriber/asyncapi.py
--rw-r--r--   0        0        0    10354 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/confluent/subscriber/usecase.py
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/kafka/__init__.py
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/kafka/annotations.py
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/kafka/message.py
--rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/kafka/parser.py
--rw-r--r--   0        0        0    21031 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/kafka/router.py
--rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/kafka/security.py
--rw-r--r--   0        0        0     5809 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/kafka/testing.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/kafka/broker/__init__.py
--rw-r--r--   0        0        0    29413 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/kafka/broker/broker.py
--rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/kafka/broker/logging.py
--rw-r--r--   0        0        0    65980 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/kafka/broker/registrator.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/kafka/fastapi/__init__.py
--rw-r--r--   0        0        0   112731 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/kafka/fastapi/fastapi.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/kafka/publisher/__init__.py
--rw-r--r--   0        0        0     5405 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/kafka/publisher/asyncapi.py
--rw-r--r--   0        0        0     3246 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/kafka/publisher/producer.py
--rw-r--r--   0        0        0     9803 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/kafka/publisher/usecase.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/kafka/schemas/__init__.py
--rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/kafka/schemas/params.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/kafka/subscriber/__init__.py
--rw-r--r--   0        0        0     5927 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/kafka/subscriber/asyncapi.py
--rw-r--r--   0        0        0    10087 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/kafka/subscriber/usecase.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/log/__init__.py
--rw-r--r--   0        0        0     2424 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/log/formatter.py
--rw-r--r--   0        0        0     1975 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/log/logging.py
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/nats/__init__.py
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/nats/annotations.py
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/nats/helpers.py
--rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/nats/message.py
--rw-r--r--   0        0        0     3351 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/nats/parser.py
--rw-r--r--   0        0        0    12265 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/nats/router.py
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/nats/security.py
--rw-r--r--   0        0        0     4281 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/nats/testing.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/nats/broker/__init__.py
--rw-r--r--   0        0        0    26992 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/nats/broker/broker.py
--rw-r--r--   0        0        0     2462 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/nats/broker/logging.py
--rw-r--r--   0        0        0    11589 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/nats/broker/registrator.py
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/nats/fastapi/__init__.py
--rw-r--r--   0        0        0    36199 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/nats/fastapi/fastapi.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/nats/publisher/__init__.py
--rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/nats/publisher/asyncapi.py
--rw-r--r--   0        0        0     5682 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/nats/publisher/producer.py
--rw-r--r--   0        0        0     5351 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/nats/publisher/usecase.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/nats/schemas/__init__.py
--rw-r--r--   0        0        0     9297 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/nats/schemas/js_stream.py
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/nats/schemas/pull_sub.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/nats/subscriber/__init__.py
--rw-r--r--   0        0        0     6287 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/nats/subscriber/asyncapi.py
--rw-r--r--   0        0        0    14843 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/nats/subscriber/usecase.py
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/rabbit/__init__.py
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/rabbit/annotations.py
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/rabbit/message.py
--rw-r--r--   0        0        0     3381 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/rabbit/parser.py
--rw-r--r--   0        0        0    11591 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/rabbit/router.py
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/rabbit/security.py
--rw-r--r--   0        0        0    10006 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/rabbit/testing.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/rabbit/types.py
--rw-r--r--   0        0        0     4125 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/rabbit/utils.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/rabbit/broker/__init__.py
--rw-r--r--   0        0        0    19471 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/rabbit/broker/broker.py
--rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/rabbit/broker/logging.py
--rw-r--r--   0        0        0    10848 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/rabbit/broker/registrator.py
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/rabbit/fastapi/__init__.py
--rw-r--r--   0        0        0    30361 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/rabbit/fastapi/router.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/rabbit/publisher/__init__.py
--rw-r--r--   0        0        0     5006 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/rabbit/publisher/asyncapi.py
--rw-r--r--   0        0        0     7595 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/rabbit/publisher/producer.py
--rw-r--r--   0        0        0     8274 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/rabbit/publisher/usecase.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/rabbit/schemas/__init__.py
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/rabbit/schemas/constants.py
--rw-r--r--   0        0        0     3919 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/rabbit/schemas/exchange.py
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/rabbit/schemas/proto.py
--rw-r--r--   0        0        0     3275 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/rabbit/schemas/queue.py
--rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/rabbit/schemas/reply.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/rabbit/subscriber/__init__.py
--rw-r--r--   0        0        0     4322 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/rabbit/subscriber/asyncapi.py
--rw-r--r--   0        0        0     6925 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/rabbit/subscriber/usecase.py
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/redis/__init__.py
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/redis/annotations.py
--rw-r--r--   0        0        0     2565 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/redis/message.py
--rw-r--r--   0        0        0     5779 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/redis/parser.py
--rw-r--r--   0        0        0     8364 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/redis/router.py
--rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/redis/security.py
--rw-r--r--   0        0        0     6361 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/redis/testing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/redis/broker/__init__.py
--rw-r--r--   0        0        0    15867 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/redis/broker/broker.py
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/redis/broker/logging.py
--rw-r--r--   0        0        0     7391 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/redis/broker/registrator.py
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/redis/fastapi/__init__.py
--rw-r--r--   0        0        0    27625 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/redis/fastapi/fastapi.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/redis/publisher/__init__.py
--rw-r--r--   0        0        0     5948 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/redis/publisher/asyncapi.py
--rw-r--r--   0        0        0     4170 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/redis/publisher/producer.py
--rw-r--r--   0        0        0    17067 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/redis/publisher/usecase.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/redis/schemas/__init__.py
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/redis/schemas/list_sub.py
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/redis/schemas/proto.py
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/redis/schemas/pub_sub.py
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/redis/schemas/stream_sub.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/redis/subscriber/__init__.py
--rw-r--r--   0        0        0     6993 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/redis/subscriber/asyncapi.py
--rw-r--r--   0        0        0    19669 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/redis/subscriber/usecase.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/testing/__init__.py
--rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/testing/app.py
--rw-r--r--   0        0        0     6392 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/testing/broker.py
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/utils/__init__.py
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/utils/ast.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/utils/classes.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/utils/data.py
--rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/utils/functions.py
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/utils/no_cast.py
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/utils/path.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/utils/context/__init__.py
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/utils/context/builders.py
--rw-r--r--   0        0        0     5117 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/utils/context/repository.py
--rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/faststream/utils/context/types.py
--rwxr-xr-x   0        0        0      915 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/scripts/build-docs-pre-commit.sh
--rwxr-xr-x   0        0        0       66 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/scripts/build-docs.sh
--rwxr-xr-x   0        0        0      909 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/scripts/lint-pre-commit.sh
--rwxr-xr-x   0        0        0      247 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/scripts/lint.sh
--rwxr-xr-x   0        0        0       51 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/scripts/publish.sh
--rwxr-xr-x   0        0        0       70 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/scripts/serve-docs.sh
--rwxr-xr-x   0        0        0      522 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/scripts/set_variables.sh
--rwxr-xr-x   0        0        0      147 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/scripts/start_test_env.sh
--rwxr-xr-x   0        0        0      197 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/scripts/static-analysis.sh
--rwxr-xr-x   0        0        0      926 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/scripts/static-pre-commit.sh
--rwxr-xr-x   0        0        0      132 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/scripts/stop_test_env.sh
--rwxr-xr-x   0        0        0      154 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/scripts/test-cov.sh
--rwxr-xr-x   0        0        0      131 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/scripts/test.sh
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/.gitignore
--rw-r--r--   0        0        0    11363 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/LICENSE
--rw-r--r--   0        0        0    14865 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/README.md
--rw-r--r--   0        0        0     9839 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/pyproject.toml
--rw-r--r--   0        0        0    19822 2020-02-02 00:00:00.000000 faststream-0.5.0rc0/PKG-INFO
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/.codespell-whitelist.txt
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     3860 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/.secrets.baseline
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/.semgrepignore
+-rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/CITATION.cff
+-rw-r--r--   0        0        0     5480 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     2630 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/SECURITY.md
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/serve.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/.github/dependabot.yml
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/.github/workflows/check-broken-links-in-docs.yaml
+-rw-r--r--   0        0        0     3520 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/.github/workflows/codeql.yml
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/.github/workflows/dependency-review.yaml
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/.github/workflows/deploy-docs.yaml
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/.github/workflows/publish_coverage.yml
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/.github/workflows/publish_pypi.yml
+-rw-r--r--   0        0        0    16399 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/.github/workflows/test.yaml
+-rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/.github/workflows/update_release_notes.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/__init__.py
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/e01_basic_consume.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/e02_1_basic_publisher.py
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/e02_2_basic_publisher.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/e02_3_basic_publisher.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/e03_miltiple_pubsub.py
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/e04_msg_filter.py
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/e05_rpc_request.py
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/e06_manual_ack.py
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/e07_ack_immediately.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/e08_testing.py
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/e09_testing_mocks.py
+-rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/e10_middlewares.py
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/e11_settings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/fastapi_integration/__init__.py
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/fastapi_integration/app.py
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/fastapi_integration/testing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/howto/__init__.py
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/howto/structlogs.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/kafka/__init__.py
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/kafka/ack_after_process.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/kafka/batch_consume.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/kafka/batch_publish_1.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/kafka/batch_publish_2.py
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/kafka/batch_publish_3.py
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/kafka/testing.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/nats/__init__.py
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/nats/e01_basic.py
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/nats/e02_basic_rpc.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/nats/e03_publisher.py
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/nats/e04_js_basic.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/nats/e05_basic_and_js.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/nats/e06_key_value.py
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/nats/e07_object_storage.py
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/nats/e08_wildcards.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/nats/e09_pull_sub.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/rabbit/__init__.py
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/rabbit/direct.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/rabbit/fanout.py
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/rabbit/header.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/rabbit/stream.py
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/rabbit/topic.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/redis/__init__.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/redis/channel_sub.py
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/redis/channel_sub_pattern.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/redis/list_sub.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/redis/list_sub_batch.py
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/redis/rpc.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/redis/stream_sub.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/redis/stream_sub_batch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/router/__init__.py
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/router/basic_consume.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/router/basic_publish.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/router/delay_registration.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/serialization/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/serialization/avro/__init__.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/serialization/avro/avro.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/serialization/avro/person.avsc
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/serialization/avro/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/serialization/msgpack/__init__.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/serialization/msgpack/pack.py
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/serialization/msgpack/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/serialization/protobuf/__init__.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/serialization/protobuf/message.proto
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/serialization/protobuf/protobuf.py
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/examples/serialization/protobuf/requirements.txt
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/__about__.py
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/__init__.py
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/__main__.py
+-rw-r--r--   0        0        0     5562 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/_compat.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/annotations.py
+-rw-r--r--   0        0        0     6985 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/app.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/constants.py
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/py.typed
+-rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/security.py
+-rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/types.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/asyncapi/__init__.py
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/asyncapi/abc.py
+-rw-r--r--   0        0        0     5963 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/asyncapi/generate.py
+-rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/asyncapi/message.py
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/asyncapi/proto.py
+-rw-r--r--   0        0        0     4739 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/asyncapi/site.py
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/asyncapi/utils.py
+-rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/asyncapi/schema/__init__.py
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/asyncapi/schema/channels.py
+-rw-r--r--   0        0        0     5067 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/asyncapi/schema/info.py
+-rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/asyncapi/schema/main.py
+-rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/asyncapi/schema/message.py
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/asyncapi/schema/operations.py
+-rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/asyncapi/schema/security.py
+-rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/asyncapi/schema/servers.py
+-rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/asyncapi/schema/utils.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/asyncapi/schema/bindings/__init__.py
+-rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/asyncapi/schema/bindings/amqp.py
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/asyncapi/schema/bindings/kafka.py
+-rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/asyncapi/schema/bindings/main.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/asyncapi/schema/bindings/nats.py
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/asyncapi/schema/bindings/redis.py
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/asyncapi/schema/bindings/sqs.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/broker/__init__.py
+-rw-r--r--   0        0        0     5992 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/broker/acknowledgement_watcher.py
+-rw-r--r--   0        0        0     2630 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/broker/message.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/broker/proto.py
+-rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/broker/router.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/broker/schemas.py
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/broker/types.py
+-rw-r--r--   0        0        0     3196 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/broker/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/broker/core/__init__.py
+-rw-r--r--   0        0        0     3366 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/broker/core/abc.py
+-rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/broker/core/logging.py
+-rw-r--r--   0        0        0    10336 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/broker/core/usecase.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/broker/fastapi/__init__.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/broker/fastapi/context.py
+-rw-r--r--   0        0        0     4309 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/broker/fastapi/get_dependant.py
+-rw-r--r--   0        0        0     9644 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/broker/fastapi/route.py
+-rw-r--r--   0        0        0    18036 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/broker/fastapi/router.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/broker/middlewares/__init__.py
+-rw-r--r--   0        0        0     3039 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/broker/middlewares/base.py
+-rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/broker/middlewares/logging.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/broker/publisher/__init__.py
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/broker/publisher/fake.py
+-rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/broker/publisher/proto.py
+-rw-r--r--   0        0        0     5012 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/broker/publisher/usecase.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/broker/subscriber/__init__.py
+-rw-r--r--   0        0        0     5169 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/broker/subscriber/call_item.py
+-rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/broker/subscriber/proto.py
+-rw-r--r--   0        0        0    12951 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/broker/subscriber/usecase.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/broker/wrapper/__init__.py
+-rw-r--r--   0        0        0     5830 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/broker/wrapper/call.py
+-rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/broker/wrapper/proto.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/cli/__init__.py
+-rw-r--r--   0        0        0     7018 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/cli/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/cli/docs/__init__.py
+-rw-r--r--   0        0        0     4814 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/cli/docs/app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/cli/supervisors/__init__.py
+-rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/cli/supervisors/basereload.py
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/cli/supervisors/multiprocess.py
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/cli/supervisors/utils.py
+-rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/cli/supervisors/watchfiles.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/cli/utils/__init__.py
+-rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/cli/utils/imports.py
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/cli/utils/logs.py
+-rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/cli/utils/parser.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/confluent/__init__.py
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/confluent/annotations.py
+-rw-r--r--   0        0        0    14880 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/confluent/client.py
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/confluent/message.py
+-rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/confluent/parser.py
+-rw-r--r--   0        0        0    19994 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/confluent/router.py
+-rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/confluent/security.py
+-rw-r--r--   0        0        0     7212 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/confluent/testing.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/confluent/broker/__init__.py
+-rw-r--r--   0        0        0    19107 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/confluent/broker/broker.py
+-rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/confluent/broker/logging.py
+-rw-r--r--   0        0        0    64895 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/confluent/broker/registrator.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/confluent/fastapi/__init__.py
+-rw-r--r--   0        0        0    99679 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/confluent/fastapi/fastapi.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/confluent/publisher/__init__.py
+-rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/confluent/publisher/asyncapi.py
+-rw-r--r--   0        0        0     3274 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/confluent/publisher/producer.py
+-rw-r--r--   0        0        0     6095 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/confluent/publisher/usecase.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/confluent/schemas/__init__.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/confluent/schemas/params.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/confluent/subscriber/__init__.py
+-rw-r--r--   0        0        0     6124 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/confluent/subscriber/asyncapi.py
+-rw-r--r--   0        0        0    10425 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/confluent/subscriber/usecase.py
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/kafka/__init__.py
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/kafka/annotations.py
+-rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/kafka/message.py
+-rw-r--r--   0        0        0     2752 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/kafka/parser.py
+-rw-r--r--   0        0        0    20332 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/kafka/router.py
+-rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/kafka/security.py
+-rw-r--r--   0        0        0     5923 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/kafka/testing.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/kafka/broker/__init__.py
+-rw-r--r--   0        0        0    29222 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/kafka/broker/broker.py
+-rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/kafka/broker/logging.py
+-rw-r--r--   0        0        0    65255 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/kafka/broker/registrator.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/kafka/fastapi/__init__.py
+-rw-r--r--   0        0        0   111507 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/kafka/fastapi/fastapi.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/kafka/publisher/__init__.py
+-rw-r--r--   0        0        0     5520 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/kafka/publisher/asyncapi.py
+-rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/kafka/publisher/producer.py
+-rw-r--r--   0        0        0     9857 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/kafka/publisher/usecase.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/kafka/schemas/__init__.py
+-rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/kafka/schemas/params.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/kafka/subscriber/__init__.py
+-rw-r--r--   0        0        0     6047 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/kafka/subscriber/asyncapi.py
+-rw-r--r--   0        0        0    10148 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/kafka/subscriber/usecase.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/log/__init__.py
+-rw-r--r--   0        0        0     2424 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/log/formatter.py
+-rw-r--r--   0        0        0     1975 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/log/logging.py
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/nats/__init__.py
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/nats/annotations.py
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/nats/helpers.py
+-rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/nats/message.py
+-rw-r--r--   0        0        0     3375 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/nats/parser.py
+-rw-r--r--   0        0        0    12261 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/nats/router.py
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/nats/security.py
+-rw-r--r--   0        0        0     4297 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/nats/testing.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/nats/broker/__init__.py
+-rw-r--r--   0        0        0    26786 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/nats/broker/broker.py
+-rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/nats/broker/logging.py
+-rw-r--r--   0        0        0    11855 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/nats/broker/registrator.py
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/nats/fastapi/__init__.py
+-rw-r--r--   0        0        0    36215 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/nats/fastapi/fastapi.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/nats/publisher/__init__.py
+-rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/nats/publisher/asyncapi.py
+-rw-r--r--   0        0        0     5503 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/nats/publisher/producer.py
+-rw-r--r--   0        0        0     5216 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/nats/publisher/usecase.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/nats/schemas/__init__.py
+-rw-r--r--   0        0        0     9297 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/nats/schemas/js_stream.py
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/nats/schemas/pull_sub.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/nats/subscriber/__init__.py
+-rw-r--r--   0        0        0     6406 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/nats/subscriber/asyncapi.py
+-rw-r--r--   0        0        0    14733 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/nats/subscriber/usecase.py
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/rabbit/__init__.py
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/rabbit/annotations.py
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/rabbit/message.py
+-rw-r--r--   0        0        0     3381 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/rabbit/parser.py
+-rw-r--r--   0        0        0    11482 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/rabbit/router.py
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/rabbit/security.py
+-rw-r--r--   0        0        0    10071 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/rabbit/testing.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/rabbit/types.py
+-rw-r--r--   0        0        0     4125 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/rabbit/utils.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/rabbit/broker/__init__.py
+-rw-r--r--   0        0        0    19378 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/rabbit/broker/broker.py
+-rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/rabbit/broker/logging.py
+-rw-r--r--   0        0        0    10779 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/rabbit/broker/registrator.py
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/rabbit/fastapi/__init__.py
+-rw-r--r--   0        0        0    30268 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/rabbit/fastapi/router.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/rabbit/publisher/__init__.py
+-rw-r--r--   0        0        0     5063 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/rabbit/publisher/asyncapi.py
+-rw-r--r--   0        0        0     7421 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/rabbit/publisher/producer.py
+-rw-r--r--   0        0        0     8271 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/rabbit/publisher/usecase.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/rabbit/schemas/__init__.py
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/rabbit/schemas/constants.py
+-rw-r--r--   0        0        0     3919 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/rabbit/schemas/exchange.py
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/rabbit/schemas/proto.py
+-rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/rabbit/schemas/queue.py
+-rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/rabbit/schemas/reply.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/rabbit/subscriber/__init__.py
+-rw-r--r--   0        0        0     4383 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/rabbit/subscriber/asyncapi.py
+-rw-r--r--   0        0        0     7021 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/rabbit/subscriber/usecase.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/redis/__init__.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/redis/annotations.py
+-rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/redis/message.py
+-rw-r--r--   0        0        0     5616 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/redis/parser.py
+-rw-r--r--   0        0        0     8192 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/redis/router.py
+-rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/redis/security.py
+-rw-r--r--   0        0        0     6635 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/redis/testing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/redis/broker/__init__.py
+-rw-r--r--   0        0        0    15800 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/redis/broker/broker.py
+-rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/redis/broker/logging.py
+-rw-r--r--   0        0        0     7557 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/redis/broker/registrator.py
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/redis/fastapi/__init__.py
+-rw-r--r--   0        0        0    27539 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/redis/fastapi/fastapi.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/redis/publisher/__init__.py
+-rw-r--r--   0        0        0     6019 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/redis/publisher/asyncapi.py
+-rw-r--r--   0        0        0     4139 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/redis/publisher/producer.py
+-rw-r--r--   0        0        0    17110 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/redis/publisher/usecase.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/redis/schemas/__init__.py
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/redis/schemas/list_sub.py
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/redis/schemas/proto.py
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/redis/schemas/pub_sub.py
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/redis/schemas/stream_sub.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/redis/subscriber/__init__.py
+-rw-r--r--   0        0        0     7044 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/redis/subscriber/asyncapi.py
+-rw-r--r--   0        0        0    21150 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/redis/subscriber/usecase.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/testing/__init__.py
+-rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/testing/app.py
+-rw-r--r--   0        0        0     6746 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/testing/broker.py
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/utils/__init__.py
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/utils/ast.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/utils/classes.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/utils/data.py
+-rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/utils/functions.py
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/utils/no_cast.py
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/utils/path.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/utils/context/__init__.py
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/utils/context/builders.py
+-rw-r--r--   0        0        0     5117 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/utils/context/repository.py
+-rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/faststream/utils/context/types.py
+-rwxr-xr-x   0        0        0      915 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/scripts/build-docs-pre-commit.sh
+-rwxr-xr-x   0        0        0       66 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/scripts/build-docs.sh
+-rwxr-xr-x   0        0        0      909 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/scripts/lint-pre-commit.sh
+-rwxr-xr-x   0        0        0      247 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/scripts/lint.sh
+-rwxr-xr-x   0        0        0       51 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/scripts/publish.sh
+-rwxr-xr-x   0        0        0       70 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/scripts/serve-docs.sh
+-rwxr-xr-x   0        0        0      522 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/scripts/set_variables.sh
+-rwxr-xr-x   0        0        0      147 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/scripts/start_test_env.sh
+-rwxr-xr-x   0        0        0      175 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/scripts/static-analysis.sh
+-rwxr-xr-x   0        0        0      926 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/scripts/static-pre-commit.sh
+-rwxr-xr-x   0        0        0      132 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/scripts/stop_test_env.sh
+-rwxr-xr-x   0        0        0      154 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/scripts/test-cov.sh
+-rwxr-xr-x   0        0        0      131 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/scripts/test.sh
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/.gitignore
+-rw-r--r--   0        0        0    11363 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/LICENSE
+-rw-r--r--   0        0        0    14865 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/README.md
+-rw-r--r--   0        0        0    10246 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/pyproject.toml
+-rw-r--r--   0        0        0    19981 2020-02-02 00:00:00.000000 faststream-0.5.0rc1/PKG-INFO
```

### Comparing `faststream-0.5.0rc0/.pre-commit-config.yaml` & `faststream-0.5.0rc1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/.secrets.baseline` & `faststream-0.5.0rc1/.secrets.baseline`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8983333333333334%*

 * *Differences: {"'generated_at'": "'2024-04-07T03:11:32Z'",*

 * * "'results'": "{'docs/docs/en/release.md': {0: {'line_number': 836}}, "*

 * *              "'examples/e10_middlewares.py': {0: {'line_number': 33}}}"}*

```diff
@@ -35,15 +35,15 @@
         {
             "path": "detect_secrets.filters.heuristic.is_swagger_file"
         },
         {
             "path": "detect_secrets.filters.heuristic.is_templated_secret"
         }
     ],
-    "generated_at": "2024-03-14T06:43:32Z",
+    "generated_at": "2024-04-07T03:11:32Z",
     "plugins_used": [
         {
             "name": "ArtifactoryDetector"
         },
         {
             "name": "AWSKeyDetector"
         },
@@ -124,25 +124,25 @@
         ],
         "docs/docs/en/release.md": [
             {
                 "filename": "docs/docs/en/release.md",
                 "hashed_secret": "35675e68f4b5af7b995d9205ad0fc43842f16450",
                 "is_secret": false,
                 "is_verified": false,
-                "line_number": 710,
+                "line_number": 836,
                 "type": "Basic Auth Credentials"
             }
         ],
         "examples/e10_middlewares.py": [
             {
                 "filename": "examples/e10_middlewares.py",
                 "hashed_secret": "35675e68f4b5af7b995d9205ad0fc43842f16450",
                 "is_secret": false,
                 "is_verified": false,
-                "line_number": 35,
+                "line_number": 33,
                 "type": "Basic Auth Credentials"
             }
         ],
         "examples/e11_settings.py": [
             {
                 "filename": "examples/e11_settings.py",
                 "hashed_secret": "35675e68f4b5af7b995d9205ad0fc43842f16450",
```

### Comparing `faststream-0.5.0rc0/CITATION.cff` & `faststream-0.5.0rc1/CITATION.cff`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/CODE_OF_CONDUCT.md` & `faststream-0.5.0rc1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/CONTRIBUTING.md` & `faststream-0.5.0rc1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/SECURITY.md` & `faststream-0.5.0rc1/SECURITY.md`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/.github/PULL_REQUEST_TEMPLATE.md` & `faststream-0.5.0rc1/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/.github/dependabot.yml` & `faststream-0.5.0rc1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/.github/ISSUE_TEMPLATE/bug_report.md` & `faststream-0.5.0rc1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/.github/ISSUE_TEMPLATE/feature_request.md` & `faststream-0.5.0rc1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/.github/workflows/check-broken-links-in-docs.yaml` & `faststream-0.5.0rc1/.github/workflows/check-broken-links-in-docs.yaml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/.github/workflows/codeql.yml` & `faststream-0.5.0rc1/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/.github/workflows/dependency-review.yaml` & `faststream-0.5.0rc1/.github/workflows/dependency-review.yaml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/.github/workflows/deploy-docs.yaml` & `faststream-0.5.0rc1/.github/workflows/deploy-docs.yaml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/.github/workflows/publish_coverage.yml` & `faststream-0.5.0rc1/.github/workflows/publish_coverage.yml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/.github/workflows/publish_pypi.yml` & `faststream-0.5.0rc1/.github/workflows/publish_pypi.yml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/.github/workflows/test.yaml` & `faststream-0.5.0rc1/.github/workflows/test.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -18,23 +18,23 @@
         with:
           python-version: 3.9
       - name: Install Dependencies and library
         shell: bash
         run: |
           set -ux
           python -m pip install --upgrade pip
-          pip install -e ".[rabbit,kafka,confluent,redis,nats,lint]"
+          pip install -e ".[lint]"
 
       - name: Run ruff
         shell: bash
-        run: ruff faststream
+        run: ruff check
 
       - name: Run mypy
         shell: bash
-        run: mypy faststream tests/mypy
+        run: mypy
 
       - name: Run bandit
         shell: bash
         run: bandit -c pyproject.toml -r faststream
 
       - name: Run Semgrep
         shell: bash
```

### Comparing `faststream-0.5.0rc0/.github/workflows/update_release_notes.yaml` & `faststream-0.5.0rc1/.github/workflows/update_release_notes.yaml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/examples/e02_1_basic_publisher.py` & `faststream-0.5.0rc1/examples/e02_1_basic_publisher.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/examples/e02_2_basic_publisher.py` & `faststream-0.5.0rc1/examples/e02_2_basic_publisher.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/examples/e02_3_basic_publisher.py` & `faststream-0.5.0rc1/examples/e02_3_basic_publisher.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/examples/e03_miltiple_pubsub.py` & `faststream-0.5.0rc1/examples/e03_miltiple_pubsub.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/examples/e04_msg_filter.py` & `faststream-0.5.0rc1/examples/e04_msg_filter.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/examples/e07_ack_immediately.py` & `faststream-0.5.0rc1/examples/e07_ack_immediately.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/examples/e09_testing_mocks.py` & `faststream-0.5.0rc1/examples/e09_testing_mocks.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/examples/e10_middlewares.py` & `faststream-0.5.0rc1/examples/e10_middlewares.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/examples/e11_settings.py` & `faststream-0.5.0rc1/examples/e11_settings.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/examples/fastapi_integration/testing.py` & `faststream-0.5.0rc1/examples/fastapi_integration/testing.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/examples/howto/structlogs.py` & `faststream-0.5.0rc1/examples/howto/structlogs.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/examples/kafka/testing.py` & `faststream-0.5.0rc1/examples/kafka/testing.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/examples/nats/e03_publisher.py` & `faststream-0.5.0rc1/examples/nats/e03_publisher.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/examples/nats/e04_js_basic.py` & `faststream-0.5.0rc1/examples/nats/e04_js_basic.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/examples/nats/e05_basic_and_js.py` & `faststream-0.5.0rc1/examples/nats/e05_basic_and_js.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/examples/nats/e06_key_value.py` & `faststream-0.5.0rc1/examples/nats/e06_key_value.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/examples/nats/e07_object_storage.py` & `faststream-0.5.0rc1/examples/nats/e07_object_storage.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/examples/rabbit/direct.py` & `faststream-0.5.0rc1/examples/rabbit/direct.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/examples/rabbit/fanout.py` & `faststream-0.5.0rc1/examples/rabbit/fanout.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/examples/rabbit/header.py` & `faststream-0.5.0rc1/examples/rabbit/header.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/examples/rabbit/topic.py` & `faststream-0.5.0rc1/examples/rabbit/topic.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/examples/redis/channel_sub_pattern.py` & `faststream-0.5.0rc1/examples/redis/channel_sub_pattern.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/examples/redis/rpc.py` & `faststream-0.5.0rc1/examples/redis/rpc.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/examples/router/basic_publish.py` & `faststream-0.5.0rc1/examples/router/basic_publish.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/examples/serialization/avro/avro.py` & `faststream-0.5.0rc1/examples/serialization/avro/avro.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/examples/serialization/msgpack/pack.py` & `faststream-0.5.0rc1/examples/serialization/msgpack/pack.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/examples/serialization/protobuf/protobuf.py` & `faststream-0.5.0rc1/examples/serialization/protobuf/protobuf.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/faststream/__init__.py` & `faststream-0.5.0rc1/faststream/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/faststream/_compat.py` & `faststream-0.5.0rc1/faststream/_compat.py`

 * *Files 9% similar despite different names*

```diff
@@ -70,21 +70,14 @@
             raise RequestValidationError(errors, ROUTER_VALIDATION_ERROR_MODEL)  # type: ignore[misc]
 
 except ImportError:
     HAS_FASTAPI = False
 
 JsonSchemaValue = Mapping[str, Any]
 
-PValidationError: Optional[Type[Exception]]
-try:
-    from pydantic import ValidationError
-    PValidationError = ValidationError
-except ImportError:
-    PValidationError = None
-
 if PYDANTIC_V2:
     if PYDANTIC_VERSION >= "2.4.0":
         from pydantic.annotated_handlers import (
             GetJsonSchemaHandler as GetJsonSchemaHandler,
         )
         from pydantic_core.core_schema import (  # type: ignore[attr-defined]
             with_info_plain_validator_function as with_info_plain_validator_function,
```

### Comparing `faststream-0.5.0rc0/faststream/app.py` & `faststream-0.5.0rc1/faststream/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,19 +11,17 @@
     TypeVar,
     Union,
 )
 
 import anyio
 from typing_extensions import ParamSpec
 
-from faststream._compat import PValidationError
 from faststream.cli.supervisors.utils import set_exit
 from faststream.exceptions import ValidationError
 from faststream.log.logging import logger
-from faststream.types import AnyDict, AsyncFunc, Lifespan, LoggerProto, SettingField
 from faststream.utils import apply_types, context
 from faststream.utils.functions import drop_response_type, fake_context, to_async
 
 P_HookParams = ParamSpec("P_HookParams")
 T_HookReturn = TypeVar("T_HookReturn")
 
 
@@ -35,41 +33,48 @@
         ExternalDocsDict,
         License,
         LicenseDict,
         Tag,
         TagDict,
     )
     from faststream.broker.core.usecase import BrokerUsecase
-    from faststream.types import AnyHttpUrl
+    from faststream.types import (
+        AnyDict,
+        AnyHttpUrl,
+        AsyncFunc,
+        Lifespan,
+        LoggerProto,
+        SettingField,
+    )
 
 
 class FastStream:
     """A class representing a FastStream application."""
 
-    _on_startup_calling: List[AsyncFunc]
-    _after_startup_calling: List[AsyncFunc]
-    _on_shutdown_calling: List[AsyncFunc]
-    _after_shutdown_calling: List[AsyncFunc]
+    _on_startup_calling: List["AsyncFunc"]
+    _after_startup_calling: List["AsyncFunc"]
+    _on_shutdown_calling: List["AsyncFunc"]
+    _after_shutdown_calling: List["AsyncFunc"]
 
     def __init__(
         self,
         broker: Optional["BrokerUsecase[Any, Any]"] = None,
-        logger: Optional[LoggerProto] = logger,
-        lifespan: Optional[Lifespan] = None,
+        logger: Optional["LoggerProto"] = logger,
+        lifespan: Optional["Lifespan"] = None,
         # AsyncAPI args,
         title: str = "FastStream",
         version: str = "0.1.0",
         description: str = "",
         terms_of_service: Optional["AnyHttpUrl"] = None,
-        license: Optional[Union["License", "LicenseDict", AnyDict]] = None,
-        contact: Optional[Union["Contact", "ContactDict", AnyDict]] = None,
+        license: Optional[Union["License", "LicenseDict", "AnyDict"]] = None,
+        contact: Optional[Union["Contact", "ContactDict", "AnyDict"]] = None,
         identifier: Optional[str] = None,
-        tags: Optional[Sequence[Union["Tag", "TagDict", AnyDict]]] = None,
+        tags: Optional[Sequence[Union["Tag", "TagDict", "AnyDict"]]] = None,
         external_docs: Optional[
-            Union["ExternalDocs", "ExternalDocsDict", AnyDict]
+            Union["ExternalDocs", "ExternalDocsDict", "AnyDict"]
         ] = None,
     ) -> None:
         context.set_global("app", self)
 
         self.broker = broker
         self.logger = logger
         self.context = context
@@ -142,15 +147,15 @@
         """Add hook running AFTER broker disconnected."""
         self._after_shutdown_calling.append(apply_types(to_async(func)))
         return func
 
     async def run(
         self,
         log_level: int = logging.INFO,
-        run_extra_options: Optional[Dict[str, SettingField]] = None,
+        run_extra_options: Optional[Dict[str, "SettingField"]] = None,
         sleep_time: float = 0.1,
     ) -> None:
         """Run FastStream Application."""
         assert self.broker, "You should setup a broker"  # nosec B101
 
         set_exit(lambda *_: self.exit(), sync=False)
 
@@ -164,31 +169,33 @@
 
     def exit(self) -> None:
         """Stop application manually."""
         self.should_exit = True
 
     async def start(
         self,
-        **run_extra_options: SettingField,
+        **run_extra_options: "SettingField",
     ) -> None:
         """Executes startup hooks and start broker."""
         for func in self._on_startup_calling:
             call = func(**run_extra_options)
 
-            if PValidationError is not None:
-                try:
-                    await call
-                except PValidationError as e:
-                    raise ValidationError(
-                        fields=[x["loc"][0] for x in e.errors()]
-                    )
+            try:
+                from pydantic import ValidationError as PValidation
 
-            else:
+            except ImportError:
                 await call
 
+            else:
+                try:
+                    await call
+                except PValidation as e:
+                    fields = [str(x["loc"][0]) for x in e.errors()]
+                    raise ValidationError(fields=fields) from e
+
         if self.broker is not None:
             await self.broker.start()
 
         for func in self._after_startup_calling:
             await func()
 
     async def stop(self) -> None:
@@ -201,15 +208,15 @@
 
         for func in self._after_shutdown_calling:
             await func()
 
     async def _startup(
         self,
         log_level: int = logging.INFO,
-        run_extra_options: Optional[Dict[str, SettingField]] = None,
+        run_extra_options: Optional[Dict[str, "SettingField"]] = None,
     ) -> None:
         self._log(log_level, "FastStream app starting...")
         await self.start(**(run_extra_options or {}))
         self._log(
             log_level, "FastStream app started successfully! To exit, press CTRL+C"
         )
```

### Comparing `faststream-0.5.0rc0/faststream/exceptions.py` & `faststream-0.5.0rc1/faststream/exceptions.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/faststream/types.py` & `faststream-0.5.0rc1/faststream/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 
     SendableMessage: TypeAlias = Union[
         BaseModel,
         BaseSendableMessage,
     ]
 
 except ImportError:
-    SendableMessage: TypeAlias = BaseSendableMessage  # type: ignore[no-redef]
+    SendableMessage: TypeAlias = BaseSendableMessage  # type: ignore[no-redef,misc]
 
 SettingField: TypeAlias = Union[
     bool,
     str,
     List[Union[bool, str]],
     List[str],
     List[bool],
```

### Comparing `faststream-0.5.0rc0/faststream/asyncapi/abc.py` & `faststream-0.5.0rc1/faststream/asyncapi/abc.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/faststream/asyncapi/generate.py` & `faststream-0.5.0rc1/faststream/asyncapi/generate.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 from typing import TYPE_CHECKING, Any, Dict, List, Union
 
 from faststream._compat import DEF_KEY, HAS_FASTAPI
-from faststream.app import FastStream
 from faststream.asyncapi.schema import (
     Channel,
     Components,
     Info,
     Message,
     Reference,
     Schema,
     Server,
 )
 from faststream.constants import ContentTypes
 
 if TYPE_CHECKING:
+    from faststream.app import FastStream
+    from faststream.broker.core.usecase import BrokerUsecase
+    from faststream.broker.types import ConnectionType, MsgType
+
     if HAS_FASTAPI:
         from faststream.broker.fastapi.router import StreamRouter
 
 
-def get_app_schema(app: Union[FastStream, "StreamRouter[Any]"]) -> Schema:
+def get_app_schema(app: Union["FastStream", "StreamRouter[Any]"]) -> Schema:
     """Get the application schema."""
     broker = app.broker
     if broker is None:  # pragma: no cover
         raise RuntimeError()
     broker.setup()
 
     servers = get_broker_server(broker)
@@ -77,15 +80,17 @@
             if broker.security is None
             else broker.security.get_schema(),
         ),
     )
     return schema
 
 
-def get_broker_server(broker) -> Dict[str, Server]:
+def get_broker_server(
+    broker: "BrokerUsecase[MsgType, ConnectionType]",
+) -> Dict[str, Server]:
     """Get the broker server for an application."""
     servers = {}
 
     broker_meta: Dict[str, Any] = {
         "protocol": broker.protocol,
         "protocolVersion": broker.protocol_version,
         "description": broker.description,
@@ -116,15 +121,17 @@
                 url=url,
                 **broker_meta,
             )
 
     return servers
 
 
-def get_broker_channels(broker) -> Dict[str, Channel]:
+def get_broker_channels(
+    broker: "BrokerUsecase[MsgType, ConnectionType]",
+) -> Dict[str, Channel]:
     """Get the broker channels for an application."""
     channels = {}
 
     for h in broker._subscribers.values():
         channels.update(h.schema())
 
     for p in broker._publishers.values():
```

### Comparing `faststream-0.5.0rc0/faststream/asyncapi/message.py` & `faststream-0.5.0rc1/faststream/asyncapi/message.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 from inspect import isclass
-from typing import Any, Dict, Optional, Sequence, Type, overload
+from typing import TYPE_CHECKING, Any, Dict, Optional, Sequence, Type, overload
 
-from fast_depends.core import CallModel
 from pydantic import BaseModel, create_model
 
 from faststream._compat import DEF_KEY, PYDANTIC_V2, get_model_fields, model_schema
 
+if TYPE_CHECKING:
+    from fast_depends.core import CallModel
 
-def parse_handler_params(call: CallModel[Any, Any], prefix: str = "") -> Dict[str, Any]:
+
+def parse_handler_params(
+    call: "CallModel[Any, Any]", prefix: str = ""
+) -> Dict[str, Any]:
     """Parses the handler parameters."""
     model = call.model
     assert model  # nosec B101
 
     body = get_model_schema(
         create_model(  # type: ignore[call-overload]
             model.__name__,
@@ -24,25 +28,25 @@
     if body is None:
         return {"title": "EmptyPayload", "type": "null"}
 
     return body
 
 
 @overload
-def get_response_schema(call: None, prefix: str = "") -> None:
-    ...
+def get_response_schema(call: None, prefix: str = "") -> None: ...
 
 
 @overload
-def get_response_schema(call: CallModel[Any, Any], prefix: str = "") -> Dict[str, Any]:
-    ...
+def get_response_schema(
+    call: "CallModel[Any, Any]", prefix: str = ""
+) -> Dict[str, Any]: ...
 
 
 def get_response_schema(
-    call: Optional[CallModel[Any, Any]],
+    call: Optional["CallModel[Any, Any]"],
     prefix: str = "",
 ) -> Optional[Dict[str, Any]]:
     """Get the response schema for a given call."""
     return get_model_schema(
         getattr(
             call, "response_model", None
         ),  # NOTE: FastAPI Dependant object compatibility
@@ -51,25 +55,23 @@
 
 
 @overload
 def get_model_schema(
     call: None,
     prefix: str = "",
     exclude: Sequence[str] = (),
-) -> None:
-    ...
+) -> None: ...
 
 
 @overload
 def get_model_schema(
     call: Type[BaseModel],
     prefix: str = "",
     exclude: Sequence[str] = (),
-) -> Dict[str, Any]:
-    ...
+) -> Dict[str, Any]: ...
 
 
 def get_model_schema(
     call: Optional[Type[BaseModel]],
     prefix: str = "",
     exclude: Sequence[str] = (),
 ) -> Optional[Dict[str, Any]]:
```

### Comparing `faststream-0.5.0rc0/faststream/asyncapi/proto.py` & `faststream-0.5.0rc1/faststream/asyncapi/proto.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from abc import abstractmethod
-from typing import Dict, Optional, Protocol
+from typing import TYPE_CHECKING, Dict, Optional, Protocol
 
 from typing_extensions import Annotated, Doc
 
-from faststream.asyncapi.schema.channels import Channel
+if TYPE_CHECKING:
+    from faststream.asyncapi.schema.channels import Channel
 
 
 class AsyncAPIProto(Protocol):
     """A class representing an asynchronous API operation."""
 
     title_: Annotated[
         Optional[str],
@@ -31,10 +32,10 @@
     @property
     @abstractmethod
     def description(self) -> Optional[str]:
         """Returns the description of the API operation."""
         ...
 
     @abstractmethod
-    def schema(self) -> Dict[str, Channel]:
+    def schema(self) -> Dict[str, "Channel"]:
         """Generate AsyncAPI schema."""
         ...
```

### Comparing `faststream-0.5.0rc0/faststream/asyncapi/site.py` & `faststream-0.5.0rc1/faststream/asyncapi/site.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from functools import partial
 from http import server
-from logging import Logger
-from typing import TYPE_CHECKING, Any, Dict, Optional
+from typing import TYPE_CHECKING, Any, Dict
 from urllib.parse import parse_qs, urlparse
 
 from faststream._compat import json_dumps
+from faststream.log import logger
 
 if TYPE_CHECKING:
     from faststream.asyncapi.schema import Schema
 
 
 def get_asyncapi_html(
     schema: "Schema",
@@ -95,20 +95,18 @@
     )
 
 
 def serve_app(
     schema: "Schema",
     host: str,
     port: int,
-    logger: Optional[Logger] = None,
 ) -> None:
     """Serve the HTTPServer with AsyncAPI schema."""
-    if logger:
-        logger.info(f"HTTPServer running on http://{host}:{port} (Press CTRL+C to quit)")
-        logger.warn("Please, do not use it in production.")
+    logger.info(f"HTTPServer running on http://{host}:{port} (Press CTRL+C to quit)")
+    logger.warn("Please, do not use it in production.")
 
     server.HTTPServer(
         (host, port),
         partial(_Handler, schema=schema),
     ).serve_forever()
```

### Comparing `faststream-0.5.0rc0/faststream/asyncapi/schema/__init__.py` & `faststream-0.5.0rc1/faststream/asyncapi/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/faststream/asyncapi/schema/channels.py` & `faststream-0.5.0rc1/faststream/asyncapi/schema/channels.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/faststream/asyncapi/schema/info.py` & `faststream-0.5.0rc1/faststream/asyncapi/schema/info.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/faststream/asyncapi/schema/main.py` & `faststream-0.5.0rc1/faststream/asyncapi/schema/main.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/faststream/asyncapi/schema/message.py` & `faststream-0.5.0rc1/faststream/asyncapi/schema/message.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/faststream/asyncapi/schema/operations.py` & `faststream-0.5.0rc1/faststream/asyncapi/schema/operations.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/faststream/asyncapi/schema/security.py` & `faststream-0.5.0rc1/faststream/asyncapi/schema/security.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/faststream/asyncapi/schema/servers.py` & `faststream-0.5.0rc1/faststream/asyncapi/schema/servers.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/faststream/asyncapi/schema/utils.py` & `faststream-0.5.0rc1/faststream/asyncapi/schema/utils.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/faststream/asyncapi/schema/bindings/amqp.py` & `faststream-0.5.0rc1/faststream/asyncapi/schema/bindings/amqp.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/faststream/asyncapi/schema/bindings/kafka.py` & `faststream-0.5.0rc1/faststream/asyncapi/schema/bindings/kafka.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/faststream/asyncapi/schema/bindings/main.py` & `faststream-0.5.0rc1/faststream/asyncapi/schema/bindings/main.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/faststream/asyncapi/schema/bindings/nats.py` & `faststream-0.5.0rc1/faststream/asyncapi/schema/bindings/nats.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/faststream/asyncapi/schema/bindings/redis.py` & `faststream-0.5.0rc1/faststream/asyncapi/schema/bindings/redis.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/faststream/asyncapi/schema/bindings/sqs.py` & `faststream-0.5.0rc1/faststream/asyncapi/schema/bindings/sqs.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/faststream/broker/acknowledgement_watcher.py` & `faststream-0.5.0rc1/faststream/broker/acknowledgement_watcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import logging
 from abc import ABC, abstractmethod
 from collections import Counter
-from types import TracebackType
 from typing import TYPE_CHECKING, Any, Optional, Type, Union
 from typing import Counter as CounterType
 
 from faststream.exceptions import (
     AckMessage,
     HandlerException,
     NackMessage,
     RejectMessage,
     SkipMessage,
 )
 
 if TYPE_CHECKING:
+    from types import TracebackType
+
     from faststream.broker.message import StreamMessage
     from faststream.broker.types import MsgType
     from faststream.types import LoggerProto
 
 
 class BaseWatcher(ABC):
     """A base class for a watcher."""
@@ -98,17 +99,21 @@
         self.memory[message_id] += 1
 
     def is_max(self, message_id: str) -> bool:
         """Check if the number of tries for a message has exceeded the maximum allowed tries."""
         is_max = self.memory[message_id] > self.max_tries
         if self.logger is not None:
             if is_max:
-                self.logger.log(logging.ERROR, f"Already retried {self.max_tries} times. Skipped.")
+                self.logger.log(
+                    logging.ERROR, f"Already retried {self.max_tries} times. Skipped."
+                )
             else:
-                self.logger.log(logging.ERROR, "Error is occurred. Pushing back to queue.")
+                self.logger.log(
+                    logging.ERROR, "Error is occurred. Pushing back to queue."
+                )
         return is_max
 
     def remove(self, message_id: str) -> None:
         """Remove a message from memory."""
         self.memory[message_id] = 0
         self.memory += Counter()
 
@@ -129,15 +134,15 @@
     async def __aenter__(self) -> None:
         self.watcher.add(self.message.message_id)
 
     async def __aexit__(
         self,
         exc_type: Optional[Type[BaseException]],
         exc_val: Optional[BaseException],
-        exc_tb: Optional[TracebackType],
+        exc_tb: Optional["TracebackType"],
     ) -> bool:
         """Exit the asynchronous context manager."""
         if not exc_type:
             await self.__ack()
 
         elif isinstance(exc_val, HandlerException):
             if isinstance(exc_val, SkipMessage):
@@ -172,14 +177,15 @@
     async def __nack(self) -> None:
         await self.message.nack(**self.extra_options)
 
     async def __reject(self) -> None:
         await self.message.reject(**self.extra_options)
         self.watcher.remove(self.message.message_id)
 
+
 def get_watcher(
     logger: Optional["LoggerProto"],
     try_number: Union[bool, int],
 ) -> BaseWatcher:
     """Get a watcher object based on the provided parameters.
 
     Args:
```

### Comparing `faststream-0.5.0rc0/faststream/broker/message.py` & `faststream-0.5.0rc1/faststream/broker/message.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,27 @@
 import json
 from contextlib import suppress
 from dataclasses import dataclass, field
-from typing import Any, Generic, Optional, Sequence, Tuple, TypeVar, Union
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Generic,
+    Optional,
+    Sequence,
+    Tuple,
+    TypeVar,
+    Union,
+)
 from uuid import uuid4
 
 from faststream._compat import dump_json, json_loads
 from faststream.constants import ContentTypes
-from faststream.types import AnyDict, DecodedMessage, SendableMessage
+
+if TYPE_CHECKING:
+    from faststream.types import AnyDict, DecodedMessage, SendableMessage
 
 # prevent circular imports
 MsgType = TypeVar("MsgType")
 
 
 def gen_cor_id() -> str:
     """Generate random string to use as ID."""
@@ -20,42 +31,42 @@
 @dataclass
 class StreamMessage(Generic[MsgType]):
     """Generic class to represent a stream message."""
 
     raw_message: "MsgType"
 
     body: Union[bytes, Any]
-    decoded_body: Optional[DecodedMessage] = None
-    headers: AnyDict = field(default_factory=dict)
-    path: AnyDict = field(default_factory=dict)
+    headers: "AnyDict" = field(default_factory=dict)
+    path: "AnyDict" = field(default_factory=dict)
 
     content_type: Optional[str] = None
     reply_to: str = ""
     message_id: str = field(default_factory=gen_cor_id)  # pragma: no cover
     correlation_id: str = field(
         default_factory=gen_cor_id  # pragma: no cover
     )
 
+    decoded_body: Optional["DecodedMessage"] = field(default=None, init=False)
     processed: bool = field(default=False, init=False)
     committed: bool = field(default=False, init=False)
 
     async def ack(self) -> None:
         self.committed = True
 
     async def nack(self) -> None:
         self.committed = True
 
     async def reject(self) -> None:
         self.committed = True
 
 
-def decode_message(message: StreamMessage[Any]) -> DecodedMessage:
+def decode_message(message: "StreamMessage[Any]") -> "DecodedMessage":
     """Decodes a message."""
     body: Any = getattr(message, "body", message)
-    m: DecodedMessage = body
+    m: "DecodedMessage" = body
 
     if content_type := getattr(message, "content_type", None):
         if ContentTypes.text.value in content_type:
             m = body.decode()
         elif ContentTypes.json.value in content_type:  # pragma: no branch
             m = json_loads(body)
         else:
@@ -65,15 +76,15 @@
         with suppress(json.JSONDecodeError):
             m = json_loads(body)
 
     return m
 
 
 def encode_message(
-    msg: Union[Sequence[SendableMessage], SendableMessage],
+    msg: Union[Sequence["SendableMessage"], "SendableMessage"],
 ) -> Tuple[bytes, Optional[str]]:
     """Encodes a message."""
     if msg is None:
         return (
             b"",
             None,
         )
```

### Comparing `faststream-0.5.0rc0/faststream/broker/router.py` & `faststream-0.5.0rc1/faststream/broker/router.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,36 +2,32 @@
     TYPE_CHECKING,
     Any,
     Callable,
     Iterable,
     Optional,
 )
 
-from fast_depends.dependencies import Depends
-
 from faststream.broker.core.abc import ABCBroker
-from faststream.broker.types import (
-    MsgType,
-)
-from faststream.types import AnyDict
+from faststream.broker.types import MsgType
 
 if TYPE_CHECKING:
-    from faststream.broker.message import StreamMessage
+    from fast_depends.dependencies import Depends
+
     from faststream.broker.types import (
         BrokerMiddleware,
-        CustomDecoder,
-        CustomParser,
+        CustomCallable,
     )
+    from faststream.types import AnyDict
 
 
 class ArgsContainer:
     """Class to store any arguments."""
 
     args: Iterable[Any]
-    kwargs: AnyDict
+    kwargs: "AnyDict"
 
     def __init__(
         self,
         *args: Any,
         **kwargs: Any,
     ) -> None:
         self.args = args
@@ -63,18 +59,18 @@
 
     def __init__(
         self,
         *,
         handlers: Iterable[SubscriberRoute],
         # base options
         prefix: str,
-        dependencies: Iterable[Depends],
+        dependencies: Iterable["Depends"],
         middlewares: Iterable["BrokerMiddleware[MsgType]"],
-        parser: Optional["CustomParser[MsgType]"],
-        decoder: Optional["CustomDecoder[StreamMessage[MsgType]]"],
+        parser: Optional["CustomCallable"],
+        decoder: Optional["CustomCallable"],
         include_in_schema: Optional[bool],
     ) -> None:
         super().__init__(
             prefix=prefix,
             dependencies=dependencies,
             middlewares=middlewares,
             parser=parser,
```

### Comparing `faststream-0.5.0rc0/faststream/broker/schemas.py` & `faststream-0.5.0rc1/faststream/broker/schemas.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,25 +21,23 @@
 
     @overload
     @classmethod
     def validate(
         cls: Type[NameRequiredCls],
         value: Union[str, NameRequiredCls],
         **kwargs: Any,
-    ) -> NameRequiredCls:
-        ...
+    ) -> NameRequiredCls: ...
 
     @overload
     @classmethod
     def validate(
         cls: Type[NameRequiredCls],
         value: None,
         **kwargs: Any,
-    ) -> None:
-        ...
+    ) -> None: ...
 
     @classmethod
     def validate(
         cls: Type[NameRequiredCls],
         value: Union[str, NameRequiredCls, None],
         **kwargs: Any,
     ) -> Optional[NameRequiredCls]:
```

### Comparing `faststream-0.5.0rc0/faststream/broker/core/abc.py` & `faststream-0.5.0rc1/faststream/broker/core/abc.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,41 +4,39 @@
     Any,
     Generic,
     Iterable,
     Mapping,
     Optional,
 )
 
-from fast_depends.dependencies import Depends
-
-from faststream.broker.publisher.proto import PublisherProto
-from faststream.broker.subscriber.proto import SubscriberProto
 from faststream.broker.types import MsgType
 
 if TYPE_CHECKING:
-    from faststream.broker.message import StreamMessage
+    from fast_depends.dependencies import Depends
+
+    from faststream.broker.publisher.proto import PublisherProto
+    from faststream.broker.subscriber.proto import SubscriberProto
     from faststream.broker.types import (
         BrokerMiddleware,
-        CustomDecoder,
-        CustomParser,
+        CustomCallable,
     )
 
 
 class ABCBroker(Generic[MsgType]):
-    _subscribers: Mapping[int, SubscriberProto[MsgType]]
-    _publishers: Mapping[int, PublisherProto[MsgType]]
+    _subscribers: Mapping[int, "SubscriberProto[MsgType]"]
+    _publishers: Mapping[int, "PublisherProto[MsgType]"]
 
     def __init__(
         self,
         *,
         prefix: str,
-        dependencies: Iterable[Depends],
+        dependencies: Iterable["Depends"],
         middlewares: Iterable["BrokerMiddleware[MsgType]"],
-        parser: Optional["CustomParser[MsgType]"],
-        decoder: Optional["CustomDecoder[StreamMessage[MsgType]]"],
+        parser: Optional["CustomCallable"],
+        decoder: Optional["CustomCallable"],
         include_in_schema: Optional[bool],
     ) -> None:
         self.prefix = prefix
         self.include_in_schema = include_in_schema
 
         self._subscribers = {}
         self._publishers = {}
@@ -47,24 +45,27 @@
         self._middlewares = middlewares
         self._parser = parser
         self._decoder = decoder
 
     @abstractmethod
     def subscriber(
         self,
-        subscriber: SubscriberProto[MsgType],
-    ) -> SubscriberProto[MsgType]:
+        subscriber: "SubscriberProto[MsgType]",
+    ) -> "SubscriberProto[MsgType]":
         subscriber.add_prefix(self.prefix)
         key = hash(subscriber)
         subscriber = self._subscribers.get(key, subscriber)
         self._subscribers = {**self._subscribers, key: subscriber}
         return subscriber
 
     @abstractmethod
-    def publisher(self, publisher: PublisherProto[MsgType]) -> PublisherProto[MsgType]:
+    def publisher(
+        self,
+        publisher: "PublisherProto[MsgType]",
+    ) -> "PublisherProto[MsgType]":
         publisher.add_prefix(self.prefix)
         key = hash(publisher)
         publisher = self._publishers.get(key, publisher)
         self._publishers = {**self._publishers, key: publisher}
         return publisher
 
     def include_router(self, router: "ABCBroker[Any]") -> None:
```

### Comparing `faststream-0.5.0rc0/faststream/broker/core/logging.py` & `faststream-0.5.0rc1/faststream/broker/core/logging.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         raise NotImplementedError()
 
     def __init__(
         self,
         *args: Any,
         default_logger: Annotated[
             logging.Logger,
-            Doc("Logger object to use if `logger` is not setted."),
+            Doc("Logger object to use if `logger` is not set."),
         ],
         logger: Annotated[
             Union["LoggerProto", None, object],
             Doc("User specified logger to pass into Context and log service messages."),
         ],
         log_level: Annotated[
             int,
```

### Comparing `faststream-0.5.0rc0/faststream/broker/core/usecase.py` & `faststream-0.5.0rc1/faststream/broker/core/usecase.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,72 +5,70 @@
     TYPE_CHECKING,
     Any,
     Callable,
     Generic,
     Iterable,
     List,
     Optional,
+    Sequence,
     Type,
     Union,
     cast,
 )
 
 from typing_extensions import Annotated, Doc, Self
 
 from faststream._compat import is_test_env
 from faststream.broker.core.logging import LoggingBroker
 from faststream.broker.middlewares.logging import CriticalLogMiddleware
 from faststream.broker.proto import SetupAble
-from faststream.broker.publisher.proto import ProducerProto, PublisherProto
 from faststream.broker.subscriber.proto import SubscriberProto
 from faststream.broker.types import (
-    AsyncCustomDecoder,
-    AsyncCustomParser,
+    AsyncCustomCallable,
     BrokerMiddleware,
     ConnectionType,
-    CustomDecoder,
-    CustomParser,
+    CustomCallable,
     MsgType,
 )
 from faststream.exceptions import NOT_CONNECTED_YET
 from faststream.log.logging import set_logger_fmt
 from faststream.utils.context.repository import context
 from faststream.utils.functions import to_async
 
 if TYPE_CHECKING:
     from types import TracebackType
 
     from fast_depends.dependencies import Depends
 
     from faststream.asyncapi.schema import Tag, TagDict
-    from faststream.broker.message import StreamMessage
+    from faststream.broker.publisher.proto import ProducerProto, PublisherProto
     from faststream.security import BaseSecurity
     from faststream.types import AnyDict, LoggerProto
 
 
 class BrokerUsecase(
     LoggingBroker[MsgType],
     SetupAble,
     Generic[MsgType, ConnectionType],
 ):
     """A class representing a broker async use case."""
 
-    url: Union[str, Iterable[str], None]
+    url: Union[str, Sequence[str]]
     _connection: Optional[ConnectionType]
-    _producer: Optional[ProducerProto]
+    _producer: Optional["ProducerProto"]
 
     def __init__(
         self,
         *,
         decoder: Annotated[
-            Optional["CustomDecoder[StreamMessage[MsgType]]"],
+            Optional["CustomCallable"],
             Doc("Custom decoder object."),
         ],
         parser: Annotated[
-            Optional["CustomParser[MsgType]"],
+            Optional["CustomCallable"],
             Doc("Custom parser object."),
         ],
         dependencies: Annotated[
             Iterable["Depends"],
             Doc("Dependencies to apply to all broker subscribers."),
         ],
         middlewares: Annotated[
@@ -82,15 +80,15 @@
             Doc(
                 "Graceful shutdown timeout. Broker waits for all running subscribers completion before shut down."
             ),
         ],
         # Logging args
         default_logger: Annotated[
             logging.Logger,
-            Doc("Logger object to use if `logger` is not setted."),
+            Doc("Logger object to use if `logger` is not set."),
         ],
         logger: Annotated[
             Union["LoggerProto", None, object],
             Doc("User specified logger to pass into Context and log service messages."),
         ],
         log_level: Annotated[
             int,
@@ -127,34 +125,34 @@
             Doc("AsyncAPI server description."),
         ],
         tags: Annotated[
             Optional[Iterable[Union["Tag", "TagDict"]]],
             Doc("AsyncAPI server tags."),
         ],
         asyncapi_url: Annotated[
-            Union[str, List[str], None],
+            Union[str, List[str]],
             Doc("AsyncAPI hardcoded server addresses."),
         ],
         security: Annotated[
             Optional["BaseSecurity"],
             Doc(
                 "Security options to connect broker and generate AsyncAPI server security."
             ),
         ],
         **connection_kwargs: Any,
     ) -> None:
         super().__init__(
             middlewares=middlewares,
             dependencies=dependencies,
             decoder=cast(
-                Optional["AsyncCustomDecoder[StreamMessage[MsgType]]"],
+                Optional["AsyncCustomCallable"],
                 to_async(decoder) if decoder else None,
             ),
             parser=cast(
-                Optional["AsyncCustomParser[MsgType]"],
+                Optional["AsyncCustomCallable"],
                 to_async(parser) if parser else None,
             ),
             # Broker is a root router
             include_in_schema=True,
             prefix="",
             # Logging args
             default_logger=default_logger,
@@ -240,15 +238,15 @@
             _get_dependant=self._get_dependant,
             **self._subscriber_setup_extra,
             **kwargs,
         )
 
     def setup_publisher(
         self,
-        publisher: PublisherProto[MsgType],
+        publisher: "PublisherProto[MsgType]",
         **kwargs: Any,
     ) -> None:
         """Setup the Publisher to prepare it to starting."""
         publisher.setup(
             producer=self._producer,
             **self._publisher_setup_extra,
             **kwargs,
@@ -258,15 +256,15 @@
     def _subscriber_setup_extra(self) -> "AnyDict":
         return {}
 
     @property
     def _publisher_setup_extra(self) -> "AnyDict":
         return {}
 
-    def publisher(self, *args: Any, **kwargs: Any) -> PublisherProto[MsgType]:
+    def publisher(self, *args: Any, **kwargs: Any) -> "PublisherProto[MsgType]":
         pub = super().publisher(*args, **kwargs)
         if self.running:
             self.setup_publisher(pub)
         return pub
 
     def _abc_start(self) -> None:
         for h in self._subscribers.values():
@@ -321,15 +319,15 @@
         """Close the object."""
         self._connection = None
 
     async def publish(
         self,
         msg: Any,
         *,
-        producer: Optional[ProducerProto],
+        producer: Optional["ProducerProto"],
         **kwargs: Any,
     ) -> Optional[Any]:
         """Publish message directly."""
         assert producer, NOT_CONNECTED_YET  # nosec B101
 
         async with AsyncExitStack() as stack:
             for m in self._middlewares:
```

### Comparing `faststream-0.5.0rc0/faststream/broker/fastapi/context.py` & `faststream-0.5.0rc1/faststream/broker/fastapi/context.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/faststream/broker/fastapi/get_dependant.py` & `faststream-0.5.0rc1/faststream/broker/fastapi/get_dependant.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-from typing import Any, Callable, Iterable, cast
+from typing import TYPE_CHECKING, Any, Callable, Iterable, cast
 
-from fastapi import params
-from fastapi.dependencies.models import Dependant
 from fastapi.dependencies.utils import get_dependant, get_parameterless_sub_dependant
 
 from faststream._compat import PYDANTIC_V2
 
+if TYPE_CHECKING:
+    from fastapi import params
+    from fastapi.dependencies.models import Dependant
+
 
 def get_fastapi_dependant(
     orig_call: Callable[..., Any],
-    dependencies: Iterable[params.Depends],
+    dependencies: Iterable["params.Depends"],
     path_name: str = "",
 ) -> Any:
     """Generate FastStream-Compatible FastAPI Dependant object."""
     dependent = get_fastapi_native_dependant(
         orig_call=orig_call,
         dependencies=dependencies,
         path_name=path_name,
@@ -22,15 +24,15 @@
     dependent = _patch_fastapi_dependent(dependent)
 
     return dependent
 
 
 def get_fastapi_native_dependant(
     orig_call: Callable[..., Any],
-    dependencies: Iterable[params.Depends],
+    dependencies: Iterable["params.Depends"],
     path_name: str = "",
 ) -> Any:
     """Generate native FastAPI Dependant."""
     dependent = get_dependant(
         path=path_name,
         call=orig_call,
     )
@@ -40,15 +42,15 @@
             0,
             get_parameterless_sub_dependant(depends=depends, path=path_name),
         )
 
     return dependent
 
 
-def _patch_fastapi_dependent(dependant: Dependant) -> Dependant:
+def _patch_fastapi_dependent(dependant: "Dependant") -> "Dependant":
     """Patch FastAPI by adding fields for AsyncAPI schema generation."""
     from pydantic import Field, create_model  # FastAPI always has pydantic
 
     from faststream._compat import PydanticUndefined
 
     params = dependant.query_params + dependant.body_params  # type: ignore[attr-defined]
```

### Comparing `faststream-0.5.0rc0/faststream/broker/fastapi/route.py` & `faststream-0.5.0rc1/faststream/broker/fastapi/route.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,53 +11,56 @@
     Generic,
     Iterable,
     List,
     Optional,
     Union,
 )
 
-from fastapi import params
-from fastapi.background import BackgroundTasks
-from fastapi.dependencies.models import Dependant
 from fastapi.dependencies.utils import solve_dependencies
 from fastapi.routing import run_endpoint_function, serialize_response
 from fastapi.utils import create_response_field
 from starlette.requests import Request
 from starlette.routing import BaseRoute
 
 from faststream._compat import FASTAPI_V106, raise_fastapi_validation_error
-from faststream.broker.core.usecase import BrokerUsecase
 from faststream.broker.fastapi.get_dependant import get_fastapi_native_dependant
-from faststream.broker.message import StreamMessage as NativeMessage
-from faststream.broker.schemas import NameRequired
 from faststream.broker.types import MsgType, P_HandlerParams, T_HandlerReturn
 from faststream.broker.wrapper.call import HandlerCallWrapper
-from faststream.types import AnyDict
 
 if TYPE_CHECKING:
+    from fastapi import params
     from fastapi._compat import ModelField
+    from fastapi.dependencies.models import Dependant
     from fastapi.types import IncEx
 
+    from faststream.broker.core.usecase import BrokerUsecase
+    from faststream.broker.message import StreamMessage as NativeMessage
+    from faststream.broker.schemas import NameRequired
+    from faststream.types import AnyDict
 
-class StreamRoute(BaseRoute, Generic[MsgType, P_HandlerParams, T_HandlerReturn]):
+
+class StreamRoute(
+    BaseRoute,  # type: ignore[misc]
+    Generic[MsgType, P_HandlerParams, T_HandlerReturn],
+):
     """A class representing a stream route."""
 
-    handler: HandlerCallWrapper[MsgType, P_HandlerParams, T_HandlerReturn]
+    handler: "HandlerCallWrapper[MsgType, P_HandlerParams, T_HandlerReturn]"
 
     def __init__(
         self,
-        path: Union[NameRequired, str, None],
+        path: Union["NameRequired", str, None],
         *extra: Any,
         provider_factory: Callable[[], Any],
         endpoint: Union[
             Callable[P_HandlerParams, T_HandlerReturn],
-            HandlerCallWrapper[MsgType, P_HandlerParams, T_HandlerReturn],
+            "HandlerCallWrapper[MsgType, P_HandlerParams, T_HandlerReturn]",
         ],
-        broker: BrokerUsecase[MsgType, Any],
-        dependencies: Iterable[params.Depends],
+        broker: "BrokerUsecase[MsgType, Any]",
+        dependencies: Iterable["params.Depends"],
         response_model: Any,
         response_model_include: Optional["IncEx"],
         response_model_exclude: Optional["IncEx"],
         response_model_by_alias: bool,
         response_model_exclude_unset: bool,
         response_model_exclude_defaults: bool,
         response_model_exclude_none: bool,
@@ -110,56 +113,57 @@
         else:
             handler = call
 
         self.handler = broker.subscriber(  # type: ignore[assignment,call-arg]
             *extra,
             dependencies=list(dependencies),
             **handle_kwargs,
-        )(handler)
+        )(
+            handler,  # type: ignore[arg-type]
+        )
 
 
-class StreamMessage(Request):
+class StreamMessage(Request):  # type: ignore[misc]
     """A class to represent a stream message."""
 
-    scope: AnyDict
-    _cookies: AnyDict
-    _headers: AnyDict  # type: ignore
-    _body: Union[AnyDict, List[Any]]  # type: ignore
-    _query_params: AnyDict  # type: ignore
-    _background: Optional[BackgroundTasks]
+    scope: "AnyDict"
+    _cookies: "AnyDict"
+    _headers: "AnyDict"  # type: ignore
+    _body: Union["AnyDict", List[Any]]  # type: ignore
+    _query_params: "AnyDict"  # type: ignore
 
     def __init__(
         self,
         *,
-        body: Union[AnyDict, List[Any]],
-        headers: AnyDict,
-        path: AnyDict,
+        body: Union["AnyDict", List[Any]],
+        headers: "AnyDict",
+        path: "AnyDict",
     ) -> None:
         """Initialize a class instance."""
         self._headers = headers
         self._body = body
         self._query_params = path
 
         self.scope = {"path_params": self._query_params}
         self._cookies = {}
 
     @classmethod
     def get_consumer(
         cls,
         *,
-        dependent: Dependant,
+        dependent: "Dependant",
         provider_factory: Callable[[], Any],
         response_field: Optional["ModelField"],
         response_model_include: Optional["IncEx"],
         response_model_exclude: Optional["IncEx"],
         response_model_by_alias: bool,
         response_model_exclude_unset: bool,
         response_model_exclude_defaults: bool,
         response_model_exclude_none: bool,
-    ) -> Callable[[NativeMessage[Any]], Awaitable[Any]]:
+    ) -> Callable[["NativeMessage[Any]"], Awaitable[Any]]:
         """Creates a session for handling requests."""
         assert dependent.call  # nosec B101
 
         consume = make_fastapi_execution(
             dependent=dependent,
             provider_factory=provider_factory,
             response_field=response_field,
@@ -177,19 +181,19 @@
             dropwhile(
                 lambda i: i in dependencies_names,
                 inspect.signature(dependent.call).parameters,
             ),
             None,
         )
 
-        async def real_consumer(message: NativeMessage[Any]) -> Any:
+        async def real_consumer(message: "NativeMessage[Any]") -> Any:
             """An asynchronous function that processes an incoming message and returns a sendable message."""
             body = message.decoded_body
 
-            fastapi_body: Union[AnyDict, List[Any]]
+            fastapi_body: Union["AnyDict", List[Any]]
             if first_arg is not None:
                 if isinstance(body, dict):
                     path = fastapi_body = body or {}
                 elif isinstance(body, list):
                     fastapi_body, path = body, {}
                 else:
                     path = fastapi_body = {first_arg: body}
@@ -211,33 +215,33 @@
 
         real_consumer.__consumer__ = True  # type: ignore[attr-defined]
         return real_consumer
 
 
 def make_fastapi_execution(
     *,
-    dependent: Dependant,
+    dependent: "Dependant",
     provider_factory: Callable[[], Any],
     response_field: Optional["ModelField"],
     response_model_include: Optional["IncEx"],
     response_model_exclude: Optional["IncEx"],
     response_model_by_alias: bool,
     response_model_exclude_unset: bool,
     response_model_exclude_defaults: bool,
     response_model_exclude_none: bool,
 ) -> Callable[
-    [StreamMessage, NativeMessage[Any]],
+    [StreamMessage, "NativeMessage[Any]"],
     Awaitable[Any],
 ]:
     """Creates a FastAPI application."""
     is_coroutine = asyncio.iscoroutinefunction(dependent.call)
 
     async def app(
         request: StreamMessage,
-        raw_message: NativeMessage[Any],
+        raw_message: "NativeMessage[Any]",
     ) -> Any:
         """Consume StreamMessage and return user function result."""
         async with AsyncExitStack() as stack:
             if FASTAPI_V106:
                 kwargs = {"async_exit_stack": stack}
             else:
                 request.scope["fastapi_astack"] = stack
```

### Comparing `faststream-0.5.0rc0/faststream/broker/fastapi/router.py` & `faststream-0.5.0rc1/faststream/broker/fastapi/router.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 from abc import abstractmethod
 from contextlib import asynccontextmanager
 from enum import Enum
-from types import TracebackType
 from typing import (
+    TYPE_CHECKING,
     Any,
     AsyncIterator,
     Awaitable,
     Callable,
     Dict,
     Generic,
     Iterable,
@@ -18,108 +18,117 @@
     Type,
     Union,
     cast,
     overload,
 )
 from weakref import WeakSet
 
-from fastapi import APIRouter, FastAPI, params
 from fastapi.background import BackgroundTasks
 from fastapi.datastructures import Default
 from fastapi.responses import HTMLResponse
-from fastapi.routing import APIRoute
-from fastapi.types import IncEx
+from fastapi.routing import APIRoute, APIRouter
 from fastapi.utils import generate_unique_id
-from starlette import routing
 from starlette.responses import JSONResponse, Response
 from starlette.routing import BaseRoute, _DefaultLifespan
-from starlette.types import ASGIApp, AppType, Lifespan
 
-from faststream.asyncapi import schema as asyncapi
-from faststream.asyncapi.schema import Schema
 from faststream.asyncapi.site import get_asyncapi_html
-from faststream.broker.core.usecase import BrokerUsecase
 from faststream.broker.fastapi.get_dependant import get_fastapi_dependant
 from faststream.broker.fastapi.route import StreamRoute
 from faststream.broker.middlewares import BaseMiddleware
-from faststream.broker.publisher.proto import PublisherProto
-from faststream.broker.schemas import NameRequired
 from faststream.broker.types import (
-    BrokerMiddleware,
     MsgType,
     P_HandlerParams,
     T_HandlerReturn,
 )
-from faststream.broker.wrapper.call import HandlerCallWrapper
-from faststream.broker.wrapper.proto import WrapperProto
-from faststream.types import AnyDict
 from faststream.utils.context.repository import context
 from faststream.utils.functions import to_async
 
+if TYPE_CHECKING:
+    from types import TracebackType
+
+    from fastapi import FastAPI, params
+    from fastapi.types import IncEx
+    from starlette import routing
+    from starlette.types import ASGIApp, AppType, Lifespan
+
+    from faststream.asyncapi import schema as asyncapi
+    from faststream.asyncapi.schema import Schema
+    from faststream.broker.core.usecase import BrokerUsecase
+    from faststream.broker.publisher.proto import PublisherProto
+    from faststream.broker.schemas import NameRequired
+    from faststream.broker.types import BrokerMiddleware
+    from faststream.broker.wrapper.call import HandlerCallWrapper
+    from faststream.types import AnyDict
+
 
 class _BackgroundMiddleware(BaseMiddleware):
     async def after_processed(
         self,
         exc_type: Optional[Type[BaseException]] = None,
         exc_val: Optional[BaseException] = None,
-        exc_tb: Optional[TracebackType] = None,
+        exc_tb: Optional["TracebackType"] = None,
     ) -> Optional[bool]:
         if not exc_type and (
-            background := cast(
+            background := cast(  # type: ignore[redundant-cast]
                 Optional[BackgroundTasks],
                 getattr(context.get_local("message"), "background", None),
             )
         ):
             await background()
 
         return await super().after_processed(exc_type, exc_val, exc_tb)
 
 
-class StreamRouter(APIRouter, Generic[MsgType]):
+class StreamRouter(
+    APIRouter,  # type: ignore[misc]
+    Generic[MsgType],
+):
     """A class to route streams."""
 
-    broker_class: Type[BrokerUsecase[MsgType, Any]]
-    broker: BrokerUsecase[MsgType, Any]
+    broker_class: Type["BrokerUsecase[MsgType, Any]"]
+    broker: "BrokerUsecase[MsgType, Any]"
     docs_router: Optional[APIRouter]
     _after_startup_hooks: List[Callable[[Any], Awaitable[Optional[Mapping[str, Any]]]]]
     _on_shutdown_hooks: List[Callable[[Any], Awaitable[None]]]
-    schema: Optional[Schema]
+    schema: Optional["Schema"]
 
     title: str
     description: str
     version: str
-    license: Optional[AnyDict]
-    contact: Optional[AnyDict]
+    license: Optional["AnyDict"]
+    contact: Optional["AnyDict"]
 
     def __init__(
         self,
         *connection_args: Any,
-        middlewares: Iterable[BrokerMiddleware[MsgType]] = (),
+        middlewares: Iterable["BrokerMiddleware[MsgType]"] = (),
         prefix: str = "",
         tags: Optional[List[Union[str, Enum]]] = None,
-        dependencies: Optional[Sequence[params.Depends]] = None,
-        default_response_class: Type[Response] = Default(JSONResponse),
-        responses: Optional[Dict[Union[int, str], AnyDict]] = None,
-        callbacks: Optional[List[routing.BaseRoute]] = None,
-        routes: Optional[List[routing.BaseRoute]] = None,
+        dependencies: Optional[Sequence["params.Depends"]] = None,
+        default_response_class: Type["Response"] = Default(JSONResponse),
+        responses: Optional[Dict[Union[int, str], "AnyDict"]] = None,
+        callbacks: Optional[List["routing.BaseRoute"]] = None,
+        routes: Optional[List["routing.BaseRoute"]] = None,
         redirect_slashes: bool = True,
-        default: Optional[ASGIApp] = None,
+        default: Optional["ASGIApp"] = None,
         dependency_overrides_provider: Optional[Any] = None,
-        route_class: Type[APIRoute] = APIRoute,
+        route_class: Type["APIRoute"] = APIRoute,
         on_startup: Optional[Sequence[Callable[[], Any]]] = None,
         on_shutdown: Optional[Sequence[Callable[[], Any]]] = None,
         deprecated: Optional[bool] = None,
         include_in_schema: bool = True,
         setup_state: bool = True,
-        lifespan: Optional[Lifespan[Any]] = None,
-        generate_unique_id_function: Callable[[APIRoute], str] = Default(
+        lifespan: Optional["Lifespan[Any]"] = None,
+        generate_unique_id_function: Callable[["APIRoute"], str] = Default(
             generate_unique_id
         ),
         # AsyncAPI information
-        asyncapi_tags: Optional[Iterable[Union[asyncapi.Tag, asyncapi.TagDict]]] = None,
+        asyncapi_tags: Optional[
+            Iterable[Union["asyncapi.Tag", "asyncapi.TagDict"]]
+        ] = None,
         schema_url: Optional[str] = "/asyncapi",
         **connection_kwars: Any,
     ) -> None:
         assert (  # nosec B101
             self.broker_class
         ), "You should specify `broker_class` at your implementation"
 
@@ -189,27 +198,27 @@
         if self.dependency_overrides_provider is not None:
             return self.dependency_overrides_provider
         else:
             return next(iter(self.weak_dependencies_provider), None)
 
     def _add_api_mq_route(
         self,
-        path: Union[NameRequired, str],
-        *extra: Union[NameRequired, str],
+        path: Union["NameRequired", str],
+        *extra: Union["NameRequired", str],
         endpoint: Callable[P_HandlerParams, T_HandlerReturn],
-        dependencies: Iterable[params.Depends],
+        dependencies: Iterable["params.Depends"],
         response_model: Any,
-        response_model_include: Optional[IncEx],
-        response_model_exclude: Optional[IncEx],
+        response_model_include: Optional["IncEx"],
+        response_model_exclude: Optional["IncEx"],
         response_model_by_alias: bool,
         response_model_exclude_unset: bool,
         response_model_exclude_defaults: bool,
         response_model_exclude_none: bool,
         **broker_kwargs: Any,
-    ) -> HandlerCallWrapper[MsgType, P_HandlerParams, T_HandlerReturn]:
+    ) -> "HandlerCallWrapper[MsgType, P_HandlerParams, T_HandlerReturn]":
         """Add an API message queue route."""
         route = StreamRoute[MsgType, P_HandlerParams, T_HandlerReturn](
             path,
             *extra,
             endpoint=endpoint,
             dependencies=(*self.dependencies, *dependencies),
             provider_factory=self._get_dependencies_overides_provider,
@@ -224,31 +233,34 @@
             **broker_kwargs,
         )
         self.routes.append(route)
         return route.handler
 
     def subscriber(
         self,
-        path: Union[str, NameRequired],
-        *extra: Union[NameRequired, str],
-        dependencies: Iterable[params.Depends],
+        path: Union[str, "NameRequired"],
+        *extra: Union["NameRequired", str],
+        dependencies: Iterable["params.Depends"],
         response_model: Any,
-        response_model_include: Optional[IncEx],
-        response_model_exclude: Optional[IncEx],
+        response_model_include: Optional["IncEx"],
+        response_model_exclude: Optional["IncEx"],
         response_model_by_alias: bool,
         response_model_exclude_unset: bool,
         response_model_exclude_defaults: bool,
         response_model_exclude_none: bool,
         **broker_kwargs: Any,
-    ) -> WrapperProto[MsgType]:
+    ) -> Callable[
+        [Callable[P_HandlerParams, T_HandlerReturn]],
+        "HandlerCallWrapper[MsgType, P_HandlerParams, T_HandlerReturn]",
+    ]:
         """A function decorator for subscribing to a message queue."""
 
         def decorator(
             func: Callable[P_HandlerParams, T_HandlerReturn],
-        ) -> HandlerCallWrapper[MsgType, P_HandlerParams, T_HandlerReturn]:
+        ) -> "HandlerCallWrapper[MsgType, P_HandlerParams, T_HandlerReturn]":
             """A decorator function."""
             return self._add_api_mq_route(
                 path,
                 *extra,
                 endpoint=func,
                 dependencies=dependencies,
                 response_model=response_model,
@@ -259,43 +271,46 @@
                 response_model_exclude_defaults=response_model_exclude_defaults,
                 response_model_exclude_none=response_model_exclude_none,
                 **broker_kwargs,
             )
 
         return decorator
 
-    def _wrap_lifespan(self, lifespan: Optional[Lifespan[Any]] = None) -> Lifespan[Any]:
+    def _wrap_lifespan(
+        self, lifespan: Optional["Lifespan[Any]"] = None
+    ) -> "Lifespan[Any]":
         lifespan_context = lifespan if lifespan is not None else _DefaultLifespan(self)
 
         @asynccontextmanager
         async def start_broker_lifespan(
-            app: FastAPI,
+            app: "FastAPI",
         ) -> AsyncIterator[Mapping[str, Any]]:
             """Starts the lifespan of a broker."""
             if not len(self.weak_dependencies_provider):
                 self.weak_dependencies_provider.add(app)
 
             if self.docs_router:
                 self.title = app.title
                 self.description = app.description
                 self.version = app.version
                 self.contact = app.contact
                 self.license = app.license_info
 
                 from faststream.asyncapi.generate import get_app_schema
+
                 self.schema = get_app_schema(self)
 
                 app.include_router(self.docs_router)
 
             if not len(self.weak_dependencies_provider):
                 self.weak_dependencies_provider.add(app)
 
             async with lifespan_context(app) as maybe_context:
                 if maybe_context is None:
-                    context: AnyDict = {}
+                    context: "AnyDict" = {}
                 else:
                     context = dict(maybe_context)
 
                 context.update({"broker": self.broker})
                 await self.broker.start()
 
                 for h in self._after_startup_hooks:
@@ -317,81 +332,81 @@
                     await self.broker.close()
 
         return start_broker_lifespan
 
     @overload
     def after_startup(
         self,
-        func: Callable[[AppType], Mapping[str, Any]],
-    ) -> Callable[[AppType], Mapping[str, Any]]: ...
+        func: Callable[["AppType"], Mapping[str, Any]],
+    ) -> Callable[["AppType"], Mapping[str, Any]]: ...
 
     @overload
     def after_startup(
         self,
-        func: Callable[[AppType], Awaitable[Mapping[str, Any]]],
-    ) -> Callable[[AppType], Awaitable[Mapping[str, Any]]]: ...
+        func: Callable[["AppType"], Awaitable[Mapping[str, Any]]],
+    ) -> Callable[["AppType"], Awaitable[Mapping[str, Any]]]: ...
 
     @overload
     def after_startup(
         self,
-        func: Callable[[AppType], None],
-    ) -> Callable[[AppType], None]: ...
+        func: Callable[["AppType"], None],
+    ) -> Callable[["AppType"], None]: ...
 
     @overload
     def after_startup(
         self,
-        func: Callable[[AppType], Awaitable[None]],
-    ) -> Callable[[AppType], Awaitable[None]]: ...
+        func: Callable[["AppType"], Awaitable[None]],
+    ) -> Callable[["AppType"], Awaitable[None]]: ...
 
     def after_startup(
         self,
         func: Union[
-            Callable[[AppType], Mapping[str, Any]],
-            Callable[[AppType], Awaitable[Mapping[str, Any]]],
-            Callable[[AppType], None],
-            Callable[[AppType], Awaitable[None]],
+            Callable[["AppType"], Mapping[str, Any]],
+            Callable[["AppType"], Awaitable[Mapping[str, Any]]],
+            Callable[["AppType"], None],
+            Callable[["AppType"], Awaitable[None]],
         ],
     ) -> Union[
-        Callable[[AppType], Mapping[str, Any]],
-        Callable[[AppType], Awaitable[Mapping[str, Any]]],
-        Callable[[AppType], None],
-        Callable[[AppType], Awaitable[None]],
+        Callable[["AppType"], Mapping[str, Any]],
+        Callable[["AppType"], Awaitable[Mapping[str, Any]]],
+        Callable[["AppType"], None],
+        Callable[["AppType"], Awaitable[None]],
     ]:
         """Register a function to be executed after startup."""
         self._after_startup_hooks.append(to_async(func))  # type: ignore
         return func
 
     @overload
     def on_broker_shutdown(
         self,
-        func: Callable[[AppType], None],
-    ) -> Callable[[AppType], None]: ...
+        func: Callable[["AppType"], None],
+    ) -> Callable[["AppType"], None]: ...
 
     @overload
     def on_broker_shutdown(
         self,
-        func: Callable[[AppType], Awaitable[None]],
-    ) -> Callable[[AppType], Awaitable[None]]: ...
+        func: Callable[["AppType"], Awaitable[None]],
+    ) -> Callable[["AppType"], Awaitable[None]]: ...
 
     def on_broker_shutdown(
         self,
         func: Union[
-            Callable[[AppType], None],
-            Callable[[AppType], Awaitable[None]],
+            Callable[["AppType"], None],
+            Callable[["AppType"], Awaitable[None]],
         ],
     ) -> Union[
-        Callable[[AppType], None],
-        Callable[[AppType], Awaitable[None]],
+        Callable[["AppType"], None],
+        Callable[["AppType"], Awaitable[None]],
     ]:
         """Register a function to be executed before broker stop."""
         self._on_shutdown_hooks.append(to_async(func))  # type: ignore
         return func
 
     @abstractmethod
-    def publisher(self) -> PublisherProto[MsgType]:
+    def publisher(self) -> "PublisherProto[MsgType]":
         """Create Publisher object."""
         raise NotImplementedError()
 
     def _asyncapi_router(self, schema_url: Optional[str]) -> Optional[APIRouter]:
         """Creates an API router for serving AsyncAPI documentation."""
         if not self.include_in_schema or not schema_url:
             return None
@@ -462,21 +477,21 @@
 
     def include_router(
         self,
         router: "APIRouter",
         *,
         prefix: str = "",
         tags: Optional[List[Union[str, Enum]]] = None,
-        dependencies: Optional[Sequence[params.Depends]] = None,
+        dependencies: Optional[Sequence["params.Depends"]] = None,
         default_response_class: Type[Response] = Default(JSONResponse),
-        responses: Optional[Dict[Union[int, str], AnyDict]] = None,
-        callbacks: Optional[List[BaseRoute]] = None,
+        responses: Optional[Dict[Union[int, str], "AnyDict"]] = None,
+        callbacks: Optional[List["BaseRoute"]] = None,
         deprecated: Optional[bool] = None,
         include_in_schema: bool = True,
-        generate_unique_id_function: Callable[[APIRoute], str] = Default(
+        generate_unique_id_function: Callable[["APIRoute"], str] = Default(
             generate_unique_id
         ),
     ) -> None:
         """Includes a router in the API."""
         if isinstance(router, StreamRouter):  # pragma: no branch
             self.broker.include_router(router.broker)
             router.weak_dependencies_provider = self.weak_dependencies_provider
```

### Comparing `faststream-0.5.0rc0/faststream/broker/middlewares/base.py` & `faststream-0.5.0rc1/faststream/broker/middlewares/base.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/faststream/broker/middlewares/logging.py` & `faststream-0.5.0rc1/faststream/broker/middlewares/logging.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,50 +1,54 @@
 import logging
-from types import TracebackType
-from typing import Any, Optional, Type
+from typing import TYPE_CHECKING, Any, Optional, Type
 
 from typing_extensions import Self
 
 from faststream.broker.middlewares.base import BaseMiddleware
 from faststream.exceptions import IgnoredException
-from faststream.types import DecodedMessage, LoggerProto
 from faststream.utils.context.repository import context
 
+if TYPE_CHECKING:
+    from types import TracebackType
+
+    from faststream.types import DecodedMessage, LoggerProto
+
 
 class CriticalLogMiddleware(BaseMiddleware):
     """A middleware class for logging critical errors."""
 
     def __init__(
         self,
-        logger: Optional[LoggerProto],
+        logger: Optional["LoggerProto"],
         log_level: int,
     ) -> None:
         """Initialize the class."""
         self.logger = logger
         self.log_level = log_level
 
-    def __call__(self, *args: Any) -> Self:
+    def __call__(self, msg: Optional[Any]) -> Self:
         """Call the object with a message."""
+        self.msg = msg
         return self
 
     async def on_consume(
         self,
-        msg: Optional[DecodedMessage],
-    ) -> Optional[DecodedMessage]:
+        msg: Optional["DecodedMessage"],
+    ) -> Optional["DecodedMessage"]:
         if self.logger is not None:
             c = context.get_local("log_context") or {}
             self.logger.log(self.log_level, "Received", extra=c)
 
         return await super().on_consume(msg)
 
     async def after_processed(
         self,
         exc_type: Optional[Type[BaseException]] = None,
         exc_val: Optional[BaseException] = None,
-        exc_tb: Optional[TracebackType] = None,
+        exc_tb: Optional["TracebackType"] = None,
     ) -> bool:
         """Asynchronously called after processing."""
         if self.logger is not None:
             c = context.get_local("log_context") or {}
 
             if exc_type:
                 if issubclass(exc_type, IgnoredException):
```

### Comparing `faststream-0.5.0rc0/faststream/broker/publisher/fake.py` & `faststream-0.5.0rc1/faststream/broker/publisher/fake.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 from contextlib import AsyncExitStack
 from itertools import chain
-from typing import Any, Awaitable, Callable, Iterable, Optional
+from typing import TYPE_CHECKING, Any, Awaitable, Callable, Iterable, Optional
 
 from faststream.broker.publisher.proto import BasePublisherProto
-from faststream.broker.types import PublisherMiddleware
-from faststream.types import AnyDict, SendableMessage
+
+if TYPE_CHECKING:
+    from faststream.broker.types import PublisherMiddleware
+    from faststream.types import AnyDict, SendableMessage
 
 
 class FakePublisher(BasePublisherProto):
     """Publisher Interface implementation to use as RPC or REPLY TO publisher."""
 
     def __init__(
         self,
-        method: Callable[..., Awaitable[SendableMessage]],
+        method: Callable[..., Awaitable["SendableMessage"]],
         *,
-        publish_kwargs: AnyDict,
-        middlewares: Iterable[PublisherMiddleware] = (),
+        publish_kwargs: "AnyDict",
+        middlewares: Iterable["PublisherMiddleware"] = (),
     ) -> None:
         """Initialize an object."""
         self.method = method
         self.publish_kwargs = publish_kwargs
         self.middlewares = middlewares
 
     async def publish(
         self,
-        message: SendableMessage,
+        message: "SendableMessage",
         *,
         correlation_id: Optional[str] = None,
-        _extra_middlewares: Iterable[PublisherMiddleware] = (),
+        _extra_middlewares: Iterable["PublisherMiddleware"] = (),
         **kwargs: Any,
     ) -> Any:
         """Publish a message."""
         publish_kwargs = {
             "correlation_id": correlation_id,
             **self.publish_kwargs,
             **kwargs,
         }
 
         async with AsyncExitStack() as stack:
             for m in chain(_extra_middlewares, self.middlewares):
-                message = await stack.enter_async_context(
-                    m(message, **publish_kwargs)
-                )
+                message = await stack.enter_async_context(m(message, **publish_kwargs))
 
             return await self.method(message, **publish_kwargs)
```

### Comparing `faststream-0.5.0rc0/faststream/broker/publisher/proto.py` & `faststream-0.5.0rc1/faststream/broker/publisher/proto.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,77 +1,77 @@
 from abc import abstractmethod
-from typing import Any, Callable, Generic, Iterable, Optional, Protocol
+from typing import TYPE_CHECKING, Any, Callable, Generic, Iterable, Optional, Protocol
 
 from typing_extensions import override
 
 from faststream.asyncapi.proto import AsyncAPIProto
 from faststream.broker.proto import EndpointProto
-from faststream.broker.types import (
-    BrokerMiddleware,
-    MsgType,
-    P_HandlerParams,
-    PublisherMiddleware,
-    T_HandlerReturn,
-)
-from faststream.types import SendableMessage
+from faststream.broker.types import MsgType
+
+if TYPE_CHECKING:
+    from faststream.broker.types import (
+        BrokerMiddleware,
+        P_HandlerParams,
+        PublisherMiddleware,
+        T_HandlerReturn,
+    )
+    from faststream.types import SendableMessage
 
 
 class ProducerProto(Protocol):
     @abstractmethod
     async def publish(
         self,
-        message: SendableMessage,
+        message: "SendableMessage",
         /,
         *,
         correlation_id: Optional[str] = None,
     ) -> Optional[Any]:
         """Publishes a message asynchronously."""
         ...
 
 
 class BasePublisherProto(Protocol):
     @abstractmethod
     async def publish(
         self,
-        message: SendableMessage,
+        message: "SendableMessage",
         /,
         *,
         correlation_id: Optional[str] = None,
-        _extra_middlewares: Iterable[PublisherMiddleware] = (),
+        _extra_middlewares: Iterable["PublisherMiddleware"] = (),
     ) -> Optional[Any]:
         """Publishes a message asynchronously."""
         ...
 
 
 class PublisherProto(
     AsyncAPIProto,
     EndpointProto,
     BasePublisherProto,
     Generic[MsgType],
 ):
     schema_: Any
 
-    _broker_middlewares: Iterable[BrokerMiddleware[MsgType]]
-    _middlewares: Iterable[PublisherMiddleware]
-    _producer: Optional[ProducerProto]
+    _broker_middlewares: Iterable["BrokerMiddleware[MsgType]"]
+    _middlewares: Iterable["PublisherMiddleware"]
+    _producer: Optional["ProducerProto"]
 
     @staticmethod
     @abstractmethod
     def create() -> "PublisherProto[MsgType]":
         """Abstract factory to create a real Publisher."""
         ...
 
     @override
     @abstractmethod
     def setup(  # type: ignore[override]
         self,
         *,
-        producer: Optional[ProducerProto],
-    ) -> None:
-        ...
+        producer: Optional["ProducerProto"],
+    ) -> None: ...
 
     @abstractmethod
     def __call__(
         self,
-        func: Callable[P_HandlerParams, T_HandlerReturn],
-    ) -> Callable[P_HandlerParams, T_HandlerReturn]:
-        ...
+        func: "Callable[P_HandlerParams, T_HandlerReturn]",
+    ) -> "Callable[P_HandlerParams, T_HandlerReturn]": ...
```

### Comparing `faststream-0.5.0rc0/faststream/broker/publisher/usecase.py` & `faststream-0.5.0rc1/faststream/broker/publisher/usecase.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from abc import ABC
 from inspect import unwrap
 from typing import (
+    TYPE_CHECKING,
     Any,
     Callable,
     Iterable,
     List,
     Optional,
     Tuple,
 )
@@ -13,24 +14,25 @@
 from fast_depends._compat import create_model, get_config_base
 from fast_depends.core import CallModel, build_call_model
 from typing_extensions import Annotated, Doc, override
 
 from faststream.asyncapi.abc import AsyncAPIOperation
 from faststream.asyncapi.message import get_response_schema
 from faststream.asyncapi.utils import to_camelcase
-from faststream.broker.publisher.proto import ProducerProto, PublisherProto
-from faststream.broker.types import (
-    BrokerMiddleware,
-    MsgType,
-    P_HandlerParams,
-    PublisherMiddleware,
-    T_HandlerReturn,
-)
+from faststream.broker.publisher.proto import PublisherProto
+from faststream.broker.types import MsgType, P_HandlerParams, T_HandlerReturn
 from faststream.broker.wrapper.call import HandlerCallWrapper
-from faststream.types import AnyDict
+
+if TYPE_CHECKING:
+    from faststream.broker.publisher.proto import ProducerProto
+    from faststream.broker.types import (
+        BrokerMiddleware,
+        PublisherMiddleware,
+    )
+    from faststream.types import AnyDict
 
 
 class PublisherUsecase(
     ABC,
     AsyncAPIOperation,
     PublisherProto[MsgType],
 ):
@@ -39,19 +41,19 @@
     mock: Optional[MagicMock]
     calls: List[Callable[..., Any]]
 
     def __init__(
         self,
         *,
         broker_middlewares: Annotated[
-            Iterable[BrokerMiddleware[MsgType]],
+            Iterable["BrokerMiddleware[MsgType]"],
             Doc("Top-level middlewares to use in direct `.publish` call."),
         ],
         middlewares: Annotated[
-            Iterable[PublisherMiddleware],
+            Iterable["PublisherMiddleware"],
             Doc("Publisher middlewares."),
         ],
         # AsyncAPI args
         schema_: Annotated[
             Optional[Any],
             Doc(
                 "AsyncAPI publishing message type"
@@ -85,15 +87,15 @@
         self.include_in_schema = include_in_schema
         self.schema_ = schema_
 
     @override
     def setup(  # type: ignore[override]
         self,
         *,
-        producer: Optional[ProducerProto],
+        producer: Optional["ProducerProto"],
     ) -> None:
         self._producer = producer
 
     def set_test(
         self,
         *,
         mock: Annotated[
@@ -124,16 +126,16 @@
             P_HandlerParams,
             T_HandlerReturn,
         ](func)
         handler_call._publishers.append(self)
         self.calls.append(handler_call._original_call)
         return handler_call
 
-    def get_payloads(self) -> List[Tuple[AnyDict, str]]:
-        payloads: List[Tuple[AnyDict, str]] = []
+    def get_payloads(self) -> List[Tuple["AnyDict", str]]:
+        payloads: List[Tuple["AnyDict", str]] = []
 
         if self.schema_:
             params = {"response__": (self.schema_, ...)}
 
             call_model: CallModel[Any, Any] = CallModel(
                 call=lambda: None,
                 model=create_model("Fake"),
```

### Comparing `faststream-0.5.0rc0/faststream/broker/subscriber/call_item.py` & `faststream-0.5.0rc1/faststream/broker/subscriber/call_item.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,19 +19,17 @@
 from faststream.exceptions import IgnoredException, SetupError
 
 if TYPE_CHECKING:
     from fast_depends.dependencies import Depends
 
     from faststream.broker.message import StreamMessage
     from faststream.broker.types import (
-        AsyncDecoder,
+        AsyncCallable,
         AsyncFilter,
-        AsyncParser,
-        CustomDecoder,
-        CustomParser,
+        CustomCallable,
         SubscriberMiddleware,
     )
     from faststream.broker.wrapper.call import HandlerCallWrapper
 
 
 class HandlerItem(SetupAble, Generic[MsgType]):
     """A class representing handler overloaded item."""
@@ -49,16 +47,16 @@
     dependant: Optional[Any]
 
     def __init__(
         self,
         *,
         handler: "HandlerCallWrapper[MsgType, ..., Any]",
         filter: "AsyncFilter[StreamMessage[MsgType]]",
-        item_parser: Optional["CustomParser[MsgType]"],
-        item_decoder: Optional["CustomDecoder[StreamMessage[MsgType]]"],
+        item_parser: Optional["CustomCallable"],
+        item_decoder: Optional["CustomCallable"],
         item_middlewares: Iterable["SubscriberMiddleware"],
         dependencies: Iterable["Depends"],
     ) -> None:
         self.handler = handler
         self.filter = filter
         self.item_parser = item_parser
         self.item_decoder = item_decoder
@@ -71,16 +69,16 @@
         filter_name = getattr(filter_call, "__name__", str(filter_call))
         return f"<'{self.call_name}': filter='{filter_name}'>"
 
     @override
     def setup(  # type: ignore[override]
         self,
         *,
-        parser: "AsyncParser[MsgType]",
-        decoder: "AsyncDecoder[StreamMessage[MsgType]]",
+        parser: "AsyncCallable",
+        decoder: "AsyncCallable",
         broker_dependencies: Iterable["Depends"],
         apply_types: bool,
         is_validate: bool,
         _get_dependant: Optional[Callable[..., Any]],
     ) -> None:
         if self.dependant is None:
             self.item_parser = parser
@@ -94,15 +92,17 @@
                 dependencies=dependencies,
                 _get_dependant=_get_dependant,
             )
 
             if _get_dependant is None:
                 self.dependant = dependant
             else:
-                self.dependant = _get_dependant(self.handler._original_call, dependencies)
+                self.dependant = _get_dependant(
+                    self.handler._original_call, dependencies
+                )
 
     @property
     def call_name(self) -> str:
         """Returns the name of the original call."""
         if self.handler is None:
             return ""
 
@@ -122,20 +122,16 @@
 
     async def is_suitable(
         self,
         msg: MsgType,
         cache: Dict[Any, Any],
     ) -> Optional["StreamMessage[MsgType]"]:
         """Check is message suite for current filter."""
-        if not (
-            parser := cast(Optional["AsyncParser[MsgType]"], self.item_parser)
-        ) or not (
-            decoder := cast(
-                Optional["AsyncDecoder[StreamMessage[MsgType]]"], self.item_decoder
-            )
+        if not (parser := cast(Optional["AsyncCallable"], self.item_parser)) or not (
+            decoder := cast(Optional["AsyncCallable"], self.item_decoder)
         ):
             raise SetupError("You should setup `HandlerItem` at first.")
 
         message = cache[parser] = cast(
             "StreamMessage[MsgType]", cache.get(parser) or await parser(msg)
         )
```

### Comparing `faststream-0.5.0rc0/faststream/broker/subscriber/proto.py` & `faststream-0.5.0rc1/faststream/broker/subscriber/proto.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,102 +1,96 @@
 from abc import abstractmethod
-from typing import Any, Callable, Dict, Iterable, List, Optional
+from typing import TYPE_CHECKING, Any, Callable, Dict, Iterable, List, Optional
 
-from fast_depends.dependencies import Depends
 from typing_extensions import Self, override
 
 from faststream.asyncapi.proto import AsyncAPIProto
-from faststream.broker.message import StreamMessage
 from faststream.broker.proto import EndpointProto
-from faststream.broker.publisher.proto import BasePublisherProto, ProducerProto
-from faststream.broker.subscriber.call_item import HandlerItem
-from faststream.broker.types import (
-    BrokerMiddleware,
-    CustomDecoder,
-    CustomParser,
-    Filter,
-    MsgType,
-    SubscriberMiddleware,
-)
+from faststream.broker.types import MsgType
 from faststream.broker.wrapper.proto import WrapperProto
-from faststream.types import AnyDict, LoggerProto
+
+if TYPE_CHECKING:
+    from fast_depends.dependencies import Depends
+
+    from faststream.broker.message import StreamMessage
+    from faststream.broker.publisher.proto import BasePublisherProto, ProducerProto
+    from faststream.broker.subscriber.call_item import HandlerItem
+    from faststream.broker.types import (
+        BrokerMiddleware,
+        CustomCallable,
+        Filter,
+        SubscriberMiddleware,
+    )
+    from faststream.types import AnyDict, LoggerProto
 
 
 class SubscriberProto(
     AsyncAPIProto,
     EndpointProto,
     WrapperProto[MsgType],
 ):
-    calls: List[HandlerItem[MsgType]]
+    calls: List["HandlerItem[MsgType]"]
     running: bool
 
-    _broker_dependecies: Iterable[Depends]
-    _broker_middlewares: Iterable[BrokerMiddleware[MsgType]]
-    _producer: Optional[ProducerProto]
+    _broker_dependecies: Iterable["Depends"]
+    _broker_middlewares: Iterable["BrokerMiddleware[MsgType]"]
+    _producer: Optional["ProducerProto"]
 
     @staticmethod
     @abstractmethod
     def create() -> "SubscriberProto[MsgType]":
         """Abstract factory to create a real Subscriber."""
         ...
 
     @abstractmethod
     def get_log_context(
         self,
-        msg: Optional[StreamMessage[MsgType]],
+        msg: Optional["StreamMessage[MsgType]"],
         /,
-    ) -> Dict[str, str]:
-        ...
+    ) -> Dict[str, str]: ...
 
     @override
     @abstractmethod
     def setup(  # type: ignore[override]
         self,
         *,
-        logger: Optional[LoggerProto],
+        logger: Optional["LoggerProto"],
         graceful_timeout: Optional[float],
-        broker_parser: Optional[CustomParser[MsgType]],
-        broker_decoder: Optional[CustomDecoder[StreamMessage[MsgType]]],
-        producer: Optional[ProducerProto],
-        extra_context: AnyDict,
+        broker_parser: Optional["CustomCallable"],
+        broker_decoder: Optional["CustomCallable"],
+        producer: Optional["ProducerProto"],
+        extra_context: "AnyDict",
         # FastDepends options
         apply_types: bool,
         is_validate: bool,
         _get_dependant: Optional[Callable[..., Any]],
-    ) -> None:
-        ...
+    ) -> None: ...
 
     @abstractmethod
     def _make_response_publisher(
         self,
-        message: StreamMessage[MsgType],
-    ) -> Iterable[BasePublisherProto]:
-        ...
+        message: "StreamMessage[MsgType]",
+    ) -> Iterable["BasePublisherProto"]: ...
 
     @property
     @abstractmethod
-    def call_name(self) -> str:
-        ...
+    def call_name(self) -> str: ...
 
     @abstractmethod
-    async def start(self) -> None:
-        ...
+    async def start(self) -> None: ...
 
     @abstractmethod
-    async def close(self) -> None:
-        ...
+    async def close(self) -> None: ...
 
     @abstractmethod
-    async def consume(self, msg: MsgType) -> Any:
-        ...
+    async def consume(self, msg: MsgType) -> Any: ...
 
     @abstractmethod
     def add_call(
         self,
         *,
-        filter_: "Filter[StreamMessage[MsgType]]",
-        parser_: "CustomParser[MsgType]",
-        decoder_: "CustomDecoder[StreamMessage[MsgType]]",
+        filter_: "Filter[Any]",
+        parser_: "CustomCallable",
+        decoder_: "CustomCallable",
         middlewares_: Iterable["SubscriberMiddleware"],
         dependencies_: Iterable["Depends"],
-    ) -> Self:
-        ...
+    ) -> Self: ...
```

### Comparing `faststream-0.5.0rc0/faststream/broker/subscriber/usecase.py` & `faststream-0.5.0rc1/faststream/broker/subscriber/usecase.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from typing import (
     TYPE_CHECKING,
     Any,
     AsyncIterator,
     Callable,
     ContextManager,
     Dict,
-    Generic,
     Iterable,
     List,
     Optional,
     Tuple,
     Union,
     overload,
 )
@@ -38,40 +37,38 @@
 
 if TYPE_CHECKING:
     from fast_depends.dependencies import Depends
 
     from faststream.broker.message import StreamMessage
     from faststream.broker.middlewares import BaseMiddleware
     from faststream.broker.types import (
-        AsyncDecoder,
-        AsyncParser,
+        AsyncCallable,
         BrokerMiddleware,
-        CustomDecoder,
-        CustomParser,
+        CustomCallable,
         Filter,
         SubscriberMiddleware,
     )
     from faststream.types import AnyDict, LoggerProto
 
 
-class _CallOptions(Generic[MsgType]):
+class _CallOptions:
     __slots__ = (
         "filter",
         "parser",
         "decoder",
         "middlewares",
         "dependencies",
     )
 
     def __init__(
         self,
         *,
-        filter: "Filter[StreamMessage[MsgType]]",
-        parser: Optional["CustomParser[MsgType]"],
-        decoder: Optional["CustomDecoder[StreamMessage[MsgType]]"],
+        filter: "Filter[Any]",
+        parser: Optional["CustomCallable"],
+        decoder: Optional["CustomCallable"],
         middlewares: Iterable["SubscriberMiddleware"],
         dependencies: Iterable["Depends"],
     ) -> None:
         self.filter = filter
         self.parser = parser
         self.decoder = decoder
         self.middlewares = middlewares
@@ -86,25 +83,25 @@
 
     lock: ContextManager[Any]
     extra_watcher_options: "AnyDict"
     extra_context: "AnyDict"
     graceful_timeout: Optional[float]
 
     _broker_dependecies: Iterable["Depends"]
-    _call_options: Optional["_CallOptions[MsgType]"]
+    _call_options: Optional["_CallOptions"]
 
     def __init__(
         self,
         *,
         no_ack: bool,
         retry: Union[bool, int],
         broker_dependencies: Iterable["Depends"],
         broker_middlewares: Iterable["BrokerMiddleware[MsgType]"],
-        default_parser: "AsyncParser[MsgType]",
-        default_decoder: "AsyncDecoder[StreamMessage[MsgType]]",
+        default_parser: "AsyncCallable",
+        default_decoder: "AsyncCallable",
         # AsyncAPI information
         title_: Optional[str],
         description_: Optional[str],
         include_in_schema: bool,
     ) -> None:
         """Initialize a new instance of the class."""
         self.calls = []
@@ -139,16 +136,16 @@
         self,
         *,
         logger: Optional["LoggerProto"],
         producer: Optional[ProducerProto],
         graceful_timeout: Optional[float],
         extra_context: Optional["AnyDict"],
         # broker options
-        broker_parser: Optional["CustomParser[MsgType]"],
-        broker_decoder: Optional["CustomDecoder[StreamMessage[MsgType]]"],
+        broker_parser: Optional["CustomCallable"],
+        broker_decoder: Optional["CustomCallable"],
         # dependant args
         apply_types: bool,
         is_validate: bool,
         _get_dependant: Optional[Callable[..., Any]],
     ) -> None:
         self.lock = MultiLock()
 
@@ -156,20 +153,24 @@
         self.graceful_timeout = graceful_timeout
         self.extra_context = extra_context or {}
 
         self.watcher = get_watcher_context(logger, self._no_ack, self._retry)
 
         for call in self.calls:
             if parser := call.item_parser or broker_parser:
-                async_parser = resolve_custom_func(to_async(parser), self._default_parser)
+                async_parser = resolve_custom_func(
+                    to_async(parser), self._default_parser
+                )
             else:
                 async_parser = self._default_parser
 
             if decoder := call.item_decoder or broker_decoder:
-                async_decoder = resolve_custom_func(to_async(decoder), self._default_decoder)
+                async_decoder = resolve_custom_func(
+                    to_async(decoder), self._default_decoder
+                )
             else:
                 async_decoder = self._default_decoder
 
             call.setup(
                 parser=async_parser,
                 decoder=async_decoder,
                 apply_types=apply_types,
@@ -194,65 +195,63 @@
         self.running = False
         if isinstance(self.lock, MultiLock):
             await self.lock.wait_release(self.graceful_timeout)
 
     def add_call(
         self,
         *,
-        filter_: "Filter[StreamMessage[MsgType]]",
-        parser_: Optional["CustomParser[MsgType]"],
-        decoder_: Optional["CustomDecoder[StreamMessage[MsgType]]"],
+        filter_: "Filter[Any]",
+        parser_: Optional["CustomCallable"],
+        decoder_: Optional["CustomCallable"],
         middlewares_: Iterable["SubscriberMiddleware"],
         dependencies_: Iterable["Depends"],
     ) -> Self:
-        self._call_options = _CallOptions[MsgType](
+        self._call_options = _CallOptions(
             filter=filter_,
             parser=parser_,
             decoder=decoder_,
             middlewares=middlewares_,
             dependencies=dependencies_,
         )
         return self
 
     @overload
     def __call__(
         self,
         func: None = None,
         *,
-        filter: Optional["Filter[StreamMessage[MsgType]]"] = None,
-        parser: Optional["CustomParser[MsgType]"] = None,
-        decoder: Optional["CustomDecoder[StreamMessage[MsgType]]"] = None,
+        filter: Optional["Filter[Any]"] = None,
+        parser: Optional["CustomCallable"] = None,
+        decoder: Optional["CustomCallable"] = None,
         middlewares: Iterable["SubscriberMiddleware"] = (),
         dependencies: Iterable["Depends"] = (),
     ) -> Callable[
         [Callable[P_HandlerParams, T_HandlerReturn]],
         "HandlerCallWrapper[MsgType, P_HandlerParams, T_HandlerReturn]",
-    ]:
-        ...
+    ]: ...
 
     @overload
     def __call__(
         self,
         func: Callable[P_HandlerParams, T_HandlerReturn],
         *,
-        filter: Optional["Filter[StreamMessage[MsgType]]"] = None,
-        parser: Optional["CustomParser[MsgType]"] = None,
-        decoder: Optional["CustomDecoder[StreamMessage[MsgType]]"] = None,
+        filter: Optional["Filter[Any]"] = None,
+        parser: Optional["CustomCallable"] = None,
+        decoder: Optional["CustomCallable"] = None,
         middlewares: Iterable["SubscriberMiddleware"] = (),
         dependencies: Iterable["Depends"] = (),
-    ) -> "HandlerCallWrapper[MsgType, P_HandlerParams, T_HandlerReturn]":
-        ...
+    ) -> "HandlerCallWrapper[MsgType, P_HandlerParams, T_HandlerReturn]": ...
 
     def __call__(
         self,
         func: Optional[Callable[P_HandlerParams, T_HandlerReturn]] = None,
         *,
-        filter: Optional["Filter[StreamMessage[MsgType]]"] = None,
-        parser: Optional["CustomParser[MsgType]"] = None,
-        decoder: Optional["CustomDecoder[StreamMessage[MsgType]]"] = None,
+        filter: Optional["Filter[Any]"] = None,
+        parser: Optional["CustomCallable"] = None,
+        decoder: Optional["CustomCallable"] = None,
         middlewares: Iterable["SubscriberMiddleware"] = (),
         dependencies: Iterable["Depends"] = (),
     ) -> Any:
         if (options := self._call_options) is None:
             raise SetupError("You can't create subscriber directly.")
 
         total_deps = (*options.dependencies, *dependencies)
```

### Comparing `faststream-0.5.0rc0/faststream/broker/wrapper/call.py` & `faststream-0.5.0rc1/faststream/broker/wrapper/call.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,38 +15,39 @@
 )
 from unittest.mock import MagicMock
 
 import anyio
 from fast_depends.core import CallModel, build_call_model
 from fast_depends.use import _InjectWrapper, inject
 
-from faststream.broker.message import StreamMessage
-from faststream.broker.publisher.proto import PublisherProto
 from faststream.broker.types import (
     MsgType,
     P_HandlerParams,
     T_HandlerReturn,
 )
 from faststream.exceptions import SetupError
 from faststream.utils.functions import to_async
 
 if TYPE_CHECKING:
     from fast_depends.dependencies import Depends
 
+    from faststream.broker.message import StreamMessage
+    from faststream.broker.publisher.proto import PublisherProto
+
 
 class HandlerCallWrapper(Generic[MsgType, P_HandlerParams, T_HandlerReturn]):
     """A generic class to wrap handler calls."""
 
     mock: Optional[MagicMock]
     future: Optional["asyncio.Future[Any]"]
     is_test: bool
 
     _wrapped_call: Optional[Callable[..., Awaitable[Any]]]
     _original_call: Callable[P_HandlerParams, T_HandlerReturn]
-    _publishers: List[PublisherProto[MsgType]]
+    _publishers: List["PublisherProto[MsgType]"]
 
     __slots__ = (
         "mock",
         "future",
         "is_test",
         "_wrapped_call",
         "_original_call",
@@ -86,15 +87,15 @@
         **kwargs: P_HandlerParams.kwargs,
     ) -> T_HandlerReturn:
         """Calls the object as a function."""
         return self._original_call(*args, **kwargs)
 
     def call_wrapped(
         self,
-        message: StreamMessage[MsgType],
+        message: "StreamMessage[MsgType]",
     ) -> Awaitable[Any]:
         """Calls the wrapped function with the given message."""
         assert self._wrapped_call, "You should use `set_wrapped` first"  # nosec B101
         if self.is_test:
             assert self.mock  # nosec B101
             self.mock(message.decoded_body)
         return self._wrapped_call(message)
@@ -155,15 +156,15 @@
         f: Callable[..., Awaitable[Any]] = to_async(self._original_call)
 
         dependent: Optional["CallModel[..., Any]"] = None
         if _get_dependant is None:
             dependent = build_call_model(
                 f,
                 cast=is_validate,
-                extra_dependencies=dependencies,
+                extra_dependencies=dependencies,  # type: ignore[arg-type]
             )
 
             if apply_types:
                 wrapper: _InjectWrapper[Any, Any] = inject(func=None)
                 f = wrapper(func=f, model=dependent)
 
             f = _wrap_decode_message(
```

### Comparing `faststream-0.5.0rc0/faststream/broker/wrapper/proto.py` & `faststream-0.5.0rc1/faststream/broker/wrapper/proto.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,73 +1,79 @@
 from typing import (
+    TYPE_CHECKING,
+    Any,
     Callable,
     Iterable,
     Optional,
     Protocol,
     Union,
     overload,
 )
 
-from fast_depends.dependencies import Depends
-
-from faststream.broker.message import StreamMessage
 from faststream.broker.types import (
-    CustomDecoder,
-    CustomParser,
+    CustomCallable,
     Filter,
     MsgType,
     P_HandlerParams,
     SubscriberMiddleware,
     T_HandlerReturn,
 )
-from faststream.broker.wrapper.call import HandlerCallWrapper
+
+if TYPE_CHECKING:
+    from fast_depends.dependencies import Depends
+
+    from faststream.broker.wrapper.call import HandlerCallWrapper
 
 
 class WrapperProto(Protocol[MsgType]):
     """Annotation class to represent @subscriber return type."""
 
     @overload
     def __call__(
         self,
         func: None = None,
         *,
-        filter: Optional["Filter[StreamMessage[MsgType]]"] = None,
-        parser: Optional["CustomParser[MsgType]"] = None,
-        decoder: Optional["CustomDecoder[StreamMessage[MsgType]]"] = None,
+        filter: Optional["Filter[Any]"] = None,
+        parser: Optional["CustomCallable"] = None,
+        decoder: Optional["CustomCallable"] = None,
         middlewares: Iterable["SubscriberMiddleware"] = (),
         dependencies: Iterable["Depends"] = (),
     ) -> Callable[
         [Callable[P_HandlerParams, T_HandlerReturn]],
-        HandlerCallWrapper[MsgType, P_HandlerParams, T_HandlerReturn],
-    ]:
-        ...
+        "HandlerCallWrapper[MsgType, P_HandlerParams, T_HandlerReturn]",
+    ]: ...
 
     @overload
     def __call__(
         self,
-        func: Callable[P_HandlerParams, T_HandlerReturn],
+        func: Union[
+            Callable[P_HandlerParams, T_HandlerReturn],
+            "HandlerCallWrapper[MsgType, P_HandlerParams, T_HandlerReturn]",
+        ],
         *,
-        filter: Optional[Filter[StreamMessage[MsgType]]] = None,
-        parser: Optional[CustomParser[MsgType]] = None,
-        decoder: Optional[CustomDecoder[StreamMessage[MsgType]]] = None,
-        middlewares: Iterable[SubscriberMiddleware] = (),
-        dependencies: Iterable[Depends] = (),
-    ) -> HandlerCallWrapper[MsgType, P_HandlerParams, T_HandlerReturn]:
-        ...
+        filter: Optional["Filter[Any]"] = None,
+        parser: Optional["CustomCallable"] = None,
+        decoder: Optional["CustomCallable"] = None,
+        middlewares: Iterable["SubscriberMiddleware"] = (),
+        dependencies: Iterable["Depends"] = (),
+    ) -> "HandlerCallWrapper[MsgType, P_HandlerParams, T_HandlerReturn]": ...
 
     def __call__(
         self,
-        func: Optional[Callable[P_HandlerParams, T_HandlerReturn]] = None,
+        func: Union[
+            Callable[P_HandlerParams, T_HandlerReturn],
+            "HandlerCallWrapper[MsgType, P_HandlerParams, T_HandlerReturn]",
+            None,
+        ] = None,
         *,
-        filter: Optional[Filter[StreamMessage[MsgType]]] = None,
-        parser: Optional[CustomParser[MsgType]] = None,
-        decoder: Optional[CustomDecoder[StreamMessage[MsgType]]] = None,
-        middlewares: Iterable[SubscriberMiddleware] = (),
-        dependencies: Iterable[Depends] = (),
+        filter: Optional["Filter[Any]"] = None,
+        parser: Optional["CustomCallable"] = None,
+        decoder: Optional["CustomCallable"] = None,
+        middlewares: Iterable["SubscriberMiddleware"] = (),
+        dependencies: Iterable["Depends"] = (),
     ) -> Union[
-        HandlerCallWrapper[MsgType, P_HandlerParams, T_HandlerReturn],
+        "HandlerCallWrapper[MsgType, P_HandlerParams, T_HandlerReturn]",
         Callable[
             [Callable[P_HandlerParams, T_HandlerReturn]],
-            HandlerCallWrapper[MsgType, P_HandlerParams, T_HandlerReturn],
+            "HandlerCallWrapper[MsgType, P_HandlerParams, T_HandlerReturn]",
         ],
-    ]:
-        ...
+    ]: ...
```

### Comparing `faststream-0.5.0rc0/faststream/cli/main.py` & `faststream-0.5.0rc1/faststream/cli/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,44 +1,42 @@
 import logging
 import sys
 import warnings
 from contextlib import suppress
-from typing import Any, Dict, List, Optional
+from typing import TYPE_CHECKING, Any, Dict, List, Optional
 
 import anyio
 import typer
 from click.exceptions import MissingParameter
 from typer.core import TyperOption
 
 from faststream import FastStream
 from faststream.__about__ import INSTALL_WATCHFILES, __version__
-from faststream.broker.core.usecase import BrokerUsecase
 from faststream.cli.docs.app import docs_app
 from faststream.cli.utils.imports import import_from_string
 from faststream.cli.utils.logs import LogLevels, get_log_level, set_log_level
 from faststream.cli.utils.parser import parse_cli_args
 from faststream.exceptions import SetupError, ValidationError
-from faststream.types import AnyDict, SettingField
+
+if TYPE_CHECKING:
+    from faststream.broker.core.usecase import BrokerUsecase
+    from faststream.types import AnyDict, SettingField
 
 cli = typer.Typer(pretty_exceptions_short=True)
 cli.add_typer(docs_app, name="docs", help="AsyncAPI schema commands")
 
 
 def version_callback(version: bool) -> None:
     """Callback function for displaying version information."""
     if version:
         import platform
 
         typer.echo(
-            "Running FastStream {} with {} {} on {}".format(
-                __version__,
-                platform.python_implementation(),
-                platform.python_version(),
-                platform.system(),
-            )
+            f"Running FastStream {__version__} with {platform.python_implementation()} "
+            f"{platform.python_version()} on {platform.system()}"
         )
 
         raise typer.Exit()
 
 
 @cli.callback()
 def main(
@@ -148,15 +146,15 @@
     else:
         _run(*args)
 
 
 def _run(
     # NOTE: we should pass `str` due FastStream is not picklable
     app: str,
-    extra_options: Dict[str, SettingField],
+    extra_options: Dict[str, "SettingField"],
     log_level: int = logging.INFO,
     app_level: int = logging.INFO,
 ) -> None:
     """Runs the specified application."""
     _, app_obj = import_from_string(app)
 
     if not isinstance(app_obj, FastStream):
@@ -229,14 +227,14 @@
             typer.echo(result)
 
     except Exception as e:
         typer.echo(f"Publish error: {e}")
         sys.exit(1)
 
 
-async def publish_message(broker: BrokerUsecase[Any, Any], extra: AnyDict) -> Any:
+async def publish_message(broker: "BrokerUsecase[Any, Any]", extra: "AnyDict") -> Any:
     try:
         async with broker:
             return await broker.publish(**extra)  # type: ignore[union-attr]
     except Exception as e:
         typer.echo(f"Error when broker was publishing: {e}")
         sys.exit(1)
```

### Comparing `faststream-0.5.0rc0/faststream/cli/docs/app.py` & `faststream-0.5.0rc1/faststream/cli/docs/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 import json
 import sys
 import warnings
 from pathlib import Path
-from typing import TYPE_CHECKING, Optional, Sequence
+from typing import Optional, Sequence
 
 import typer
 
 from faststream.__about__ import INSTALL_WATCHFILES, INSTALL_YAML
 from faststream._compat import json_dumps, model_parse
 from faststream.asyncapi.generate import get_app_schema
 from faststream.asyncapi.schema import Schema
 from faststream.asyncapi.site import serve_app
 from faststream.cli.utils.imports import import_from_string
-from faststream.log import logger as default_logger
-
-if TYPE_CHECKING:
-    from logging import Logger
 
 docs_app = typer.Typer(pretty_exceptions_short=True)
 
 
 @docs_app.command(name="serve")
 def serve(
     app: str = typer.Argument(
@@ -139,20 +135,17 @@
 
 
 def _parse_and_serve(
     app: str,
     host: str = "localhost",
     port: int = 8000,
 ) -> None:
-    logger: Optional["Logger"] = None
-
     if ":" in app:
         _, app_obj = import_from_string(app)
         raw_schema = get_app_schema(app_obj)
-        logger = app_obj.logger
 
     else:
         schema_filepath = Path.cwd() / app
 
         if schema_filepath.suffix == ".json":
             data = schema_filepath.read_bytes()
 
@@ -171,8 +164,8 @@
         else:
             raise ValueError(
                 f"Unknown extension given - {app}; Please provide app in format [python_module:FastStream] or [asyncapi.yaml/.json] - path to your application or documentation"
             )
 
         raw_schema = model_parse(Schema, data)
 
-    serve_app(raw_schema, host, port, logger=logger or default_logger)
+    serve_app(raw_schema, host, port)
```

### Comparing `faststream-0.5.0rc0/faststream/cli/supervisors/basereload.py` & `faststream-0.5.0rc1/faststream/cli/supervisors/basereload.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,81 +1,37 @@
 import os
 import threading
 from multiprocessing.context import SpawnProcess
-from typing import Any, Optional, Tuple
+from typing import TYPE_CHECKING, Any, Optional, Tuple
 
 from faststream.cli.supervisors.utils import get_subprocess, set_exit
 from faststream.log import logger
-from faststream.types import DecoratedCallable
 
+if TYPE_CHECKING:
+    from faststream.types import DecoratedCallable
 
-class BaseReload:
-    """A base class for implementing a reloader process.
-
-    Attributes:
-        _process : The spawned process
-        _target : The target callable function
-        _args : The arguments to be passed to the target function
-        reload_delay : The delay between reloads
-        should_exit : A threading event to signal the reloader to exit
-        pid : The process ID of the reloader
-        reloader_name : The name of the reloader
-
-    Methods:
-        __init__(self, target: DecoratedCallable, args: Tuple[Any, ...], reload_delay: Optional[float] = 0.5) -> None:
-            Initializes the BaseReload object.
-
-        run(self) -> None:
-            Runs the reloader process.
-
-        startup(self) -> None:
-            Performs startup operations for the reloader process.
-
-        restart(self) -> None:
-            Restarts the process.
 
-        shutdown(self) -> None:
-            Shuts down the reloader process.
-
-        _stop_process(self) -> None:
-            Stops the spawned process.
-
-        _start_process(self) -> SpawnProcess:
-            Starts the spawned process.
-
-        should_restart(self) -> bool:
-            Determines whether the process should be restarted.
-
-    """
+class BaseReload:
+    """A base class for implementing a reloader process."""
 
     _process: SpawnProcess
-    _target: DecoratedCallable
+    _target: "DecoratedCallable"
     _args: Tuple[Any, ...]
 
     reload_delay: Optional[float]
     should_exit: threading.Event
     pid: int
     reloader_name: str = ""
 
     def __init__(
         self,
-        target: DecoratedCallable,
+        target: "DecoratedCallable",
         args: Tuple[Any, ...],
         reload_delay: Optional[float] = 0.5,
     ) -> None:
-        """Initialize a class instance.
-
-        Args:
-            target: The target callable object
-            args: Tuple of arguments to be passed to the target callable
-            reload_delay: Optional delay in seconds before reloading the target callable (default is 0.5 seconds)
-
-        Returns:
-            None
-        """
         self._target = target
         self._args = args
 
         self.should_exit = threading.Event()
         self.pid = os.getpid()
         self.reload_delay = reload_delay
```

### Comparing `faststream-0.5.0rc0/faststream/cli/supervisors/utils.py` & `faststream-0.5.0rc1/faststream/cli/supervisors/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 import asyncio
 import multiprocessing
 import os
 import signal
 import sys
 from contextlib import suppress
-from multiprocessing.context import SpawnProcess
-from types import FrameType
-from typing import Any, Callable, Optional
+from typing import TYPE_CHECKING, Any, Callable, Optional
 
-from faststream.types import DecoratedCallableNone
+if TYPE_CHECKING:
+    from multiprocessing.context import SpawnProcess
+    from types import FrameType
+
+    from faststream.types import DecoratedCallableNone
 
 multiprocessing.allow_connection_pickling()
 spawn = multiprocessing.get_context("spawn")
 
 
 HANDLED_SIGNALS = (
     signal.SIGINT,  # Unix signal 2. Sent by Ctrl+C.
     signal.SIGTERM,  # Unix signal 15. Sent by `kill <pid>`.
 )
 
 
 def set_exit(
-    func: Callable[[int, Optional[FrameType]], Any],
+    func: Callable[[int, Optional["FrameType"]], Any],
     *,
     sync: bool = False,
 ) -> None:
     """Set exit handler for signals.
 
     Args:
         func: A callable object that takes an integer and an optional frame type as arguments and returns any value.
@@ -41,27 +43,16 @@
             return
 
     # Windows or sync mode
     for sig in HANDLED_SIGNALS:
         signal.signal(sig, func)
 
 
-def get_subprocess(target: DecoratedCallableNone, args: Any) -> SpawnProcess:
-    """Spawn a subprocess.
-
-    Args:
-        target: The target function to be executed in the subprocess.
-        args: The arguments to be passed to the target function.
-
-    Returns:
-        The spawned subprocess.
-
-    Raises:
-        OSError: If there is an error getting the file descriptor of sys.stdin.
-    """
+def get_subprocess(target: "DecoratedCallableNone", args: Any) -> "SpawnProcess":
+    """Spawn a subprocess."""
     stdin_fileno: Optional[int]
     try:
         stdin_fileno = sys.stdin.fileno()
     except OSError:
         stdin_fileno = None
 
     return spawn.Process(
@@ -69,24 +60,14 @@
         args=args,
         kwargs={"t": target, "stdin_fileno": stdin_fileno},
     )
 
 
 def subprocess_started(
     *args: Any,
-    t: DecoratedCallableNone,
+    t: "DecoratedCallableNone",
     stdin_fileno: Optional[int],
 ) -> None:
-    """Start a subprocess.
-
-    Args:
-        *args: Arguments to be passed to the subprocess.
-        t: The decorated callable function.
-        stdin_fileno: File descriptor for the standard input of the subprocess.
-
-    Returns:
-        None
-
-    """
+    """Start a subprocess."""
     if stdin_fileno is not None:  # pragma: no cover
         sys.stdin = os.fdopen(stdin_fileno)
     t(*args)
```

### Comparing `faststream-0.5.0rc0/faststream/cli/utils/logs.py` & `faststream-0.5.0rc1/faststream/cli/utils/logs.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import logging
 from collections import defaultdict
 from enum import Enum
 from typing import TYPE_CHECKING, DefaultDict, Optional, Union
 
-from faststream.app import FastStream
-
 if TYPE_CHECKING:
+    from faststream.app import FastStream
     from faststream.types import LoggerProto
 
 
 class LogLevels(str, Enum):
     """A class to represent log levels.
 
     Attributes:
@@ -55,23 +54,15 @@
     if isinstance(level, LogLevels):
         return LOG_LEVELS[level.value]
 
     if isinstance(level, str):  # pragma: no branch
         return LOG_LEVELS[level.lower()]
 
 
-def set_log_level(level: int, app: FastStream) -> None:
-    """Sets the log level for an application.
-
-    Args:
-        level (int): The log level to set.
-        app (FastStream): The application object.
-
-    Returns:
-        None
-    """
+def set_log_level(level: int, app: "FastStream") -> None:
+    """Sets the log level for an application."""
     if app.logger and isinstance(app.logger, logging.Logger):
         app.logger.setLevel(level)
 
     broker_logger: Optional["LoggerProto"] = getattr(app.broker, "logger", None)
     if broker_logger is not None and isinstance(broker_logger, logging.Logger):
         broker_logger.setLevel(level)
```

### Comparing `faststream-0.5.0rc0/faststream/cli/utils/parser.py` & `faststream-0.5.0rc1/faststream/cli/utils/parser.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,20 @@
 from functools import reduce
-from typing import Dict, List, Tuple
+from typing import TYPE_CHECKING, Dict, List, Tuple
 
-from faststream.types import SettingField
+if TYPE_CHECKING:
+    from faststream.types import SettingField
 
 
-def parse_cli_args(*args: str) -> Tuple[str, Dict[str, SettingField]]:
-    """Parses command line arguments.
-
-    Args:
-        *args: Command line arguments as strings.
-
-    Returns:
-        A tuple containing the application name and a dictionary of additional keyword arguments.
-    """
-    extra_kwargs: Dict[str, SettingField] = {}
+def parse_cli_args(*args: str) -> Tuple[str, Dict[str, "SettingField"]]:
+    """Parses command line arguments."""
+    extra_kwargs: Dict[str, "SettingField"] = {}
 
     k: str = ""
-    v: SettingField
+    v: "SettingField"
 
     field_args: List[str] = []
     app = ""
     for item in [
         *reduce(
             lambda acc, x: acc + x.split("="),  # type: ignore
             args,
```

### Comparing `faststream-0.5.0rc0/faststream/confluent/annotations.py` & `faststream-0.5.0rc1/faststream/confluent/annotations.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/faststream/confluent/client.py` & `faststream-0.5.0rc1/faststream/confluent/client.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/faststream/confluent/message.py` & `faststream-0.5.0rc1/faststream/confluent/message.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from typing import Any, Protocol, Tuple, Union
-
-from confluent_kafka import Message
+from typing import TYPE_CHECKING, Any, Protocol, Tuple, Union
 
 from faststream.broker.message import StreamMessage
 
+if TYPE_CHECKING:
+    from confluent_kafka import Message
+
 
 class ConsumerProtocol(Protocol):
     """A protocol for Kafka consumers."""
 
-    async def commit(self) -> None:
-        ...
+    async def commit(self) -> None: ...
 
 
 class FakeConsumer:
     """A fake Kafka consumer."""
 
     async def commit(self) -> None:
         pass
@@ -21,16 +21,16 @@
 
 FAKE_CONSUMER = FakeConsumer()
 
 
 class KafkaMessage(
     StreamMessage[
         Union[
-            Message,
-            Tuple[Message, ...],
+            "Message",
+            Tuple["Message", ...],
         ]
     ]
 ):
     """Represents a Kafka message in the FastStream framework.
 
     This class extends `StreamMessage` and is specialized for handling confluent_kafka.Message objects.
     """
```

### Comparing `faststream-0.5.0rc0/faststream/confluent/parser.py` & `faststream-0.5.0rc1/faststream/confluent/parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from typing import TYPE_CHECKING, Any, Optional, Tuple
 
-from confluent_kafka import Message
-
-from faststream.broker.message import StreamMessage, decode_message, gen_cor_id
+from faststream.broker.message import decode_message, gen_cor_id
 from faststream.confluent.message import FAKE_CONSUMER, KafkaMessage
-from faststream.types import DecodedMessage
 from faststream.utils.context.repository import context
 
 if TYPE_CHECKING:
+    from confluent_kafka import Message
+
+    from faststream.broker.message import StreamMessage
     from faststream.confluent.subscriber.usecase import LogicSubscriber
+    from faststream.types import DecodedMessage
 
 
 class AsyncConfluentParser:
     """A class to parse Kafka messages."""
 
     @staticmethod
     async def parse_message(
-        message: Message,
-    ) -> StreamMessage[Message]:
+        message: "Message",
+    ) -> "StreamMessage[Message]":
         """Parses a Kafka message."""
         headers = {}
         if message.headers() is not None:
             for i, j in message.headers():  # type: ignore[union-attr]
                 if isinstance(j, str):
                     headers[i] = j
                 else:
@@ -41,16 +42,16 @@
             raw_message=message,
             consumer=getattr(handler, "consumer", None) or FAKE_CONSUMER,
             is_manual=getattr(handler, "is_manual", True),
         )
 
     @staticmethod
     async def parse_message_batch(
-        message: Tuple[Message, ...],
-    ) -> StreamMessage[Tuple[Message, ...]]:
+        message: Tuple["Message", ...],
+    ) -> "StreamMessage[Tuple[Message, ...]]":
         """Parses a batch of messages from a Kafka consumer."""
         first = message[0]
         last = message[-1]
 
         headers = {}
         if first.headers() is not None:
             for i, j in first.headers():  # type: ignore[union-attr]
@@ -73,17 +74,20 @@
             correlation_id=headers.get("correlation_id", gen_cor_id()),
             raw_message=message,
             consumer=getattr(handler, "consumer", None) or FAKE_CONSUMER,
             is_manual=getattr(handler, "is_manual", True),
         )
 
     @staticmethod
-    async def decode_message(msg: StreamMessage[Message]) -> DecodedMessage:
+    async def decode_message(
+        msg: "StreamMessage[Message]",
+    ) -> "DecodedMessage":
         """Decodes a message."""
         return decode_message(msg)
 
     @classmethod
     async def decode_message_batch(
-        cls, msg: StreamMessage[Tuple[Message, ...]]
-    ) -> DecodedMessage:
+        cls,
+        msg: "StreamMessage[Tuple[Message, ...]]",
+    ) -> "DecodedMessage":
         """Decode a batch of messages."""
         return [decode_message(await cls.parse_message(m)) for m in msg.raw_message]
```

### Comparing `faststream-0.5.0rc0/faststream/confluent/router.py` & `faststream-0.5.0rc1/faststream/nats/router.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,92 +1,75 @@
-from typing import (
-    Any,
-    Callable,
-    Dict,
-    Iterable,
-    Literal,
-    Optional,
-    Sequence,
-    Tuple,
-    Union,
-)
+from typing import TYPE_CHECKING, Any, Callable, Dict, Iterable, Optional, Union
 
-from confluent_kafka import Message
-from fast_depends.dependencies import Depends
+from nats.js import api
 from typing_extensions import Annotated, Doc, deprecated
 
-from faststream.broker.message import StreamMessage
 from faststream.broker.router import ArgsContainer, BrokerRouter, SubscriberRoute
-from faststream.broker.types import (
-    BrokerMiddleware,
-    CustomDecoder,
-    CustomParser,
-    Filter,
-    PublisherMiddleware,
-    SubscriberMiddleware,
-)
 from faststream.broker.utils import default_filter
-from faststream.confluent.broker.registrator import KafkaRegistrator
-from faststream.types import SendableMessage
+from faststream.nats.broker.registrator import NatsRegistrator
 
+if TYPE_CHECKING:
+    from fast_depends.dependencies import Depends
+    from nats.aio.msg import Msg
+
+    from faststream.broker.types import (
+        BrokerMiddleware,
+        CustomCallable,
+        Filter,
+        PublisherMiddleware,
+        SubscriberMiddleware,
+    )
+    from faststream.nats.message import NatsBatchMessage, NatsMessage
+    from faststream.nats.schemas import JStream, PullSub
+    from faststream.types import SendableMessage
 
-class KafkaPublisher(ArgsContainer):
-    """Delayed KafkaPublisher registration object.
+
+class NatsPublisher(ArgsContainer):
+    """Delayed NatsPublisher registration object.
 
     Just a copy of `KafkaRegistrator.publisher(...)` arguments.
     """
 
     def __init__(
         self,
-        topic: Annotated[
+        subject: Annotated[
             str,
-            Doc("Topic where the message will be published."),
+            Doc("NATS subject to send message."),
         ],
         *,
-        key: Annotated[
-            Union[bytes, Any, None],
-            Doc("""
-            A key to associate with the message. Can be used to
-            determine which partition to send the message to. If partition
-            is `None` (and producer's partitioner config is left as default),
-            then messages with the same key will be delivered to the same
-            partition (but if key is `None`, partition is chosen randomly).
-            Must be type `bytes`, or be serializable to bytes via configured
-            `key_serializer`.
-            """),
-        ] = None,
-        partition: Annotated[
-            Optional[int],
-            Doc("""
-            Specify a partition. If not set, the partition will be
-            selected using the configured `partitioner`.
-            """),
-        ] = None,
         headers: Annotated[
             Optional[Dict[str, str]],
             Doc(
                 "Message headers to store metainformation. "
                 "**content-type** and **correlation_id** will be set automatically by framework anyway. "
                 "Can be overridden by `publish.headers` if specified."
             ),
         ] = None,
         reply_to: Annotated[
             str,
-            Doc("Topic name to send response."),
+            Doc("NATS subject name to send response."),
         ] = "",
-        batch: Annotated[
-            bool,
-            Doc("Whether to send messages in batches or not."),
-        ] = False,
+        # JS
+        stream: Annotated[
+            Union[str, "JStream", None],
+            Doc(
+                "This option validates that the target `subject` is in presented stream. "
+                "Can be omitted without any effect."
+            ),
+        ] = None,
+        timeout: Annotated[
+            Optional[float],
+            Doc("Timeout to send message to NATS."),
+        ] = None,
         # basic args
         middlewares: Annotated[
-            Iterable[PublisherMiddleware],
+            Iterable["PublisherMiddleware"],
             Doc("Publisher middlewares to wrap outgoing messages."),
         ] = (),
-        # AsyncAPI args
+        # AsyncAPI information
         title: Annotated[
             Optional[str],
             Doc("AsyncAPI publisher object title."),
         ] = None,
         description: Annotated[
             Optional[str],
             Doc("AsyncAPI publisher object description."),
@@ -100,126 +83,179 @@
         ] = None,
         include_in_schema: Annotated[
             bool,
             Doc("Whetever to include operation in AsyncAPI schema or not."),
         ] = True,
     ) -> None:
         super().__init__(
-            topic=topic,
-            key=key,
-            partition=partition,
-            batch=batch,
+            subject=subject,
             headers=headers,
             reply_to=reply_to,
-            # basic args
+            stream=stream,
+            timeout=timeout,
             middlewares=middlewares,
-            # AsyncAPI args
             title=title,
             description=description,
             schema=schema,
             include_in_schema=include_in_schema,
         )
 
 
-class KafkaRoute(SubscriberRoute):
-    """Class to store delaied KafkaBroker subscriber registration."""
+class NatsRoute(SubscriberRoute):
+    """Class to store delayed NatsBroker subscriber registration."""
 
     def __init__(
         self,
         call: Annotated[
-            Callable[..., SendableMessage],
-            Doc("Message handler function."),
+            Callable[..., "SendableMessage"],
+            Doc(
+                "Message handler function "
+                "to wrap the same with `@broker.subscriber(...)` way."
+            ),
+        ],
+        subject: Annotated[
+            str,
+            Doc("NATS subject to subscribe."),
         ],
-        *topics: str,
         publishers: Annotated[
-            Iterable[KafkaPublisher],
-            Doc("Kafka publishers to broadcast the handler result."),
+            Iterable[NatsPublisher],
+            Doc("Nats publishers to broadcast the handler result."),
         ] = (),
-        group_id: Optional[str] = None,
-        key_deserializer: Optional[Callable[[bytes], Any]] = None,
-        value_deserializer: Optional[Callable[[bytes], Any]] = None,
-        fetch_max_wait_ms: int = 500,
-        fetch_max_bytes: int = 52428800,
-        fetch_min_bytes: int = 1,
-        max_partition_fetch_bytes: int = 1 * 1024 * 1024,
-        auto_offset_reset: Literal[
-            "latest",
-            "earliest",
-            "none",
-        ] = "latest",
-        auto_commit: bool = True,
-        auto_commit_interval_ms: int = 5000,
-        check_crcs: bool = True,
-        partition_assignment_strategy: Sequence[str] = (
-            "roundrobin",
-        ),
-        max_poll_interval_ms: int = 300000,
-        rebalance_timeout_ms: Optional[int] = None,
-        session_timeout_ms: int = 10000,
-        heartbeat_interval_ms: int = 3000,
-        consumer_timeout_ms: int = 200,
-        max_poll_records: Optional[int] = None,
-        exclude_internal_topics: bool = True,
-        isolation_level: Literal[
-            "read_uncommitted",
-            "read_committed",
-        ] = "read_uncommitted",
-        batch: bool = False,
-        max_records: Optional[int] = None,
-        batch_timeout_ms: int = 200,
-        # broker args
+        queue: Annotated[
+            str,
+            Doc(
+                "Subscribers' NATS queue name. Subscribers with same queue name will be load balanced by the NATS "
+                "server."
+            ),
+        ] = "",
+        pending_msgs_limit: Annotated[
+            Optional[int],
+            Doc(
+                "Limit of messages, considered by NATS server as possible to be delivered to the client without "
+                "been answered. In case of NATS Core, if that limits exceeds, you will receive NATS 'Slow Consumer' "
+                "error. "
+                "That's literally means that your worker can't handle the whole load. In case of NATS JetStream, "
+                "you will no longer receive messages until some of delivered messages will be acked in any way."
+            ),
+        ] = None,
+        pending_bytes_limit: Annotated[
+            Optional[int],
+            Doc(
+                "The number of bytes, considered by NATS server as possible to be delivered to the client without "
+                "been answered. In case of NATS Core, if that limit exceeds, you will receive NATS 'Slow Consumer' "
+                "error."
+                "That's literally means that your worker can't handle the whole load. In case of NATS JetStream, "
+                "you will no longer receive messages until some of delivered messages will be acked in any way."
+            ),
+        ] = None,
+        # Core arguments
+        max_msgs: Annotated[
+            int,
+            Doc("Consuming messages limiter. Automatically disconnect if reached."),
+        ] = 0,
+        # JS arguments
+        durable: Annotated[
+            Optional[str],
+            Doc(
+                "Name of the durable consumer to which the the subscription should be bound."
+            ),
+        ] = None,
+        config: Annotated[
+            Optional["api.ConsumerConfig"],
+            Doc("Configuration of JetStream consumer to be subscribed with."),
+        ] = None,
+        ordered_consumer: Annotated[
+            bool,
+            Doc("Enable ordered consumer mode."),
+        ] = False,
+        idle_heartbeat: Annotated[
+            Optional[float],
+            Doc("Enable Heartbeats for a consumer to detect failures."),
+        ] = None,
+        flow_control: Annotated[
+            bool,
+            Doc("Enable Flow Control for a consumer."),
+        ] = False,
+        deliver_policy: Annotated[
+            Optional["api.DeliverPolicy"],
+            Doc("Deliver Policy to be used for subscription."),
+        ] = None,
+        headers_only: Annotated[
+            Optional[bool],
+            Doc(
+                "Should be message delivered without payload, only headers and metadata."
+            ),
+        ] = None,
+        # pull arguments
+        pull_sub: Annotated[
+            Optional["PullSub"],
+            Doc(
+                "NATS Pull consumer parameters container. "
+                "Should be used with `stream` only."
+            ),
+        ] = None,
+        inbox_prefix: Annotated[
+            bytes,
+            Doc(
+                "Prefix for generating unique inboxes, subjects with that prefix and NUID."
+            ),
+        ] = api.INBOX_PREFIX,
+        # custom
+        ack_first: Annotated[
+            bool,
+            Doc("Whether to `ack` message at start of consuming or not."),
+        ] = False,
+        stream: Annotated[
+            Union[str, "JStream", None],
+            Doc("Subscribe to NATS Stream with `subject` filter."),
+        ] = None,
+        # broker arguments
         dependencies: Annotated[
-            Iterable[Depends],
+            Iterable["Depends"],
             Doc("Dependencies list (`[Depends(),]`) to apply to the subscriber."),
         ] = (),
         parser: Annotated[
-            Optional[
-                Union[
-                    CustomParser[Message],
-                    CustomParser[Tuple[Message, ...]],
-                ]
-            ],
-            Doc("Parser to map original **Message** object to FastStream one."),
+            Optional["CustomCallable"],
+            Doc("Parser to map original **nats-py** Msg to FastStream one."),
         ] = None,
         decoder: Annotated[
-            Optional[
-                Union[
-                    CustomDecoder[StreamMessage[Message]],
-                    CustomDecoder[StreamMessage[Tuple[Message, ...]]],
-                ]
-            ],
+            Optional["CustomCallable"],
             Doc("Function to decode FastStream msg bytes body to python objects."),
         ] = None,
         middlewares: Annotated[
-            Iterable[SubscriberMiddleware],
+            Iterable["SubscriberMiddleware"],
             Doc("Subscriber middlewares to wrap incoming message processing."),
         ] = (),
         filter: Annotated[
             Union[
-                Filter[StreamMessage[Message]],
-                Filter[StreamMessage[Tuple[Message, ...]]],
+                "Filter[NatsMessage]",
+                "Filter[NatsBatchMessage]",
             ],
             Doc(
                 "Overload subscriber to consume various messages from the same source."
             ),
             deprecated(
                 "Deprecated in **FastStream 0.5.0**. "
                 "Please, create `subscriber` object and use it explicitly instead. "
                 "Argument will be removed in **FastStream 0.6.0**."
             ),
         ] = default_filter,
+        max_workers: Annotated[
+            int,
+            Doc("Number of workers to process messages concurrently."),
+        ] = 1,
         retry: Annotated[
             bool,
             Doc("Whether to `nack` message at processing exception."),
         ] = False,
         no_ack: Annotated[
             bool,
             Doc("Whether to disable **FastStream** autoacknowledgement logic or not."),
         ] = False,
-        # AsyncAPI args
+        # AsyncAPI information
         title: Annotated[
             Optional[str],
             Doc("AsyncAPI subscriber object title."),
         ] = None,
         description: Annotated[
             Optional[str],
             Doc(
@@ -230,100 +266,78 @@
         include_in_schema: Annotated[
             bool,
             Doc("Whetever to include operation in AsyncAPI schema or not."),
         ] = True,
     ) -> None:
         super().__init__(
             call,
-            *topics,
+            subject=subject,
             publishers=publishers,
-            group_id=group_id,
-            key_deserializer=key_deserializer,
-            value_deserializer=value_deserializer,
-            fetch_max_wait_ms=fetch_max_wait_ms,
-            fetch_max_bytes=fetch_max_bytes,
-            fetch_min_bytes=fetch_min_bytes,
-            max_partition_fetch_bytes=max_partition_fetch_bytes,
-            auto_offset_reset=auto_offset_reset,
-            auto_commit=auto_commit,
-            auto_commit_interval_ms=auto_commit_interval_ms,
-            check_crcs=check_crcs,
-            partition_assignment_strategy=partition_assignment_strategy,
-            max_poll_interval_ms=max_poll_interval_ms,
-            rebalance_timeout_ms=rebalance_timeout_ms,
-            session_timeout_ms=session_timeout_ms,
-            heartbeat_interval_ms=heartbeat_interval_ms,
-            consumer_timeout_ms=consumer_timeout_ms,
-            max_poll_records=max_poll_records,
-            exclude_internal_topics=exclude_internal_topics,
-            isolation_level=isolation_level,
-            max_records=max_records,
-            batch_timeout_ms=batch_timeout_ms,
-            batch=batch,
-            # basic args
+            pending_msgs_limit=pending_msgs_limit,
+            pending_bytes_limit=pending_bytes_limit,
+            max_msgs=max_msgs,
+            durable=durable,
+            config=config,
+            ordered_consumer=ordered_consumer,
+            idle_heartbeat=idle_heartbeat,
+            flow_control=flow_control,
+            deliver_policy=deliver_policy,
+            headers_only=headers_only,
+            pull_sub=pull_sub,
+            inbox_prefix=inbox_prefix,
+            ack_first=ack_first,
+            stream=stream,
+            max_workers=max_workers,
+            queue=queue,
             dependencies=dependencies,
             parser=parser,
             decoder=decoder,
             middlewares=middlewares,
             filter=filter,
-            # AsyncAPI args
+            retry=retry,
+            no_ack=no_ack,
             title=title,
             description=description,
             include_in_schema=include_in_schema,
-            # FastDepends args
-            retry=retry,
-            no_ack=no_ack,
         )
 
 
-class KafkaRouter(
-    BrokerRouter[Union[
-        Message,
-        Tuple[Message, ...],
-    ]],
-    KafkaRegistrator,
+class NatsRouter(
+    BrokerRouter["Msg"],
+    NatsRegistrator,
 ):
-    """Includable to KafkaBroker router."""
+    """Includable to NatsBroker router."""
 
     def __init__(
         self,
         prefix: Annotated[
             str,
-            Doc("String prefix to add to all subscribers queues."),
+            Doc("String prefix to add to all subscribers subjects."),
         ] = "",
         handlers: Annotated[
-            Iterable[KafkaRoute],
+            Iterable[NatsRoute],
             Doc("Route object to include."),
         ] = (),
         *,
         dependencies: Annotated[
-            Iterable[Depends],
+            Iterable["Depends"],
             Doc(
                 "Dependencies list (`[Depends(),]`) to apply to all routers' publishers/subscribers."
             ),
         ] = (),
         middlewares: Annotated[
-            Iterable[Union[
-                BrokerMiddleware[Message],
-                BrokerMiddleware[Tuple[Message, ...]],
-            ]],
+            Iterable["BrokerMiddleware[Msg]"],
             Doc("Router middlewares to apply to all routers' publishers/subscribers."),
         ] = (),
         parser: Annotated[
-            Optional[Union[
-                CustomParser[Message],
-                CustomParser[Tuple[Message, ...]],
-            ]],
-            Doc("Parser to map original **Message** object to FastStream one."),
+            Optional["CustomCallable"],
+            Doc("Parser to map original **IncomingMessage** Msg to FastStream one."),
         ] = None,
         decoder: Annotated[
-            Optional[Union[
-                CustomDecoder[StreamMessage[Message]],
-                CustomDecoder[StreamMessage[Tuple[Message, ...]]],
-            ]],
+            Optional["CustomCallable"],
             Doc("Function to decode FastStream msg bytes body to python objects."),
         ] = None,
         include_in_schema: Annotated[
             Optional[bool],
             Doc("Whetever to include operation in AsyncAPI schema or not."),
         ] = None,
     ) -> None:
```

### Comparing `faststream-0.5.0rc0/faststream/confluent/security.py` & `faststream-0.5.0rc1/faststream/confluent/security.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,45 @@
 import warnings
-from typing import Optional
+from typing import TYPE_CHECKING, Optional
 
 from faststream.security import (
     BaseSecurity,
     SASLPlaintext,
     SASLScram256,
     SASLScram512,
     ssl_not_set_error_msg,
 )
-from faststream.types import AnyDict
 
+if TYPE_CHECKING:
+    from faststream.types import AnyDict
 
-def parse_security(security: Optional[BaseSecurity]) -> AnyDict:
+
+def parse_security(security: Optional[BaseSecurity]) -> "AnyDict":
     if security is None:
         return {}
     elif type(security) == BaseSecurity:
         return _parse_base_security(security)
     elif type(security) == SASLPlaintext:
         return _parse_sasl_plaintext(security)
     elif type(security) == SASLScram256:
         return _parse_sasl_scram256(security)
     elif type(security) == SASLScram512:
         return _parse_sasl_scram512(security)
     else:
         raise NotImplementedError(f"KafkaBroker does not support `{type(security)}`.")
 
 
-def _parse_base_security(security: BaseSecurity) -> AnyDict:
+def _parse_base_security(security: BaseSecurity) -> "AnyDict":
     return {
         "security_protocol": "SSL" if security.use_ssl else "PLAINTEXT",
         "ssl_context": security.ssl_context,
     }
 
 
-def _parse_sasl_plaintext(security: SASLPlaintext) -> AnyDict:
+def _parse_sasl_plaintext(security: SASLPlaintext) -> "AnyDict":
     if security.ssl_context is None:
         warnings.warn(
             message=ssl_not_set_error_msg,
             category=RuntimeWarning,
             stacklevel=1,
         )
 
@@ -46,25 +48,25 @@
         "ssl_context": security.ssl_context,
         "sasl_mechanism": "PLAIN",
         "sasl_plain_username": security.username,
         "sasl_plain_password": security.password,
     }
 
 
-def _parse_sasl_scram256(security: SASLScram256) -> AnyDict:
+def _parse_sasl_scram256(security: SASLScram256) -> "AnyDict":
     return {
         "security_protocol": "SASL_SSL" if security.use_ssl else "SASL_PLAINTEXT",
         "ssl_context": security.ssl_context,
         "sasl_mechanism": "SCRAM-SHA-256",
         "sasl_plain_username": security.username,
         "sasl_plain_password": security.password,
     }
 
 
-def _parse_sasl_scram512(security: SASLScram512) -> AnyDict:
+def _parse_sasl_scram512(security: SASLScram512) -> "AnyDict":
     return {
         "security_protocol": "SASL_SSL" if security.use_ssl else "SASL_PLAINTEXT",
         "ssl_context": security.ssl_context,
         "sasl_mechanism": "SCRAM-SHA-512",
         "sasl_plain_username": security.username,
         "sasl_plain_password": security.password,
     }
```

### Comparing `faststream-0.5.0rc0/faststream/confluent/testing.py` & `faststream-0.5.0rc1/faststream/confluent/testing.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,58 +1,58 @@
 from datetime import datetime
-from typing import Any, Dict, List, Optional, Tuple
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple
 
 from typing_extensions import override
 
 from faststream.broker.message import encode_message, gen_cor_id
-from faststream.broker.wrapper.call import HandlerCallWrapper
 from faststream.confluent.broker import KafkaBroker
-from faststream.confluent.publisher.asyncapi import (
-    AsyncAPIBatchPublisher,
-    AsyncAPIPublisher,
-)
+from faststream.confluent.publisher.asyncapi import AsyncAPIBatchPublisher
 from faststream.confluent.publisher.producer import AsyncConfluentFastProducer
 from faststream.confluent.subscriber.asyncapi import AsyncAPIBatchSubscriber
 from faststream.testing.broker import TestBroker, call_handler
-from faststream.types import SendableMessage
+
+if TYPE_CHECKING:
+    from faststream.broker.wrapper.call import HandlerCallWrapper
+    from faststream.confluent.publisher.asyncapi import AsyncAPIPublisher
+    from faststream.types import SendableMessage
 
 __all__ = ("TestKafkaBroker",)
 
 
 class TestKafkaBroker(TestBroker[KafkaBroker]):
     """A class to test Kafka brokers."""
 
     @staticmethod
     async def _fake_connect(broker: KafkaBroker, *args: Any, **kwargs: Any) -> None:
         broker._producer = FakeProducer(broker)
 
     @staticmethod
     def create_publisher_fake_subscriber(
         broker: KafkaBroker,
-        publisher: AsyncAPIPublisher,
-    ) -> HandlerCallWrapper[Any, Any, Any]:
+        publisher: "AsyncAPIPublisher[Any]",
+    ) -> "HandlerCallWrapper[Any, Any, Any]":
         sub = broker.subscriber(  # type: ignore[call-overload,misc]
             publisher.topic,
             batch=isinstance(publisher, AsyncAPIBatchPublisher),
         )
 
         if not sub.calls:
 
-            @sub
+            @sub  # type: ignore[misc]
             def f(msg: Any) -> None:
                 pass
 
             broker.setup_subscriber(sub)
 
         return sub.calls[0].handler
 
     @staticmethod
     def remove_publisher_fake_subscriber(
         broker: KafkaBroker,
-        publisher: AsyncAPIPublisher,
+        publisher: "AsyncAPIPublisher[Any]",
     ) -> None:
         broker._subscribers.pop(hash(publisher), None)
 
 
 class FakeProducer(AsyncConfluentFastProducer):
     """A fake Kafka producer for testing purposes.
 
@@ -61,15 +61,15 @@
 
     def __init__(self, broker: KafkaBroker) -> None:
         self.broker = broker
 
     @override
     async def publish(  # type: ignore[override]
         self,
-        message: SendableMessage,
+        message: "SendableMessage",
         topic: str,
         key: Optional[bytes] = None,
         partition: Optional[int] = None,
         timestamp_ms: Optional[int] = None,
         headers: Optional[Dict[str, str]] = None,
         correlation_id: Optional[str] = None,
         *,
@@ -104,15 +104,15 @@
                     raise_timeout=raise_timeout,
                 )
 
         return None
 
     async def publish_batch(
         self,
-        *msgs: SendableMessage,
+        *msgs: "SendableMessage",
         topic: str,
         partition: Optional[int] = None,
         timestamp_ms: Optional[int] = None,
         headers: Optional[Dict[str, str]] = None,
         reply_to: str = "",
         correlation_id: Optional[str] = None,
     ) -> None:
@@ -196,39 +196,25 @@
         return self._topic
 
     def value(self) -> bytes:
         return self._raw_msg
 
 
 def build_message(
-    message: SendableMessage,
+    message: "SendableMessage",
     topic: str,
     *,
     correlation_id: str,
     partition: Optional[int] = None,
     timestamp_ms: Optional[int] = None,
     key: Optional[bytes] = None,
     headers: Optional[Dict[str, str]] = None,
     reply_to: str = "",
 ) -> MockConfluentMessage:
-    """Build a mock confluent_kafka.Message for a sendable message.
-
-    Args:
-        message (SendableMessage): The sendable message to be encoded.
-        topic (str): The Kafka topic for the message.
-        partition (Optional[int], optional): The Kafka partition for the message. Defaults to None.
-        timestamp_ms (Optional[int], optional): The message timestamp in milliseconds. Defaults to None.
-        key (Optional[bytes], optional): The message key. Defaults to None.
-        headers (Optional[Dict[str, str]], optional): Additional headers for the message. Defaults to None.
-        correlation_id (Optional[str], optional): The correlation ID for the message. Defaults to None.
-        reply_to (str, optional): The topic to which responses should be sent. Defaults to "".
-
-    Returns:
-        MockConfluentMessage: A mock confluent_kafka.Message object.
-    """
+    """Build a mock confluent_kafka.Message for a sendable message."""
     msg, content_type = encode_message(message)
     k = key or b""
     headers = {
         "content-type": content_type or "",
         "correlation_id": correlation_id,
         "reply_to": reply_to,
         **(headers or {}),
```

### Comparing `faststream-0.5.0rc0/faststream/confluent/broker/broker.py` & `faststream-0.5.0rc1/faststream/confluent/broker/broker.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,49 +1,53 @@
 import logging
 from asyncio import AbstractEventLoop
 from contextlib import AsyncExitStack
 from inspect import Parameter
-from types import TracebackType
 from typing import (
+    TYPE_CHECKING,
     Any,
     Callable,
     Dict,
     Iterable,
     List,
     Literal,
     Optional,
     Tuple,
     Type,
     TypeVar,
     Union,
 )
 
-from confluent_kafka import Message
-from fast_depends.dependencies import Depends
 from typing_extensions import Annotated, Doc, override
 
 from faststream.__about__ import SERVICE_NAME
-from faststream.asyncapi import schema as asyncapi
-from faststream.broker.message import StreamMessage, gen_cor_id
-from faststream.broker.types import (
-    BrokerMiddleware,
-    CustomDecoder,
-    CustomParser,
-)
+from faststream.broker.message import gen_cor_id
 from faststream.confluent.broker.logging import KafkaLoggingBroker
 from faststream.confluent.broker.registrator import KafkaRegistrator
 from faststream.confluent.client import AsyncConfluentProducer, _missing
 from faststream.confluent.publisher.producer import AsyncConfluentFastProducer
 from faststream.confluent.schemas.params import ConsumerConnectionParams
 from faststream.confluent.security import parse_security
 from faststream.exceptions import NOT_CONNECTED_YET
-from faststream.security import BaseSecurity
-from faststream.types import AnyDict, SendableMessage
 from faststream.utils.data import filter_by_dict
 
+if TYPE_CHECKING:
+    from types import TracebackType
+
+    from confluent_kafka import Message
+    from fast_depends.dependencies import Depends
+
+    from faststream.asyncapi import schema as asyncapi
+    from faststream.broker.types import (
+        BrokerMiddleware,
+        CustomCallable,
+    )
+    from faststream.security import BaseSecurity
+    from faststream.types import AnyDict, LoggerProto, SendableMessage
+
 Partition = TypeVar("Partition")
 
 
 class KafkaBroker(
     KafkaRegistrator,
     KafkaLoggingBroker,
 ):
@@ -242,35 +246,30 @@
         graceful_timeout: Annotated[
             Optional[float],
             Doc(
                 "Graceful shutdown timeout. Broker waits for all running subscribers completion before shut down."
             ),
         ] = 15.0,
         decoder: Annotated[
-            Optional[
-                Union[
-                    CustomDecoder[StreamMessage[Message]],
-                    CustomDecoder[StreamMessage[Tuple[Message, ...]]],
-                ]
-            ],
+            Optional["CustomCallable"],
             Doc("Custom decoder object."),
         ] = None,
         parser: Annotated[
-            Optional[Union[CustomParser[Message], CustomParser[Tuple[Message, ...]]]],
+            Optional["CustomCallable"],
             Doc("Custom parser object."),
         ] = None,
         dependencies: Annotated[
-            Iterable[Depends],
+            Iterable["Depends"],
             Doc("Dependencies to apply to all broker subscribers."),
         ] = (),
         middlewares: Annotated[
             Iterable[
                 Union[
-                    BrokerMiddleware[Message],
-                    BrokerMiddleware[Tuple[Message, ...]],
+                    "BrokerMiddleware[Message]",
+                    "BrokerMiddleware[Tuple[Message, ...]]",
                 ]
             ],
             Doc("Middlewares to apply to all broker publishers/subscribers."),
         ] = (),
         # AsyncAPI args
         security: Annotated[
             Optional["BaseSecurity"],
@@ -296,15 +295,15 @@
         ] = None,
         tags: Annotated[
             Optional[Iterable[Union["asyncapi.Tag", "asyncapi.TagDict"]]],
             Doc("AsyncAPI server tags."),
         ] = None,
         # logging args
         logger: Annotated[
-            Union[logging.Logger, None, object],
+            Union["LoggerProto", None, object],
             Doc("User specified logger to pass into Context and log service messages."),
         ] = Parameter.empty,
         log_level: Annotated[
             int,
             Doc("Service messages log level."),
         ] = logging.INFO,
         log_fmt: Annotated[
@@ -396,15 +395,15 @@
         self.client_id = client_id
         self._producer = None
 
     async def _close(
         self,
         exc_type: Optional[Type[BaseException]] = None,
         exc_val: Optional[BaseException] = None,
-        exc_tb: Optional[TracebackType] = None,
+        exc_tb: Optional["TracebackType"] = None,
     ) -> None:
         if self._producer is not None:  # pragma: no branch
             await self._producer.stop()
             self._producer = None
 
         await super()._close(exc_type, exc_val, exc_tb)
 
@@ -446,21 +445,21 @@
             self._log(
                 f"`{handler.call_name}` waiting for messages",
                 extra=handler.get_log_context(None),
             )
             await handler.start()
 
     @property
-    def _subscriber_setup_extra(self) -> AnyDict:
+    def _subscriber_setup_extra(self) -> "AnyDict":
         return {"client_id": self.client_id, "connection_data": self._connection or {}}
 
     @override
     async def publish(  # type: ignore[override]
         self,
-        message: SendableMessage,
+        message: "SendableMessage",
         topic: str,
         key: Optional[bytes] = None,
         partition: Optional[int] = None,
         timestamp_ms: Optional[int] = None,
         headers: Optional[Dict[str, str]] = None,
         correlation_id: Optional[str] = None,
         *,
@@ -481,15 +480,15 @@
             correlation_id=correlation_id,
             reply_to=reply_to,
             **kwargs,
         )
 
     async def publish_batch(
         self,
-        *msgs: SendableMessage,
+        *msgs: "SendableMessage",
         topic: str,
         partition: Optional[int] = None,
         timestamp_ms: Optional[int] = None,
         headers: Optional[Dict[str, str]] = None,
         reply_to: str = "",
         correlation_id: Optional[str] = None,
     ) -> None:
```

### Comparing `faststream-0.5.0rc0/faststream/confluent/broker/logging.py` & `faststream-0.5.0rc1/faststream/confluent/broker/logging.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 import logging
 from inspect import Parameter
-from typing import Any, ClassVar, Optional, Tuple, Union
-
-import confluent_kafka
+from typing import TYPE_CHECKING, Any, ClassVar, Optional, Tuple, Union
 
 from faststream.broker.core.usecase import BrokerUsecase
 from faststream.confluent.schemas.params import ConsumerConnectionParams
 from faststream.log.logging import get_broker_logger
 
+if TYPE_CHECKING:
+    import confluent_kafka
+
+    from faststream.types import LoggerProto
+
 
-class KafkaLoggingBroker(BrokerUsecase[
-    Union[
-        confluent_kafka.Message,
-        Tuple[confluent_kafka.Message, ...]
-    ],
-    ConsumerConnectionParams,
-]):
+class KafkaLoggingBroker(
+    BrokerUsecase[
+        Union["confluent_kafka.Message", Tuple["confluent_kafka.Message", ...]],
+        ConsumerConnectionParams,
+    ]
+):
     """A class that extends the LoggingMixin class and adds additional functionality for logging Kafka related information."""
 
     _max_topic_len: int
     _max_group_len: int
     __max_msg_id_ln: ClassVar[int] = 10
 
     def __init__(
         self,
         *args: Any,
-        logger: Union[logging.Logger, object, None] = Parameter.empty,
+        logger: Union["LoggerProto", object, None] = Parameter.empty,
         log_level: int = logging.INFO,
         log_fmt: Optional[str] = None,
         **kwargs: Any,
     ) -> None:
         """Initialize the class."""
         super().__init__(
             *args,
```

### Comparing `faststream-0.5.0rc0/faststream/confluent/broker/registrator.py` & `faststream-0.5.0rc1/faststream/confluent/router.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,223 +1,48 @@
-from functools import partial
 from typing import (
+    TYPE_CHECKING,
     Any,
     Callable,
     Dict,
     Iterable,
     Literal,
     Optional,
     Sequence,
     Tuple,
     Union,
-    cast,
-    overload,
 )
 
-from confluent_kafka import Message
-from fast_depends.dependencies import Depends
-from typing_extensions import Annotated, Doc, deprecated, override
-
-from faststream.broker.core.abc import ABCBroker
-from faststream.broker.message import StreamMessage
-from faststream.broker.types import (
-    CustomDecoder,
-    CustomParser,
-    Filter,
-    PublisherMiddleware,
-    SubscriberMiddleware,
-)
+from typing_extensions import Annotated, Doc, deprecated
+
+from faststream.broker.router import ArgsContainer, BrokerRouter, SubscriberRoute
 from faststream.broker.utils import default_filter
-from faststream.confluent.client import AsyncConfluentConsumer
-from faststream.confluent.publisher.asyncapi import (
-    AsyncAPIBatchPublisher,
-    AsyncAPIDefaultPublisher,
-    AsyncAPIPublisher,
-)
-from faststream.confluent.subscriber.asyncapi import (
-    AsyncAPIBatchSubscriber,
-    AsyncAPIDefaultSubscriber,
-    AsyncAPISubscriber,
-)
-from faststream.exceptions import SetupError
+from faststream.confluent.broker.registrator import KafkaRegistrator
 
+if TYPE_CHECKING:
+    from confluent_kafka import Message
+    from fast_depends.dependencies import Depends
+
+    from faststream.broker.types import (
+        BrokerMiddleware,
+        CustomCallable,
+        Filter,
+        PublisherMiddleware,
+        SubscriberMiddleware,
+    )
+    from faststream.confluent.message import KafkaMessage
+    from faststream.types import SendableMessage
 
-class KafkaRegistrator(ABCBroker[Union[
-    Message,
-    Tuple[Message, ...],
-]]):
-    """Includable to KafkaBroker router."""
 
-    _subscribers: Dict[int, Union[AsyncAPIBatchSubscriber, AsyncAPIDefaultSubscriber]]
-    _publishers: Dict[int, Union[AsyncAPIBatchPublisher, AsyncAPIDefaultPublisher]]
+class KafkaPublisher(ArgsContainer):
+    """Delayed KafkaPublisher registration object.
 
-    @override
-    def subscriber(  # type: ignore[override]
-        self,
-        *topics: str,
-        group_id: Optional[str] = None,
-        key_deserializer: Optional[Callable[[bytes], Any]] = None,
-        value_deserializer: Optional[Callable[[bytes], Any]] = None,
-        fetch_max_wait_ms: int = 500,
-        fetch_max_bytes: int = 52428800,
-        fetch_min_bytes: int = 1,
-        max_partition_fetch_bytes: int = 1 * 1024 * 1024,
-        auto_offset_reset: Literal[
-            "latest",
-            "earliest",
-            "none"
-        ] = "latest",
-        auto_commit: bool = True,
-        auto_commit_interval_ms: int = 5 * 1000,
-        check_crcs: bool = True,
-        partition_assignment_strategy: Sequence[str] = (
-            "roundrobin",
-        ),
-        max_poll_interval_ms: int = 5 * 60 * 1000,
-        rebalance_timeout_ms: Optional[int] = None,
-        session_timeout_ms: int = 10 * 1000,
-        heartbeat_interval_ms: int = 3 * 1000,
-        consumer_timeout_ms: int = 200,
-        max_poll_records: Optional[int] = None,
-        exclude_internal_topics: bool = True,
-        isolation_level: Literal[
-            "read_uncommitted",
-            "read_committed"
-        ] = "read_uncommitted",
-        batch: bool = False,
-        max_records: Optional[int] = None,
-        batch_timeout_ms: int = 200,
-        # broker args
-        dependencies: Annotated[
-            Iterable[Depends],
-            Doc("Dependencies list (`[Depends(),]`) to apply to the subscriber."),
-        ] = (),
-        parser: Annotated[
-            Optional[
-                Union[
-                    CustomParser[Message],
-                    CustomParser[Tuple[Message, ...]],
-                ]
-            ],
-            Doc("Parser to map original **Message** object to FastStream one."),
-        ] = None,
-        decoder: Annotated[
-            Optional[
-                Union[
-                    CustomDecoder[StreamMessage[Message]],
-                    CustomDecoder[StreamMessage[Tuple[Message, ...]]],
-                ]
-            ],
-            Doc("Function to decode FastStream msg bytes body to python objects."),
-        ] = None,
-        middlewares: Annotated[
-            Iterable[SubscriberMiddleware],
-            Doc("Subscriber middlewares to wrap incoming message processing."),
-        ] = (),
-        filter: Annotated[
-            Union[
-                Filter[StreamMessage[Message]],
-                Filter[StreamMessage[Tuple[Message, ...]]],
-            ],
-            Doc(
-                "Overload subscriber to consume various messages from the same source."
-            ),
-            deprecated(
-                "Deprecated in **FastStream 0.5.0**. "
-                "Please, create `subscriber` object and use it explicitly instead. "
-                "Argument will be removed in **FastStream 0.6.0**."
-            ),
-        ] = default_filter,
-        retry: Annotated[
-            bool,
-            Doc("Whether to `nack` message at processing exception."),
-        ] = False,
-        no_ack: Annotated[
-            bool,
-            Doc("Whether to disable **FastStream** autoacknowledgement logic or not."),
-        ] = False,
-        # AsyncAPI args
-        title: Annotated[
-            Optional[str],
-            Doc("AsyncAPI subscriber object title."),
-        ] = None,
-        description: Annotated[
-            Optional[str],
-            Doc(
-                "AsyncAPI subscriber object description. "
-                "Uses decorated docstring as default."
-            ),
-        ] = None,
-        include_in_schema: Annotated[
-            bool,
-            Doc("Whetever to include operation in AsyncAPI schema or not."),
-        ] = True,
-    ) -> AsyncAPISubscriber:
-        if not auto_commit and not group_id:
-            raise SetupError(
-                "You should install `group_id` with manual commit mode")
+    Just a copy of `KafkaRegistrator.publisher(...)` arguments.
+    """
 
-        builder = partial(
-            AsyncConfluentConsumer,
-            key_deserializer=key_deserializer,
-            value_deserializer=value_deserializer,
-            fetch_max_wait_ms=fetch_max_wait_ms,
-            fetch_max_bytes=fetch_max_bytes,
-            fetch_min_bytes=fetch_min_bytes,
-            max_partition_fetch_bytes=max_partition_fetch_bytes,
-            auto_offset_reset=auto_offset_reset,
-            enable_auto_commit=auto_commit,
-            auto_commit_interval_ms=auto_commit_interval_ms,
-            check_crcs=check_crcs,
-            partition_assignment_strategy=partition_assignment_strategy,
-            max_poll_interval_ms=max_poll_interval_ms,
-            rebalance_timeout_ms=rebalance_timeout_ms,
-            session_timeout_ms=session_timeout_ms,
-            heartbeat_interval_ms=heartbeat_interval_ms,
-            consumer_timeout_ms=consumer_timeout_ms,
-            max_poll_records=max_poll_records,
-            exclude_internal_topics=exclude_internal_topics,
-            isolation_level=isolation_level,
-        )
-
-        subscriber = cast(
-            AsyncAPISubscriber,
-            super().subscriber(
-                AsyncAPISubscriber.create(
-                    *topics,
-                    batch=batch,
-                    batch_timeout_ms=batch_timeout_ms,
-                    max_records=max_records,
-                    group_id=group_id,
-                    builder=builder,
-                    is_manual=not auto_commit,
-                    # subscriber args
-                    no_ack=no_ack,
-                    retry=retry,
-                    broker_middlewares=self._middlewares,
-                    broker_dependencies=self._dependencies,
-                    # AsyncAPI
-                    title_=title,
-                    description_=description,
-                    include_in_schema=self._solve_include_in_schema(
-                        include_in_schema),
-                )
-            ),
-        )
-
-        return subscriber.add_call(
-            filter_=filter,
-            parser_=parser or self._parser,
-            decoder_=decoder or self._decoder,
-            dependencies_=dependencies,
-            middlewares_=middlewares,
-        )
-
-    @overload  # type: ignore[override]
-    def publisher(
+    def __init__(
         self,
         topic: Annotated[
             str,
             Doc("Topic where the message will be published."),
         ],
         *,
         key: Annotated[
@@ -239,29 +64,29 @@
             selected using the configured `partitioner`.
             """),
         ] = None,
         headers: Annotated[
             Optional[Dict[str, str]],
             Doc(
                 "Message headers to store metainformation. "
-                "**content-type** and **correlation_id** will be setted automatically by framework anyway. "
+                "**content-type** and **correlation_id** will be set automatically by framework anyway. "
                 "Can be overridden by `publish.headers` if specified."
             ),
         ] = None,
         reply_to: Annotated[
             str,
             Doc("Topic name to send response."),
         ] = "",
         batch: Annotated[
-            Literal[False],
+            bool,
             Doc("Whether to send messages in batches or not."),
         ] = False,
         # basic args
         middlewares: Annotated[
-            Iterable[PublisherMiddleware],
+            Iterable["PublisherMiddleware"],
             Doc("Publisher middlewares to wrap outgoing messages."),
         ] = (),
         # AsyncAPI args
         title: Annotated[
             Optional[str],
             Doc("AsyncAPI publisher object title."),
         ] = None,
@@ -276,255 +101,429 @@
                 "Should be any python-native object annotation or `pydantic.BaseModel`."
             ),
         ] = None,
         include_in_schema: Annotated[
             bool,
             Doc("Whetever to include operation in AsyncAPI schema or not."),
         ] = True,
-    ) -> AsyncAPIDefaultPublisher: ...
+    ) -> None:
+        super().__init__(
+            topic=topic,
+            key=key,
+            partition=partition,
+            batch=batch,
+            headers=headers,
+            reply_to=reply_to,
+            # basic args
+            middlewares=middlewares,
+            # AsyncAPI args
+            title=title,
+            description=description,
+            schema=schema,
+            include_in_schema=include_in_schema,
+        )
+
 
-    @overload
-    def publisher(
+class KafkaRoute(SubscriberRoute):
+    """Class to store delaied KafkaBroker subscriber registration."""
+
+    def __init__(
         self,
-        topic: Annotated[
+        call: Annotated[
+            Callable[..., "SendableMessage"],
+            Doc("Message handler function."),
+        ],
+        *topics: Annotated[
             str,
-            Doc("Topic where the message will be published."),
+            Doc("Kafka topics to consume messages from."),
         ],
-        *,
-        key: Annotated[
-            Union[bytes, Any, None],
-            Doc("""
-            A key to associate with the message. Can be used to
-            determine which partition to send the message to. If partition
-            is `None` (and producer's partitioner config is left as default),
-            then messages with the same key will be delivered to the same
-            partition (but if key is `None`, partition is chosen randomly).
-            Must be type `bytes`, or be serializable to bytes via configured
-            `key_serializer`.
-            """),
-        ] = None,
-        partition: Annotated[
-            Optional[int],
+        publishers: Annotated[
+            Iterable[KafkaPublisher],
+            Doc("Kafka publishers to broadcast the handler result."),
+        ] = (),
+        group_id: Annotated[
+            Optional[str],
             Doc("""
-            Specify a partition. If not set, the partition will be
-            selected using the configured `partitioner`.
+            Name of the consumer group to join for dynamic
+            partition assignment (if enabled), and to use for fetching and
+            committing offsets. If `None`, auto-partition assignment (via
+            group coordinator) and offset commits are disabled.
             """),
         ] = None,
-        headers: Annotated[
-            Optional[Dict[str, str]],
+        key_deserializer: Annotated[
+            Optional[Callable[[bytes], Any]],
             Doc(
-                "Message headers to store metainformation. "
-                "**content-type** and **correlation_id** will be setted automatically by framework anyway. "
-                "Can be overridden by `publish.headers` if specified."
+                "Any callable that takes a raw message `bytes` "
+                "key and returns a deserialized one."
             ),
         ] = None,
-        reply_to: Annotated[
-            str,
-            Doc("Topic name to send response."),
-        ] = "",
-        batch: Annotated[
-            Literal[True],
-            Doc("Whether to send messages in batches or not."),
-        ],
-        # basic args
-        middlewares: Annotated[
-            Iterable[PublisherMiddleware],
-            Doc("Publisher middlewares to wrap outgoing messages."),
-        ] = (),
-        # AsyncAPI args
-        title: Annotated[
-            Optional[str],
-            Doc("AsyncAPI publisher object title."),
-        ] = None,
-        description: Annotated[
-            Optional[str],
-            Doc("AsyncAPI publisher object description."),
-        ] = None,
-        schema: Annotated[
-            Optional[Any],
+        value_deserializer: Annotated[
+            Optional[Callable[[bytes], Any]],
             Doc(
-                "AsyncAPI publishing message type. "
-                "Should be any python-native object annotation or `pydantic.BaseModel`."
+                "Any callable that takes a raw message `bytes` "
+                "value and returns a deserialized value."
             ),
         ] = None,
-        include_in_schema: Annotated[
+        fetch_max_wait_ms: Annotated[
+            int,
+            Doc("""
+            The maximum amount of time in milliseconds
+            the server will block before answering the fetch request if
+            there isn't sufficient data to immediately satisfy the
+            requirement given by `fetch_min_bytes`.
+            """),
+        ] = 500,
+        fetch_max_bytes: Annotated[
+            int,
+            Doc("""
+            The maximum amount of data the server should
+            return for a fetch request. This is not an absolute maximum, if
+            the first message in the first non-empty partition of the fetch
+            is larger than this value, the message will still be returned
+            to ensure that the consumer can make progress. NOTE: consumer
+            performs fetches to multiple brokers in parallel so memory
+            usage will depend on the number of brokers containing
+            partitions for the topic.
+            """),
+        ] = 50 * 1024 * 1024,
+        fetch_min_bytes: Annotated[
+            int,
+            Doc("""
+            Minimum amount of data the server should
+            return for a fetch request, otherwise wait up to
+            `fetch_max_wait_ms` for more data to accumulate.
+            """),
+        ] = 1,
+        max_partition_fetch_bytes: Annotated[
+            int,
+            Doc("""
+            The maximum amount of data
+            per-partition the server will return. The maximum total memory
+            used for a request ``= #partitions * max_partition_fetch_bytes``.
+            This size must be at least as large as the maximum message size
+            the server allows or else it is possible for the producer to
+            send messages larger than the consumer can fetch. If that
+            happens, the consumer can get stuck trying to fetch a large
+            message on a certain partition.
+            """),
+        ] = 1 * 1024 * 1024,
+        auto_offset_reset: Annotated[
+            Literal["latest", "earliest", "none"],
+            Doc("""
+            A policy for resetting offsets on `OffsetOutOfRangeError` errors:
+
+            * `earliest` will move to the oldest available message
+            * `latest` will move to the most recent
+            * `none` will raise an exception so you can handle this case
+            """),
+        ] = "latest",
+        auto_commit: Annotated[
             bool,
-            Doc("Whetever to include operation in AsyncAPI schema or not."),
+            Doc("""
+            If `True` the consumer's offset will be
+            periodically committed in the background.
+            """),
         ] = True,
-    ) -> AsyncAPIBatchPublisher: ...
-
-    @overload
-    def publisher(
-        self,
-        topic: Annotated[
-            str,
-            Doc("Topic where the message will be published."),
-        ],
-        *,
-        key: Annotated[
-            Union[bytes, Any, None],
+        auto_commit_interval_ms: Annotated[
+            int,
             Doc("""
-            A key to associate with the message. Can be used to
-            determine which partition to send the message to. If partition
-            is `None` (and producer's partitioner config is left as default),
-            then messages with the same key will be delivered to the same
-            partition (but if key is `None`, partition is chosen randomly).
-            Must be type `bytes`, or be serializable to bytes via configured
-            `key_serializer`.
+            Milliseconds between automatic
+            offset commits, if `auto_commit` is `True`."""),
+        ] = 5 * 1000,
+        check_crcs: Annotated[
+            bool,
+            Doc("""
+            Automatically check the CRC32 of the records
+            consumed. This ensures no on-the-wire or on-disk corruption to
+            the messages occurred. This check adds some overhead, so it may
+            be disabled in cases seeking extreme performance.
             """),
-        ] = None,
-        partition: Annotated[
+        ] = True,
+        partition_assignment_strategy: Annotated[
+            Sequence[str],
+            Doc("""
+            List of objects to use to
+            distribute partition ownership amongst consumer instances when
+            group management is used. This preference is implicit in the order
+            of the strategies in the list. When assignment strategy changes:
+            to support a change to the assignment strategy, new versions must
+            enable support both for the old assignment strategy and the new
+            one. The coordinator will choose the old assignment strategy until
+            all members have been updated. Then it will choose the new
+            strategy.
+            """),
+        ] = ("roundrobin",),
+        max_poll_interval_ms: Annotated[
+            int,
+            Doc("""
+            Maximum allowed time between calls to
+            consume messages in batches. If this interval
+            is exceeded the consumer is considered failed and the group will
+            rebalance in order to reassign the partitions to another consumer
+            group member. If API methods block waiting for messages, that time
+            does not count against this timeout.
+            """),
+        ] = 5 * 60 * 1000,
+        rebalance_timeout_ms: Annotated[
             Optional[int],
             Doc("""
-            Specify a partition. If not set, the partition will be
-            selected using the configured `partitioner`.
+            The maximum time server will wait for this
+            consumer to rejoin the group in a case of rebalance. In Java client
+            this behaviour is bound to `max.poll.interval.ms` configuration,
+            but as ``aiokafka`` will rejoin the group in the background, we
+            decouple this setting to allow finer tuning by users that use
+            `ConsumerRebalanceListener` to delay rebalacing. Defaults
+            to ``session_timeout_ms``
             """),
         ] = None,
-        headers: Annotated[
-            Optional[Dict[str, str]],
-            Doc(
-                "Message headers to store metainformation. "
-                "**content-type** and **correlation_id** will be setted automatically by framework anyway. "
-                "Can be overridden by `publish.headers` if specified."
-            ),
+        session_timeout_ms: Annotated[
+            int,
+            Doc("""
+            Client group session and failure detection
+            timeout. The consumer sends periodic heartbeats
+            (`heartbeat.interval.ms`) to indicate its liveness to the broker.
+            If no hearts are received by the broker for a group member within
+            the session timeout, the broker will remove the consumer from the
+            group and trigger a rebalance. The allowed range is configured with
+            the **broker** configuration properties
+            `group.min.session.timeout.ms` and `group.max.session.timeout.ms`.
+            """),
+        ] = 10 * 1000,
+        heartbeat_interval_ms: Annotated[
+            int,
+            Doc("""
+            The expected time in milliseconds
+            between heartbeats to the consumer coordinator when using
+            Kafka's group management feature. Heartbeats are used to ensure
+            that the consumer's session stays active and to facilitate
+            rebalancing when new consumers join or leave the group. The
+            value must be set lower than `session_timeout_ms`, but typically
+            should be set no higher than 1/3 of that value. It can be
+            adjusted even lower to control the expected time for normal
+            rebalances.
+            """),
+        ] = 3 * 1000,
+        consumer_timeout_ms: Annotated[
+            int,
+            Doc("""
+            Maximum wait timeout for background fetching
+            routine. Mostly defines how fast the system will see rebalance and
+            request new data for new partitions.
+            """),
+        ] = 200,
+        max_poll_records: Annotated[
+            Optional[int],
+            Doc("""
+            The maximum number of records returned in a
+            single call by batch consumer. Has no limit by default.
+            """),
         ] = None,
-        reply_to: Annotated[
-            str,
-            Doc("Topic name to send response."),
-        ] = "",
+        exclude_internal_topics: Annotated[
+            bool,
+            Doc("""
+            Whether records from internal topics
+            (such as offsets) should be exposed to the consumer. If set to True
+            the only way to receive records from an internal topic is
+            subscribing to it.
+            """),
+        ] = True,
+        isolation_level: Annotated[
+            Literal["read_uncommitted", "read_committed"],
+            Doc("""
+            Controls how to read messages written
+            transactionally.
+
+            * `read_committed`, batch consumer will only return
+            transactional messages which have been committed.
+
+            * `read_uncommitted` (the default), batch consumer will
+            return all messages, even transactional messages which have been
+            aborted.
+
+            Non-transactional messages will be returned unconditionally in
+            either mode.
+
+            Messages will always be returned in offset order. Hence, in
+            `read_committed` mode, batch consumer will only return
+            messages up to the last stable offset (LSO), which is the one less
+            than the offset of the first open transaction. In particular any
+            messages appearing after messages belonging to ongoing transactions
+            will be withheld until the relevant transaction has been completed.
+            As a result, `read_committed` consumers will not be able to read up
+            to the high watermark when there are in flight transactions.
+            Further, when in `read_committed` the seek_to_end method will
+            return the LSO. See method docs below.
+            """),
+        ] = "read_uncommitted",
         batch: Annotated[
             bool,
-            Doc("Whether to send messages in batches or not."),
+            Doc("Whether to consume messages in batches or not."),
         ] = False,
-        # basic args
+        batch_timeout_ms: Annotated[
+            int,
+            Doc("""
+            Milliseconds spent waiting if
+            data is not available in the buffer. If 0, returns immediately
+            with any records that are available currently in the buffer,
+            else returns empty.
+            """),
+        ] = 200,
+        max_records: Annotated[
+            Optional[int],
+            Doc("Number of messages to consume as one batch."),
+        ] = None,
+        # broker args
+        dependencies: Annotated[
+            Iterable["Depends"],
+            Doc("Dependencies list (`[Depends(),]`) to apply to the subscriber."),
+        ] = (),
+        parser: Annotated[
+            Optional["CustomCallable"],
+            Doc("Parser to map original **Message** object to FastStream one."),
+        ] = None,
+        decoder: Annotated[
+            Optional["CustomCallable"],
+            Doc("Function to decode FastStream msg bytes body to python objects."),
+        ] = None,
         middlewares: Annotated[
-            Iterable[PublisherMiddleware],
-            Doc("Publisher middlewares to wrap outgoing messages."),
+            Iterable["SubscriberMiddleware"],
+            Doc("Subscriber middlewares to wrap incoming message processing."),
         ] = (),
+        filter: Annotated[
+            "Filter[KafkaMessage]",
+            Doc(
+                "Overload subscriber to consume various messages from the same source."
+            ),
+            deprecated(
+                "Deprecated in **FastStream 0.5.0**. "
+                "Please, create `subscriber` object and use it explicitly instead. "
+                "Argument will be removed in **FastStream 0.6.0**."
+            ),
+        ] = default_filter,
+        retry: Annotated[
+            bool,
+            Doc("Whether to `nack` message at processing exception."),
+        ] = False,
+        no_ack: Annotated[
+            bool,
+            Doc("Whether to disable **FastStream** autoacknowledgement logic or not."),
+        ] = False,
         # AsyncAPI args
         title: Annotated[
             Optional[str],
-            Doc("AsyncAPI publisher object title."),
+            Doc("AsyncAPI subscriber object title."),
         ] = None,
         description: Annotated[
             Optional[str],
-            Doc("AsyncAPI publisher object description."),
-        ] = None,
-        schema: Annotated[
-            Optional[Any],
             Doc(
-                "AsyncAPI publishing message type. "
-                "Should be any python-native object annotation or `pydantic.BaseModel`."
+                "AsyncAPI subscriber object description. "
+                "Uses decorated docstring as default."
             ),
         ] = None,
         include_in_schema: Annotated[
             bool,
             Doc("Whetever to include operation in AsyncAPI schema or not."),
         ] = True,
-    ) -> Union[
-        AsyncAPIBatchPublisher,
-        AsyncAPIDefaultPublisher,
-    ]: ...
+    ) -> None:
+        super().__init__(
+            call,
+            *topics,
+            publishers=publishers,
+            group_id=group_id,
+            key_deserializer=key_deserializer,
+            value_deserializer=value_deserializer,
+            fetch_max_wait_ms=fetch_max_wait_ms,
+            fetch_max_bytes=fetch_max_bytes,
+            fetch_min_bytes=fetch_min_bytes,
+            max_partition_fetch_bytes=max_partition_fetch_bytes,
+            auto_offset_reset=auto_offset_reset,
+            auto_commit=auto_commit,
+            auto_commit_interval_ms=auto_commit_interval_ms,
+            check_crcs=check_crcs,
+            partition_assignment_strategy=partition_assignment_strategy,
+            max_poll_interval_ms=max_poll_interval_ms,
+            rebalance_timeout_ms=rebalance_timeout_ms,
+            session_timeout_ms=session_timeout_ms,
+            heartbeat_interval_ms=heartbeat_interval_ms,
+            consumer_timeout_ms=consumer_timeout_ms,
+            max_poll_records=max_poll_records,
+            exclude_internal_topics=exclude_internal_topics,
+            isolation_level=isolation_level,
+            max_records=max_records,
+            batch_timeout_ms=batch_timeout_ms,
+            batch=batch,
+            # basic args
+            dependencies=dependencies,
+            parser=parser,
+            decoder=decoder,
+            middlewares=middlewares,
+            filter=filter,
+            # AsyncAPI args
+            title=title,
+            description=description,
+            include_in_schema=include_in_schema,
+            # FastDepends args
+            retry=retry,
+            no_ack=no_ack,
+        )
+
+
+class KafkaRouter(
+    BrokerRouter[
+        Union[
+            "Message",
+            Tuple["Message", ...],
+        ]
+    ],
+    KafkaRegistrator,
+):
+    """Includable to KafkaBroker router."""
 
-    @override
-    def publisher(
+    def __init__(
         self,
-        topic: Annotated[
+        prefix: Annotated[
             str,
-            Doc("Topic where the message will be published."),
-        ],
+            Doc("String prefix to add to all subscribers queues."),
+        ] = "",
+        handlers: Annotated[
+            Iterable[KafkaRoute],
+            Doc("Route object to include."),
+        ] = (),
         *,
-        key: Annotated[
-            Union[bytes, Any, None],
-            Doc("""
-            A key to associate with the message. Can be used to
-            determine which partition to send the message to. If partition
-            is `None` (and producer's partitioner config is left as default),
-            then messages with the same key will be delivered to the same
-            partition (but if key is `None`, partition is chosen randomly).
-            Must be type `bytes`, or be serializable to bytes via configured
-            `key_serializer`.
-            """),
-        ] = None,
-        partition: Annotated[
-            Optional[int],
-            Doc("""
-            Specify a partition. If not set, the partition will be
-            selected using the configured `partitioner`.
-            """),
-        ] = None,
-        headers: Annotated[
-            Optional[Dict[str, str]],
+        dependencies: Annotated[
+            Iterable["Depends"],
             Doc(
-                "Message headers to store metainformation. "
-                "**content-type** and **correlation_id** will be setted automatically by framework anyway. "
-                "Can be overridden by `publish.headers` if specified."
+                "Dependencies list (`[Depends(),]`) to apply to all routers' publishers/subscribers."
             ),
-        ] = None,
-        reply_to: Annotated[
-            str,
-            Doc("Topic name to send response."),
-        ] = "",
-        batch: Annotated[
-            bool,
-            Doc("Whether to send messages in batches or not."),
-        ] = False,
-        # basic args
+        ] = (),
         middlewares: Annotated[
-            Iterable[PublisherMiddleware],
-            Doc("Publisher middlewares to wrap outgoing messages."),
+            Iterable[
+                Union[
+                    "BrokerMiddleware[Message]",
+                    "BrokerMiddleware[Tuple[Message, ...]]",
+                ]
+            ],
+            Doc("Router middlewares to apply to all routers' publishers/subscribers."),
         ] = (),
-        # AsyncAPI args
-        title: Annotated[
-            Optional[str],
-            Doc("AsyncAPI publisher object title."),
-        ] = None,
-        description: Annotated[
-            Optional[str],
-            Doc("AsyncAPI publisher object description."),
+        parser: Annotated[
+            Optional["CustomCallable"],
+            Doc("Parser to map original **Message** object to FastStream one."),
         ] = None,
-        schema: Annotated[
-            Optional[Any],
-            Doc(
-                "AsyncAPI publishing message type. "
-                "Should be any python-native object annotation or `pydantic.BaseModel`."
-            ),
+        decoder: Annotated[
+            Optional["CustomCallable"],
+            Doc("Function to decode FastStream msg bytes body to python objects."),
         ] = None,
         include_in_schema: Annotated[
-            bool,
+            Optional[bool],
             Doc("Whetever to include operation in AsyncAPI schema or not."),
-        ] = True,
-    ) -> Union[
-        AsyncAPIBatchPublisher,
-        AsyncAPIDefaultPublisher,
-    ]:
-        """Creates long-living and AsyncAPI-documented publisher object.
-
-        You can use it as a handler decorator (handler should be decorated by `@broker.subscriber(...)` too) - `@broker.publisher(...)`.
-        In such case publisher will publish your handler return value.
-
-        Or you can create a publisher object to call it lately - `broker.publisher(...).publish(...)`.
-        """
-        publisher = AsyncAPIPublisher.create(
-            # batch flag
-            batch=batch,
-            # default args
-            key=key,
-            # both args
-            topic=topic,
-            partition=partition,
-            headers=headers,
-            reply_to=reply_to,
-            # publisher-specific
-            broker_middlewares=self._middlewares,
+        ] = None,
+    ) -> None:
+        super().__init__(
+            handlers=handlers,
+            # basic args
+            prefix=prefix,
+            dependencies=dependencies,
             middlewares=middlewares,
-            # AsyncAPI
-            title_=title,
-            description_=description,
-            schema_=schema,
-            include_in_schema=self._solve_include_in_schema(include_in_schema),
+            parser=parser,
+            decoder=decoder,
+            include_in_schema=include_in_schema,
         )
-
-        if batch:
-            return cast(AsyncAPIBatchPublisher, super().publisher(publisher))
-        else:
-            return cast(AsyncAPIDefaultPublisher, super().publisher(publisher))
```

### Comparing `faststream-0.5.0rc0/faststream/confluent/fastapi/__init__.py` & `faststream-0.5.0rc1/faststream/confluent/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/faststream/confluent/fastapi/fastapi.py` & `faststream-0.5.0rc1/faststream/redis/fastapi/fastapi.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,97 +1,114 @@
 import logging
-from enum import Enum
 from inspect import Parameter
 from typing import (
+    TYPE_CHECKING,
     Any,
     Callable,
     Dict,
     Iterable,
     List,
-    Literal,
+    Mapping,
     Optional,
     Sequence,
-    Tuple,
     Type,
     Union,
     cast,
 )
 
-from confluent_kafka import Message
-from fastapi import params
 from fastapi.datastructures import Default
 from fastapi.routing import APIRoute
-from fastapi.types import IncEx
 from fastapi.utils import generate_unique_id
-from starlette.responses import JSONResponse, Response
+from redis.asyncio.connection import (
+    Connection,
+    DefaultParser,
+    Encoder,
+)
+from starlette.responses import JSONResponse
 from starlette.routing import BaseRoute
-from starlette.types import ASGIApp, Lifespan
 from typing_extensions import Annotated, Doc, deprecated, override
 
 from faststream.__about__ import SERVICE_NAME
-from faststream.asyncapi import schema as asyncapi
 from faststream.broker.fastapi.router import StreamRouter
-from faststream.broker.message import StreamMessage
-from faststream.broker.types import (
-    BrokerMiddleware,
-    CustomDecoder,
-    CustomParser,
-    Filter,
-    PublisherMiddleware,
-    SubscriberMiddleware,
-)
 from faststream.broker.utils import default_filter
-from faststream.confluent.broker.broker import KafkaBroker as KB
-from faststream.confluent.publisher.asyncapi import AsyncAPIPublisher
-from faststream.confluent.subscriber.asyncapi import AsyncAPISubscriber
-from faststream.security import BaseSecurity
-from faststream.types import AnyDict
+from faststream.redis.broker.broker import RedisBroker as RB
+from faststream.redis.message import UnifyRedisDict
+from faststream.redis.publisher.asyncapi import AsyncAPIPublisher
+from faststream.redis.schemas import ListSub, PubSub, StreamSub
+from faststream.redis.subscriber.asyncapi import AsyncAPISubscriber
+
+if TYPE_CHECKING:
+    from enum import Enum
+
+    from fastapi import params
+    from fastapi.types import IncEx
+    from redis.asyncio.connection import BaseParser
+    from starlette.responses import Response
+    from starlette.types import ASGIApp, Lifespan
+
+    from faststream.asyncapi import schema as asyncapi
+    from faststream.broker.types import (
+        BrokerMiddleware,
+        CustomCallable,
+        Filter,
+        PublisherMiddleware,
+        SubscriberMiddleware,
+    )
+    from faststream.redis.message import UnifyRedisMessage
+    from faststream.security import BaseSecurity
+    from faststream.types import AnyDict, LoggerProto
 
 
-class KafkaRouter(StreamRouter[Union[Message, Tuple[Message, ...]]]):
-    """A class to represent a Kafka router."""
+class RedisRouter(StreamRouter[UnifyRedisDict]):
+    """A class to represent a Redis router."""
 
-    broker_class = KB
-    broker: KB
+    broker_class = RB
+    broker: RB
 
     def __init__(
         self,
-        bootstrap_servers: Union[str, Iterable[str]] = "localhost",
+        url: str = "redis://localhost:6379",
+        polling_interval: Optional[float] = None,
         *,
-        client_id: Annotated[
-            Optional[str],
-            Doc("Application name to mark connections by."),
-        ] = SERVICE_NAME,
+        host: str = "localhost",
+        port: Union[str, int] = 6379,
+        db: Union[str, int] = 0,
+        client_name: Optional[str] = SERVICE_NAME,
+        health_check_interval: float = 0,
+        max_connections: Optional[int] = None,
+        socket_timeout: Optional[float] = None,
+        socket_connect_timeout: Optional[float] = None,
+        socket_read_size: int = 65536,
+        socket_keepalive: bool = False,
+        socket_keepalive_options: Optional[Mapping[int, Union[int, bytes]]] = None,
+        socket_type: int = 0,
+        retry_on_timeout: bool = False,
+        encoding: str = "utf-8",
+        encoding_errors: str = "strict",
+        decode_responses: bool = False,
+        parser_class: Type["BaseParser"] = DefaultParser,
+        connection_class: Type["Connection"] = Connection,
+        encoder_class: Type["Encoder"] = Encoder,
         # broker base args
         graceful_timeout: Annotated[
             Optional[float],
             Doc(
                 "Graceful shutdown timeout. Broker waits for all running subscribers completion before shut down."
             ),
         ] = 15.0,
         decoder: Annotated[
-            Optional[
-                Union[
-                    CustomDecoder[StreamMessage[Message]],
-                    CustomDecoder[StreamMessage[Tuple[Message, ...]]],
-                ]
-            ],
+            Optional["CustomCallable"],
             Doc("Custom decoder object."),
         ] = None,
         parser: Annotated[
-            Optional[Union[CustomParser[Message], CustomParser[Tuple[Message, ...]]]],
+            Optional["CustomCallable"],
             Doc("Custom parser object."),
         ] = None,
         middlewares: Annotated[
-            Iterable[
-                Union[
-                    BrokerMiddleware[Message],
-                    BrokerMiddleware[Tuple[Message, ...]],
-                ]
-            ],
+            Iterable["BrokerMiddleware[UnifyRedisDict]"],
             Doc("Middlewares to apply to all broker publishers/subscribers."),
         ] = (),
         # AsyncAPI args
         security: Annotated[
             Optional["BaseSecurity"],
             Doc(
                 "Security options to connect broker and generate AsyncAPI server security information."
@@ -104,26 +121,26 @@
         protocol: Annotated[
             Optional[str],
             Doc("AsyncAPI server protocol."),
         ] = None,
         protocol_version: Annotated[
             Optional[str],
             Doc("AsyncAPI server protocol version."),
-        ] = "auto",
+        ] = "custom",
         description: Annotated[
             Optional[str],
             Doc("AsyncAPI server description."),
         ] = None,
         asyncapi_tags: Annotated[
             Optional[Iterable[Union["asyncapi.Tag", "asyncapi.TagDict"]]],
             Doc("AsyncAPI server tags."),
         ] = None,
         # logging args
         logger: Annotated[
-            Union[logging.Logger, None, object],
+            Union["LoggerProto", None, object],
             Doc("User specified logger to pass into Context and log service messages."),
         ] = Parameter.empty,
         log_level: Annotated[
             int,
             Doc("Service messages log level."),
         ] = logging.INFO,
         log_fmt: Annotated[
@@ -355,21 +372,39 @@
                 Read more about it in the
                 [FastAPI docs about how to Generate Clients](https://fastapi.tiangolo.com/advanced/generate-clients/#custom-generate-unique-id-function).
                 """
             ),
         ] = Default(generate_unique_id),
     ) -> None:
         super().__init__(
-            bootstrap_servers=bootstrap_servers,
-            client_id=client_id,
-            # broker args
+            url=url,
+            polling_interval=polling_interval,
+            host=host,
+            port=port,
+            db=db,
+            health_check_interval=health_check_interval,
+            max_connections=max_connections,
+            socket_timeout=socket_timeout,
+            socket_connect_timeout=socket_connect_timeout,
+            socket_read_size=socket_read_size,
+            socket_keepalive=socket_keepalive,
+            socket_keepalive_options=socket_keepalive_options,
+            retry_on_timeout=retry_on_timeout,
+            encoding=encoding,
+            encoding_errors=encoding_errors,
+            decode_responses=decode_responses,
+            parser_class=parser_class,
+            connection_class=connection_class,
+            encoder_class=encoder_class,
             graceful_timeout=graceful_timeout,
             decoder=decoder,
             parser=parser,
             middlewares=middlewares,
+            socket_type=socket_type,
+            client_name=client_name,
             schema_url=schema_url,
             setup_state=setup_state,
             # logger options
             logger=logger,
             log_level=log_level,
             log_fmt=log_fmt,
             # AsyncAPI options
@@ -398,70 +433,81 @@
             lifespan=lifespan,
             generate_unique_id_function=generate_unique_id_function,
         )
 
     @override
     def subscriber(  # type: ignore[override]
         self,
-        *topics: str,
-        group_id: Optional[str] = None,
-        key_deserializer: Optional[Callable[[bytes], Any]] = None,
-        value_deserializer: Optional[Callable[[bytes], Any]] = None,
-        fetch_max_wait_ms: int = 500,
-        fetch_max_bytes: int = 52428800,
-        fetch_min_bytes: int = 1,
-        max_partition_fetch_bytes: int = 1 * 1024 * 1024,
-        auto_offset_reset: Literal[
-            "latest",
-            "earliest",
-            "none",
-        ] = "latest",
-        auto_commit: bool = True,
-        auto_commit_interval_ms: int = 5000,
-        check_crcs: bool = True,
-        partition_assignment_strategy: Sequence[str] = ("roundrobin",),
-        max_poll_interval_ms: int = 300000,
-        rebalance_timeout_ms: Optional[int] = None,
-        session_timeout_ms: int = 10000,
-        heartbeat_interval_ms: int = 3000,
-        consumer_timeout_ms: int = 200,
-        max_poll_records: Optional[int] = None,
-        exclude_internal_topics: bool = True,
-        isolation_level: Literal[
-            "read_uncommitted",
-            "read_committed",
-        ] = "read_uncommitted",
+        channel: Annotated[
+            Union[str, PubSub, None],
+            Doc("Redis PubSub object name to send message."),
+        ] = None,
+        *,
+        list: Annotated[
+            Union[str, ListSub, None],
+            Doc("Redis List object name to send message."),
+        ] = None,
+        stream: Annotated[
+            Union[str, StreamSub, None],
+            Doc("Redis Stream object name to send message."),
+        ] = None,
         # broker arguments
-        dependencies: Iterable[params.Depends] = (),
-        parser: Optional[
-            Union[
-                CustomParser[Message],
-                CustomParser[Tuple[Message, ...]],
-            ]
-        ] = None,
-        decoder: Optional[
-            Union[
-                CustomDecoder[StreamMessage[Message]],
-                CustomDecoder[StreamMessage[Tuple[Message, ...]]],
-            ]
-        ] = None,
-        middlewares: Iterable[SubscriberMiddleware] = (),
-        filter: Union[
-            Filter[StreamMessage[Message]],
-            Filter[StreamMessage[Tuple[Message, ...]]],
+        dependencies: Annotated[
+            Iterable["params.Depends"],
+            Doc("Dependencies list (`[Depends(),]`) to apply to the subscriber."),
+        ] = (),
+        parser: Annotated[
+            Optional["CustomCallable"],
+            Doc(
+                "Parser to map original **aio_pika.IncomingMessage** Msg to FastStream one."
+            ),
+        ] = None,
+        decoder: Annotated[
+            Optional["CustomCallable"],
+            Doc("Function to decode FastStream msg bytes body to python objects."),
+        ] = None,
+        middlewares: Annotated[
+            Iterable["SubscriberMiddleware"],
+            Doc("Subscriber middlewares to wrap incoming message processing."),
+        ] = (),
+        filter: Annotated[
+            "Filter[UnifyRedisMessage]",
+            Doc(
+                "Overload subscriber to consume various messages from the same source."
+            ),
+            deprecated(
+                "Deprecated in **FastStream 0.5.0**. "
+                "Please, create `subscriber` object and use it explicitly instead. "
+                "Argument will be removed in **FastStream 0.6.0**."
+            ),
         ] = default_filter,
-        batch: bool = False,
-        max_records: Optional[int] = None,
-        batch_timeout_ms: int = 200,
-        no_ack: bool = False,
-        retry: bool = False,
+        retry: Annotated[
+            bool,
+            Doc("Whether to `nack` message at processing exception."),
+        ] = False,
+        no_ack: Annotated[
+            bool,
+            Doc("Whether to disable **FastStream** autoacknowledgement logic or not."),
+        ] = False,
         # AsyncAPI information
-        title: Optional[str] = None,
-        description: Optional[str] = None,
-        include_in_schema: bool = True,
+        title: Annotated[
+            Optional[str],
+            Doc("AsyncAPI subscriber object title."),
+        ] = None,
+        description: Annotated[
+            Optional[str],
+            Doc(
+                "AsyncAPI subscriber object description. "
+                "Uses decorated docstring as default."
+            ),
+        ] = None,
+        include_in_schema: Annotated[
+            bool,
+            Doc("Whetever to include operation in AsyncAPI schema or not."),
+        ] = True,
         # FastAPI args
         response_model: Annotated[
             Any,
             Doc(
                 """
                 The type to use for the response.
 
@@ -577,44 +623,28 @@
                 when it makes sense.
 
                 Read more about it in the
                 [FastAPI docs for Response Model - Return Type](https://fastapi.tiangolo.com/tutorial/response-model/#response_model_exclude_none).
                 """
             ),
         ] = False,
-    ) -> AsyncAPISubscriber[Union[Message, Tuple[Message, ...]]]:
+    ) -> AsyncAPISubscriber:
+        list_sub = ListSub.validate(list)
+        channel = PubSub.validate(channel)
+        stream_sub = StreamSub.validate(stream)
+
+        any_of = list_sub or channel or stream_sub
+
         return cast(
-            AsyncAPISubscriber[Union[Message, Tuple[Message, ...]]],
+            AsyncAPISubscriber,
             super().subscriber(
-                topics[0],  # path
-                *topics,
-                group_id=group_id,
-                key_deserializer=key_deserializer,
-                value_deserializer=value_deserializer,
-                fetch_max_wait_ms=fetch_max_wait_ms,
-                fetch_max_bytes=fetch_max_bytes,
-                fetch_min_bytes=fetch_min_bytes,
-                max_partition_fetch_bytes=max_partition_fetch_bytes,
-                auto_offset_reset=auto_offset_reset,
-                auto_commit=auto_commit,
-                auto_commit_interval_ms=auto_commit_interval_ms,
-                check_crcs=check_crcs,
-                partition_assignment_strategy=partition_assignment_strategy,
-                max_poll_interval_ms=max_poll_interval_ms,
-                rebalance_timeout_ms=rebalance_timeout_ms,
-                session_timeout_ms=session_timeout_ms,
-                heartbeat_interval_ms=heartbeat_interval_ms,
-                consumer_timeout_ms=consumer_timeout_ms,
-                max_poll_records=max_poll_records,
-                exclude_internal_topics=exclude_internal_topics,
-                isolation_level=isolation_level,
-                batch=batch,
-                max_records=max_records,
-                batch_timeout_ms=batch_timeout_ms,
-                # broker args
+                path=getattr(any_of, "name", ""),
+                channel=channel,
+                list=list_sub,
+                stream=stream_sub,
                 dependencies=dependencies,
                 parser=parser,
                 decoder=decoder,
                 middlewares=middlewares,
                 filter=filter,
                 retry=retry,
                 no_ack=no_ack,
@@ -631,23 +661,39 @@
                 response_model_exclude_none=response_model_exclude_none,
             ),
         )
 
     @override
     def publisher(  # type: ignore[override]
         self,
-        topic: str,
-        key: Optional[bytes] = None,
-        partition: Optional[int] = None,
-        headers: Optional[Dict[str, str]] = None,
-        reply_to: str = "",
-        batch: bool = False,
-        # basic args
+        channel: Annotated[
+            Union[str, PubSub, None],
+            Doc("Redis PubSub object name to send message."),
+        ] = None,
+        list: Annotated[
+            Union[str, ListSub, None],
+            Doc("Redis List object name to send message."),
+        ] = None,
+        stream: Annotated[
+            Union[str, StreamSub, None],
+            Doc("Redis Stream object name to send message."),
+        ] = None,
+        headers: Annotated[
+            Optional["AnyDict"],
+            Doc(
+                "Message headers to store metainformation. "
+                "Can be overridden by `publish.headers` if specified."
+            ),
+        ] = None,
+        reply_to: Annotated[
+            str,
+            Doc("Reply message destination PubSub object name."),
+        ] = "",
         middlewares: Annotated[
-            Iterable[PublisherMiddleware],
+            Iterable["PublisherMiddleware"],
             Doc("Publisher middlewares to wrap outgoing messages."),
         ] = (),
         # AsyncAPI information
         title: Annotated[
             Optional[str],
             Doc("AsyncAPI publisher object title."),
         ] = None,
@@ -664,19 +710,18 @@
         ] = None,
         include_in_schema: Annotated[
             bool,
             Doc("Whetever to include operation in AsyncAPI schema or not."),
         ] = True,
     ) -> AsyncAPIPublisher:
         return self.broker.publisher(
-            topic=topic,
-            key=key,
-            partition=partition,
+            channel,
+            list=list,
+            stream=stream,
             headers=headers,
-            batch=batch,
             reply_to=reply_to,
             # broker options
             middlewares=middlewares,
             # AsyncAPI options
             title=title,
             description=description,
             schema=schema,
```

### Comparing `faststream-0.5.0rc0/faststream/confluent/publisher/asyncapi.py` & `faststream-0.5.0rc1/faststream/confluent/publisher/asyncapi.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,45 @@
-from typing import Any, Dict, Iterable, Literal, Optional, Tuple, Union, overload
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Dict,
+    Iterable,
+    Literal,
+    Optional,
+    Tuple,
+    Union,
+    overload,
+)
 
-from confluent_kafka import Message as ConfluentMsg
 from typing_extensions import override
 
 from faststream.asyncapi.schema import (
     Channel,
     ChannelBinding,
     CorrelationId,
     Message,
     Operation,
 )
 from faststream.asyncapi.schema.bindings import kafka
 from faststream.asyncapi.utils import resolve_payloads
-from faststream.broker.types import BrokerMiddleware, PublisherMiddleware
+from faststream.broker.types import MsgType
 from faststream.confluent.publisher.usecase import (
     BatchPublisher,
     DefaultPublisher,
     LogicPublisher,
 )
 from faststream.exceptions import SetupError
 
+if TYPE_CHECKING:
+    from confluent_kafka import Message as ConfluentMsg
+
+    from faststream.broker.types import BrokerMiddleware, PublisherMiddleware
+
 
-class AsyncAPIPublisher(LogicPublisher):
+class AsyncAPIPublisher(LogicPublisher[MsgType]):
     """A class representing a publisher."""
 
     def get_name(self) -> str:
         return f"{self.topic}:Publisher"
 
     def get_schema(self) -> Dict[str, Channel]:
         payloads = self.get_payloads()
@@ -53,88 +67,83 @@
         batch: Literal[True],
         key: Optional[bytes],
         topic: str,
         partition: Optional[int],
         headers: Optional[Dict[str, str]],
         reply_to: str,
         # Publisher args
-        broker_middlewares: Iterable[BrokerMiddleware[Tuple[ConfluentMsg, ...]]],
-        middlewares: Iterable[PublisherMiddleware],
+        broker_middlewares: Iterable["BrokerMiddleware[Tuple[ConfluentMsg, ...]]"],
+        middlewares: Iterable["PublisherMiddleware"],
         # AsyncAPI args
         schema_: Optional[Any],
         title_: Optional[str],
         description_: Optional[str],
         include_in_schema: bool,
-    ) -> "AsyncAPIBatchPublisher":
-        ...
+    ) -> "AsyncAPIBatchPublisher": ...
 
     @overload
     @staticmethod
     def create(
         *,
         batch: Literal[False],
         key: Optional[bytes],
         topic: str,
         partition: Optional[int],
         headers: Optional[Dict[str, str]],
         reply_to: str,
         # Publisher args
-        broker_middlewares: Iterable[BrokerMiddleware[ConfluentMsg]],
-        middlewares: Iterable[PublisherMiddleware],
+        broker_middlewares: Iterable["BrokerMiddleware[ConfluentMsg]"],
+        middlewares: Iterable["PublisherMiddleware"],
         # AsyncAPI args
         schema_: Optional[Any],
         title_: Optional[str],
         description_: Optional[str],
         include_in_schema: bool,
-    ) -> "AsyncAPIDefaultPublisher":
-        ...
+    ) -> "AsyncAPIDefaultPublisher": ...
 
     @overload
     @staticmethod
     def create(
         *,
         batch: bool,
         key: Optional[bytes],
         topic: str,
         partition: Optional[int],
         headers: Optional[Dict[str, str]],
         reply_to: str,
         # Publisher args
-        broker_middlewares: Iterable[BrokerMiddleware[Union[
-            Tuple[ConfluentMsg, ...],
-            ConfluentMsg
-        ]]],
-        middlewares: Iterable[PublisherMiddleware],
+        broker_middlewares: Iterable[
+            "BrokerMiddleware[Union[Tuple[ConfluentMsg, ...], ConfluentMsg]]"
+        ],
+        middlewares: Iterable["PublisherMiddleware"],
         # AsyncAPI args
         schema_: Optional[Any],
         title_: Optional[str],
         description_: Optional[str],
         include_in_schema: bool,
     ) -> Union[
         "AsyncAPIBatchPublisher",
         "AsyncAPIDefaultPublisher",
-    ]:
-        ...
+    ]: ...
 
     @override
     @staticmethod
     def create(
         *,
         batch: bool,
         key: Optional[bytes],
         topic: str,
         partition: Optional[int],
         headers: Optional[Dict[str, str]],
         reply_to: str,
         # Publisher args
-        broker_middlewares: Iterable[BrokerMiddleware[Union[
-            Tuple[ConfluentMsg, ...],
-            ConfluentMsg
-        ]]],
-        middlewares: Iterable[PublisherMiddleware],
+        broker_middlewares: Iterable[
+            "BrokerMiddleware[Union[Tuple[ConfluentMsg, ...], ConfluentMsg]]"
+        ],
+        middlewares: Iterable["PublisherMiddleware"],
         # AsyncAPI args
         schema_: Optional[Any],
         title_: Optional[str],
         description_: Optional[str],
         include_in_schema: bool,
     ) -> Union[
         "AsyncAPIBatchPublisher",
@@ -169,13 +178,19 @@
                 schema_=schema_,
                 title_=title_,
                 description_=description_,
                 include_in_schema=include_in_schema,
             )
 
 
-class AsyncAPIBatchPublisher(BatchPublisher, AsyncAPIPublisher):
+class AsyncAPIBatchPublisher(
+    BatchPublisher,
+    AsyncAPIPublisher[Tuple["ConfluentMsg", ...]],
+):
     pass
 
 
-class AsyncAPIDefaultPublisher(DefaultPublisher, AsyncAPIPublisher):
+class AsyncAPIDefaultPublisher(
+    DefaultPublisher,
+    AsyncAPIPublisher["ConfluentMsg"],
+):
     pass
```

### Comparing `faststream-0.5.0rc0/faststream/confluent/publisher/producer.py` & `faststream-0.5.0rc1/faststream/confluent/publisher/producer.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,35 @@
-from typing import Dict, Optional
+from typing import TYPE_CHECKING, Dict, Optional
 
 from typing_extensions import override
 
 from faststream.broker.message import encode_message
 from faststream.broker.publisher.proto import ProducerProto
-from faststream.confluent.client import AsyncConfluentProducer
 from faststream.exceptions import NOT_CONNECTED_YET
-from faststream.types import SendableMessage
+
+if TYPE_CHECKING:
+    from faststream.confluent.client import AsyncConfluentProducer
+    from faststream.types import SendableMessage
 
 
 class AsyncConfluentFastProducer(ProducerProto):
     """A class to represent Kafka producer."""
 
-    _producer: Optional[AsyncConfluentProducer]
+    _producer: Optional["AsyncConfluentProducer"]
 
     def __init__(
         self,
-        producer: AsyncConfluentProducer,
+        producer: "AsyncConfluentProducer",
     ) -> None:
         self._producer = producer
 
     @override
     async def publish(  # type: ignore[override]
         self,
-        message: SendableMessage,
+        message: "SendableMessage",
         topic: str,
         *,
         key: Optional[bytes] = None,
         partition: Optional[int] = None,
         timestamp_ms: Optional[int] = None,
         headers: Optional[Dict[str, str]] = None,
         correlation_id: str = "",
@@ -52,41 +54,37 @@
 
         await self._producer.send(
             topic=topic,
             value=message,
             key=key,
             partition=partition,
             timestamp_ms=timestamp_ms,
-            headers=[(i, (j or "").encode())
-                     for i, j in headers_to_send.items()],
+            headers=[(i, (j or "").encode()) for i, j in headers_to_send.items()],
         )
 
     async def stop(self) -> None:
         if self._producer is not None:  # pragma: no branch
             await self._producer.stop()
 
     async def publish_batch(
         self,
-        *msgs: SendableMessage,
+        *msgs: "SendableMessage",
         topic: str,
         partition: Optional[int] = None,
         timestamp_ms: Optional[int] = None,
         headers: Optional[Dict[str, str]] = None,
         reply_to: str = "",
         correlation_id: str = "",
     ) -> None:
         """Publish a batch of messages to a topic."""
         assert self._producer, NOT_CONNECTED_YET  # nosec B101
 
         batch = self._producer.create_batch()
 
-        headers_to_send = {
-            "correlation_id": correlation_id,
-            **(headers or {})
-        }
+        headers_to_send = {"correlation_id": correlation_id, **(headers or {})}
 
         if reply_to:
             headers_to_send["reply_to"] = headers_to_send.get(
                 "reply_to",
                 reply_to,
             )
```

### Comparing `faststream-0.5.0rc0/faststream/confluent/publisher/usecase.py` & `faststream-0.5.0rc1/faststream/confluent/publisher/usecase.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 from contextlib import AsyncExitStack
 from itertools import chain
-from typing import Any, Dict, Iterable, Optional, Tuple, Union, cast
+from typing import TYPE_CHECKING, Any, Dict, Iterable, Optional, Tuple, Union, cast
 
 from confluent_kafka import Message
 from typing_extensions import override
 
 from faststream.broker.message import gen_cor_id
 from faststream.broker.publisher.usecase import PublisherUsecase
-from faststream.broker.types import BrokerMiddleware, MsgType, PublisherMiddleware
-from faststream.confluent.publisher.producer import AsyncConfluentFastProducer
+from faststream.broker.types import MsgType
 from faststream.exceptions import NOT_CONNECTED_YET
-from faststream.types import AnyDict, SendableMessage
+
+if TYPE_CHECKING:
+    from faststream.broker.types import BrokerMiddleware, PublisherMiddleware
+    from faststream.confluent.publisher.producer import AsyncConfluentFastProducer
+    from faststream.types import AnyDict, SendableMessage
 
 
 class LogicPublisher(PublisherUsecase[MsgType]):
     """A class to publish messages to a Kafka topic."""
 
-    _producer: Optional[AsyncConfluentFastProducer]
+    _producer: Optional["AsyncConfluentFastProducer"]
 
     def __init__(
         self,
         *,
         topic: str,
         partition: Optional[int],
         headers: Optional[Dict[str, str]],
         reply_to: Optional[str],
         # Publisher args
-        broker_middlewares: Iterable[BrokerMiddleware[MsgType]],
-        middlewares: Iterable[PublisherMiddleware],
+        broker_middlewares: Iterable["BrokerMiddleware[MsgType]"],
+        middlewares: Iterable["PublisherMiddleware"],
         # AsyncAPI args
         schema_: Optional[Any],
         title_: Optional[str],
         description_: Optional[str],
         include_in_schema: bool,
     ) -> None:
         super().__init__(
@@ -64,16 +67,16 @@
         *,
         key: Optional[bytes],
         topic: str,
         partition: Optional[int],
         headers: Optional[Dict[str, str]],
         reply_to: Optional[str],
         # Publisher args
-        broker_middlewares: Iterable[BrokerMiddleware[Message]],
-        middlewares: Iterable[PublisherMiddleware],
+        broker_middlewares: Iterable["BrokerMiddleware[Message]"],
+        middlewares: Iterable["PublisherMiddleware"],
         # AsyncAPI args
         schema_: Optional[Any],
         title_: Optional[str],
         description_: Optional[str],
         include_in_schema: bool,
     ) -> None:
         super().__init__(
@@ -92,25 +95,25 @@
         )
 
         self.key = key
 
     @override
     async def publish(
         self,
-        message: SendableMessage,
+        message: "SendableMessage",
         topic: str = "",
         *,
         key: Optional[bytes] = None,
         partition: Optional[int] = None,
         timestamp_ms: Optional[int] = None,
         headers: Optional[Dict[str, str]] = None,
         correlation_id: Optional[str] = None,
         reply_to: str = "",
         # publisher specific
-        _extra_middlewares: Iterable[PublisherMiddleware] = (),
+        _extra_middlewares: Iterable["PublisherMiddleware"] = (),
     ) -> None:
         assert self._producer, NOT_CONNECTED_YET  # nosec B101
 
         kwargs: "AnyDict" = {
             "key": key or self.key,
             # basic args
             "topic": topic or self.topic,
@@ -123,60 +126,56 @@
 
         async with AsyncExitStack() as stack:
             for m in chain(
                 _extra_middlewares
                 or (m(None).publish_scope for m in self._broker_middlewares),
                 self._middlewares,
             ):
-                message = await stack.enter_async_context(
-                    m(message, **kwargs)
-                )
+                message = await stack.enter_async_context(m(message, **kwargs))
 
             return await self._producer.publish(message=message, **kwargs)
 
         return None
 
 
 class BatchPublisher(LogicPublisher[Tuple[Message, ...]]):
     @override
     async def publish(  # type: ignore[override]
         self,
-        message: Union[SendableMessage, Iterable[SendableMessage]],
-        *extra_messages: SendableMessage,
+        message: Union["SendableMessage", Iterable["SendableMessage"]],
+        *extra_messages: "SendableMessage",
         topic: str = "",
         partition: Optional[int] = None,
         timestamp_ms: Optional[int] = None,
         headers: Optional[Dict[str, str]] = None,
         reply_to: str = "",
         correlation_id: Optional[str] = None,
         # publisher specific
-        _extra_middlewares: Iterable[PublisherMiddleware] = (),
+        _extra_middlewares: Iterable["PublisherMiddleware"] = (),
     ) -> None:
         assert self._producer, NOT_CONNECTED_YET  # nosec B101
 
-        msgs: Iterable[SendableMessage]
+        msgs: Iterable["SendableMessage"]
         if extra_messages:
-            msgs = (cast(SendableMessage, message), *extra_messages)
+            msgs = (cast("SendableMessage", message), *extra_messages)
         else:
-            msgs = cast(Iterable[SendableMessage], message)
+            msgs = cast(Iterable["SendableMessage"], message)
 
         kwargs: "AnyDict" = {
             "topic": topic or self.topic,
             "partition": partition or self.partition,
             "timestamp_ms": timestamp_ms,
             "headers": headers or self.headers,
             "reply_to": reply_to or self.reply_to,
             "correlation_id": correlation_id or gen_cor_id(),
         }
 
         async with AsyncExitStack() as stack:
             wrapped_messages = [
-                await stack.enter_async_context(
-                    middleware(msg, **kwargs)
-                )
+                await stack.enter_async_context(middleware(msg, **kwargs))
                 for msg in msgs
                 for middleware in chain(
                     _extra_middlewares
                     or (m(None).publish_scope for m in self._broker_middlewares),
                     self._middlewares,
                 )
             ] or msgs
```

### Comparing `faststream-0.5.0rc0/faststream/confluent/schemas/params.py` & `faststream-0.5.0rc1/faststream/confluent/schemas/params.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/faststream/confluent/subscriber/asyncapi.py` & `faststream-0.5.0rc1/faststream/confluent/subscriber/asyncapi.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,44 @@
-from typing import Callable, Dict, Iterable, Literal, Optional, Tuple, Union, overload
+from typing import (
+    TYPE_CHECKING,
+    Callable,
+    Dict,
+    Iterable,
+    Literal,
+    Optional,
+    Tuple,
+    Union,
+    overload,
+)
 
-from confluent_kafka import Message as ConfluentMsg
-from fast_depends.dependencies import Depends
 from typing_extensions import override
 
 from faststream.asyncapi.schema import (
     Channel,
     ChannelBinding,
     CorrelationId,
     Message,
     Operation,
 )
 from faststream.asyncapi.schema.bindings import kafka
 from faststream.asyncapi.utils import resolve_payloads
-from faststream.broker.types import BrokerMiddleware, MsgType
-from faststream.confluent.client import AsyncConfluentConsumer
+from faststream.broker.types import MsgType
 from faststream.confluent.subscriber.usecase import (
     BatchSubscriber,
     DefaultSubscriber,
     LogicSubscriber,
 )
 
+if TYPE_CHECKING:
+    from confluent_kafka import Message as ConfluentMsg
+    from fast_depends.dependencies import Depends
+
+    from faststream.broker.types import BrokerMiddleware
+    from faststream.confluent.client import AsyncConfluentConsumer
+
 
 class AsyncAPISubscriber(LogicSubscriber[MsgType]):
     """A class to handle logic and async API operations."""
 
     def get_name(self) -> str:
         return f'{",".join(self.topics)}:{self.call_name}'
 
@@ -59,99 +73,94 @@
     def create(
         *topics: str,
         batch: Literal[True],
         batch_timeout_ms: int,
         max_records: Optional[int],
         # Kafka information
         group_id: Optional[str],
-        builder: Callable[..., AsyncConfluentConsumer],
+        builder: Callable[..., "AsyncConfluentConsumer"],
         is_manual: bool,
         # Subscriber args
         no_ack: bool,
         retry: bool,
-        broker_dependencies: Iterable[Depends],
-        broker_middlewares: Iterable[BrokerMiddleware[Tuple[ConfluentMsg, ...]]],
+        broker_dependencies: Iterable["Depends"],
+        broker_middlewares: Iterable["BrokerMiddleware[Tuple[ConfluentMsg, ...]]"],
         # AsyncAPI args
         title_: Optional[str],
         description_: Optional[str],
         include_in_schema: bool,
-    ) -> "AsyncAPIBatchSubscriber":
-        ...
+    ) -> "AsyncAPIBatchSubscriber": ...
 
     @overload
     @staticmethod
     def create(
         *topics: str,
         batch: Literal[False],
         batch_timeout_ms: int,
         max_records: Optional[int],
         # Kafka information
         group_id: Optional[str],
-        builder: Callable[..., AsyncConfluentConsumer],
+        builder: Callable[..., "AsyncConfluentConsumer"],
         is_manual: bool,
         # Subscriber args
         no_ack: bool,
         retry: bool,
-        broker_dependencies: Iterable[Depends],
-        broker_middlewares: Iterable[BrokerMiddleware[ConfluentMsg]],
+        broker_dependencies: Iterable["Depends"],
+        broker_middlewares: Iterable["BrokerMiddleware[ConfluentMsg]"],
         # AsyncAPI args
         title_: Optional[str],
         description_: Optional[str],
         include_in_schema: bool,
-    ) -> "AsyncAPIDefaultSubscriber":
-        ...
+    ) -> "AsyncAPIDefaultSubscriber": ...
 
     @overload
     @staticmethod
     def create(
         *topics: str,
         batch: bool,
         batch_timeout_ms: int,
         max_records: Optional[int],
         # Kafka information
         group_id: Optional[str],
-        builder: Callable[..., AsyncConfluentConsumer],
+        builder: Callable[..., "AsyncConfluentConsumer"],
         is_manual: bool,
         # Subscriber args
         no_ack: bool,
         retry: bool,
-        broker_dependencies: Iterable[Depends],
-        broker_middlewares: Iterable[BrokerMiddleware[Union[
-            ConfluentMsg,
-            Tuple[ConfluentMsg, ...]],
-        ]],
+        broker_dependencies: Iterable["Depends"],
+        broker_middlewares: Iterable[
+            "BrokerMiddleware[Union[ConfluentMsg, Tuple[ConfluentMsg, ...]]]"
+        ],
         # AsyncAPI args
         title_: Optional[str],
         description_: Optional[str],
         include_in_schema: bool,
     ) -> Union[
         "AsyncAPIDefaultSubscriber",
         "AsyncAPIBatchSubscriber",
-    ]:
-        ...
+    ]: ...
 
     @override
     @staticmethod
     def create(
         *topics: str,
         batch: bool,
         batch_timeout_ms: int,
         max_records: Optional[int],
         # Kafka information
         group_id: Optional[str],
-        builder: Callable[..., AsyncConfluentConsumer],
+        builder: Callable[..., "AsyncConfluentConsumer"],
         is_manual: bool,
         # Subscriber args
         no_ack: bool,
         retry: bool,
-        broker_dependencies: Iterable[Depends],
-        broker_middlewares: Iterable[BrokerMiddleware[Union[
-            ConfluentMsg,
-            Tuple[ConfluentMsg, ...]],
-        ]],
+        broker_dependencies: Iterable["Depends"],
+        broker_middlewares: Iterable[
+            "BrokerMiddleware[Union[ConfluentMsg, Tuple[ConfluentMsg, ...]]]"
+        ],
         # AsyncAPI args
         title_: Optional[str],
         description_: Optional[str],
         include_in_schema: bool,
     ) -> Union[
         "AsyncAPIDefaultSubscriber",
         "AsyncAPIBatchSubscriber",
@@ -186,17 +195,17 @@
                 description_=description_,
                 include_in_schema=include_in_schema,
             )
 
 
 class AsyncAPIDefaultSubscriber(
     DefaultSubscriber,
-    AsyncAPISubscriber[ConfluentMsg],
+    AsyncAPISubscriber["ConfluentMsg"],
 ):
     pass
 
 
 class AsyncAPIBatchSubscriber(
     BatchSubscriber,
-    AsyncAPISubscriber[Tuple[ConfluentMsg, ...]],
+    AsyncAPISubscriber[Tuple["ConfluentMsg", ...]],
 ):
     pass
```

### Comparing `faststream-0.5.0rc0/faststream/confluent/subscriber/usecase.py` & `faststream-0.5.0rc1/faststream/confluent/subscriber/usecase.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,59 +1,68 @@
 import asyncio
 from abc import ABC, abstractmethod
-from typing import Any, Callable, Dict, Iterable, Optional, Sequence, Tuple
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    Dict,
+    Iterable,
+    Optional,
+    Sequence,
+    Tuple,
+)
 
 import anyio
 from confluent_kafka import KafkaException, Message
-from fast_depends.dependencies import Depends
 from typing_extensions import override
 
-from faststream.broker.message import StreamMessage
 from faststream.broker.publisher.fake import FakePublisher
-from faststream.broker.publisher.proto import ProducerProto
 from faststream.broker.subscriber.usecase import SubscriberUsecase
-from faststream.broker.types import (
-    AsyncDecoder,
-    AsyncParser,
-    BrokerMiddleware,
-    CustomDecoder,
-    CustomParser,
-    MsgType,
-)
-from faststream.confluent.client import AsyncConfluentConsumer
+from faststream.broker.types import MsgType
 from faststream.confluent.parser import AsyncConfluentParser
 from faststream.confluent.schemas.params import ConsumerConnectionParams
-from faststream.types import AnyDict, LoggerProto
+
+if TYPE_CHECKING:
+    from fast_depends.dependencies import Depends
+
+    from faststream.broker.message import StreamMessage
+    from faststream.broker.publisher.proto import ProducerProto
+    from faststream.broker.types import (
+        AsyncCallable,
+        BrokerMiddleware,
+        CustomCallable,
+    )
+    from faststream.confluent.client import AsyncConfluentConsumer
+    from faststream.types import AnyDict, LoggerProto
 
 
 class LogicSubscriber(ABC, SubscriberUsecase[MsgType]):
     """A class to handle logic for consuming messages from Kafka."""
 
     topics: Sequence[str]
     group_id: Optional[str]
 
-    consumer: Optional[AsyncConfluentConsumer]
+    consumer: Optional["AsyncConfluentConsumer"]
     task: Optional["asyncio.Task[None]"]
     client_id: Optional[str]
-    batch: bool
 
     def __init__(
         self,
         *topics: str,
         # Kafka information
         group_id: Optional[str],
-        builder: Callable[..., AsyncConfluentConsumer],
+        builder: Callable[..., "AsyncConfluentConsumer"],
         is_manual: bool,
         # Subscriber args
-        default_parser: AsyncParser[MsgType],
-        default_decoder: AsyncDecoder[StreamMessage[MsgType]],
+        default_parser: "AsyncCallable",
+        default_decoder: "AsyncCallable",
         no_ack: bool,
         retry: bool,
-        broker_dependencies: Iterable[Depends],
-        broker_middlewares: Iterable[BrokerMiddleware[MsgType]],
+        broker_dependencies: Iterable["Depends"],
+        broker_middlewares: Iterable["BrokerMiddleware[MsgType]"],
         # AsyncAPI args
         title_: Optional[str],
         description_: Optional[str],
         include_in_schema: bool,
     ) -> None:
         super().__init__(
             default_parser=default_parser,
@@ -81,23 +90,23 @@
         self.__connection_data = ConsumerConnectionParams()
 
     @override
     def setup(  # type: ignore[override]
         self,
         *,
         client_id: Optional[str],
-        connection_data: ConsumerConnectionParams,
+        connection_data: "ConsumerConnectionParams",
         # basic args
-        logger: Optional[LoggerProto],
-        producer: Optional[ProducerProto],
+        logger: Optional["LoggerProto"],
+        producer: Optional["ProducerProto"],
         graceful_timeout: Optional[float],
-        extra_context: Optional[AnyDict],
+        extra_context: Optional["AnyDict"],
         # broker options
-        broker_parser: Optional["CustomParser[MsgType]"],
-        broker_decoder: Optional["CustomDecoder[StreamMessage[MsgType]]"],
+        broker_parser: Optional["CustomCallable"],
+        broker_decoder: Optional["CustomCallable"],
         # dependant args
         apply_types: bool,
         is_validate: bool,
         _get_dependant: Optional[Callable[..., Any]],
     ) -> None:
         self.client_id = client_id
         self.__connection_data = connection_data
@@ -204,21 +213,21 @@
 
 class DefaultSubscriber(LogicSubscriber[Message]):
     def __init__(
         self,
         *topics: str,
         # Kafka information
         group_id: Optional[str],
-        builder: Callable[..., AsyncConfluentConsumer],
+        builder: Callable[..., "AsyncConfluentConsumer"],
         is_manual: bool,
         # Subscriber args
         no_ack: bool,
         retry: bool,
-        broker_dependencies: Iterable[Depends],
-        broker_middlewares: Iterable[BrokerMiddleware[Message]],
+        broker_dependencies: Iterable["Depends"],
+        broker_middlewares: Iterable["BrokerMiddleware[Message]"],
         # AsyncAPI args
         title_: Optional[str],
         description_: Optional[str],
         include_in_schema: bool,
     ) -> None:
         super().__init__(
             *topics,
@@ -235,15 +244,15 @@
             broker_dependencies=broker_dependencies,
             # AsyncAPI args
             title_=title_,
             description_=description_,
             include_in_schema=include_in_schema,
         )
 
-    async def get_msg(self) -> Optional[Message]:
+    async def get_msg(self) -> Optional["Message"]:
         assert self.consumer, "You should setup subscriber at first."  # nosec B101
         return await self.consumer.getone()
 
     def get_log_context(
         self,
         message: Optional["StreamMessage[Message]"],
     ) -> Dict[str, str]:
@@ -254,29 +263,30 @@
 
         return self.build_log_context(
             message=message,
             topic=topic,
             group_id=self.group_id,
         )
 
+
 class BatchSubscriber(LogicSubscriber[Tuple[Message, ...]]):
     def __init__(
         self,
         *topics: str,
         batch_timeout_ms: int,
         max_records: Optional[int],
         # Kafka information
         group_id: Optional[str],
-        builder: Callable[..., AsyncConfluentConsumer],
+        builder: Callable[..., "AsyncConfluentConsumer"],
         is_manual: bool,
         # Subscriber args
         no_ack: bool,
         retry: bool,
-        broker_dependencies: Iterable[Depends],
-        broker_middlewares: Iterable[BrokerMiddleware[Tuple[Message, ...]]],
+        broker_dependencies: Iterable["Depends"],
+        broker_middlewares: Iterable["BrokerMiddleware[Tuple[Message, ...]]"],
         # AsyncAPI args
         title_: Optional[str],
         description_: Optional[str],
         include_in_schema: bool,
     ) -> None:
         self.batch_timeout_ms = batch_timeout_ms
         self.max_records = max_records
@@ -296,15 +306,15 @@
             broker_dependencies=broker_dependencies,
             # AsyncAPI args
             title_=title_,
             description_=description_,
             include_in_schema=include_in_schema,
         )
 
-    async def get_msg(self) -> Optional[Tuple[Message, ...]]:
+    async def get_msg(self) -> Optional[Tuple["Message", ...]]:
         assert self.consumer, "You should setup subscriber at first."  # nosec B101
 
         messages = await self.consumer.getmany(
             timeout_ms=self.batch_timeout_ms,
             max_records=self.max_records,
         )
```

### Comparing `faststream-0.5.0rc0/faststream/kafka/annotations.py` & `faststream-0.5.0rc1/faststream/kafka/annotations.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/faststream/kafka/message.py` & `faststream-0.5.0rc1/faststream/kafka/message.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from typing import Any, Protocol, Tuple, Union
-
-from aiokafka import ConsumerRecord
+from typing import TYPE_CHECKING, Any, Protocol, Tuple, Union
 
 from faststream.broker.message import StreamMessage
 
+if TYPE_CHECKING:
+    from aiokafka import ConsumerRecord
+
 
 class ConsumerProtocol(Protocol):
     """A protocol for Kafka consumers."""
 
-    async def commit(self) -> None:
-        ...
+    async def commit(self) -> None: ...
 
 
 class FakeConsumer:
     """A fake Kafka consumer."""
 
     async def commit(self) -> None:
         pass
@@ -21,16 +21,16 @@
 
 FAKE_CONSUMER = FakeConsumer()
 
 
 class KafkaMessage(
     StreamMessage[
         Union[
-            ConsumerRecord,
-            Tuple[ConsumerRecord, ...],
+            "ConsumerRecord",
+            Tuple["ConsumerRecord", ...],
         ]
     ]
 ):
     """Represents a Kafka message in the FastStream framework.
 
     This class extends `StreamMessage` and is specialized for handling Kafka ConsumerRecord objects.
     """
```

### Comparing `faststream-0.5.0rc0/faststream/kafka/parser.py` & `faststream-0.5.0rc1/faststream/kafka/parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from typing import TYPE_CHECKING, Any, Optional, Tuple
 
-from aiokafka import ConsumerRecord
-
-from faststream.broker.message import StreamMessage, decode_message, gen_cor_id
+from faststream.broker.message import decode_message, gen_cor_id
 from faststream.kafka.message import FAKE_CONSUMER, KafkaMessage
-from faststream.types import DecodedMessage
 from faststream.utils.context.repository import context
 
 if TYPE_CHECKING:
+    from aiokafka import ConsumerRecord
+
+    from faststream.broker.message import StreamMessage
     from faststream.kafka.subscriber.usecase import LogicSubscriber
+    from faststream.types import DecodedMessage
 
 
 class AioKafkaParser:
     """A class to parse Kafka messages."""
 
     @staticmethod
     async def parse_message(
-        message: ConsumerRecord,
-    ) -> StreamMessage[ConsumerRecord]:
+        message: "ConsumerRecord",
+    ) -> "StreamMessage[ConsumerRecord]":
         """Parses a Kafka message."""
         headers = {i: j.decode() for i, j in message.headers}
         handler: Optional["LogicSubscriber[Any]"] = context.get_local("handler_")
         return KafkaMessage(
             body=message.value,
             headers=headers,
             reply_to=headers.get("reply_to", ""),
@@ -31,16 +32,16 @@
             raw_message=message,
             consumer=getattr(handler, "consumer", None) or FAKE_CONSUMER,
             is_manual=getattr(handler, "is_manual", True),
         )
 
     @staticmethod
     async def parse_message_batch(
-        message: Tuple[ConsumerRecord, ...],
-    ) -> StreamMessage[Tuple[ConsumerRecord, ...]]:
+        message: Tuple["ConsumerRecord", ...],
+    ) -> "StreamMessage[Tuple[ConsumerRecord, ...]]":
         """Parses a batch of messages from a Kafka consumer."""
         first = message[0]
         last = message[-1]
         headers = {i: j.decode() for i, j in first.headers}
         handler: Optional["LogicSubscriber[Any]"] = context.get_local("handler_")
         return KafkaMessage(
             body=[m.value for m in message],
@@ -51,17 +52,18 @@
             correlation_id=headers.get("correlation_id", gen_cor_id()),
             raw_message=message,
             consumer=getattr(handler, "consumer", None) or FAKE_CONSUMER,
             is_manual=getattr(handler, "is_manual", True),
         )
 
     @staticmethod
-    async def decode_message(msg: StreamMessage[ConsumerRecord]) -> DecodedMessage:
+    async def decode_message(msg: "StreamMessage[ConsumerRecord]") -> "DecodedMessage":
         """Decodes a message."""
         return decode_message(msg)
 
     @classmethod
     async def decode_message_batch(
-        cls, msg: StreamMessage[Tuple[ConsumerRecord, ...]]
-    ) -> DecodedMessage:
+        cls,
+        msg: "StreamMessage[Tuple[ConsumerRecord, ...]]",
+    ) -> "DecodedMessage":
         """Decode a batch of messages."""
         return [decode_message(await cls.parse_message(m)) for m in msg.raw_message]
```

### Comparing `faststream-0.5.0rc0/faststream/kafka/router.py` & `faststream-0.5.0rc1/faststream/kafka/router.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 from typing import (
+    TYPE_CHECKING,
     Any,
     Callable,
     Dict,
     Iterable,
     Literal,
     Optional,
     Sequence,
     Tuple,
     Union,
 )
 
-from aiokafka import ConsumerRecord
-from aiokafka.coordinator.assignors.abstract import AbstractPartitionAssignor
 from aiokafka.coordinator.assignors.roundrobin import RoundRobinPartitionAssignor
-from fast_depends.dependencies import Depends
 from typing_extensions import Annotated, Doc, deprecated
 
-from faststream.broker.message import StreamMessage
 from faststream.broker.router import ArgsContainer, BrokerRouter, SubscriberRoute
-from faststream.broker.types import (
-    BrokerMiddleware,
-    CustomDecoder,
-    CustomParser,
-    Filter,
-    PublisherMiddleware,
-    SubscriberMiddleware,
-)
 from faststream.broker.utils import default_filter
 from faststream.kafka.broker.registrator import KafkaRegistrator
-from faststream.types import SendableMessage
+
+if TYPE_CHECKING:
+    from aiokafka import ConsumerRecord
+    from aiokafka.coordinator.assignors.abstract import AbstractPartitionAssignor
+    from fast_depends.dependencies import Depends
+
+    from faststream.broker.types import (
+        BrokerMiddleware,
+        CustomCallable,
+        Filter,
+        PublisherMiddleware,
+        SubscriberMiddleware,
+    )
+    from faststream.kafka.message import KafkaMessage
+    from faststream.types import SendableMessage
 
 
 class KafkaPublisher(ArgsContainer):
     """Delayed KafkaPublisher registration object.
 
     Just a copy of `KafkaRegistrator.publisher(...)` arguments.
     """
@@ -63,29 +66,29 @@
             selected using the configured `partitioner`.
             """),
         ] = None,
         headers: Annotated[
             Optional[Dict[str, str]],
             Doc(
                 "Message headers to store metainformation. "
-                "**content-type** and **correlation_id** will be setted automatically by framework anyway. "
+                "**content-type** and **correlation_id** will be set automatically by framework anyway. "
                 "Can be overridden by `publish.headers` if specified."
             ),
         ] = None,
         reply_to: Annotated[
             str,
             Doc("Topic name to send response."),
         ] = "",
         batch: Annotated[
             bool,
             Doc("Whether to send messages in batches or not."),
         ] = False,
         # basic args
         middlewares: Annotated[
-            Iterable[PublisherMiddleware],
+            Iterable["PublisherMiddleware"],
             Doc("Publisher middlewares to wrap outgoing messages."),
         ] = (),
         # AsyncAPI args
         title: Annotated[
             Optional[str],
             Doc("AsyncAPI publisher object title."),
         ] = None,
@@ -124,15 +127,15 @@
 
 class KafkaRoute(SubscriberRoute):
     """Class to store delayed KafkaBroker subscriber registration."""
 
     def __init__(
         self,
         call: Annotated[
-            Callable[..., SendableMessage],
+            Callable[..., "SendableMessage"],
             Doc(
                 "Message handler function "
                 "to wrap the same with `@broker.subscriber(...)` way."
             ),
         ],
         *topics: Annotated[
             str,
@@ -241,15 +244,15 @@
             Automatically check the CRC32 of the records
             consumed. This ensures no on-the-wire or on-disk corruption to
             the messages occurred. This check adds some overhead, so it may
             be disabled in cases seeking extreme performance.
             """),
         ] = True,
         partition_assignment_strategy: Annotated[
-            Sequence[AbstractPartitionAssignor],
+            Sequence["AbstractPartitionAssignor"],
             Doc("""
             List of objects to use to
             distribute partition ownership amongst consumer instances when
             group management is used. This preference is implicit in the order
             of the strategies in the list. When assignment strategy changes:
             to support a change to the assignment strategy, new versions must
             enable support both for the old assignment strategy and the new
@@ -371,44 +374,31 @@
         ] = 200,
         max_records: Annotated[
             Optional[int],
             Doc("Number of messages to consume as one batch."),
         ] = None,
         # broker args
         dependencies: Annotated[
-            Iterable[Depends],
+            Iterable["Depends"],
             Doc("Dependencies list (`[Depends(),]`) to apply to the subscriber."),
         ] = (),
         parser: Annotated[
-            Optional[
-                Union[
-                    CustomParser[ConsumerRecord],
-                    CustomParser[Tuple[ConsumerRecord, ...]],
-                ]
-            ],
+            Optional["CustomCallable"],
             Doc("Parser to map original **ConsumerRecord** object to FastStream one."),
         ] = None,
         decoder: Annotated[
-            Optional[
-                Union[
-                    CustomDecoder[StreamMessage[ConsumerRecord]],
-                    CustomDecoder[StreamMessage[Tuple[ConsumerRecord, ...]]],
-                ]
-            ],
+            Optional["CustomCallable"],
             Doc("Function to decode FastStream msg bytes body to python objects."),
         ] = None,
         middlewares: Annotated[
-            Iterable[SubscriberMiddleware],
+            Iterable["SubscriberMiddleware"],
             Doc("Subscriber middlewares to wrap incoming message processing."),
         ] = (),
         filter: Annotated[
-            Union[
-                Filter[StreamMessage[ConsumerRecord]],
-                Filter[StreamMessage[Tuple[ConsumerRecord, ...]]],
-            ],
+            "Filter[KafkaMessage]",
             Doc(
                 "Overload subscriber to consume various messages from the same source."
             ),
             deprecated(
                 "Deprecated in **FastStream 0.5.0**. "
                 "Please, create `subscriber` object and use it explicitly instead. "
                 "Argument will be removed in **FastStream 0.6.0**."
@@ -481,16 +471,16 @@
             no_ack=no_ack,
         )
 
 
 class KafkaRouter(
     BrokerRouter[
         Union[
-            ConsumerRecord,
-            Tuple[ConsumerRecord, ...],
+            "ConsumerRecord",
+            Tuple["ConsumerRecord", ...],
         ]
     ],
     KafkaRegistrator,
 ):
     """Includable to KafkaBroker router."""
 
     def __init__(
@@ -501,44 +491,34 @@
         ] = "",
         handlers: Annotated[
             Iterable[KafkaRoute],
             Doc("Route object to include."),
         ] = (),
         *,
         dependencies: Annotated[
-            Iterable[Depends],
+            Iterable["Depends"],
             Doc(
                 "Dependencies list (`[Depends(),]`) to apply to all routers' publishers/subscribers."
             ),
         ] = (),
         middlewares: Annotated[
             Iterable[
                 Union[
-                    BrokerMiddleware[ConsumerRecord],
-                    BrokerMiddleware[Tuple[ConsumerRecord, ...]],
+                    "BrokerMiddleware[ConsumerRecord]",
+                    "BrokerMiddleware[Tuple[ConsumerRecord, ...]]",
                 ]
             ],
             Doc("Router middlewares to apply to all routers' publishers/subscribers."),
         ] = (),
         parser: Annotated[
-            Optional[
-                Union[
-                    CustomParser[ConsumerRecord],
-                    CustomParser[Tuple[ConsumerRecord, ...]],
-                ]
-            ],
+            Optional["CustomCallable"],
             Doc("Parser to map original **ConsumerRecord** object to FastStream one."),
         ] = None,
         decoder: Annotated[
-            Optional[
-                Union[
-                    CustomDecoder[StreamMessage[ConsumerRecord]],
-                    CustomDecoder[StreamMessage[Tuple[ConsumerRecord, ...]]],
-                ]
-            ],
+            Optional["CustomCallable"],
             Doc("Function to decode FastStream msg bytes body to python objects."),
         ] = None,
         include_in_schema: Annotated[
             Optional[bool],
             Doc("Whetever to include operation in AsyncAPI schema or not."),
         ] = None,
     ) -> None:
```

### Comparing `faststream-0.5.0rc0/faststream/kafka/security.py` & `faststream-0.5.0rc1/faststream/kafka/security.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,45 @@
 import warnings
-from typing import Optional
+from typing import TYPE_CHECKING, Optional
 
 from faststream.security import (
     BaseSecurity,
     SASLPlaintext,
     SASLScram256,
     SASLScram512,
     ssl_not_set_error_msg,
 )
-from faststream.types import AnyDict
 
+if TYPE_CHECKING:
+    from faststream.types import AnyDict
 
-def parse_security(security: Optional[BaseSecurity]) -> AnyDict:
+
+def parse_security(security: Optional[BaseSecurity]) -> "AnyDict":
     if security is None:
         return {}
     elif type(security) == BaseSecurity:
         return _parse_base_security(security)
     elif type(security) == SASLPlaintext:
         return _parse_sasl_plaintext(security)
     elif type(security) == SASLScram256:
         return _parse_sasl_scram256(security)
     elif type(security) == SASLScram512:
         return _parse_sasl_scram512(security)
     else:
         raise NotImplementedError(f"KafkaBroker does not support `{type(security)}`.")
 
 
-def _parse_base_security(security: BaseSecurity) -> AnyDict:
+def _parse_base_security(security: BaseSecurity) -> "AnyDict":
     return {
         "security_protocol": "SSL" if security.use_ssl else "PLAINTEXT",
         "ssl_context": security.ssl_context,
     }
 
 
-def _parse_sasl_plaintext(security: SASLPlaintext) -> AnyDict:
+def _parse_sasl_plaintext(security: SASLPlaintext) -> "AnyDict":
     if security.ssl_context is None:
         warnings.warn(
             message=ssl_not_set_error_msg,
             category=RuntimeWarning,
             stacklevel=1,
         )
 
@@ -46,25 +48,25 @@
         "ssl_context": security.ssl_context,
         "sasl_mechanism": "PLAIN",
         "sasl_plain_username": security.username,
         "sasl_plain_password": security.password,
     }
 
 
-def _parse_sasl_scram256(security: SASLScram256) -> AnyDict:
+def _parse_sasl_scram256(security: SASLScram256) -> "AnyDict":
     return {
         "security_protocol": "SASL_SSL" if security.use_ssl else "SASL_PLAINTEXT",
         "ssl_context": security.ssl_context,
         "sasl_mechanism": "SCRAM-SHA-256",
         "sasl_plain_username": security.username,
         "sasl_plain_password": security.password,
     }
 
 
-def _parse_sasl_scram512(security: SASLScram512) -> AnyDict:
+def _parse_sasl_scram512(security: SASLScram512) -> "AnyDict":
     return {
         "security_protocol": "SASL_SSL" if security.use_ssl else "SASL_PLAINTEXT",
         "ssl_context": security.ssl_context,
         "sasl_mechanism": "SCRAM-SHA-512",
         "sasl_plain_username": security.username,
         "sasl_plain_password": security.password,
     }
```

### Comparing `faststream-0.5.0rc0/faststream/kafka/testing.py` & `faststream-0.5.0rc1/faststream/kafka/testing.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,59 +1,59 @@
 from datetime import datetime
-from typing import Any, Dict, Optional
+from typing import TYPE_CHECKING, Any, Dict, Optional
 
 from aiokafka import ConsumerRecord
 from typing_extensions import override
 
 from faststream.broker.message import encode_message, gen_cor_id
-from faststream.broker.wrapper.call import HandlerCallWrapper
 from faststream.kafka.broker import KafkaBroker
-from faststream.kafka.publisher.asyncapi import (
-    AsyncAPIBatchPublisher,
-    AsyncAPIPublisher,
-)
+from faststream.kafka.publisher.asyncapi import AsyncAPIBatchPublisher
 from faststream.kafka.publisher.producer import AioKafkaFastProducer
 from faststream.kafka.subscriber.asyncapi import AsyncAPIBatchSubscriber
 from faststream.testing.broker import TestBroker, call_handler
-from faststream.types import SendableMessage
+
+if TYPE_CHECKING:
+    from faststream.broker.wrapper.call import HandlerCallWrapper
+    from faststream.kafka.publisher.asyncapi import AsyncAPIPublisher
+    from faststream.types import SendableMessage
 
 __all__ = ("TestKafkaBroker",)
 
 
 class TestKafkaBroker(TestBroker[KafkaBroker]):
     """A class to test Kafka brokers."""
 
     @staticmethod
     async def _fake_connect(broker: KafkaBroker, *args: Any, **kwargs: Any) -> None:
         broker._producer = FakeProducer(broker)
 
     @staticmethod
     def create_publisher_fake_subscriber(
         broker: KafkaBroker,
-        publisher: AsyncAPIPublisher[Any],
-    ) -> HandlerCallWrapper[Any, Any, Any]:
+        publisher: "AsyncAPIPublisher[Any]",
+    ) -> "HandlerCallWrapper[Any, Any, Any]":
         sub = broker.subscriber(
             publisher.topic,
             batch=isinstance(publisher, AsyncAPIBatchPublisher),
         )
 
         if not sub.calls:
 
-            @sub
+            @sub  # type: ignore[misc]
             def f(msg: Any) -> None:
                 pass
 
             broker.setup_subscriber(sub)
 
         return sub.calls[0].handler
 
     @staticmethod
     def remove_publisher_fake_subscriber(
         broker: KafkaBroker,
-        publisher: AsyncAPIPublisher[Any],
+        publisher: "AsyncAPIPublisher[Any]",
     ) -> None:
         broker._subscribers.pop(hash(publisher), None)
 
 
 class FakeProducer(AioKafkaFastProducer):
     """A fake Kafka producer for testing purposes.
 
@@ -62,15 +62,15 @@
 
     def __init__(self, broker: KafkaBroker) -> None:
         self.broker = broker
 
     @override
     async def publish(  # type: ignore[override]
         self,
-        message: SendableMessage,
+        message: "SendableMessage",
         topic: str,
         key: Optional[bytes] = None,
         partition: Optional[int] = None,
         timestamp_ms: Optional[int] = None,
         headers: Optional[Dict[str, str]] = None,
         correlation_id: Optional[str] = None,
         *,
@@ -103,15 +103,15 @@
                     raise_timeout=raise_timeout,
                 )
 
         return None
 
     async def publish_batch(
         self,
-        *msgs: SendableMessage,
+        *msgs: "SendableMessage",
         topic: str,
         partition: Optional[int] = None,
         timestamp_ms: Optional[int] = None,
         headers: Optional[Dict[str, str]] = None,
         reply_to: str = "",
         correlation_id: Optional[str] = None,
     ) -> None:
@@ -143,15 +143,15 @@
                             handler=handler,
                             message=m,
                         )
         return None
 
 
 def build_message(
-    message: SendableMessage,
+    message: "SendableMessage",
     topic: str,
     partition: Optional[int] = None,
     timestamp_ms: Optional[int] = None,
     key: Optional[bytes] = None,
     headers: Optional[Dict[str, str]] = None,
     correlation_id: Optional[str] = None,
     *,
```

### Comparing `faststream-0.5.0rc0/faststream/kafka/broker/broker.py` & `faststream-0.5.0rc1/faststream/kafka/broker/broker.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 import logging
-from asyncio import AbstractEventLoop
 from contextlib import AsyncExitStack
 from inspect import Parameter
-from types import TracebackType
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Dict,
     Iterable,
     List,
@@ -15,44 +13,48 @@
     Tuple,
     Type,
     TypeVar,
     Union,
 )
 
 import aiokafka
-from aiokafka import ConsumerRecord
-from aiokafka.abc import AbstractTokenProvider
 from aiokafka.partitioner import DefaultPartitioner
 from aiokafka.producer.producer import _missing
-from fast_depends.dependencies import Depends
 from typing_extensions import Annotated, Doc, override
 
 from faststream.__about__ import SERVICE_NAME
-from faststream.asyncapi import schema as asyncapi
-from faststream.broker.message import StreamMessage, gen_cor_id
-from faststream.broker.types import (
-    BrokerMiddleware,
-    CustomDecoder,
-    CustomParser,
-)
+from faststream.broker.message import gen_cor_id
 from faststream.exceptions import NOT_CONNECTED_YET
 from faststream.kafka.broker.logging import KafkaLoggingBroker
 from faststream.kafka.broker.registrator import KafkaRegistrator
 from faststream.kafka.publisher.producer import AioKafkaFastProducer
 from faststream.kafka.schemas.params import ConsumerConnectionParams
 from faststream.kafka.security import parse_security
-from faststream.security import BaseSecurity
 from faststream.types import AnyDict, SendableMessage
 from faststream.utils.data import filter_by_dict
 
 Partition = TypeVar("Partition")
 
 if TYPE_CHECKING:
+    from asyncio import AbstractEventLoop
+    from types import TracebackType
+
+    from aiokafka import ConsumerRecord
+    from aiokafka.abc import AbstractTokenProvider
+    from fast_depends.dependencies import Depends
     from typing_extensions import TypedDict, Unpack
 
+    from faststream.asyncapi import schema as asyncapi
+    from faststream.broker.types import (
+        BrokerMiddleware,
+        CustomCallable,
+    )
+    from faststream.security import BaseSecurity
+    from faststream.types import LoggerProto
+
     class KafkaInitKwargs(TypedDict, total=False):
         request_timeout_ms: Annotated[
             int,
             Doc("Client request timeout in milliseconds."),
         ]
         retry_backoff_ms: Annotated[
             int,
@@ -75,15 +77,15 @@
             disable idle checks.
             """),
         ]
         sasl_kerberos_service_name: str
         sasl_kerberos_domain_name: Optional[str]
         sasl_oauth_token_provider: Annotated[
             Optional[AbstractTokenProvider],
-            Doc("OAuthBearer token provider instance.")
+            Doc("OAuthBearer token provider instance."),
         ]
         loop: Optional[AbstractEventLoop]
         client_id: Annotated[
             Optional[str],
             Doc("""
             A name for this client. This string is passed in
             each request to servers and can be used to identify specific
@@ -120,15 +122,15 @@
 
             If unset, defaults to ``acks=1``. If `enable_idempotence` is
             :data:`True` defaults to ``acks=all``.
             """),
         ]
         key_serializer: Annotated[
             Optional[Callable[[Any], bytes]],
-            Doc("Used to convert user-supplied keys to bytes.")
+            Doc("Used to convert user-supplied keys to bytes."),
         ]
         value_serializer: Annotated[
             Optional[Callable[[Any], bytes]],
             Doc("used to convert user-supplied message values to bytes."),
         ]
         compression_type: Annotated[
             Optional[Literal["gzip", "snappy", "lz4", "zstd"]],
@@ -166,15 +168,15 @@
             int,
             Doc("""
             The maximum size of a request. This is also
             effectively a cap on the maximum record size. Note that the server
             has its own cap on record size which may be different from this.
             This setting will limit the number of record batches the producer
             will send in a single request to avoid sending huge requests.
-            """)
+            """),
         ]
         linger_ms: Annotated[
             int,
             Doc("""
             The producer groups together any records that arrive
             in between request transmissions into a single batched request.
             Normally this occurs only under load when records arrive faster
@@ -202,15 +204,15 @@
 
 
 class KafkaBroker(
     KafkaRegistrator,
     KafkaLoggingBroker,
 ):
     url: List[str]
-    _producer: Optional[AioKafkaFastProducer]
+    _producer: Optional["AioKafkaFastProducer"]
 
     def __init__(
         self,
         bootstrap_servers: Annotated[
             Union[str, Iterable[str]],
             Doc("""
             A `host[:port]` string (or list of `host[:port]` strings) that the consumer should contact to bootstrap
@@ -247,18 +249,18 @@
             of milliseconds specified by this config. Specifying `None` will
             disable idle checks.
             """),
         ] = 9 * 60 * 1000,
         sasl_kerberos_service_name: str = "kafka",
         sasl_kerberos_domain_name: Optional[str] = None,
         sasl_oauth_token_provider: Annotated[
-            Optional[AbstractTokenProvider],
-            Doc("OAuthBearer token provider instance.")
+            Optional["AbstractTokenProvider"],
+            Doc("OAuthBearer token provider instance."),
         ] = None,
-        loop: Optional[AbstractEventLoop] = None,
+        loop: Optional["AbstractEventLoop"] = None,
         client_id: Annotated[
             Optional[str],
             Doc("""
             A name for this client. This string is passed in
             each request to servers and can be used to identify specific
             server-side log entries that correspond to this client. Also
             submitted to :class:`~.consumer.group_coordinator.GroupCoordinator`
@@ -293,15 +295,15 @@
 
             If unset, defaults to ``acks=1``. If `enable_idempotence` is
             :data:`True` defaults to ``acks=all``.
             """),
         ] = _missing,
         key_serializer: Annotated[
             Optional[Callable[[Any], bytes]],
-            Doc("Used to convert user-supplied keys to bytes.")
+            Doc("Used to convert user-supplied keys to bytes."),
         ] = None,
         value_serializer: Annotated[
             Optional[Callable[[Any], bytes]],
             Doc("used to convert user-supplied message values to bytes."),
         ] = None,
         compression_type: Annotated[
             Optional[Literal["gzip", "snappy", "lz4", "zstd"]],
@@ -339,15 +341,15 @@
             int,
             Doc("""
             The maximum size of a request. This is also
             effectively a cap on the maximum record size. Note that the server
             has its own cap on record size which may be different from this.
             This setting will limit the number of record batches the producer
             will send in a single request to avoid sending huge requests.
-            """)
+            """),
         ] = 1024 * 1024,
         linger_ms: Annotated[
             int,
             Doc("""
             The producer groups together any records that arrive
             in between request transmissions into a single batched request.
             Normally this occurs only under load when records arrive faster
@@ -376,36 +378,32 @@
         graceful_timeout: Annotated[
             Optional[float],
             Doc(
                 "Graceful shutdown timeout. Broker waits for all running subscribers completion before shut down."
             ),
         ] = 15.0,
         decoder: Annotated[
-            Optional[Union[
-                CustomDecoder[StreamMessage[ConsumerRecord]],
-                CustomDecoder[StreamMessage[Tuple[ConsumerRecord, ...]]],
-            ]],
+            Optional["CustomCallable"],
             Doc("Custom decoder object."),
         ] = None,
         parser: Annotated[
-            Optional[Union[
-                CustomParser[ConsumerRecord],
-                CustomParser[Tuple[ConsumerRecord, ...]]
-            ]],
+            Optional["CustomCallable"],
             Doc("Custom parser object."),
         ] = None,
         dependencies: Annotated[
-            Iterable[Depends],
+            Iterable["Depends"],
             Doc("Dependencies to apply to all broker subscribers."),
         ] = (),
         middlewares: Annotated[
-            Iterable[Union[
-                BrokerMiddleware[ConsumerRecord],
-                BrokerMiddleware[Tuple[ConsumerRecord, ...]],
-            ]],
+            Iterable[
+                Union[
+                    "BrokerMiddleware[ConsumerRecord]",
+                    "BrokerMiddleware[Tuple[ConsumerRecord, ...]]",
+                ]
+            ],
             Doc("Middlewares to apply to all broker publishers/subscribers."),
         ] = (),
         # AsyncAPI args
         security: Annotated[
             Optional["BaseSecurity"],
             Doc(
                 "Security options to connect broker and generate AsyncAPI server security information."
@@ -429,15 +427,15 @@
         ] = None,
         tags: Annotated[
             Optional[Iterable[Union["asyncapi.Tag", "asyncapi.TagDict"]]],
             Doc("AsyncAPI server tags."),
         ] = None,
         # logging args
         logger: Annotated[
-            Union[logging.Logger, None, object],
+            Union["LoggerProto", None, object],
             Doc("User specified logger to pass into Context and log service messages."),
         ] = Parameter.empty,
         log_level: Annotated[
             int,
             Doc("Service messages log level."),
         ] = logging.INFO,
         log_fmt: Annotated[
@@ -460,16 +458,19 @@
     ) -> None:
         if protocol is None:
             if security is not None and security.use_ssl:
                 protocol = "kafka-secure"
             else:
                 protocol = "kafka"
 
-        servers = [bootstrap_servers] if isinstance(
-            bootstrap_servers, str) else list(bootstrap_servers)
+        servers = (
+            [bootstrap_servers]
+            if isinstance(bootstrap_servers, str)
+            else list(bootstrap_servers)
+        )
 
         if asyncapi_url is not None:
             if isinstance(asyncapi_url, str):
                 asyncapi_url = [asyncapi_url]
             else:
                 asyncapi_url = list(asyncapi_url)
         else:
@@ -526,15 +527,15 @@
         self.client_id = client_id
         self._producer = None
 
     async def _close(
         self,
         exc_type: Optional[Type[BaseException]] = None,
         exc_val: Optional[BaseException] = None,
-        exc_tb: Optional[TracebackType] = None,
+        exc_tb: Optional["TracebackType"] = None,
     ) -> None:
         if self._producer is not None:  # pragma: no branch
             await self._producer.stop()
             self._producer = None
 
         await super()._close(exc_type, exc_val, exc_tb)
 
@@ -549,18 +550,15 @@
     ) -> ConsumerConnectionParams:
         """Connect to Kafka servers manually.
 
         Consumes the same with `KafkaBroker.__init__` arguments and overrides them.
         To startup subscribers too you should use `broker.start()` after/instead this method.
         """
         if bootstrap_servers is not Parameter.empty:
-            connect_kwargs: AnyDict = {
-                **kwargs,
-                "bootstrap_servers": bootstrap_servers
-            }
+            connect_kwargs: AnyDict = {**kwargs, "bootstrap_servers": bootstrap_servers}
         else:
             connect_kwargs = {**kwargs}
 
         return await super().connect(**connect_kwargs)
 
     @override
     async def _connect(  # type: ignore[override]
@@ -599,15 +597,15 @@
             "connection_args": self._connection or {},
         }
 
     @override
     async def publish(  # type: ignore[override]
         self,
         message: Annotated[
-            SendableMessage,
+            "SendableMessage",
             Doc("Message body to send."),
         ],
         topic: Annotated[
             str,
             Doc("Topic where the message will be published."),
         ],
         *,
@@ -617,46 +615,44 @@
             A key to associate with the message. Can be used to
             determine which partition to send the message to. If partition
             is `None` (and producer's partitioner config is left as default),
             then messages with the same key will be delivered to the same
             partition (but if key is `None`, partition is chosen randomly).
             Must be type `bytes`, or be serializable to bytes via configured
             `key_serializer`.
-            """)
+            """),
         ] = None,
         partition: Annotated[
             Optional[int],
             Doc("""
             Specify a partition. If not set, the partition will be
             selected using the configured `partitioner`.
             """),
         ] = None,
         timestamp_ms: Annotated[
             Optional[int],
             Doc("""
             Epoch milliseconds (from Jan 1 1970 UTC) to use as
             the message timestamp. Defaults to current time.
-            """)
+            """),
         ] = None,
         headers: Annotated[
             Optional[Dict[str, str]],
             Doc("Message headers to store metainformation."),
         ] = None,
         correlation_id: Annotated[
             Optional[str],
             Doc(
                 "Manual message **correlation_id** setter. "
                 "**correlation_id** is a useful option to trace messages."
             ),
         ] = None,
         reply_to: Annotated[
             str,
-            Doc(
-                "Reply message topic name to send response."
-            ),
+            Doc("Reply message topic name to send response."),
         ] = "",
         # extra options to be compatible with test client
         **kwargs: Any,
     ) -> Optional[Any]:
         """Publish message directly.
 
         This method allows you to publish message in not AsyncAPI-documented way. You can use it in another frameworks
@@ -678,15 +674,15 @@
             reply_to=reply_to,
             **kwargs,
         )
 
     async def publish_batch(
         self,
         *msgs: Annotated[
-            SendableMessage,
+            "SendableMessage",
             Doc("Messages bodies to send."),
         ],
         topic: Annotated[
             str,
             Doc("Topic where the message will be published."),
         ],
         partition: Annotated[
@@ -697,25 +693,23 @@
             """),
         ] = None,
         timestamp_ms: Annotated[
             Optional[int],
             Doc("""
             Epoch milliseconds (from Jan 1 1970 UTC) to use as
             the message timestamp. Defaults to current time.
-            """)
+            """),
         ] = None,
         headers: Annotated[
             Optional[Dict[str, str]],
             Doc("Messages headers to store metainformation."),
         ] = None,
         reply_to: Annotated[
             str,
-            Doc(
-                "Reply message topic name to send response."
-            ),
+            Doc("Reply message topic name to send response."),
         ] = "",
         correlation_id: Annotated[
             Optional[str],
             Doc(
                 "Manual message **correlation_id** setter. "
                 "**correlation_id** is a useful option to trace messages."
             ),
```

### Comparing `faststream-0.5.0rc0/faststream/kafka/broker/logging.py` & `faststream-0.5.0rc1/faststream/kafka/broker/logging.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 import logging
 from inspect import Parameter
-from typing import Any, ClassVar, Optional, Tuple, Union
-
-import aiokafka
+from typing import TYPE_CHECKING, Any, ClassVar, Optional, Tuple, Union
 
 from faststream.broker.core.usecase import BrokerUsecase
 from faststream.kafka.schemas.params import ConsumerConnectionParams
 from faststream.log.logging import get_broker_logger
 
+if TYPE_CHECKING:
+    import aiokafka
+
+    from faststream.types import LoggerProto
+
 
-class KafkaLoggingBroker(BrokerUsecase[
-    Union[
-        aiokafka.ConsumerRecord,
-        Tuple[aiokafka.ConsumerRecord, ...]
-    ],
-    ConsumerConnectionParams,
-]):
+class KafkaLoggingBroker(
+    BrokerUsecase[
+        Union["aiokafka.ConsumerRecord", Tuple["aiokafka.ConsumerRecord", ...]],
+        ConsumerConnectionParams,
+    ]
+):
     """A class that extends the LoggingMixin class and adds additional functionality for logging Kafka related information."""
 
     _max_topic_len: int
     _max_group_len: int
     __max_msg_id_ln: ClassVar[int] = 10
 
     def __init__(
         self,
         *args: Any,
-        logger: Union[logging.Logger, object, None] = Parameter.empty,
+        logger: Union["LoggerProto", object, None] = Parameter.empty,
         log_level: int = logging.INFO,
         log_fmt: Optional[str] = None,
         **kwargs: Any,
     ) -> None:
         """Initialize the class."""
         super().__init__(
             *args,
```

### Comparing `faststream-0.5.0rc0/faststream/kafka/broker/registrator.py` & `faststream-0.5.0rc1/faststream/kafka/broker/registrator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,63 +1,73 @@
 from functools import partial
 from typing import (
+    TYPE_CHECKING,
     Any,
     Callable,
     Dict,
     Iterable,
     Literal,
     Optional,
     Sequence,
     Tuple,
     Union,
     cast,
     overload,
 )
 
 from aiokafka import AIOKafkaConsumer, ConsumerRecord
-from aiokafka.coordinator.assignors.abstract import AbstractPartitionAssignor
 from aiokafka.coordinator.assignors.roundrobin import RoundRobinPartitionAssignor
-from fast_depends.dependencies import Depends
 from typing_extensions import Annotated, Doc, deprecated, override
 
 from faststream.broker.core.abc import ABCBroker
-from faststream.broker.message import StreamMessage
-from faststream.broker.types import (
-    CustomDecoder,
-    CustomParser,
-    Filter,
-    PublisherMiddleware,
-    SubscriberMiddleware,
-)
 from faststream.broker.utils import default_filter
 from faststream.exceptions import SetupError
-from faststream.kafka.publisher.asyncapi import (
-    AsyncAPIBatchPublisher,
-    AsyncAPIDefaultPublisher,
-    AsyncAPIPublisher,
-)
-from faststream.kafka.subscriber.asyncapi import (
-    AsyncAPIBatchSubscriber,
-    AsyncAPIDefaultSubscriber,
-    AsyncAPISubscriber,
-)
+from faststream.kafka.publisher.asyncapi import AsyncAPIPublisher
+from faststream.kafka.subscriber.asyncapi import AsyncAPISubscriber
+
+if TYPE_CHECKING:
+    from aiokafka import ConsumerRecord
+    from aiokafka.coordinator.assignors.abstract import AbstractPartitionAssignor
+    from fast_depends.dependencies import Depends
+
+    from faststream.broker.types import (
+        CustomCallable,
+        Filter,
+        PublisherMiddleware,
+        SubscriberMiddleware,
+    )
+    from faststream.kafka.message import KafkaMessage
+    from faststream.kafka.publisher.asyncapi import (
+        AsyncAPIBatchPublisher,
+        AsyncAPIDefaultPublisher,
+    )
+    from faststream.kafka.subscriber.asyncapi import (
+        AsyncAPIBatchSubscriber,
+        AsyncAPIDefaultSubscriber,
+    )
 
 
 class KafkaRegistrator(
     ABCBroker[
         Union[
-            ConsumerRecord,
-            Tuple[ConsumerRecord, ...],
+            "ConsumerRecord",
+            Tuple["ConsumerRecord", ...],
         ]
     ]
 ):
     """Includable to KafkaBroker router."""
 
-    _subscribers: Dict[int, Union[AsyncAPIBatchSubscriber, AsyncAPIDefaultSubscriber]]
-    _publishers: Dict[int, Union[AsyncAPIBatchPublisher, AsyncAPIDefaultPublisher]]
+    _subscribers: Dict[
+        int,
+        Union["AsyncAPIBatchSubscriber", "AsyncAPIDefaultSubscriber"],
+    ]
+    _publishers: Dict[
+        int,
+        Union["AsyncAPIBatchPublisher", "AsyncAPIDefaultPublisher"],
+    ]
 
     @overload  # type: ignore[override]
     def subscriber(
         self,
         *topics: Annotated[
             str,
             Doc("Kafka topics to consume messages from."),
@@ -161,15 +171,15 @@
             Automatically check the CRC32 of the records
             consumed. This ensures no on-the-wire or on-disk corruption to
             the messages occurred. This check adds some overhead, so it may
             be disabled in cases seeking extreme performance.
             """),
         ] = True,
         partition_assignment_strategy: Annotated[
-            Sequence[AbstractPartitionAssignor],
+            Sequence["AbstractPartitionAssignor"],
             Doc("""
             List of objects to use to
             distribute partition ownership amongst consumer instances when
             group management is used. This preference is implicit in the order
             of the strategies in the list. When assignment strategy changes:
             to support a change to the assignment strategy, new versions must
             enable support both for the old assignment strategy and the new
@@ -291,31 +301,31 @@
         ] = 200,
         max_records: Annotated[
             Optional[int],
             Doc("Number of messages to consume as one batch."),
         ] = None,
         # broker args
         dependencies: Annotated[
-            Iterable[Depends],
+            Iterable["Depends"],
             Doc("Dependencies list (`[Depends(),]`) to apply to the subscriber."),
         ] = (),
         parser: Annotated[
-            Optional[CustomParser[ConsumerRecord]],
+            Optional["CustomCallable"],
             Doc("Parser to map original **ConsumerRecord** object to FastStream one."),
         ] = None,
         decoder: Annotated[
-            Optional[CustomDecoder[StreamMessage[ConsumerRecord]]],
+            Optional["CustomCallable"],
             Doc("Function to decode FastStream msg bytes body to python objects."),
         ] = None,
         middlewares: Annotated[
-            Iterable[SubscriberMiddleware],
+            Iterable["SubscriberMiddleware"],
             Doc("Subscriber middlewares to wrap incoming message processing."),
         ] = (),
         filter: Annotated[
-            Filter[StreamMessage[ConsumerRecord]],
+            "Filter[KafkaMessage]",
             Doc(
                 "Overload subscriber to consume various messages from the same source."
             ),
             deprecated(
                 "Deprecated in **FastStream 0.5.0**. "
                 "Please, create `subscriber` object and use it explicitly instead. "
                 "Argument will be removed in **FastStream 0.6.0**."
@@ -341,15 +351,15 @@
                 "Uses decorated docstring as default."
             ),
         ] = None,
         include_in_schema: Annotated[
             bool,
             Doc("Whetever to include operation in AsyncAPI schema or not."),
         ] = True,
-    ) -> AsyncAPIDefaultSubscriber: ...
+    ) -> "AsyncAPIDefaultSubscriber": ...
 
     @overload
     def subscriber(
         self,
         *topics: Annotated[
             str,
             Doc("Kafka topics to consume messages from."),
@@ -453,15 +463,15 @@
             Automatically check the CRC32 of the records
             consumed. This ensures no on-the-wire or on-disk corruption to
             the messages occurred. This check adds some overhead, so it may
             be disabled in cases seeking extreme performance.
             """),
         ] = True,
         partition_assignment_strategy: Annotated[
-            Sequence[AbstractPartitionAssignor],
+            Sequence["AbstractPartitionAssignor"],
             Doc("""
             List of objects to use to
             distribute partition ownership amongst consumer instances when
             group management is used. This preference is implicit in the order
             of the strategies in the list. When assignment strategy changes:
             to support a change to the assignment strategy, new versions must
             enable support both for the old assignment strategy and the new
@@ -583,31 +593,31 @@
         ] = 200,
         max_records: Annotated[
             Optional[int],
             Doc("Number of messages to consume as one batch."),
         ] = None,
         # broker args
         dependencies: Annotated[
-            Iterable[Depends],
+            Iterable["Depends"],
             Doc("Dependencies list (`[Depends(),]`) to apply to the subscriber."),
         ] = (),
         parser: Annotated[
-            Optional[CustomParser[Tuple[ConsumerRecord, ...]]],
+            Optional["CustomCallable"],
             Doc("Parser to map original **ConsumerRecord** object to FastStream one."),
         ] = None,
         decoder: Annotated[
-            Optional[CustomDecoder[StreamMessage[Tuple[ConsumerRecord, ...]]]],
+            Optional["CustomCallable"],
             Doc("Function to decode FastStream msg bytes body to python objects."),
         ] = None,
         middlewares: Annotated[
-            Iterable[SubscriberMiddleware],
+            Iterable["SubscriberMiddleware"],
             Doc("Subscriber middlewares to wrap incoming message processing."),
         ] = (),
         filter: Annotated[
-            Filter[StreamMessage[Tuple[ConsumerRecord, ...]]],
+            "Filter[KafkaMessage]",
             Doc(
                 "Overload subscriber to consume various messages from the same source."
             ),
             deprecated(
                 "Deprecated in **FastStream 0.5.0**. "
                 "Please, create `subscriber` object and use it explicitly instead. "
                 "Argument will be removed in **FastStream 0.6.0**."
@@ -633,15 +643,15 @@
                 "Uses decorated docstring as default."
             ),
         ] = None,
         include_in_schema: Annotated[
             bool,
             Doc("Whetever to include operation in AsyncAPI schema or not."),
         ] = True,
-    ) -> AsyncAPIBatchSubscriber: ...
+    ) -> "AsyncAPIBatchSubscriber": ...
 
     @overload
     def subscriber(
         self,
         *topics: Annotated[
             str,
             Doc("Kafka topics to consume messages from."),
@@ -745,15 +755,15 @@
             Automatically check the CRC32 of the records
             consumed. This ensures no on-the-wire or on-disk corruption to
             the messages occurred. This check adds some overhead, so it may
             be disabled in cases seeking extreme performance.
             """),
         ] = True,
         partition_assignment_strategy: Annotated[
-            Sequence[AbstractPartitionAssignor],
+            Sequence["AbstractPartitionAssignor"],
             Doc("""
             List of objects to use to
             distribute partition ownership amongst consumer instances when
             group management is used. This preference is implicit in the order
             of the strategies in the list. When assignment strategy changes:
             to support a change to the assignment strategy, new versions must
             enable support both for the old assignment strategy and the new
@@ -875,44 +885,31 @@
         ] = 200,
         max_records: Annotated[
             Optional[int],
             Doc("Number of messages to consume as one batch."),
         ] = None,
         # broker args
         dependencies: Annotated[
-            Iterable[Depends],
+            Iterable["Depends"],
             Doc("Dependencies list (`[Depends(),]`) to apply to the subscriber."),
         ] = (),
         parser: Annotated[
-            Optional[
-                Union[
-                    CustomParser[ConsumerRecord],
-                    CustomParser[Tuple[ConsumerRecord, ...]],
-                ]
-            ],
+            Optional["CustomCallable"],
             Doc("Parser to map original **ConsumerRecord** object to FastStream one."),
         ] = None,
         decoder: Annotated[
-            Optional[
-                Union[
-                    CustomDecoder[StreamMessage[ConsumerRecord]],
-                    CustomDecoder[StreamMessage[Tuple[ConsumerRecord, ...]]],
-                ]
-            ],
+            Optional["CustomCallable"],
             Doc("Function to decode FastStream msg bytes body to python objects."),
         ] = None,
         middlewares: Annotated[
-            Iterable[SubscriberMiddleware],
+            Iterable["SubscriberMiddleware"],
             Doc("Subscriber middlewares to wrap incoming message processing."),
         ] = (),
         filter: Annotated[
-            Union[
-                Filter[StreamMessage[ConsumerRecord]],
-                Filter[StreamMessage[Tuple[ConsumerRecord, ...]]],
-            ],
+            "Filter[KafkaMessage]",
             Doc(
                 "Overload subscriber to consume various messages from the same source."
             ),
             deprecated(
                 "Deprecated in **FastStream 0.5.0**. "
                 "Please, create `subscriber` object and use it explicitly instead. "
                 "Argument will be removed in **FastStream 0.6.0**."
@@ -939,16 +936,16 @@
             ),
         ] = None,
         include_in_schema: Annotated[
             bool,
             Doc("Whetever to include operation in AsyncAPI schema or not."),
         ] = True,
     ) -> Union[
-        AsyncAPIDefaultSubscriber,
-        AsyncAPIBatchSubscriber,
+        "AsyncAPIDefaultSubscriber",
+        "AsyncAPIBatchSubscriber",
     ]: ...
 
     @override
     def subscriber(
         self,
         *topics: Annotated[
             str,
@@ -1053,15 +1050,15 @@
             Automatically check the CRC32 of the records
             consumed. This ensures no on-the-wire or on-disk corruption to
             the messages occurred. This check adds some overhead, so it may
             be disabled in cases seeking extreme performance.
             """),
         ] = True,
         partition_assignment_strategy: Annotated[
-            Sequence[AbstractPartitionAssignor],
+            Sequence["AbstractPartitionAssignor"],
             Doc("""
             List of objects to use to
             distribute partition ownership amongst consumer instances when
             group management is used. This preference is implicit in the order
             of the strategies in the list. When assignment strategy changes:
             to support a change to the assignment strategy, new versions must
             enable support both for the old assignment strategy and the new
@@ -1183,44 +1180,31 @@
         ] = 200,
         max_records: Annotated[
             Optional[int],
             Doc("Number of messages to consume as one batch."),
         ] = None,
         # broker args
         dependencies: Annotated[
-            Iterable[Depends],
+            Iterable["Depends"],
             Doc("Dependencies list (`[Depends(),]`) to apply to the subscriber."),
         ] = (),
         parser: Annotated[
-            Optional[
-                Union[
-                    CustomParser[ConsumerRecord],
-                    CustomParser[Tuple[ConsumerRecord, ...]],
-                ]
-            ],
+            Optional["CustomCallable"],
             Doc("Parser to map original **ConsumerRecord** object to FastStream one."),
         ] = None,
         decoder: Annotated[
-            Optional[
-                Union[
-                    CustomDecoder[StreamMessage[ConsumerRecord]],
-                    CustomDecoder[StreamMessage[Tuple[ConsumerRecord, ...]]],
-                ]
-            ],
+            Optional["CustomCallable"],
             Doc("Function to decode FastStream msg bytes body to python objects."),
         ] = None,
         middlewares: Annotated[
-            Iterable[SubscriberMiddleware],
+            Iterable["SubscriberMiddleware"],
             Doc("Subscriber middlewares to wrap incoming message processing."),
         ] = (),
         filter: Annotated[
-            Union[
-                Filter[StreamMessage[ConsumerRecord]],
-                Filter[StreamMessage[Tuple[ConsumerRecord, ...]]],
-            ],
+            "Filter[KafkaMessage]",
             Doc(
                 "Overload subscriber to consume various messages from the same source."
             ),
             deprecated(
                 "Deprecated in **FastStream 0.5.0**. "
                 "Please, create `subscriber` object and use it explicitly instead. "
                 "Argument will be removed in **FastStream 0.6.0**."
@@ -1247,16 +1231,16 @@
             ),
         ] = None,
         include_in_schema: Annotated[
             bool,
             Doc("Whetever to include operation in AsyncAPI schema or not."),
         ] = True,
     ) -> Union[
-        AsyncAPIDefaultSubscriber,
-        AsyncAPIBatchSubscriber,
+        "AsyncAPIDefaultSubscriber",
+        "AsyncAPIBatchSubscriber",
     ]:
         if not auto_commit and not group_id:
             raise SetupError("You should install `group_id` with manual commit mode")
 
         builder = partial(
             AIOKafkaConsumer,
             key_deserializer=key_deserializer,
@@ -1298,24 +1282,24 @@
                 title_=title,
                 description_=description,
                 include_in_schema=self._solve_include_in_schema(include_in_schema),
             )
         )
 
         if batch:
-            return cast(AsyncAPIBatchSubscriber, subscriber).add_call(
+            return cast("AsyncAPIBatchSubscriber", subscriber).add_call(
                 filter_=filter,
                 parser_=parser or self._parser,
                 decoder_=decoder or self._decoder,
                 dependencies_=dependencies,
                 middlewares_=middlewares,
             )
 
         else:
-            return cast(AsyncAPIDefaultSubscriber, subscriber).add_call(
+            return cast("AsyncAPIDefaultSubscriber", subscriber).add_call(
                 filter_=filter,
                 parser_=parser or self._parser,
                 decoder_=decoder or self._decoder,
                 dependencies_=dependencies,
                 middlewares_=middlewares,
             )
 
@@ -1346,29 +1330,29 @@
             selected using the configured `partitioner`.
             """),
         ] = None,
         headers: Annotated[
             Optional[Dict[str, str]],
             Doc(
                 "Message headers to store metainformation. "
-                "**content-type** and **correlation_id** will be setted automatically by framework anyway. "
+                "**content-type** and **correlation_id** will be set automatically by framework anyway. "
                 "Can be overridden by `publish.headers` if specified."
             ),
         ] = None,
         reply_to: Annotated[
             str,
             Doc("Topic name to send response."),
         ] = "",
         batch: Annotated[
             Literal[False],
             Doc("Whether to send messages in batches or not."),
         ] = False,
         # basic args
         middlewares: Annotated[
-            Iterable[PublisherMiddleware],
+            Iterable["PublisherMiddleware"],
             Doc("Publisher middlewares to wrap outgoing messages."),
         ] = (),
         # AsyncAPI args
         title: Annotated[
             Optional[str],
             Doc("AsyncAPI publisher object title."),
         ] = None,
@@ -1383,15 +1367,15 @@
                 "Should be any python-native object annotation or `pydantic.BaseModel`."
             ),
         ] = None,
         include_in_schema: Annotated[
             bool,
             Doc("Whetever to include operation in AsyncAPI schema or not."),
         ] = True,
-    ) -> AsyncAPIDefaultPublisher: ...
+    ) -> "AsyncAPIDefaultPublisher": ...
 
     @overload
     def publisher(
         self,
         topic: Annotated[
             str,
             Doc("Topic where the message will be published."),
@@ -1416,29 +1400,29 @@
             selected using the configured `partitioner`.
             """),
         ] = None,
         headers: Annotated[
             Optional[Dict[str, str]],
             Doc(
                 "Message headers to store metainformation. "
-                "**content-type** and **correlation_id** will be setted automatically by framework anyway. "
+                "**content-type** and **correlation_id** will be set automatically by framework anyway. "
                 "Can be overridden by `publish.headers` if specified."
             ),
         ] = None,
         reply_to: Annotated[
             str,
             Doc("Topic name to send response."),
         ] = "",
         batch: Annotated[
             Literal[True],
             Doc("Whether to send messages in batches or not."),
         ],
         # basic args
         middlewares: Annotated[
-            Iterable[PublisherMiddleware],
+            Iterable["PublisherMiddleware"],
             Doc("Publisher middlewares to wrap outgoing messages."),
         ] = (),
         # AsyncAPI args
         title: Annotated[
             Optional[str],
             Doc("AsyncAPI publisher object title."),
         ] = None,
@@ -1453,15 +1437,15 @@
                 "Should be any python-native object annotation or `pydantic.BaseModel`."
             ),
         ] = None,
         include_in_schema: Annotated[
             bool,
             Doc("Whetever to include operation in AsyncAPI schema or not."),
         ] = True,
-    ) -> AsyncAPIBatchPublisher: ...
+    ) -> "AsyncAPIBatchPublisher": ...
 
     @overload
     def publisher(
         self,
         topic: Annotated[
             str,
             Doc("Topic where the message will be published."),
@@ -1486,29 +1470,29 @@
             selected using the configured `partitioner`.
             """),
         ] = None,
         headers: Annotated[
             Optional[Dict[str, str]],
             Doc(
                 "Message headers to store metainformation. "
-                "**content-type** and **correlation_id** will be setted automatically by framework anyway. "
+                "**content-type** and **correlation_id** will be set automatically by framework anyway. "
                 "Can be overridden by `publish.headers` if specified."
             ),
         ] = None,
         reply_to: Annotated[
             str,
             Doc("Topic name to send response."),
         ] = "",
         batch: Annotated[
             bool,
             Doc("Whether to send messages in batches or not."),
         ] = False,
         # basic args
         middlewares: Annotated[
-            Iterable[PublisherMiddleware],
+            Iterable["PublisherMiddleware"],
             Doc("Publisher middlewares to wrap outgoing messages."),
         ] = (),
         # AsyncAPI args
         title: Annotated[
             Optional[str],
             Doc("AsyncAPI publisher object title."),
         ] = None,
@@ -1524,16 +1508,16 @@
             ),
         ] = None,
         include_in_schema: Annotated[
             bool,
             Doc("Whetever to include operation in AsyncAPI schema or not."),
         ] = True,
     ) -> Union[
-        AsyncAPIBatchPublisher,
-        AsyncAPIDefaultPublisher,
+        "AsyncAPIBatchPublisher",
+        "AsyncAPIDefaultPublisher",
     ]: ...
 
     @override
     def publisher(
         self,
         topic: Annotated[
             str,
@@ -1559,29 +1543,29 @@
             selected using the configured `partitioner`.
             """),
         ] = None,
         headers: Annotated[
             Optional[Dict[str, str]],
             Doc(
                 "Message headers to store metainformation. "
-                "**content-type** and **correlation_id** will be setted automatically by framework anyway. "
+                "**content-type** and **correlation_id** will be set automatically by framework anyway. "
                 "Can be overridden by `publish.headers` if specified."
             ),
         ] = None,
         reply_to: Annotated[
             str,
             Doc("Topic name to send response."),
         ] = "",
         batch: Annotated[
             bool,
             Doc("Whether to send messages in batches or not."),
         ] = False,
         # basic args
         middlewares: Annotated[
-            Iterable[PublisherMiddleware],
+            Iterable["PublisherMiddleware"],
             Doc("Publisher middlewares to wrap outgoing messages."),
         ] = (),
         # AsyncAPI args
         title: Annotated[
             Optional[str],
             Doc("AsyncAPI publisher object title."),
         ] = None,
@@ -1597,16 +1581,16 @@
             ),
         ] = None,
         include_in_schema: Annotated[
             bool,
             Doc("Whetever to include operation in AsyncAPI schema or not."),
         ] = True,
     ) -> Union[
-        AsyncAPIBatchPublisher,
-        AsyncAPIDefaultPublisher,
+        "AsyncAPIBatchPublisher",
+        "AsyncAPIDefaultPublisher",
     ]:
         """Creates long-living and AsyncAPI-documented publisher object.
 
         You can use it as a handler decorator (handler should be decorated by `@broker.subscriber(...)` too) - `@broker.publisher(...)`.
         In such case publisher will publish your handler return value.
 
         Or you can create a publisher object to call it lately - `broker.publisher(...).publish(...)`.
@@ -1628,10 +1612,10 @@
             title_=title,
             description_=description,
             schema_=schema,
             include_in_schema=self._solve_include_in_schema(include_in_schema),
         )
 
         if batch:
-            return cast(AsyncAPIBatchPublisher, super().publisher(publisher))
+            return cast("AsyncAPIBatchPublisher", super().publisher(publisher))
         else:
-            return cast(AsyncAPIDefaultPublisher, super().publisher(publisher))
+            return cast("AsyncAPIDefaultPublisher", super().publisher(publisher))
```

### Comparing `faststream-0.5.0rc0/faststream/kafka/fastapi/__init__.py` & `faststream-0.5.0rc1/faststream/kafka/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/faststream/kafka/fastapi/fastapi.py` & `faststream-0.5.0rc1/faststream/kafka/fastapi/fastapi.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import logging
-from asyncio import AbstractEventLoop
-from enum import Enum
 from inspect import Parameter
 from typing import (
+    TYPE_CHECKING,
     Any,
     Callable,
     Dict,
     Iterable,
     List,
     Literal,
     Optional,
@@ -16,53 +15,58 @@
     TypeVar,
     Union,
     cast,
     overload,
 )
 
 from aiokafka import ConsumerRecord
-from aiokafka.abc import AbstractTokenProvider
-from aiokafka.coordinator.assignors.abstract import AbstractPartitionAssignor
 from aiokafka.coordinator.assignors.roundrobin import RoundRobinPartitionAssignor
 from aiokafka.partitioner import DefaultPartitioner
 from aiokafka.producer.producer import _missing
-from fastapi import params
 from fastapi.datastructures import Default
 from fastapi.routing import APIRoute
-from fastapi.types import IncEx
 from fastapi.utils import generate_unique_id
 from starlette.responses import JSONResponse, Response
 from starlette.routing import BaseRoute
-from starlette.types import ASGIApp, Lifespan
 from typing_extensions import Annotated, Doc, deprecated, override
 
 from faststream.__about__ import SERVICE_NAME
-from faststream.asyncapi import schema as asyncapi
 from faststream.broker.fastapi.router import StreamRouter
-from faststream.broker.message import StreamMessage
-from faststream.broker.types import (
-    BrokerMiddleware,
-    CustomDecoder,
-    CustomParser,
-    Filter,
-    PublisherMiddleware,
-    SubscriberMiddleware,
-)
 from faststream.broker.utils import default_filter
 from faststream.kafka.broker.broker import KafkaBroker as KB
-from faststream.kafka.publisher.asyncapi import (
-    AsyncAPIBatchPublisher,
-    AsyncAPIDefaultPublisher,
-)
-from faststream.kafka.subscriber.asyncapi import (
-    AsyncAPIBatchSubscriber,
-    AsyncAPIDefaultSubscriber,
-)
-from faststream.security import BaseSecurity
-from faststream.types import AnyDict
+
+if TYPE_CHECKING:
+    from asyncio import AbstractEventLoop
+    from enum import Enum
+
+    from aiokafka.abc import AbstractTokenProvider
+    from aiokafka.coordinator.assignors.abstract import AbstractPartitionAssignor
+    from fastapi import params
+    from fastapi.types import IncEx
+    from starlette.types import ASGIApp, Lifespan
+
+    from faststream.asyncapi import schema as asyncapi
+    from faststream.broker.types import (
+        BrokerMiddleware,
+        CustomCallable,
+        Filter,
+        PublisherMiddleware,
+        SubscriberMiddleware,
+    )
+    from faststream.kafka.message import KafkaMessage
+    from faststream.kafka.publisher.asyncapi import (
+        AsyncAPIBatchPublisher,
+        AsyncAPIDefaultPublisher,
+    )
+    from faststream.kafka.subscriber.asyncapi import (
+        AsyncAPIBatchSubscriber,
+        AsyncAPIDefaultSubscriber,
+    )
+    from faststream.security import BaseSecurity
+    from faststream.types import AnyDict, LoggerProto
 
 Partition = TypeVar("Partition")
 
 
 class KafkaRouter(StreamRouter[Union[ConsumerRecord, Tuple[ConsumerRecord, ...]]]):
     """A class to represent a Kafka router."""
 
@@ -114,17 +118,18 @@
             disable idle checks.
             """
             ),
         ] = 9 * 60 * 1000,
         sasl_kerberos_service_name: str = "kafka",
         sasl_kerberos_domain_name: Optional[str] = None,
         sasl_oauth_token_provider: Annotated[
-            Optional[AbstractTokenProvider], Doc("OAuthBearer token provider instance.")
+            Optional["AbstractTokenProvider"],
+            Doc("OAuthBearer token provider instance."),
         ] = None,
-        loop: Optional[AbstractEventLoop] = None,
+        loop: Optional["AbstractEventLoop"] = None,
         client_id: Annotated[
             Optional[str],
             Doc(
                 """
             A name for this client. This string is passed in
             each request to servers and can be used to identify specific
             server-side log entries that correspond to this client. Also
@@ -258,36 +263,26 @@
         graceful_timeout: Annotated[
             Optional[float],
             Doc(
                 "Graceful shutdown timeout. Broker waits for all running subscribers completion before shut down."
             ),
         ] = 15.0,
         decoder: Annotated[
-            Optional[
-                Union[
-                    CustomDecoder[StreamMessage[ConsumerRecord]],
-                    CustomDecoder[StreamMessage[Tuple[ConsumerRecord, ...]]],
-                ]
-            ],
+            Optional["CustomCallable"],
             Doc("Custom decoder object."),
         ] = None,
         parser: Annotated[
-            Optional[
-                Union[
-                    CustomParser[ConsumerRecord],
-                    CustomParser[Tuple[ConsumerRecord, ...]],
-                ]
-            ],
+            Optional["CustomCallable"],
             Doc("Custom parser object."),
         ] = None,
         middlewares: Annotated[
             Iterable[
                 Union[
-                    BrokerMiddleware[ConsumerRecord],
-                    BrokerMiddleware[Tuple[ConsumerRecord, ...]],
+                    "BrokerMiddleware[ConsumerRecord]",
+                    "BrokerMiddleware[Tuple[ConsumerRecord, ...]]",
                 ]
             ],
             Doc("Middlewares to apply to all broker publishers/subscribers."),
         ] = (),
         # AsyncAPI args
         security: Annotated[
             Optional["BaseSecurity"],
@@ -313,15 +308,15 @@
         ] = None,
         asyncapi_tags: Annotated[
             Optional[Iterable[Union["asyncapi.Tag", "asyncapi.TagDict"]]],
             Doc("AsyncAPI server tags."),
         ] = None,
         # logging args
         logger: Annotated[
-            Union[logging.Logger, None, object],
+            Union["LoggerProto", None, object],
             Doc("User specified logger to pass into Context and log service messages."),
         ] = Parameter.empty,
         log_level: Annotated[
             int,
             Doc("Service messages log level."),
         ] = logging.INFO,
         log_fmt: Annotated[
@@ -736,15 +731,15 @@
             consumed. This ensures no on-the-wire or on-disk corruption to
             the messages occurred. This check adds some overhead, so it may
             be disabled in cases seeking extreme performance.
             """
             ),
         ] = True,
         partition_assignment_strategy: Annotated[
-            Sequence[AbstractPartitionAssignor],
+            Sequence["AbstractPartitionAssignor"],
             Doc(
                 """
             List of objects to use to
             distribute partition ownership amongst consumer instances when
             group management is used. This preference is implicit in the order
             of the strategies in the list. When assignment strategy changes:
             to support a change to the assignment strategy, new versions must
@@ -890,31 +885,31 @@
         ] = None,
         batch: Annotated[
             Literal[False],
             Doc("Whether to consume messages in batches or not."),
         ] = False,
         # broker args
         dependencies: Annotated[
-            Iterable[params.Depends],
+            Iterable["params.Depends"],
             Doc("Dependencies list (`[Depends(),]`) to apply to the subscriber."),
         ] = (),
         parser: Annotated[
-            Optional[CustomParser[ConsumerRecord]],
+            Optional["CustomCallable"],
             Doc("Parser to map original **ConsumerRecord** object to FastStream one."),
         ] = None,
         decoder: Annotated[
-            Optional[CustomDecoder[StreamMessage[ConsumerRecord]]],
+            Optional["CustomCallable"],
             Doc("Function to decode FastStream msg bytes body to python objects."),
         ] = None,
         middlewares: Annotated[
-            Iterable[SubscriberMiddleware],
+            Iterable["SubscriberMiddleware"],
             Doc("Subscriber middlewares to wrap incoming message processing."),
         ] = (),
         filter: Annotated[
-            Filter[StreamMessage[ConsumerRecord]],
+            "Filter[KafkaMessage]",
             Doc(
                 "Overload subscriber to consume various messages from the same source."
             ),
             deprecated(
                 "Deprecated in **FastStream 0.5.0**. "
                 "Please, create `subscriber` object and use it explicitly instead. "
                 "Argument will be removed in **FastStream 0.6.0**."
@@ -1063,16 +1058,15 @@
                 when it makes sense.
 
                 Read more about it in the
                 [FastAPI docs for Response Model - Return Type](https://fastapi.tiangolo.com/tutorial/response-model/#response_model_exclude_none).
                 """
             ),
         ] = False,
-    ) -> AsyncAPIDefaultSubscriber:
-        ...
+    ) -> "AsyncAPIDefaultSubscriber": ...
 
     @overload
     def subscriber(
         self,
         *topics: Annotated[str, Doc("Kafka topics to consume messages from.")],
         group_id: Annotated[
             Optional[str],
@@ -1187,15 +1181,15 @@
             consumed. This ensures no on-the-wire or on-disk corruption to
             the messages occurred. This check adds some overhead, so it may
             be disabled in cases seeking extreme performance.
             """
             ),
         ] = True,
         partition_assignment_strategy: Annotated[
-            Sequence[AbstractPartitionAssignor],
+            Sequence["AbstractPartitionAssignor"],
             Doc(
                 """
             List of objects to use to
             distribute partition ownership amongst consumer instances when
             group management is used. This preference is implicit in the order
             of the strategies in the list. When assignment strategy changes:
             to support a change to the assignment strategy, new versions must
@@ -1341,31 +1335,31 @@
         ] = None,
         batch: Annotated[
             Literal[True],
             Doc("Whether to consume messages in batches or not."),
         ],
         # broker args
         dependencies: Annotated[
-            Iterable[params.Depends],
+            Iterable["params.Depends"],
             Doc("Dependencies list (`[Depends(),]`) to apply to the subscriber."),
         ] = (),
         parser: Annotated[
-            Optional[CustomParser[Tuple[ConsumerRecord, ...]]],
+            Optional["CustomCallable"],
             Doc("Parser to map original **ConsumerRecord** object to FastStream one."),
         ] = None,
         decoder: Annotated[
-            Optional[CustomDecoder[StreamMessage[Tuple[ConsumerRecord, ...]]]],
+            Optional["CustomCallable"],
             Doc("Function to decode FastStream msg bytes body to python objects."),
         ] = None,
         middlewares: Annotated[
-            Iterable[SubscriberMiddleware],
+            Iterable["SubscriberMiddleware"],
             Doc("Subscriber middlewares to wrap incoming message processing."),
         ] = (),
         filter: Annotated[
-            Filter[StreamMessage[Tuple[ConsumerRecord, ...]]],
+            "Filter[KafkaMessage]",
             Doc(
                 "Overload subscriber to consume various messages from the same source."
             ),
             deprecated(
                 "Deprecated in **FastStream 0.5.0**. "
                 "Please, create `subscriber` object and use it explicitly instead. "
                 "Argument will be removed in **FastStream 0.6.0**."
@@ -1514,16 +1508,15 @@
                 when it makes sense.
 
                 Read more about it in the
                 [FastAPI docs for Response Model - Return Type](https://fastapi.tiangolo.com/tutorial/response-model/#response_model_exclude_none).
                 """
             ),
         ] = False,
-    ) -> AsyncAPIBatchSubscriber:
-        ...
+    ) -> "AsyncAPIBatchSubscriber": ...
 
     @overload
     def subscriber(
         self,
         *topics: Annotated[str, Doc("Kafka topics to consume messages from.")],
         group_id: Annotated[
             Optional[str],
@@ -1638,15 +1631,15 @@
             consumed. This ensures no on-the-wire or on-disk corruption to
             the messages occurred. This check adds some overhead, so it may
             be disabled in cases seeking extreme performance.
             """
             ),
         ] = True,
         partition_assignment_strategy: Annotated[
-            Sequence[AbstractPartitionAssignor],
+            Sequence["AbstractPartitionAssignor"],
             Doc(
                 """
             List of objects to use to
             distribute partition ownership amongst consumer instances when
             group management is used. This preference is implicit in the order
             of the strategies in the list. When assignment strategy changes:
             to support a change to the assignment strategy, new versions must
@@ -1792,44 +1785,31 @@
         ] = None,
         batch: Annotated[
             bool,
             Doc("Whether to consume messages in batches or not."),
         ] = False,
         # broker args
         dependencies: Annotated[
-            Iterable[params.Depends],
+            Iterable["params.Depends"],
             Doc("Dependencies list (`[Depends(),]`) to apply to the subscriber."),
         ] = (),
         parser: Annotated[
-            Optional[
-                Union[
-                    CustomParser[ConsumerRecord],
-                    CustomParser[Tuple[ConsumerRecord, ...]],
-                ]
-            ],
+            Optional["CustomCallable"],
             Doc("Parser to map original **ConsumerRecord** object to FastStream one."),
         ] = None,
         decoder: Annotated[
-            Optional[
-                Union[
-                    CustomDecoder[StreamMessage[ConsumerRecord]],
-                    CustomDecoder[StreamMessage[Tuple[ConsumerRecord, ...]]],
-                ]
-            ],
+            Optional["CustomCallable"],
             Doc("Function to decode FastStream msg bytes body to python objects."),
         ] = None,
         middlewares: Annotated[
-            Iterable[SubscriberMiddleware],
+            Iterable["SubscriberMiddleware"],
             Doc("Subscriber middlewares to wrap incoming message processing."),
         ] = (),
         filter: Annotated[
-            Union[
-                Filter[StreamMessage[ConsumerRecord]],
-                Filter[StreamMessage[Tuple[ConsumerRecord, ...]]],
-            ],
+            "Filter[KafkaMessage]",
             Doc(
                 "Overload subscriber to consume various messages from the same source."
             ),
             deprecated(
                 "Deprecated in **FastStream 0.5.0**. "
                 "Please, create `subscriber` object and use it explicitly instead. "
                 "Argument will be removed in **FastStream 0.6.0**."
@@ -1979,18 +1959,17 @@
 
                 Read more about it in the
                 [FastAPI docs for Response Model - Return Type](https://fastapi.tiangolo.com/tutorial/response-model/#response_model_exclude_none).
                 """
             ),
         ] = False,
     ) -> Union[
-        AsyncAPIBatchSubscriber,
-        AsyncAPIDefaultSubscriber,
-    ]:
-        ...
+        "AsyncAPIBatchSubscriber",
+        "AsyncAPIDefaultSubscriber",
+    ]: ...
 
     @override
     def subscriber(
         self,
         *topics: Annotated[str, Doc("Kafka topics to consume messages from.")],
         group_id: Annotated[
             Optional[str],
@@ -2105,15 +2084,15 @@
             consumed. This ensures no on-the-wire or on-disk corruption to
             the messages occurred. This check adds some overhead, so it may
             be disabled in cases seeking extreme performance.
             """
             ),
         ] = True,
         partition_assignment_strategy: Annotated[
-            Sequence[AbstractPartitionAssignor],
+            Sequence["AbstractPartitionAssignor"],
             Doc(
                 """
             List of objects to use to
             distribute partition ownership amongst consumer instances when
             group management is used. This preference is implicit in the order
             of the strategies in the list. When assignment strategy changes:
             to support a change to the assignment strategy, new versions must
@@ -2259,44 +2238,31 @@
         ] = None,
         batch: Annotated[
             bool,
             Doc("Whether to consume messages in batches or not."),
         ] = False,
         # broker args
         dependencies: Annotated[
-            Iterable[params.Depends],
+            Iterable["params.Depends"],
             Doc("Dependencies list (`[Depends(),]`) to apply to the subscriber."),
         ] = (),
         parser: Annotated[
-            Optional[
-                Union[
-                    CustomParser[ConsumerRecord],
-                    CustomParser[Tuple[ConsumerRecord, ...]],
-                ]
-            ],
+            Optional["CustomCallable"],
             Doc("Parser to map original **ConsumerRecord** object to FastStream one."),
         ] = None,
         decoder: Annotated[
-            Optional[
-                Union[
-                    CustomDecoder[StreamMessage[ConsumerRecord]],
-                    CustomDecoder[StreamMessage[Tuple[ConsumerRecord, ...]]],
-                ]
-            ],
+            Optional["CustomCallable"],
             Doc("Function to decode FastStream msg bytes body to python objects."),
         ] = None,
         middlewares: Annotated[
-            Iterable[SubscriberMiddleware],
+            Iterable["SubscriberMiddleware"],
             Doc("Subscriber middlewares to wrap incoming message processing."),
         ] = (),
         filter: Annotated[
-            Union[
-                Filter[StreamMessage[ConsumerRecord]],
-                Filter[StreamMessage[Tuple[ConsumerRecord, ...]]],
-            ],
+            "Filter[KafkaMessage]",
             Doc(
                 "Overload subscriber to consume various messages from the same source."
             ),
             deprecated(
                 "Deprecated in **FastStream 0.5.0**. "
                 "Please, create `subscriber` object and use it explicitly instead. "
                 "Argument will be removed in **FastStream 0.6.0**."
@@ -2446,16 +2412,16 @@
 
                 Read more about it in the
                 [FastAPI docs for Response Model - Return Type](https://fastapi.tiangolo.com/tutorial/response-model/#response_model_exclude_none).
                 """
             ),
         ] = False,
     ) -> Union[
-        AsyncAPIBatchSubscriber,
-        AsyncAPIDefaultSubscriber,
+        "AsyncAPIBatchSubscriber",
+        "AsyncAPIDefaultSubscriber",
     ]:
         subscriber = super().subscriber(
             topics[0],  # path
             *topics,
             group_id=group_id,
             key_deserializer=key_deserializer,
             value_deserializer=value_deserializer,
@@ -2497,17 +2463,17 @@
             response_model_by_alias=response_model_by_alias,
             response_model_exclude_unset=response_model_exclude_unset,
             response_model_exclude_defaults=response_model_exclude_defaults,
             response_model_exclude_none=response_model_exclude_none,
         )
 
         if batch:
-            return cast(AsyncAPIBatchSubscriber, subscriber)
+            return cast("AsyncAPIBatchSubscriber", subscriber)
         else:
-            return cast(AsyncAPIDefaultSubscriber, subscriber)
+            return cast("AsyncAPIDefaultSubscriber", subscriber)
 
     @overload  # type: ignore[override]
     def publisher(
         self,
         topic: Annotated[
             str,
             Doc("Topic where the message will be published."),
@@ -2536,29 +2502,29 @@
             """
             ),
         ] = None,
         headers: Annotated[
             Optional[Dict[str, str]],
             Doc(
                 "Message headers to store metainformation. "
-                "**content-type** and **correlation_id** will be setted automatically by framework anyway. "
+                "**content-type** and **correlation_id** will be set automatically by framework anyway. "
                 "Can be overridden by `publish.headers` if specified."
             ),
         ] = None,
         reply_to: Annotated[
             str,
             Doc("Topic name to send response."),
         ] = "",
         batch: Annotated[
             Literal[False],
             Doc("Whether to send messages in batches or not."),
         ] = False,
         # basic args
         middlewares: Annotated[
-            Iterable[PublisherMiddleware],
+            Iterable["PublisherMiddleware"],
             Doc("Publisher middlewares to wrap outgoing messages."),
         ] = (),
         # AsyncAPI args
         title: Annotated[
             Optional[str],
             Doc("AsyncAPI publisher object title."),
         ] = None,
@@ -2573,16 +2539,15 @@
                 "Should be any python-native object annotation or `pydantic.BaseModel`."
             ),
         ] = None,
         include_in_schema: Annotated[
             bool,
             Doc("Whetever to include operation in AsyncAPI schema or not."),
         ] = True,
-    ) -> AsyncAPIDefaultPublisher:
-        ...
+    ) -> "AsyncAPIDefaultPublisher": ...
 
     @overload
     def publisher(
         self,
         topic: Annotated[
             str,
             Doc("Topic where the message will be published."),
@@ -2611,29 +2576,29 @@
             """
             ),
         ] = None,
         headers: Annotated[
             Optional[Dict[str, str]],
             Doc(
                 "Message headers to store metainformation. "
-                "**content-type** and **correlation_id** will be setted automatically by framework anyway. "
+                "**content-type** and **correlation_id** will be set automatically by framework anyway. "
                 "Can be overridden by `publish.headers` if specified."
             ),
         ] = None,
         reply_to: Annotated[
             str,
             Doc("Topic name to send response."),
         ] = "",
         batch: Annotated[
             Literal[True],
             Doc("Whether to send messages in batches or not."),
         ],
         # basic args
         middlewares: Annotated[
-            Iterable[PublisherMiddleware],
+            Iterable["PublisherMiddleware"],
             Doc("Publisher middlewares to wrap outgoing messages."),
         ] = (),
         # AsyncAPI args
         title: Annotated[
             Optional[str],
             Doc("AsyncAPI publisher object title."),
         ] = None,
@@ -2648,16 +2613,15 @@
                 "Should be any python-native object annotation or `pydantic.BaseModel`."
             ),
         ] = None,
         include_in_schema: Annotated[
             bool,
             Doc("Whetever to include operation in AsyncAPI schema or not."),
         ] = True,
-    ) -> AsyncAPIBatchPublisher:
-        ...
+    ) -> "AsyncAPIBatchPublisher": ...
 
     @overload
     def publisher(
         self,
         topic: Annotated[
             str,
             Doc("Topic where the message will be published."),
@@ -2686,29 +2650,29 @@
             """
             ),
         ] = None,
         headers: Annotated[
             Optional[Dict[str, str]],
             Doc(
                 "Message headers to store metainformation. "
-                "**content-type** and **correlation_id** will be setted automatically by framework anyway. "
+                "**content-type** and **correlation_id** will be set automatically by framework anyway. "
                 "Can be overridden by `publish.headers` if specified."
             ),
         ] = None,
         reply_to: Annotated[
             str,
             Doc("Topic name to send response."),
         ] = "",
         batch: Annotated[
             bool,
             Doc("Whether to send messages in batches or not."),
         ] = False,
         # basic args
         middlewares: Annotated[
-            Iterable[PublisherMiddleware],
+            Iterable["PublisherMiddleware"],
             Doc("Publisher middlewares to wrap outgoing messages."),
         ] = (),
         # AsyncAPI args
         title: Annotated[
             Optional[str],
             Doc("AsyncAPI publisher object title."),
         ] = None,
@@ -2724,18 +2688,17 @@
             ),
         ] = None,
         include_in_schema: Annotated[
             bool,
             Doc("Whetever to include operation in AsyncAPI schema or not."),
         ] = True,
     ) -> Union[
-        AsyncAPIBatchPublisher,
-        AsyncAPIDefaultPublisher,
-    ]:
-        ...
+        "AsyncAPIBatchPublisher",
+        "AsyncAPIDefaultPublisher",
+    ]: ...
 
     @override
     def publisher(
         self,
         topic: Annotated[
             str,
             Doc("Topic where the message will be published."),
@@ -2764,29 +2727,29 @@
             """
             ),
         ] = None,
         headers: Annotated[
             Optional[Dict[str, str]],
             Doc(
                 "Message headers to store metainformation. "
-                "**content-type** and **correlation_id** will be setted automatically by framework anyway. "
+                "**content-type** and **correlation_id** will be set automatically by framework anyway. "
                 "Can be overridden by `publish.headers` if specified."
             ),
         ] = None,
         reply_to: Annotated[
             str,
             Doc("Topic name to send response."),
         ] = "",
         batch: Annotated[
             bool,
             Doc("Whether to send messages in batches or not."),
         ] = False,
         # basic args
         middlewares: Annotated[
-            Iterable[PublisherMiddleware],
+            Iterable["PublisherMiddleware"],
             Doc("Publisher middlewares to wrap outgoing messages."),
         ] = (),
         # AsyncAPI args
         title: Annotated[
             Optional[str],
             Doc("AsyncAPI publisher object title."),
         ] = None,
@@ -2802,16 +2765,16 @@
             ),
         ] = None,
         include_in_schema: Annotated[
             bool,
             Doc("Whetever to include operation in AsyncAPI schema or not."),
         ] = True,
     ) -> Union[
-        AsyncAPIBatchPublisher,
-        AsyncAPIDefaultPublisher,
+        "AsyncAPIBatchPublisher",
+        "AsyncAPIDefaultPublisher",
     ]:
         return self.broker.publisher(
             topic=topic,
             key=key,
             partition=partition,
             headers=headers,
             batch=batch,
```

### Comparing `faststream-0.5.0rc0/faststream/kafka/publisher/asyncapi.py` & `faststream-0.5.0rc1/faststream/kafka/publisher/asyncapi.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,43 @@
-from typing import Any, Dict, Iterable, Literal, Optional, Tuple, Union, overload
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Dict,
+    Iterable,
+    Literal,
+    Optional,
+    Tuple,
+    Union,
+    overload,
+)
 
-from aiokafka import ConsumerRecord
 from typing_extensions import override
 
 from faststream.asyncapi.schema import (
     Channel,
     ChannelBinding,
     CorrelationId,
     Message,
     Operation,
 )
 from faststream.asyncapi.schema.bindings import kafka
 from faststream.asyncapi.utils import resolve_payloads
-from faststream.broker.types import BrokerMiddleware, MsgType, PublisherMiddleware
+from faststream.broker.types import MsgType
 from faststream.exceptions import SetupError
 from faststream.kafka.publisher.usecase import (
     BatchPublisher,
     DefaultPublisher,
     LogicPublisher,
 )
 
+if TYPE_CHECKING:
+    from aiokafka import ConsumerRecord
+
+    from faststream.broker.types import BrokerMiddleware, PublisherMiddleware
+
 
 class AsyncAPIPublisher(LogicPublisher[MsgType]):
     """A class representing a publisher."""
 
     def get_name(self) -> str:
         return f"{self.topic}:Publisher"
 
@@ -53,86 +67,83 @@
         batch: Literal[True],
         key: Optional[bytes],
         topic: str,
         partition: Optional[int],
         headers: Optional[Dict[str, str]],
         reply_to: str,
         # Publisher args
-        broker_middlewares: Iterable[BrokerMiddleware[Tuple[ConsumerRecord, ...]]],
-        middlewares: Iterable[PublisherMiddleware],
+        broker_middlewares: Iterable["BrokerMiddleware[Tuple[ConsumerRecord, ...]]"],
+        middlewares: Iterable["PublisherMiddleware"],
         # AsyncAPI args
         schema_: Optional[Any],
         title_: Optional[str],
         description_: Optional[str],
         include_in_schema: bool,
-    ) -> "AsyncAPIBatchPublisher":
-        ...
+    ) -> "AsyncAPIBatchPublisher": ...
 
     @overload
     @staticmethod
     def create(
         *,
         batch: Literal[False],
         key: Optional[bytes],
         topic: str,
         partition: Optional[int],
         headers: Optional[Dict[str, str]],
         reply_to: str,
         # Publisher args
-        broker_middlewares: Iterable[BrokerMiddleware[ConsumerRecord]],
-        middlewares: Iterable[PublisherMiddleware],
+        broker_middlewares: Iterable["BrokerMiddleware[ConsumerRecord]"],
+        middlewares: Iterable["PublisherMiddleware"],
         # AsyncAPI args
         schema_: Optional[Any],
         title_: Optional[str],
         description_: Optional[str],
         include_in_schema: bool,
-    ) -> "AsyncAPIDefaultPublisher":
-        ...
+    ) -> "AsyncAPIDefaultPublisher": ...
 
     @overload
     @staticmethod
     def create(
         *,
         batch: bool,
         key: Optional[bytes],
         topic: str,
         partition: Optional[int],
         headers: Optional[Dict[str, str]],
         reply_to: str,
         # Publisher args
         broker_middlewares: Iterable[
-            BrokerMiddleware[Union[Tuple[ConsumerRecord, ...], ConsumerRecord]]
+            "BrokerMiddleware[Union[Tuple[ConsumerRecord, ...], ConsumerRecord]]"
         ],
-        middlewares: Iterable[PublisherMiddleware],
+        middlewares: Iterable["PublisherMiddleware"],
         # AsyncAPI args
         schema_: Optional[Any],
         title_: Optional[str],
         description_: Optional[str],
         include_in_schema: bool,
     ) -> Union[
         "AsyncAPIBatchPublisher",
         "AsyncAPIDefaultPublisher",
-    ]:
-        ...
+    ]: ...
 
     @override
     @staticmethod
     def create(
         *,
         batch: bool,
         key: Optional[bytes],
         topic: str,
         partition: Optional[int],
         headers: Optional[Dict[str, str]],
         reply_to: str,
         # Publisher args
         broker_middlewares: Iterable[
-            BrokerMiddleware[Union[Tuple[ConsumerRecord, ...], ConsumerRecord]]
+            "BrokerMiddleware[Union[Tuple[ConsumerRecord, ...], ConsumerRecord]]"
         ],
-        middlewares: Iterable[PublisherMiddleware],
+        middlewares: Iterable["PublisherMiddleware"],
         # AsyncAPI args
         schema_: Optional[Any],
         title_: Optional[str],
         description_: Optional[str],
         include_in_schema: bool,
     ) -> Union[
         "AsyncAPIBatchPublisher",
@@ -169,17 +180,17 @@
                 description_=description_,
                 include_in_schema=include_in_schema,
             )
 
 
 class AsyncAPIBatchPublisher(
     BatchPublisher,
-    AsyncAPIPublisher[Tuple[ConsumerRecord, ...]],
+    AsyncAPIPublisher[Tuple["ConsumerRecord", ...]],
 ):
     pass
 
 
 class AsyncAPIDefaultPublisher(
     DefaultPublisher,
-    AsyncAPIPublisher[ConsumerRecord],
+    AsyncAPIPublisher["ConsumerRecord"],
 ):
     pass
```

### Comparing `faststream-0.5.0rc0/faststream/kafka/publisher/producer.py` & `faststream-0.5.0rc1/faststream/kafka/publisher/producer.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,36 @@
-from typing import Any, Dict, Optional, Union
+from typing import TYPE_CHECKING, Any, Dict, Optional, Union
 
-from aiokafka import AIOKafkaProducer
 from typing_extensions import override
 
 from faststream.broker.message import encode_message
 from faststream.broker.publisher.proto import ProducerProto
 from faststream.exceptions import NOT_CONNECTED_YET
-from faststream.types import SendableMessage
+
+if TYPE_CHECKING:
+    from aiokafka import AIOKafkaProducer
+
+    from faststream.types import SendableMessage
 
 
 class AioKafkaFastProducer(ProducerProto):
     """A class to represent Kafka producer."""
 
-    _producer: Optional[AIOKafkaProducer]
+    _producer: Optional["AIOKafkaProducer"]
 
     def __init__(
         self,
-        producer: AIOKafkaProducer,
+        producer: "AIOKafkaProducer",
     ) -> None:
         self._producer = producer
 
     @override
     async def publish(  # type: ignore[override]
         self,
-        message: SendableMessage,
+        message: "SendableMessage",
         topic: str,
         *,
         correlation_id: str,
         key: Union[bytes, Any, None] = None,
         partition: Optional[int] = None,
         timestamp_ms: Optional[int] = None,
         headers: Optional[Dict[str, str]] = None,
@@ -52,41 +55,37 @@
 
         await self._producer.send(
             topic=topic,
             value=message,
             key=key,
             partition=partition,
             timestamp_ms=timestamp_ms,
-            headers=[(i, (j or "").encode())
-                     for i, j in headers_to_send.items()],
+            headers=[(i, (j or "").encode()) for i, j in headers_to_send.items()],
         )
 
     async def stop(self) -> None:
         if self._producer is not None:  # pragma: no branch
             await self._producer.stop()
 
     async def publish_batch(
         self,
-        *msgs: SendableMessage,
+        *msgs: "SendableMessage",
         correlation_id: str,
         topic: str,
         partition: Optional[int] = None,
         timestamp_ms: Optional[int] = None,
         headers: Optional[Dict[str, str]] = None,
         reply_to: str = "",
     ) -> None:
         """Publish a batch of messages to a topic."""
         assert self._producer, NOT_CONNECTED_YET  # nosec B101
 
         batch = self._producer.create_batch()
 
-        headers_to_send = {
-            "correlation_id": correlation_id,
-            **(headers or {})
-        }
+        headers_to_send = {"correlation_id": correlation_id, **(headers or {})}
 
         if reply_to:
             headers_to_send["reply_to"] = headers_to_send.get(
                 "reply_to",
                 reply_to,
             )
```

### Comparing `faststream-0.5.0rc0/faststream/kafka/publisher/usecase.py` & `faststream-0.5.0rc1/faststream/kafka/publisher/usecase.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 from contextlib import AsyncExitStack
 from itertools import chain
-from typing import Any, Dict, Iterable, Optional, Tuple, Union, cast
+from typing import TYPE_CHECKING, Any, Dict, Iterable, Optional, Tuple, Union, cast
 
 from aiokafka import ConsumerRecord
 from typing_extensions import Annotated, Doc, override
 
 from faststream.broker.message import gen_cor_id
 from faststream.broker.publisher.usecase import PublisherUsecase
-from faststream.broker.types import BrokerMiddleware, MsgType, PublisherMiddleware
+from faststream.broker.types import MsgType
 from faststream.exceptions import NOT_CONNECTED_YET
-from faststream.kafka.publisher.producer import AioKafkaFastProducer
-from faststream.types import SendableMessage
+
+if TYPE_CHECKING:
+    from faststream.broker.types import BrokerMiddleware, PublisherMiddleware
+    from faststream.kafka.publisher.producer import AioKafkaFastProducer
+    from faststream.types import SendableMessage
 
 
 class LogicPublisher(PublisherUsecase[MsgType]):
     """A class to publish messages to a Kafka topic."""
 
-    _producer: Optional[AioKafkaFastProducer]
+    _producer: Optional["AioKafkaFastProducer"]
 
     def __init__(
         self,
         *,
         topic: str,
         partition: Optional[int],
         headers: Optional[Dict[str, str]],
         reply_to: str,
         # Publisher args
-        broker_middlewares: Iterable[BrokerMiddleware[MsgType]],
-        middlewares: Iterable[PublisherMiddleware],
+        broker_middlewares: Iterable["BrokerMiddleware[MsgType]"],
+        middlewares: Iterable["PublisherMiddleware"],
         # AsyncAPI args
         schema_: Optional[Any],
         title_: Optional[str],
         description_: Optional[str],
         include_in_schema: bool,
     ) -> None:
         super().__init__(
@@ -64,16 +67,16 @@
         *,
         key: Optional[bytes],
         topic: str,
         partition: Optional[int],
         headers: Optional[Dict[str, str]],
         reply_to: str,
         # Publisher args
-        broker_middlewares: Iterable[BrokerMiddleware[ConsumerRecord]],
-        middlewares: Iterable[PublisherMiddleware],
+        broker_middlewares: Iterable["BrokerMiddleware[ConsumerRecord]"],
+        middlewares: Iterable["PublisherMiddleware"],
         # AsyncAPI args
         schema_: Optional[Any],
         title_: Optional[str],
         description_: Optional[str],
         include_in_schema: bool,
     ) -> None:
         super().__init__(
@@ -93,15 +96,15 @@
 
         self.key = key
 
     @override
     async def publish(
         self,
         message: Annotated[
-            SendableMessage,
+            "SendableMessage",
             Doc("Message body to send."),
         ],
         topic: Annotated[
             str,
             Doc("Topic where the message will be published."),
         ] = "",
         *,
@@ -111,50 +114,48 @@
             A key to associate with the message. Can be used to
             determine which partition to send the message to. If partition
             is `None` (and producer's partitioner config is left as default),
             then messages with the same key will be delivered to the same
             partition (but if key is `None`, partition is chosen randomly).
             Must be type `bytes`, or be serializable to bytes via configured
             `key_serializer`.
-            """)
+            """),
         ] = None,
         partition: Annotated[
             Optional[int],
             Doc("""
             Specify a partition. If not set, the partition will be
             selected using the configured `partitioner`.
             """),
         ] = None,
         timestamp_ms: Annotated[
             Optional[int],
             Doc("""
             Epoch milliseconds (from Jan 1 1970 UTC) to use as
             the message timestamp. Defaults to current time.
-            """)
+            """),
         ] = None,
         headers: Annotated[
             Optional[Dict[str, str]],
             Doc("Message headers to store metainformation."),
         ] = None,
         correlation_id: Annotated[
             Optional[str],
             Doc(
                 "Manual message **correlation_id** setter. "
                 "**correlation_id** is a useful option to trace messages."
             ),
         ] = None,
         reply_to: Annotated[
             str,
-            Doc(
-                "Reply message topic name to send response."
-            ),
+            Doc("Reply message topic name to send response."),
         ] = "",
         # publisher specific
         _extra_middlewares: Annotated[
-            Iterable[PublisherMiddleware],
+            Iterable["PublisherMiddleware"],
             Doc("Extra middlewares to wrap publishing process."),
         ] = (),
     ) -> None:
         assert self._producer, NOT_CONNECTED_YET  # nosec B101
 
         topic = topic or self.topic
         key = key or self.key
@@ -192,24 +193,24 @@
                 correlation_id=correlation_id,
                 timestamp_ms=timestamp_ms,
             )
 
         return None
 
 
-class BatchPublisher(LogicPublisher[Tuple[ConsumerRecord, ...]]):
+class BatchPublisher(LogicPublisher[Tuple["ConsumerRecord", ...]]):
     @override
     async def publish(  # type: ignore[override]
         self,
         message: Annotated[
-            Union[SendableMessage, Iterable[SendableMessage]],
+            Union["SendableMessage", Iterable["SendableMessage"]],
             Doc("One message or iterable messages bodies to send."),
         ],
         *extra_messages: Annotated[
-            SendableMessage,
+            "SendableMessage",
             Doc("Messages bodies to send."),
         ],
         topic: Annotated[
             str,
             Doc("Topic where the message will be published."),
         ] = "",
         partition: Annotated[
@@ -220,46 +221,44 @@
             """),
         ] = None,
         timestamp_ms: Annotated[
             Optional[int],
             Doc("""
             Epoch milliseconds (from Jan 1 1970 UTC) to use as
             the message timestamp. Defaults to current time.
-            """)
+            """),
         ] = None,
         headers: Annotated[
             Optional[Dict[str, str]],
             Doc("Messages headers to store metainformation."),
         ] = None,
         reply_to: Annotated[
             str,
-            Doc(
-                "Reply message topic name to send response."
-            ),
+            Doc("Reply message topic name to send response."),
         ] = "",
         correlation_id: Annotated[
             Optional[str],
             Doc(
                 "Manual message **correlation_id** setter. "
                 "**correlation_id** is a useful option to trace messages."
             ),
         ] = None,
         # publisher specific
         _extra_middlewares: Annotated[
-            Iterable[PublisherMiddleware],
+            Iterable["PublisherMiddleware"],
             Doc("Extra middlewares to wrap publishing process."),
         ] = (),
     ) -> None:
         assert self._producer, NOT_CONNECTED_YET  # nosec B101
 
-        msgs: Iterable[SendableMessage]
+        msgs: Iterable["SendableMessage"]
         if extra_messages:
-            msgs = (cast(SendableMessage, message), *extra_messages)
+            msgs = (cast("SendableMessage", message), *extra_messages)
         else:
-            msgs = cast(Iterable[SendableMessage], message)
+            msgs = cast(Iterable["SendableMessage"], message)
 
         topic = topic or self.topic
         partition = partition or self.partition
         headers = headers or self.headers
         reply_to = reply_to or self.reply_to
         correlation_id = correlation_id or gen_cor_id()
```

### Comparing `faststream-0.5.0rc0/faststream/kafka/schemas/params.py` & `faststream-0.5.0rc1/faststream/kafka/schemas/params.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/faststream/kafka/subscriber/asyncapi.py` & `faststream-0.5.0rc1/faststream/kafka/subscriber/asyncapi.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,43 @@
-from typing import Callable, Dict, Iterable, Literal, Optional, Tuple, Union, overload
+from typing import (
+    TYPE_CHECKING,
+    Callable,
+    Dict,
+    Iterable,
+    Literal,
+    Optional,
+    Tuple,
+    Union,
+    overload,
+)
 
-from aiokafka import AIOKafkaConsumer, ConsumerRecord
-from fast_depends.dependencies import Depends
 from typing_extensions import override
 
 from faststream.asyncapi.schema import (
     Channel,
     ChannelBinding,
     CorrelationId,
     Message,
     Operation,
 )
 from faststream.asyncapi.schema.bindings import kafka
 from faststream.asyncapi.utils import resolve_payloads
-from faststream.broker.types import BrokerMiddleware, MsgType
+from faststream.broker.types import MsgType
 from faststream.kafka.subscriber.usecase import (
     BatchSubscriber,
     DefaultSubscriber,
     LogicSubscriber,
 )
 
+if TYPE_CHECKING:
+    from aiokafka import AIOKafkaConsumer, ConsumerRecord
+    from fast_depends.dependencies import Depends
+
+    from faststream.broker.types import BrokerMiddleware
+
 
 class AsyncAPISubscriber(LogicSubscriber[MsgType]):
     """A class to handle logic and async API operations."""
 
     def get_name(self) -> str:
         return f'{",".join(self.topics)}:{self.call_name}'
 
@@ -58,99 +72,94 @@
     def create(
         *topics: str,
         batch: Literal[True],
         batch_timeout_ms: int,
         max_records: Optional[int],
         # Kafka information
         group_id: Optional[str],
-        builder: Callable[..., AIOKafkaConsumer],
+        builder: Callable[..., "AIOKafkaConsumer"],
         is_manual: bool,
         # Subscriber args
         no_ack: bool,
         retry: bool,
-        broker_dependencies: Iterable[Depends],
-        broker_middlewares: Iterable[BrokerMiddleware[Tuple[ConsumerRecord, ...]]],
+        broker_dependencies: Iterable["Depends"],
+        broker_middlewares: Iterable["BrokerMiddleware[Tuple[ConsumerRecord, ...]]"],
         # AsyncAPI args
         title_: Optional[str],
         description_: Optional[str],
         include_in_schema: bool,
-    ) -> "AsyncAPIBatchSubscriber":
-        ...
+    ) -> "AsyncAPIBatchSubscriber": ...
 
     @overload
     @staticmethod
     def create(
         *topics: str,
         batch: Literal[False],
         batch_timeout_ms: int,
         max_records: Optional[int],
         # Kafka information
         group_id: Optional[str],
-        builder: Callable[..., AIOKafkaConsumer],
+        builder: Callable[..., "AIOKafkaConsumer"],
         is_manual: bool,
         # Subscriber args
         no_ack: bool,
         retry: bool,
-        broker_dependencies: Iterable[Depends],
-        broker_middlewares: Iterable[BrokerMiddleware[ConsumerRecord]],
+        broker_dependencies: Iterable["Depends"],
+        broker_middlewares: Iterable["BrokerMiddleware[ConsumerRecord]"],
         # AsyncAPI args
         title_: Optional[str],
         description_: Optional[str],
         include_in_schema: bool,
-    ) -> "AsyncAPIDefaultSubscriber":
-        ...
+    ) -> "AsyncAPIDefaultSubscriber": ...
 
     @overload
     @staticmethod
     def create(
         *topics: str,
         batch: bool,
         batch_timeout_ms: int,
         max_records: Optional[int],
         # Kafka information
         group_id: Optional[str],
-        builder: Callable[..., AIOKafkaConsumer],
+        builder: Callable[..., "AIOKafkaConsumer"],
         is_manual: bool,
         # Subscriber args
         no_ack: bool,
         retry: bool,
-        broker_dependencies: Iterable[Depends],
-        broker_middlewares: Iterable[BrokerMiddleware[Union[
-            ConsumerRecord,
-            Tuple[ConsumerRecord, ...]],
-        ]],
+        broker_dependencies: Iterable["Depends"],
+        broker_middlewares: Iterable[
+            "BrokerMiddleware[Union[ConsumerRecord, Tuple[ConsumerRecord, ...]]]"
+        ],
         # AsyncAPI args
         title_: Optional[str],
         description_: Optional[str],
         include_in_schema: bool,
     ) -> Union[
         "AsyncAPIDefaultSubscriber",
         "AsyncAPIBatchSubscriber",
-    ]:
-        ...
+    ]: ...
 
     @override
     @staticmethod
     def create(
         *topics: str,
         batch: bool,
         batch_timeout_ms: int,
         max_records: Optional[int],
         # Kafka information
         group_id: Optional[str],
-        builder: Callable[..., AIOKafkaConsumer],
+        builder: Callable[..., "AIOKafkaConsumer"],
         is_manual: bool,
         # Subscriber args
         no_ack: bool,
         retry: bool,
-        broker_dependencies: Iterable[Depends],
-        broker_middlewares: Iterable[BrokerMiddleware[Union[
-            ConsumerRecord,
-            Tuple[ConsumerRecord, ...]],
-        ]],
+        broker_dependencies: Iterable["Depends"],
+        broker_middlewares: Iterable[
+            "BrokerMiddleware[Union[ConsumerRecord, Tuple[ConsumerRecord, ...]]]"
+        ],
         # AsyncAPI args
         title_: Optional[str],
         description_: Optional[str],
         include_in_schema: bool,
     ) -> Union[
         "AsyncAPIDefaultSubscriber",
         "AsyncAPIBatchSubscriber",
@@ -183,14 +192,19 @@
                 broker_middlewares=broker_middlewares,
                 title_=title_,
                 description_=description_,
                 include_in_schema=include_in_schema,
             )
 
 
-
-class AsyncAPIDefaultSubscriber(DefaultSubscriber, AsyncAPISubscriber[ConsumerRecord],):
+class AsyncAPIDefaultSubscriber(
+    DefaultSubscriber,
+    AsyncAPISubscriber["ConsumerRecord"],
+):
     pass
 
 
-class AsyncAPIBatchSubscriber(BatchSubscriber, AsyncAPISubscriber[Tuple[ConsumerRecord, ...]],):
+class AsyncAPIBatchSubscriber(
+    BatchSubscriber,
+    AsyncAPISubscriber[Tuple["ConsumerRecord", ...]],
+):
     pass
```

### Comparing `faststream-0.5.0rc0/faststream/kafka/subscriber/usecase.py` & `faststream-0.5.0rc1/faststream/kafka/subscriber/usecase.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,68 +1,70 @@
 import asyncio
 from abc import ABC, abstractmethod
 from itertools import chain
 from typing import (
+    TYPE_CHECKING,
     Any,
     Callable,
     Dict,
     Iterable,
     Optional,
     Sequence,
     Tuple,
 )
 
 import anyio
-from aiokafka import AIOKafkaConsumer, ConsumerRecord
 from aiokafka.errors import ConsumerStoppedError, KafkaError
-from fast_depends.dependencies import Depends
 from typing_extensions import override
 
-from faststream.broker.message import StreamMessage
 from faststream.broker.publisher.fake import FakePublisher
-from faststream.broker.publisher.proto import ProducerProto
 from faststream.broker.subscriber.usecase import SubscriberUsecase
 from faststream.broker.types import (
-    AsyncDecoder,
-    AsyncParser,
+    AsyncCallable,
     BrokerMiddleware,
-    CustomDecoder,
-    CustomParser,
+    CustomCallable,
     MsgType,
 )
 from faststream.kafka.parser import AioKafkaParser
-from faststream.kafka.schemas.params import ConsumerConnectionParams
-from faststream.types import AnyDict, LoggerProto
+
+if TYPE_CHECKING:
+    from aiokafka import AIOKafkaConsumer, ConsumerRecord
+    from fast_depends.dependencies import Depends
+
+    from faststream.broker.message import StreamMessage
+    from faststream.broker.publisher.proto import ProducerProto
+    from faststream.kafka.schemas.params import ConsumerConnectionParams
+    from faststream.types import AnyDict, LoggerProto
 
 
 class LogicSubscriber(ABC, SubscriberUsecase[MsgType]):
     """A class to handle logic for consuming messages from Kafka."""
 
     topics: Sequence[str]
     group_id: Optional[str]
 
-    consumer: Optional[AIOKafkaConsumer]
+    consumer: Optional["AIOKafkaConsumer"]
     task: Optional["asyncio.Task[None]"]
     client_id: Optional[str]
     batch: bool
 
     def __init__(
         self,
         *topics: str,
         # Kafka information
         group_id: Optional[str],
-        builder: Callable[..., AIOKafkaConsumer],
+        builder: Callable[..., "AIOKafkaConsumer"],
         is_manual: bool,
         # Subscriber args
-        default_parser: AsyncParser[MsgType],
-        default_decoder: AsyncDecoder[StreamMessage[MsgType]],
+        default_parser: "AsyncCallable",
+        default_decoder: "AsyncCallable",
         no_ack: bool,
         retry: bool,
-        broker_dependencies: Iterable[Depends],
-        broker_middlewares: Iterable[BrokerMiddleware[MsgType]],
+        broker_dependencies: Iterable["Depends"],
+        broker_middlewares: Iterable["BrokerMiddleware[MsgType]"],
         # AsyncAPI args
         title_: Optional[str],
         description_: Optional[str],
         include_in_schema: bool,
     ) -> None:
         super().__init__(
             default_parser=default_parser,
@@ -83,30 +85,30 @@
         self.is_manual = is_manual
         self.builder = builder
         self.consumer = None
         self.task = None
 
         # Setup it later
         self.client_id = ""
-        self.__connection_args: ConsumerConnectionParams = {}
+        self.__connection_args: "ConsumerConnectionParams" = {}
 
     @override
     def setup(  # type: ignore[override]
         self,
         *,
         client_id: Optional[str],
-        connection_args: ConsumerConnectionParams,
+        connection_args: "ConsumerConnectionParams",
         # basic args
-        logger: Optional[LoggerProto],
-        producer: Optional[ProducerProto],
+        logger: Optional["LoggerProto"],
+        producer: Optional["ProducerProto"],
         graceful_timeout: Optional[float],
-        extra_context: Optional[AnyDict],
+        extra_context: Optional["AnyDict"],
         # broker options
-        broker_parser: Optional["CustomParser[MsgType]"],
-        broker_decoder: Optional["CustomDecoder[StreamMessage[MsgType]]"],
+        broker_parser: Optional["CustomCallable"],
+        broker_decoder: Optional["CustomCallable"],
         # dependant args
         apply_types: bool,
         is_validate: bool,
         _get_dependant: Optional[Callable[..., Any]],
     ) -> None:
         self.client_id = client_id
         self.__connection_args = connection_args
@@ -146,15 +148,16 @@
 
         if self.task is not None and not self.task.done():
             self.task.cancel()
 
         self.task = None
 
     def _make_response_publisher(
-        self, message: "StreamMessage[Any]"
+        self,
+        message: "StreamMessage[Any]",
     ) -> Sequence[FakePublisher]:
         if not message.reply_to or self._producer is None:
             return ()
 
         return (
             FakePublisher(
                 self._producer.publish,
@@ -172,15 +175,16 @@
         assert self.consumer, "You should setup subscriber at first."  # nosec B101
 
         connected = True
         while self.running:
             try:
                 msg = await self.get_msg()
 
-            except KafkaError:  # pragma: no cover
+            # pragma: no cover
+            except KafkaError:  # noqa: PERF203
                 if connected:
                     connected = False
                 await anyio.sleep(5)
 
             except ConsumerStoppedError:
                 return
 
@@ -188,15 +192,18 @@
                 if not connected:  # pragma: no cover
                     connected = True
 
                 if msg:
                     await self.consume(msg)
 
     @staticmethod
-    def get_routing_hash(topics: Iterable[str], group_id: Optional[str] = None) -> int:
+    def get_routing_hash(
+        topics: Iterable[str],
+        group_id: Optional[str] = None,
+    ) -> int:
         return hash("".join((*topics, group_id or "")))
 
     def __hash__(self) -> int:
         return self.get_routing_hash(self.topics, self.group_id)
 
     @staticmethod
     def build_log_context(
@@ -224,32 +231,30 @@
         return self.build_log_context(
             message=message,
             topic=topic,
             group_id=self.group_id,
         )
 
     def add_prefix(self, prefix: str) -> None:
-        self.topics = tuple(
-            "".join((prefix, t))
-            for t in self.topics
-        )
+        self.topics = tuple("".join((prefix, t)) for t in self.topics)
+
 
-class DefaultSubscriber(LogicSubscriber[ConsumerRecord]):
+class DefaultSubscriber(LogicSubscriber["ConsumerRecord"]):
     def __init__(
         self,
         *topics: str,
         # Kafka information
         group_id: Optional[str],
-        builder: Callable[..., AIOKafkaConsumer],
+        builder: Callable[..., "AIOKafkaConsumer"],
         is_manual: bool,
         # Subscriber args
         no_ack: bool,
         retry: bool,
-        broker_dependencies: Iterable[Depends],
-        broker_middlewares: Iterable[BrokerMiddleware[ConsumerRecord]],
+        broker_dependencies: Iterable["Depends"],
+        broker_middlewares: Iterable["BrokerMiddleware[ConsumerRecord]"],
         # AsyncAPI args
         title_: Optional[str],
         description_: Optional[str],
         include_in_schema: bool,
     ) -> None:
         super().__init__(
             *topics,
@@ -266,34 +271,36 @@
             broker_dependencies=broker_dependencies,
             # AsyncAPI args
             title_=title_,
             description_=description_,
             include_in_schema=include_in_schema,
         )
 
-    async def get_msg(self) -> ConsumerRecord:
+    async def get_msg(self) -> "ConsumerRecord":
         assert self.consumer, "You should setup subscriber at first."  # nosec B101
         return await self.consumer.getone()
 
 
-class BatchSubscriber(LogicSubscriber[Tuple[ConsumerRecord, ...]]):
+class BatchSubscriber(LogicSubscriber[Tuple["ConsumerRecord", ...]]):
     def __init__(
         self,
         *topics: str,
         batch_timeout_ms: int,
         max_records: Optional[int],
         # Kafka information
         group_id: Optional[str],
-        builder: Callable[..., AIOKafkaConsumer],
+        builder: Callable[..., "AIOKafkaConsumer"],
         is_manual: bool,
         # Subscriber args
         no_ack: bool,
         retry: bool,
-        broker_dependencies: Iterable[Depends],
-        broker_middlewares: Iterable[BrokerMiddleware[Sequence[Tuple[ConsumerRecord, ...]]]],
+        broker_dependencies: Iterable["Depends"],
+        broker_middlewares: Iterable[
+            "BrokerMiddleware[Sequence[Tuple[ConsumerRecord, ...]]]"
+        ],
         # AsyncAPI args
         title_: Optional[str],
         description_: Optional[str],
         include_in_schema: bool,
     ) -> None:
         self.batch_timeout_ms = batch_timeout_ms
         self.max_records = max_records
@@ -313,15 +320,15 @@
             broker_dependencies=broker_dependencies,
             # AsyncAPI args
             title_=title_,
             description_=description_,
             include_in_schema=include_in_schema,
         )
 
-    async def get_msg(self) -> Tuple[ConsumerRecord, ...]:
+    async def get_msg(self) -> Tuple["ConsumerRecord", ...]:
         assert self.consumer, "You should setup subscriber at first."  # nosec B101
 
         messages = await self.consumer.getmany(
             timeout_ms=self.batch_timeout_ms,
             max_records=self.max_records,
         )
```

### Comparing `faststream-0.5.0rc0/faststream/log/formatter.py` & `faststream-0.5.0rc1/faststream/log/formatter.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/faststream/log/logging.py` & `faststream-0.5.0rc1/faststream/log/logging.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/faststream/nats/__init__.py` & `faststream-0.5.0rc1/faststream/nats/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/faststream/nats/annotations.py` & `faststream-0.5.0rc1/faststream/nats/annotations.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/faststream/nats/helpers.py` & `faststream-0.5.0rc1/faststream/nats/helpers.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/faststream/nats/message.py` & `faststream-0.5.0rc1/faststream/nats/message.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/faststream/nats/parser.py` & `faststream-0.5.0rc1/faststream/nats/parser.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 from typing import TYPE_CHECKING, Any, List, Optional
 
-from nats.aio.msg import Msg
-
 from faststream.broker.message import StreamMessage, decode_message, gen_cor_id
 from faststream.nats.message import NatsBatchMessage, NatsMessage
-from faststream.types import AnyDict, DecodedMessage
 from faststream.utils.context.repository import context
 
 if TYPE_CHECKING:
+    from nats.aio.msg import Msg
+
     from faststream.nats.subscriber.usecase import LogicSubscriber
+    from faststream.types import AnyDict, DecodedMessage
 
 
 class NatsBaseParser:
     """A class to parse NATS messages."""
 
     @staticmethod
     def get_path(
         subject: str,
-    ) -> Optional[AnyDict]:
-        path: Optional[AnyDict] = None
+    ) -> Optional["AnyDict"]:
+        path: Optional["AnyDict"] = None
 
         handler: Optional["LogicSubscriber[Any]"]
         if (
             (handler := context.get_local("handler_")) is not None
             and (path_re := handler.path_regex) is not None
             and (match := path_re.match(subject)) is not None
         ):
             path = match.groupdict()
 
         return path
 
     @staticmethod
     async def decode_message(
-        msg: StreamMessage["Msg"],
-    ) -> DecodedMessage:
+        msg: "StreamMessage[Msg]",
+    ) -> "DecodedMessage":
         return decode_message(msg)
 
 
 class NatsParser(NatsBaseParser):
     """A class to parse NATS core messages."""
 
     @classmethod
     async def parse_message(
         cls,
         message: "Msg",
         *,
-        path: Optional[AnyDict] = None,
-    ) -> StreamMessage["Msg"]:
+        path: Optional["AnyDict"] = None,
+    ) -> "StreamMessage[Msg]":
         if path is None:
             path = cls.get_path(message.subject)
 
         headers = message.header or {}
 
         return StreamMessage["Msg"](
             raw_message=message,
@@ -68,16 +68,16 @@
     """A class to parse NATS JS messages."""
 
     @classmethod
     async def parse_message(
         cls,
         message: "Msg",
         *,
-        path: Optional[AnyDict] = None,
-    ) -> StreamMessage["Msg"]:
+        path: Optional["AnyDict"] = None,
+    ) -> "StreamMessage[Msg]":
         if path is None:
             path = cls.get_path(message.subject)
 
         headers = message.header or {}
 
         return NatsMessage(
             raw_message=message,
@@ -93,28 +93,28 @@
 
 class BatchParser(JsParser):
     """A class to parse NATS batch messages."""
 
     @staticmethod
     async def parse_batch(
         message: List["Msg"],
-    ) -> StreamMessage[List["Msg"]]:
+    ) -> "StreamMessage[List[Msg]]":
         return NatsBatchMessage(
             raw_message=message,
             body=[m.data for m in message],
         )
 
     @classmethod
     async def decode_batch(
         cls,
-        msg: StreamMessage[List["Msg"]],
-    ) -> List[DecodedMessage]:
-        data: List[DecodedMessage] = []
+        msg: "StreamMessage[List[Msg]]",
+    ) -> List["DecodedMessage"]:
+        data: List["DecodedMessage"] = []
 
-        path: Optional[AnyDict] = None
+        path: Optional["AnyDict"] = None
         for m in msg.raw_message:
             one_msg = await cls.parse_message(m, path=path)
             path = one_msg.path
 
             data.append(decode_message(one_msg))
 
         return data
```

### Comparing `faststream-0.5.0rc0/faststream/nats/router.py` & `faststream-0.5.0rc1/faststream/nats/broker/registrator.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,130 +1,44 @@
-from typing import TYPE_CHECKING, Any, Callable, Dict, Iterable, Optional, Union
+from typing import TYPE_CHECKING, Any, Dict, Iterable, Optional, Union, cast
 
 from nats.js import api
-from typing_extensions import Annotated, Doc, deprecated
+from typing_extensions import Annotated, Doc, deprecated, override
 
-from faststream.broker.router import ArgsContainer, BrokerRouter, SubscriberRoute
-from faststream.broker.types import PublisherMiddleware
+from faststream.broker.core.abc import ABCBroker
 from faststream.broker.utils import default_filter
-from faststream.nats.broker.registrator import NatsRegistrator
+from faststream.nats.publisher.asyncapi import AsyncAPIPublisher
+from faststream.nats.subscriber.asyncapi import AsyncAPISubscriber
 
 if TYPE_CHECKING:
     from fast_depends.dependencies import Depends
-    from nats.aio.msg import Msg
+    from nats.aio.msg import Msg  # noqa: F401
 
-    from faststream.broker.message import StreamMessage
     from faststream.broker.types import (
-        BrokerMiddleware,
-        CustomDecoder,
-        CustomParser,
+        CustomCallable,
         Filter,
+        PublisherMiddleware,
         SubscriberMiddleware,
     )
+    from faststream.nats.message import NatsBatchMessage, NatsMessage
     from faststream.nats.schemas import JStream, PullSub
-    from faststream.types import SendableMessage
 
 
-class NatsPublisher(ArgsContainer):
-    """Delayed NatsPublisher registration object.
+class NatsRegistrator(ABCBroker["Msg"]):
+    """Includable to RabbitBroker router."""
 
-    Just a copy of `KafkaRegistrator.publisher(...)` arguments.
-    """
+    _subscribers: Dict[int, "AsyncAPISubscriber"]
+    _publishers: Dict[int, "AsyncAPIPublisher"]
 
-    def __init__(
+    @override
+    def subscriber(  # type: ignore[override]
         self,
         subject: Annotated[
             str,
-            Doc("NATS subject to send message."),
-        ],
-        *,
-        headers: Annotated[
-            Optional[Dict[str, str]],
-            Doc(
-                "Message headers to store metainformation. "
-                "**content-type** and **correlation_id** will be setted automatically by framework anyway. "
-                "Can be overridden by `publish.headers` if specified."
-            ),
-        ] = None,
-        reply_to: Annotated[
-            str,
-            Doc("NATS subject name to send response."),
-        ] = "",
-        # JS
-        stream: Annotated[
-            Union[str, "JStream", None],
-            Doc(
-                "This option validates that the target `subject` is in presented stream. "
-                "Can be omitted without any effect."
-            ),
-        ] = None,
-        timeout: Annotated[
-            Optional[float],
-            Doc("Timeout to send message to NATS."),
-        ] = None,
-        # basic args
-        middlewares: Annotated[
-            Iterable[PublisherMiddleware],
-            Doc("Publisher middlewares to wrap outgoing messages."),
-        ] = (),
-        # AsyncAPI information
-        title: Annotated[
-            Optional[str],
-            Doc("AsyncAPI publisher object title."),
-        ] = None,
-        description: Annotated[
-            Optional[str],
-            Doc("AsyncAPI publisher object description."),
-        ] = None,
-        schema: Annotated[
-            Optional[Any],
-            Doc(
-                "AsyncAPI publishing message type. "
-                "Should be any python-native object annotation or `pydantic.BaseModel`."
-            ),
-        ] = None,
-        include_in_schema: Annotated[
-            bool,
-            Doc("Whetever to include operation in AsyncAPI schema or not."),
-        ] = True,
-    ) -> None:
-        super().__init__(
-            subject=subject,
-            headers=headers,
-            reply_to=reply_to,
-            stream=stream,
-            timeout=timeout,
-            middlewares=middlewares,
-            title=title,
-            description=description,
-            schema=schema,
-            include_in_schema=include_in_schema,
-        )
-
-
-class NatsRoute(SubscriberRoute):
-    """Class to store delayed NatsBroker subscriber registration."""
-
-    def __init__(
-        self,
-        call: Annotated[
-            Callable[..., "SendableMessage"],
-            Doc(
-                "Message handler function "
-                "to wrap the same with `@broker.subscriber(...)` way."
-            ),
-        ],
-        subject: Annotated[
-            str,
             Doc("NATS subject to subscribe."),
         ],
-        publishers: Annotated[
-            Iterable[NatsPublisher],
-            Doc("Nats publishers to broadcast the handler result."),
-        ] = (),
         queue: Annotated[
             str,
             Doc(
                 "Subscribers' NATS queue name. Subscribers with same queue name will be load balanced by the NATS "
                 "server."
             ),
         ] = "",
@@ -211,27 +125,30 @@
         ] = None,
         # broker arguments
         dependencies: Annotated[
             Iterable["Depends"],
             Doc("Dependencies list (`[Depends(),]`) to apply to the subscriber."),
         ] = (),
         parser: Annotated[
-            Optional["CustomParser[Msg]"],
+            Optional["CustomCallable"],
             Doc("Parser to map original **nats-py** Msg to FastStream one."),
         ] = None,
         decoder: Annotated[
-            Optional["CustomDecoder[StreamMessage[Msg]]"],
+            Optional["CustomCallable"],
             Doc("Function to decode FastStream msg bytes body to python objects."),
         ] = None,
         middlewares: Annotated[
             Iterable["SubscriberMiddleware"],
             Doc("Subscriber middlewares to wrap incoming message processing."),
         ] = (),
         filter: Annotated[
-            "Filter[StreamMessage[Msg]]",
+            Union[
+                "Filter[NatsMessage]",
+                "Filter[NatsBatchMessage]",
+            ],
             Doc(
                 "Overload subscriber to consume various messages from the same source."
             ),
             deprecated(
                 "Deprecated in **FastStream 0.5.0**. "
                 "Please, create `subscriber` object and use it explicitly instead. "
                 "Argument will be removed in **FastStream 0.6.0**."
@@ -261,91 +178,143 @@
                 "Uses decorated docstring as default."
             ),
         ] = None,
         include_in_schema: Annotated[
             bool,
             Doc("Whetever to include operation in AsyncAPI schema or not."),
         ] = True,
-    ) -> None:
-        super().__init__(
-            call,
-            subject=subject,
-            publishers=publishers,
-            pending_msgs_limit=pending_msgs_limit,
-            pending_bytes_limit=pending_bytes_limit,
-            max_msgs=max_msgs,
-            durable=durable,
-            config=config,
-            ordered_consumer=ordered_consumer,
-            idle_heartbeat=idle_heartbeat,
-            flow_control=flow_control,
-            deliver_policy=deliver_policy,
-            headers_only=headers_only,
-            pull_sub=pull_sub,
-            inbox_prefix=inbox_prefix,
-            ack_first=ack_first,
-            stream=stream,
-            max_workers=max_workers,
-            queue=queue,
-            dependencies=dependencies,
-            parser=parser,
-            decoder=decoder,
-            middlewares=middlewares,
-            filter=filter,
-            retry=retry,
-            no_ack=no_ack,
-            title=title,
-            description=description,
-            include_in_schema=include_in_schema,
-        )
+    ) -> AsyncAPISubscriber:
+        """Creates NATS subscriber object.
 
+        You can use it as a handler decorator `@broker.subscriber(...)`.
+        """
+        subscriber = cast(
+            AsyncAPISubscriber,
+            super().subscriber(
+                AsyncAPISubscriber.create(
+                    subject=subject,
+                    queue=queue,
+                    stream=stream,
+                    pull_sub=pull_sub,
+                    max_workers=max_workers,
+                    # extra args
+                    pending_msgs_limit=pending_msgs_limit,
+                    pending_bytes_limit=pending_bytes_limit,
+                    max_msgs=max_msgs,
+                    durable=durable,
+                    config=config,
+                    ordered_consumer=ordered_consumer,
+                    idle_heartbeat=idle_heartbeat,
+                    flow_control=flow_control,
+                    deliver_policy=deliver_policy,
+                    headers_only=headers_only,
+                    inbox_prefix=inbox_prefix,
+                    ack_first=ack_first,
+                    # subscriber args
+                    no_ack=no_ack,
+                    retry=retry,
+                    broker_middlewares=self._middlewares,
+                    broker_dependencies=self._dependencies,
+                    # AsyncAPI
+                    title_=title,
+                    description_=description,
+                    include_in_schema=self._solve_include_in_schema(include_in_schema),
+                )
+            ),
+        )
 
-class NatsRouter(
-    BrokerRouter["Msg"],
-    NatsRegistrator,
-):
-    """Includable to NatsBroker router."""
+        return subscriber.add_call(
+            filter_=filter,
+            parser_=parser or self._parser,
+            decoder_=decoder or self._decoder,
+            dependencies_=dependencies,
+            middlewares_=middlewares,
+        )
 
-    def __init__(
+    @override
+    def publisher(  # type: ignore[override]
         self,
-        prefix: Annotated[
+        subject: Annotated[
             str,
-            Doc("String prefix to add to all subscribers subjects."),
-        ] = "",
-        handlers: Annotated[
-            Iterable[NatsRoute],
-            Doc("Route object to include."),
-        ] = (),
+            Doc("NATS subject to send message."),
+        ],
         *,
-        dependencies: Annotated[
-            Iterable["Depends"],
+        headers: Annotated[
+            Optional[Dict[str, str]],
+            Doc(
+                "Message headers to store metainformation. "
+                "**content-type** and **correlation_id** will be set automatically by framework anyway. "
+                "Can be overridden by `publish.headers` if specified."
+            ),
+        ] = None,
+        reply_to: Annotated[
+            str,
+            Doc("NATS subject name to send response."),
+        ] = "",
+        # JS
+        stream: Annotated[
+            Union[str, "JStream", None],
             Doc(
-                "Dependencies list (`[Depends(),]`) to apply to all routers' publishers/subscribers."
+                "This option validates that the target `subject` is in presented stream. "
+                "Can be omitted without any effect."
             ),
-        ] = (),
+        ] = None,
+        timeout: Annotated[
+            Optional[float],
+            Doc("Timeout to send message to NATS."),
+        ] = None,
+        # basic args
         middlewares: Annotated[
-            Iterable["BrokerMiddleware[Msg]"],
-            Doc("Router middlewares to apply to all routers' publishers/subscribers."),
+            Iterable["PublisherMiddleware"],
+            Doc("Publisher middlewares to wrap outgoing messages."),
         ] = (),
-        parser: Annotated[
-            Optional["CustomParser[Msg]"],
-            Doc("Parser to map original **IncomingMessage** Msg to FastStream one."),
+        # AsyncAPI information
+        title: Annotated[
+            Optional[str],
+            Doc("AsyncAPI publisher object title."),
         ] = None,
-        decoder: Annotated[
-            Optional["CustomDecoder[StreamMessage[Msg]]"],
-            Doc("Function to decode FastStream msg bytes body to python objects."),
+        description: Annotated[
+            Optional[str],
+            Doc("AsyncAPI publisher object description."),
+        ] = None,
+        schema: Annotated[
+            Optional[Any],
+            Doc(
+                "AsyncAPI publishing message type. "
+                "Should be any python-native object annotation or `pydantic.BaseModel`."
+            ),
         ] = None,
         include_in_schema: Annotated[
-            Optional[bool],
+            bool,
             Doc("Whetever to include operation in AsyncAPI schema or not."),
-        ] = None,
-    ) -> None:
-        super().__init__(
-            handlers=handlers,
-            # basic args
-            prefix=prefix,
-            dependencies=dependencies,
-            middlewares=middlewares,
-            parser=parser,
-            decoder=decoder,
-            include_in_schema=include_in_schema,
+        ] = True,
+    ) -> "AsyncAPIPublisher":
+        """Creates long-living and AsyncAPI-documented publisher object.
+
+        You can use it as a handler decorator (handler should be decorated by `@broker.subscriber(...)` too) - `@broker.publisher(...)`.
+        In such case publisher will publish your handler return value.
+
+        Or you can create a publisher object to call it lately - `broker.publisher(...).publish(...)`.
+        """
+        publisher = cast(
+            AsyncAPIPublisher,
+            super().publisher(
+                publisher=AsyncAPIPublisher.create(
+                    subject=subject,
+                    headers=headers,
+                    # Core
+                    reply_to=reply_to,
+                    # JS
+                    timeout=timeout,
+                    stream=stream,
+                    # Specific
+                    broker_middlewares=self._middlewares,
+                    middlewares=middlewares,
+                    # AsyncAPI
+                    title_=title,
+                    description_=description,
+                    schema_=schema,
+                    include_in_schema=self._solve_include_in_schema(include_in_schema),
+                )
+            ),
         )
+        return publisher
```

### Comparing `faststream-0.5.0rc0/faststream/nats/security.py` & `faststream-0.5.0rc1/faststream/nats/security.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,34 @@
-from typing import Optional
+from typing import TYPE_CHECKING, Optional
 
 from faststream.security import (
     BaseSecurity,
     SASLPlaintext,
 )
-from faststream.types import AnyDict
 
+if TYPE_CHECKING:
+    from faststream.types import AnyDict
 
-def parse_security(security: Optional[BaseSecurity]) -> AnyDict:
+
+def parse_security(security: Optional[BaseSecurity]) -> "AnyDict":
     if security is None:
         return {}
     elif isinstance(security, SASLPlaintext):
         return _parse_sasl_plaintext(security)
     elif isinstance(security, BaseSecurity):
         return _parse_base_security(security)
     else:
         raise NotImplementedError(f"NatsBroker does not support {type(security)}")
 
 
-def _parse_base_security(security: BaseSecurity) -> AnyDict:
+def _parse_base_security(security: BaseSecurity) -> "AnyDict":
     return {
         "tls": security.ssl_context,
     }
 
 
-def _parse_sasl_plaintext(security: SASLPlaintext) -> AnyDict:
+def _parse_sasl_plaintext(security: SASLPlaintext) -> "AnyDict":
     return {
         "tls": security.ssl_context,
         "user": security.username,
         "password": security.password,
     }
```

### Comparing `faststream-0.5.0rc0/faststream/nats/testing.py` & `faststream-0.5.0rc1/faststream/nats/testing.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Union
 
 from nats.aio.msg import Msg
 from typing_extensions import override
 
 from faststream.broker.message import encode_message, gen_cor_id
-from faststream.broker.wrapper.call import HandlerCallWrapper
 from faststream.nats.broker import NatsBroker
 from faststream.nats.publisher.producer import NatsFastProducer
 from faststream.nats.schemas.js_stream import is_subject_match_wildcard
 from faststream.nats.subscriber.asyncapi import AsyncAPISubscriber
 from faststream.testing.broker import TestBroker, call_handler
-from faststream.types import AnyDict, SendableMessage
 
 if TYPE_CHECKING:
+    from faststream.broker.wrapper.call import HandlerCallWrapper
     from faststream.nats.publisher.asyncapi import AsyncAPIPublisher
+    from faststream.types import AnyDict, SendableMessage
 
 __all__ = ("TestNatsBroker",)
 
 
 class TestNatsBroker(TestBroker[NatsBroker]):
     """A class to test NATS brokers."""
 
     @staticmethod
     def create_publisher_fake_subscriber(
         broker: NatsBroker,
         publisher: "AsyncAPIPublisher",
-    ) -> HandlerCallWrapper[Any, Any, Any]:
+    ) -> "HandlerCallWrapper[Any, Any, Any]":
         sub = broker.subscriber(publisher.subject)
 
         if not sub.calls:
 
             @sub
             def f(msg: Any) -> None:
                 pass
@@ -54,15 +54,15 @@
 class FakeProducer(NatsFastProducer):
     def __init__(self, broker: NatsBroker) -> None:
         self.broker = broker
 
     @override
     async def publish(  # type: ignore[override]
         self,
-        message: SendableMessage,
+        message: "SendableMessage",
         subject: str,
         reply_to: str = "",
         headers: Optional[Dict[str, str]] = None,
         correlation_id: Optional[str] = None,
         # NatsJSFastProducer compatibility
         timeout: Optional[float] = None,
         stream: Optional[str] = None,
@@ -101,20 +101,20 @@
                 if rpc:
                     return r
 
         return None
 
 
 def build_message(
-    message: SendableMessage,
+    message: "SendableMessage",
     subject: str,
     *,
     reply_to: str = "",
     correlation_id: Optional[str] = None,
-    headers: Optional[AnyDict] = None,
+    headers: Optional["AnyDict"] = None,
 ) -> "PatchedMessage":
     msg, content_type = encode_message(message)
     return PatchedMessage(
         _client=None,  # type: ignore
         subject=subject,
         reply=reply_to,
         data=msg,
```

### Comparing `faststream-0.5.0rc0/faststream/nats/broker/broker.py` & `faststream-0.5.0rc1/faststream/nats/broker/broker.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,22 +27,19 @@
 )
 from nats.errors import Error
 from nats.js.errors import BadRequestError
 from typing_extensions import Annotated, Doc, override
 
 from faststream.__about__ import SERVICE_NAME
 from faststream.broker.message import gen_cor_id
-from faststream.broker.publisher.proto import ProducerProto
 from faststream.nats.broker.logging import NatsLoggingBroker
 from faststream.nats.broker.registrator import NatsRegistrator
-from faststream.nats.publisher.asyncapi import AsyncAPIPublisher
 from faststream.nats.publisher.producer import NatsFastProducer, NatsJSFastProducer
 from faststream.nats.security import parse_security
 from faststream.nats.subscriber.asyncapi import AsyncAPISubscriber
-from faststream.types import AnyDict
 
 if TYPE_CHECKING:
     import ssl
     from types import TracebackType
 
     from fast_depends.dependencies import Depends
     from nats.aio.client import (
@@ -54,22 +51,22 @@
         SignatureCallback,
     )
     from nats.aio.msg import Msg
     from nats.js.client import JetStreamContext
     from typing_extensions import TypedDict, Unpack
 
     from faststream.asyncapi import schema as asyncapi
-    from faststream.broker.message import StreamMessage
+    from faststream.broker.publisher.proto import ProducerProto
     from faststream.broker.types import (
         BrokerMiddleware,
-        CustomDecoder,
-        CustomParser,
+        CustomCallable,
     )
+    from faststream.nats.publisher.asyncapi import AsyncAPIPublisher
     from faststream.security import BaseSecurity
-    from faststream.types import AnyDict, DecodedMessage, SendableMessage
+    from faststream.types import AnyDict, DecodedMessage, LoggerProto, SendableMessage
 
     class NatsInitKwargs(TypedDict, total=False):
         """NatsBroker.connect() method type hints."""
 
         error_cb: Annotated[
             Optional["ErrorCallback"],
             Doc("Callback to report errors."),
@@ -83,16 +80,15 @@
             Doc("Callback to report when client stops reconnection to NATS."),
         ]
         discovered_server_cb: Annotated[
             Optional["Callback"],
             Doc("Callback to report when a new server joins the cluster."),
         ]
         reconnected_cb: Annotated[
-            Optional["Callback"], Doc(
-                "Callback to report success reconnection.")
+            Optional["Callback"], Doc("Callback to report success reconnection.")
         ]
         name: Annotated[
             Optional[str],
             Doc("Label the connection with name (shown in NATS monitoring)."),
         ]
         pedantic: Annotated[
             bool,
@@ -237,16 +233,15 @@
             Doc("Callback to report when client stops reconnection to NATS."),
         ] = None,
         discovered_server_cb: Annotated[
             Optional["Callback"],
             Doc("Callback to report when a new server joins the cluster."),
         ] = None,
         reconnected_cb: Annotated[
-            Optional["Callback"], Doc(
-                "Callback to report success reconnection.")
+            Optional["Callback"], Doc("Callback to report success reconnection.")
         ] = None,
         name: Annotated[
             Optional[str],
             Doc("Label the connection with name (shown in NATS monitoring)."),
         ] = SERVICE_NAME,
         pedantic: Annotated[
             bool,
@@ -361,19 +356,19 @@
         graceful_timeout: Annotated[
             Optional[float],
             Doc(
                 "Graceful shutdown timeout. Broker waits for all running subscribers completion before shut down."
             ),
         ] = None,
         decoder: Annotated[
-            Optional["CustomDecoder[StreamMessage[Msg]]"],
+            Optional["CustomCallable"],
             Doc("Custom decoder object."),
         ] = None,
         parser: Annotated[
-            Optional["CustomParser[Msg]"],
+            Optional["CustomCallable"],
             Doc("Custom parser object."),
         ] = None,
         dependencies: Annotated[
             Iterable["Depends"],
             Doc("Dependencies to apply to all broker subscribers."),
         ] = (),
         middlewares: Annotated[
@@ -405,15 +400,15 @@
         ] = None,
         tags: Annotated[
             Optional[Iterable[Union["asyncapi.Tag", "asyncapi.TagDict"]]],
             Doc("AsyncAPI server tags."),
         ] = None,
         # logging args
         logger: Annotated[
-            Union[logging.Logger, None, object],
+            Union["LoggerProto", None, object],
             Doc("User specified logger to pass into Context and log service messages."),
         ] = Parameter.empty,
         log_level: Annotated[
             int,
             Doc("Service messages log level."),
         ] = logging.INFO,
         log_fmt: Annotated[
@@ -623,22 +618,20 @@
                         e.description
                         == "stream name already in use with a different configuration"
                     ):
                         self._log(str(e), logging.WARNING, log_context)
                         await self.stream.update_stream(
                             config=stream.config,
                             subjects=tuple(
-                                set(old_config.subjects or ()).union(
-                                    stream.subjects)
+                                set(old_config.subjects or ()).union(stream.subjects)
                             ),
                         )
 
                     else:  # pragma: no cover
-                        self._log(str(e), logging.ERROR,
-                                  log_context, exc_info=e)
+                        self._log(str(e), logging.ERROR, log_context, exc_info=e)
 
                 finally:
                     # prevent from double declaration
                     stream.declare = False
 
             self._log(
                 f"`{handler.call_name}` waiting for messages",
@@ -660,15 +653,15 @@
             str,
             Doc("NATS subject to send message."),
         ],
         headers: Annotated[
             Optional[Dict[str, str]],
             Doc(
                 "Message headers to store metainformation. "
-                "**content-type** and **correlation_id** will be setted automatically by framework anyway."
+                "**content-type** and **correlation_id** will be set automatically by framework anyway."
             ),
         ] = None,
         reply_to: Annotated[
             str,
             Doc("NATS subject name to send response."),
         ] = "",
         correlation_id: Annotated[
@@ -709,58 +702,57 @@
         """Publish message directly.
 
         This method allows you to publish message in not AsyncAPI-documented way. You can use it in another frameworks
         applications or to publish messages from time to time.
 
         Please, use `@broker.publisher(...)` or `broker.publisher(...).publish(...)` instead in a regular way.
         """
-        publihs_kwargs = dict(
-            subject=subject,
-            headers=headers,
-            reply_to=reply_to,
-            correlation_id=correlation_id or gen_cor_id(),
-            rpc=rpc,
-            rpc_timeout=rpc_timeout,
-            raise_timeout=raise_timeout,
-        )
+        publihs_kwargs = {
+            "subject": subject,
+            "headers": headers,
+            "reply_to": reply_to,
+            "correlation_id": correlation_id or gen_cor_id(),
+            "rpc": rpc,
+            "rpc_timeout": rpc_timeout,
+            "raise_timeout": raise_timeout,
+        }
 
         producer: Optional[ProducerProto]
         if stream is None:
             producer = self._producer
         else:
             producer = self._js_producer
-            publihs_kwargs.update(dict(
-                stream=stream,
-                timeout=timeout,
-            ))
+            publihs_kwargs.update(
+                {
+                    "stream": stream,
+                    "timeout": timeout,
+                }
+            )
 
         return await super().publish(
             message,
             producer=producer,
             **publihs_kwargs,
         )
 
     @override
     def setup_subscriber(  # type: ignore[override]
         self,
-        subscriber: AsyncAPISubscriber,
+        subscriber: "AsyncAPISubscriber",
     ) -> None:
         connection: Union["Client", "JetStreamContext", None] = None
 
-        if subscriber.stream is None:
-            connection = self._connection
-        else:
-            connection = self.stream
+        connection = self._connection if subscriber.stream is None else self.stream
 
         return super().setup_subscriber(subscriber, connection=connection)
 
     @override
     def setup_publisher(  # type: ignore[override]
         self,
-        publisher: AsyncAPIPublisher,
+        publisher: "AsyncAPIPublisher",
     ) -> None:
         producer: Optional[ProducerProto] = None
 
         if publisher.stream is not None:
             if self._js_producer is not None:
                 producer = self._js_producer
```

### Comparing `faststream-0.5.0rc0/faststream/nats/broker/logging.py` & `faststream-0.5.0rc1/faststream/nats/broker/logging.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 import logging
 from inspect import Parameter
-from typing import Any, ClassVar, Optional, Union
+from typing import TYPE_CHECKING, Any, ClassVar, Optional, Union
 
 from nats.aio.client import Client
 from nats.aio.msg import Msg
 
 from faststream.broker.core.usecase import BrokerUsecase
 from faststream.log.logging import get_broker_logger
 
+if TYPE_CHECKING:
+    from faststream.types import LoggerProto
+
 
 class NatsLoggingBroker(BrokerUsecase[Msg, Client]):
     """A class that extends the LoggingMixin class and adds additional functionality for logging NATS related information."""
 
     _max_queue_len: int
     _max_subject_len: int
     __max_msg_id_ln: ClassVar[int] = 10
 
     def __init__(
         self,
         *args: Any,
-        logger: Union[logging.Logger, object, None] = Parameter.empty,
+        logger: Union["LoggerProto", object, None] = Parameter.empty,
         log_level: int = logging.INFO,
         log_fmt: Optional[str] = None,
         **kwargs: Any,
     ) -> None:
         """Initialize the NATS logging mixin."""
         super().__init__(
             *args,
```

### Comparing `faststream-0.5.0rc0/faststream/nats/broker/registrator.py` & `faststream-0.5.0rc1/faststream/rabbit/broker/registrator.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,164 +1,100 @@
-from typing import Any, Dict, Iterable, Optional, Union, cast
+from typing import TYPE_CHECKING, Any, Dict, Iterable, Optional, Union, cast
 
-from fast_depends.dependencies import Depends
-from nats.aio.msg import Msg
-from nats.js import api
 from typing_extensions import Annotated, Doc, deprecated, override
 
 from faststream.broker.core.abc import ABCBroker
-from faststream.broker.message import StreamMessage
-from faststream.broker.types import (
-    CustomDecoder,
-    CustomParser,
-    Filter,
-    PublisherMiddleware,
-    SubscriberMiddleware,
-)
 from faststream.broker.utils import default_filter
-from faststream.nats.publisher.asyncapi import AsyncAPIPublisher
-from faststream.nats.schemas import JStream, PullSub
-from faststream.nats.subscriber.asyncapi import AsyncAPISubscriber
+from faststream.rabbit.publisher.asyncapi import AsyncAPIPublisher
+from faststream.rabbit.publisher.usecase import PublishKwargs
+from faststream.rabbit.schemas import (
+    RabbitExchange,
+    RabbitQueue,
+)
+from faststream.rabbit.subscriber.asyncapi import AsyncAPISubscriber
+
+if TYPE_CHECKING:
+    from aio_pika import IncomingMessage  # noqa: F401
+    from aio_pika.abc import DateType, HeadersType, TimeoutType
+    from fast_depends.dependencies import Depends
+
+    from faststream.broker.types import (
+        CustomCallable,
+        Filter,
+        PublisherMiddleware,
+        SubscriberMiddleware,
+    )
+    from faststream.rabbit.message import RabbitMessage
+    from faststream.rabbit.schemas.reply import ReplyConfig
+    from faststream.types import AnyDict
 
 
-class NatsRegistrator(ABCBroker["Msg"]):
+class RabbitRegistrator(ABCBroker["IncomingMessage"]):
     """Includable to RabbitBroker router."""
 
-    _subscribers: Dict[int, AsyncAPISubscriber]
-    _publishers: Dict[int, AsyncAPIPublisher]
+    _subscribers: Dict[int, "AsyncAPISubscriber"]
+    _publishers: Dict[int, "AsyncAPIPublisher"]
 
     @override
     def subscriber(  # type: ignore[override]
         self,
-        subject: Annotated[
-            str,
-            Doc("NATS subject to subscribe."),
-        ],
         queue: Annotated[
-            str,
-            Doc(
-                "Subscribers' NATS queue name. Subscribers with same queue name will be load balanced by the NATS "
-                "server."
-            ),
-        ] = "",
-        pending_msgs_limit: Annotated[
-            Optional[int],
-            Doc(
-                "Limit of messages, considered by NATS server as possible to be delivered to the client without "
-                "been answered. In case of NATS Core, if that limits exceeds, you will receive NATS 'Slow Consumer' "
-                "error. "
-                "That's literally means that your worker can't handle the whole load. In case of NATS JetStream, "
-                "you will no longer receive messages until some of delivered messages will be acked in any way."
-            ),
-        ] = None,
-        pending_bytes_limit: Annotated[
-            Optional[int],
-            Doc(
-                "The number of bytes, considered by NATS server as possible to be delivered to the client without "
-                "been answered. In case of NATS Core, if that limit exceeds, you will receive NATS 'Slow Consumer' "
-                "error."
-                "That's literally means that your worker can't handle the whole load. In case of NATS JetStream, "
-                "you will no longer receive messages until some of delivered messages will be acked in any way."
-            ),
-        ] = None,
-        # Core arguments
-        max_msgs: Annotated[
-            int,
-            Doc("Consuming messages limiter. Automatically disconnect if reached."),
-        ] = 0,
-        # JS arguments
-        durable: Annotated[
-            Optional[str],
-            Doc(
-                "Name of the durable consumer to which the the subscription should be bound."
-            ),
-        ] = None,
-        config: Annotated[
-            Optional["api.ConsumerConfig"],
-            Doc("Configuration of JetStream consumer to be subscribed with."),
-        ] = None,
-        ordered_consumer: Annotated[
-            bool,
-            Doc("Enable ordered consumer mode."),
-        ] = False,
-        idle_heartbeat: Annotated[
-            Optional[float],
-            Doc("Enable Heartbeats for a consumer to detect failures."),
-        ] = None,
-        flow_control: Annotated[
-            bool,
-            Doc("Enable Flow Control for a consumer."),
-        ] = False,
-        deliver_policy: Annotated[
-            Optional["api.DeliverPolicy"],
-            Doc("Deliver Policy to be used for subscription."),
-        ] = None,
-        headers_only: Annotated[
-            Optional[bool],
+            Union[str, "RabbitQueue"],
             Doc(
-                "Should be message delivered without payload, only headers and metadata."
+                "RabbitMQ queue to listen. "
+                "**FastStream** declares and binds queue object to `exchange` automatically if it is not passive (by default)."
             ),
-        ] = None,
-        # pull arguments
-        pull_sub: Annotated[
-            Optional["PullSub"],
+        ],
+        exchange: Annotated[
+            Union[str, "RabbitExchange", None],
             Doc(
-                "NATS Pull consumer parameters container. "
-                "Should be used with `stream` only."
+                "RabbitMQ exchange to bind queue to. "
+                "Uses default exchange if not presented. "
+                "**FastStream** declares exchange object automatically if it is not passive (by default)."
             ),
         ] = None,
-        inbox_prefix: Annotated[
-            bytes,
-            Doc(
-                "Prefix for generating unique inboxes, subjects with that prefix and NUID."
-            ),
-        ] = api.INBOX_PREFIX,
-        # custom
-        ack_first: Annotated[
-            bool,
-            Doc("Whether to `ack` message at start of consuming or not."),
-        ] = False,
-        stream: Annotated[
-            Union[str, "JStream", None],
-            Doc("Subscribe to NATS Stream with `subject` filter."),
+        *,
+        consume_args: Annotated[
+            Optional["AnyDict"],
+            Doc("Extra consumer arguments to use in `queue.consume(...)` method."),
+        ] = None,
+        reply_config: Annotated[
+            Optional["ReplyConfig"],
+            Doc("Extra options to use at replies publishing."),
         ] = None,
         # broker arguments
         dependencies: Annotated[
-            Iterable[Depends],
+            Iterable["Depends"],
             Doc("Dependencies list (`[Depends(),]`) to apply to the subscriber."),
         ] = (),
         parser: Annotated[
-            Optional["CustomParser[Msg]"],
-            Doc("Parser to map original **nats-py** Msg to FastStream one."),
+            Optional["CustomCallable"],
+            Doc("Parser to map original **IncomingMessage** Msg to FastStream one."),
         ] = None,
         decoder: Annotated[
-            Optional["CustomDecoder[StreamMessage[Msg]]"],
+            Optional["CustomCallable"],
             Doc("Function to decode FastStream msg bytes body to python objects."),
         ] = None,
         middlewares: Annotated[
             Iterable["SubscriberMiddleware"],
             Doc("Subscriber middlewares to wrap incoming message processing."),
         ] = (),
         filter: Annotated[
-            "Filter[StreamMessage[Msg]]",
+            "Filter[RabbitMessage]",
             Doc(
                 "Overload subscriber to consume various messages from the same source."
             ),
             deprecated(
                 "Deprecated in **FastStream 0.5.0**. "
                 "Please, create `subscriber` object and use it explicitly instead. "
                 "Argument will be removed in **FastStream 0.6.0**."
             ),
         ] = default_filter,
-        max_workers: Annotated[
-            int,
-            Doc("Number of workers to process messages concurrently."),
-        ] = 1,
         retry: Annotated[
-            bool,
+            Union[bool, int],
             Doc("Whether to `nack` message at processing exception."),
         ] = False,
         no_ack: Annotated[
             bool,
             Doc("Whether to disable **FastStream** autoacknowledgement logic or not."),
         ] = False,
         # AsyncAPI information
@@ -174,95 +110,97 @@
             ),
         ] = None,
         include_in_schema: Annotated[
             bool,
             Doc("Whetever to include operation in AsyncAPI schema or not."),
         ] = True,
     ) -> AsyncAPISubscriber:
-        """Creates NATS subscriber object.
-
-        You can use it as a handler decorator `@broker.subscriber(...)`.
-        """
         subscriber = cast(
             AsyncAPISubscriber,
-            super().subscriber(AsyncAPISubscriber.create(
-                subject=subject,
-                queue=queue,
-                stream=stream,
-                pull_sub=pull_sub,
-                max_workers=max_workers,
-                # extra args
-                pending_msgs_limit=pending_msgs_limit,
-                pending_bytes_limit=pending_bytes_limit,
-                max_msgs=max_msgs,
-                durable=durable,
-                config=config,
-                ordered_consumer=ordered_consumer,
-                idle_heartbeat=idle_heartbeat,
-                flow_control=flow_control,
-                deliver_policy=deliver_policy,
-                headers_only=headers_only,
-                inbox_prefix=inbox_prefix,
-                ack_first=ack_first,
-                # subscriber args
-                no_ack=no_ack,
-                retry=retry,
-                broker_middlewares=self._middlewares,
-                broker_dependencies=self._dependencies,
-                # AsyncAPI
-                title_=title,
-                description_=description,
-                include_in_schema=self._solve_include_in_schema(
-                    include_in_schema),
-            ))
+            super().subscriber(
+                AsyncAPISubscriber.create(
+                    queue=RabbitQueue.validate(queue),
+                    exchange=RabbitExchange.validate(exchange),
+                    consume_args=consume_args,
+                    reply_config=reply_config,
+                    # subscriber args
+                    no_ack=no_ack,
+                    retry=retry,
+                    broker_middlewares=self._middlewares,
+                    broker_dependencies=self._dependencies,
+                    # AsyncAPI
+                    title_=title,
+                    description_=description,
+                    include_in_schema=self._solve_include_in_schema(include_in_schema),
+                )
+            ),
         )
 
         return subscriber.add_call(
             filter_=filter,
             parser_=parser or self._parser,
             decoder_=decoder or self._decoder,
             dependencies_=dependencies,
             middlewares_=middlewares,
         )
 
     @override
     def publisher(  # type: ignore[override]
         self,
-        subject: Annotated[
-            str,
-            Doc("NATS subject to send message."),
-        ],
+        queue: Annotated[
+            Union["RabbitQueue", str],
+            Doc("Default message routing key to publish with."),
+        ] = "",
+        exchange: Annotated[
+            Union["RabbitExchange", str, None],
+            Doc("Target exchange to publish message to."),
+        ] = None,
         *,
-        headers: Annotated[
-            Optional[Dict[str, str]],
+        routing_key: Annotated[
+            str,
             Doc(
-                "Message headers to store metainformation. "
-                "**content-type** and **correlation_id** will be setted automatically by framework anyway. "
-                "Can be overridden by `publish.headers` if specified."
+                "Default message routing key to publish with. "
+                "Overrides `queue` option if presented."
+            ),
+        ] = "",
+        mandatory: Annotated[
+            bool,
+            Doc(
+                "Client waits for confirmation that the message is placed to some queue. "
+                "RabbitMQ returns message to client if there is no suitable queue."
             ),
+        ] = True,
+        immediate: Annotated[
+            bool,
+            Doc(
+                "Client expects that there is consumer ready to take the message to work. "
+                "RabbitMQ returns message to client if there is no suitable consumer."
+            ),
+        ] = False,
+        timeout: Annotated[
+            "TimeoutType",
+            Doc("Send confirmation time from RabbitMQ."),
         ] = None,
+        persist: Annotated[
+            bool,
+            Doc("Restore the message on RabbitMQ reboot."),
+        ] = False,
         reply_to: Annotated[
-            str,
-            Doc("NATS subject name to send response."),
-        ] = "",
-        # JS
-        stream: Annotated[
-            Union[str, "JStream", None],
+            Optional[str],
             Doc(
-                "This option validates that the target `subject` is in presented stream. "
-                "Can be omitted without any effect."
+                "Reply message routing key to send with (always sending to default exchange)."
             ),
         ] = None,
-        timeout: Annotated[
-            Optional[float],
-            Doc("Timeout to send message to NATS."),
+        priority: Annotated[
+            Optional[int],
+            Doc("The message priority (0 by default)."),
         ] = None,
-        # basic args
+        # specific
         middlewares: Annotated[
-            Iterable[PublisherMiddleware],
+            Iterable["PublisherMiddleware"],
             Doc("Publisher middlewares to wrap outgoing messages."),
         ] = (),
         # AsyncAPI information
         title: Annotated[
             Optional[str],
             Doc("AsyncAPI publisher object title."),
         ] = None,
@@ -277,38 +215,83 @@
                 "Should be any python-native object annotation or `pydantic.BaseModel`."
             ),
         ] = None,
         include_in_schema: Annotated[
             bool,
             Doc("Whetever to include operation in AsyncAPI schema or not."),
         ] = True,
-    ) -> "AsyncAPIPublisher":
+        # message args
+        headers: Annotated[
+            Optional["HeadersType"],
+            Doc(
+                "Message headers to store metainformation. "
+                "Can be overridden by `publish.headers` if specified."
+            ),
+        ] = None,
+        content_type: Annotated[
+            Optional[str],
+            Doc(
+                "Message **content-type** header. "
+                "Used by application, not core RabbitMQ. "
+                "Will be set automatically if not specified."
+            ),
+        ] = None,
+        content_encoding: Annotated[
+            Optional[str],
+            Doc("Message body content encoding, e.g. **gzip**."),
+        ] = None,
+        expiration: Annotated[
+            Optional["DateType"],
+            Doc("Message expiration (lifetime) in seconds (or datetime or timedelta)."),
+        ] = None,
+        message_type: Annotated[
+            Optional[str],
+            Doc("Application-specific message type, e.g. **orders.created**."),
+        ] = None,
+        user_id: Annotated[
+            Optional[str],
+            Doc("Publisher connection User ID, validated if set."),
+        ] = None,
+    ) -> AsyncAPIPublisher:
         """Creates long-living and AsyncAPI-documented publisher object.
 
         You can use it as a handler decorator (handler should be decorated by `@broker.subscriber(...)` too) - `@broker.publisher(...)`.
         In such case publisher will publish your handler return value.
 
         Or you can create a publisher object to call it lately - `broker.publisher(...).publish(...)`.
         """
+        message_kwargs = PublishKwargs(
+            mandatory=mandatory,
+            immediate=immediate,
+            timeout=timeout,
+            persist=persist,
+            reply_to=reply_to,
+            headers=headers,
+            priority=priority,
+            content_type=content_type,
+            content_encoding=content_encoding,
+            message_type=message_type,
+            user_id=user_id,
+            expiration=expiration,
+        )
+
         publisher = cast(
             AsyncAPIPublisher,
             super().publisher(
-                publisher=AsyncAPIPublisher.create(
-                    subject=subject,
-                    headers=headers,
-                    # Core
-                    reply_to=reply_to,
-                    # JS
-                    timeout=timeout,
-                    stream=stream,
+                AsyncAPIPublisher.create(
+                    routing_key=routing_key,
+                    queue=RabbitQueue.validate(queue),
+                    exchange=RabbitExchange.validate(exchange),
+                    message_kwargs=message_kwargs,
                     # Specific
                     broker_middlewares=self._middlewares,
                     middlewares=middlewares,
                     # AsyncAPI
                     title_=title,
                     description_=description,
                     schema_=schema,
                     include_in_schema=self._solve_include_in_schema(include_in_schema),
                 )
             ),
         )
+
         return publisher
```

### Comparing `faststream-0.5.0rc0/faststream/nats/fastapi/__init__.py` & `faststream-0.5.0rc1/faststream/nats/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/faststream/nats/fastapi/fastapi.py` & `faststream-0.5.0rc1/faststream/nats/fastapi/fastapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,26 +54,25 @@
         SignatureCallback,
     )
     from nats.aio.msg import Msg
     from starlette.responses import Response
     from starlette.types import ASGIApp, Lifespan
 
     from faststream.asyncapi import schema as asyncapi
-    from faststream.broker.message import StreamMessage
     from faststream.broker.types import (
         BrokerMiddleware,
-        CustomDecoder,
-        CustomParser,
+        CustomCallable,
         Filter,
         PublisherMiddleware,
         SubscriberMiddleware,
     )
+    from faststream.nats.message import NatsBatchMessage, NatsMessage
     from faststream.nats.schemas import JStream, PullSub
     from faststream.security import BaseSecurity
-    from faststream.types import AnyDict
+    from faststream.types import AnyDict, LoggerProto
 
 
 class NatsRouter(StreamRouter["Msg"]):
     """A class to represent a NATS router."""
 
     broker_class = NatsBroker
     broker: NatsBroker
@@ -99,16 +98,15 @@
             Doc("Callback to report when client stops reconnection to NATS."),
         ] = None,
         discovered_server_cb: Annotated[
             Optional["Callback"],
             Doc("Callback to report when a new server joins the cluster."),
         ] = None,
         reconnected_cb: Annotated[
-            Optional["Callback"], Doc(
-                "Callback to report success reconnection.")
+            Optional["Callback"], Doc("Callback to report success reconnection.")
         ] = None,
         name: Annotated[
             Optional[str],
             Doc("Label the connection with name (shown in NATS monitoring)."),
         ] = SERVICE_NAME,
         pedantic: Annotated[
             bool,
@@ -223,19 +221,19 @@
         graceful_timeout: Annotated[
             Optional[float],
             Doc(
                 "Graceful shutdown timeout. Broker waits for all running subscribers completion before shut down."
             ),
         ] = 15.0,
         decoder: Annotated[
-            Optional["CustomDecoder[StreamMessage[Msg]]"],
+            Optional["CustomCallable"],
             Doc("Custom decoder object."),
         ] = None,
         parser: Annotated[
-            Optional["CustomParser[Msg]"],
+            Optional["CustomCallable"],
             Doc("Custom parser object."),
         ] = None,
         middlewares: Annotated[
             Iterable["BrokerMiddleware[Msg]"],
             Doc("Middlewares to apply to all broker publishers/subscribers."),
         ] = (),
         # AsyncAPI args
@@ -263,15 +261,15 @@
         ] = None,
         asyncapi_tags: Annotated[
             Optional[Iterable[Union["asyncapi.Tag", "asyncapi.TagDict"]]],
             Doc("AsyncAPI server tags."),
         ] = None,
         # logging args
         logger: Annotated[
-            Union[logging.Logger, None, object],
+            Union["LoggerProto", None, object],
             Doc("User specified logger to pass into Context and log service messages."),
         ] = Parameter.empty,
         log_level: Annotated[
             int,
             Doc("Service messages log level."),
         ] = logging.INFO,
         log_fmt: Annotated[
@@ -670,27 +668,30 @@
         ] = None,
         # broker arguments
         dependencies: Annotated[
             Iterable["params.Depends"],
             Doc("Dependencies list (`[Depends(),]`) to apply to the subscriber."),
         ] = (),
         parser: Annotated[
-            Optional["CustomParser[Msg]"],
+            Optional["CustomCallable"],
             Doc("Parser to map original **nats-py** Msg to FastStream one."),
         ] = None,
         decoder: Annotated[
-            Optional["CustomDecoder[StreamMessage[Msg]]"],
+            Optional["CustomCallable"],
             Doc("Function to decode FastStream msg bytes body to python objects."),
         ] = None,
         middlewares: Annotated[
             Iterable["SubscriberMiddleware"],
             Doc("Subscriber middlewares to wrap incoming message processing."),
         ] = (),
         filter: Annotated[
-            "Filter[StreamMessage[Msg]]",
+            Union[
+                "Filter[NatsMessage]",
+                "Filter[NatsBatchMessage]",
+            ],
             Doc(
                 "Overload subscriber to consume various messages from the same source."
             ),
             deprecated(
                 "Deprecated in **FastStream 0.5.0**. "
                 "Please, create `subscriber` object and use it explicitly instead. "
                 "Argument will be removed in **FastStream 0.6.0**."
@@ -897,15 +898,15 @@
             str,
             Doc("NATS subject to send message."),
         ],
         headers: Annotated[
             Optional[Dict[str, str]],
             Doc(
                 "Message headers to store metainformation. "
-                "**content-type** and **correlation_id** will be setted automatically by framework anyway. "
+                "**content-type** and **correlation_id** will be set automatically by framework anyway. "
                 "Can be overridden by `publish.headers` if specified."
             ),
         ] = None,
         reply_to: Annotated[
             str,
             Doc("NATS subject name to send response."),
         ] = "",
```

### Comparing `faststream-0.5.0rc0/faststream/nats/publisher/asyncapi.py` & `faststream-0.5.0rc1/faststream/nats/publisher/asyncapi.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,28 @@
-from typing import Any, Dict, Iterable, Optional, Union
+from typing import TYPE_CHECKING, Any, Dict, Iterable, Optional, Union
 
-from nats.aio.msg import Msg
 from typing_extensions import override
 
 from faststream.asyncapi.schema import (
     Channel,
     ChannelBinding,
     CorrelationId,
     Message,
     Operation,
 )
 from faststream.asyncapi.schema.bindings import nats
 from faststream.asyncapi.utils import resolve_payloads
-from faststream.broker.types import BrokerMiddleware, PublisherMiddleware
 from faststream.nats.helpers import stream_builder
 from faststream.nats.publisher.usecase import LogicPublisher
-from faststream.nats.schemas.js_stream import JStream
+
+if TYPE_CHECKING:
+    from nats.aio.msg import Msg
+
+    from faststream.broker.types import BrokerMiddleware, PublisherMiddleware
+    from faststream.nats.schemas.js_stream import JStream
 
 
 class AsyncAPIPublisher(LogicPublisher):
     """A class to represent a NATS publisher."""
 
     def get_name(self) -> str:
         return f"{self.subject}:Publisher"
@@ -54,23 +57,23 @@
         *,
         subject: str,
         reply_to: str,
         headers: Optional[Dict[str, str]],
         stream: Union[str, "JStream", None],
         timeout: Optional[float],
         # Publisher args
-        broker_middlewares: Iterable[BrokerMiddleware[Msg]],
-        middlewares: Iterable[PublisherMiddleware],
+        broker_middlewares: Iterable["BrokerMiddleware[Msg]"],
+        middlewares: Iterable["PublisherMiddleware"],
         # AsyncAPI args
         schema_: Optional[Any],
         title_: Optional[str],
         description_: Optional[str],
         include_in_schema: bool,
     ) -> "AsyncAPIPublisher":
-        if (stream := stream_builder.stream(stream)):
+        if stream := stream_builder.stream(stream):
             stream.add_subject(subject)
 
         return cls(
             subject=subject,
             reply_to=reply_to,
             headers=headers,
             stream=stream,
```

### Comparing `faststream-0.5.0rc0/faststream/nats/publisher/producer.py` & `faststream-0.5.0rc1/faststream/nats/publisher/producer.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,52 +7,49 @@
 from typing_extensions import override
 
 from faststream.broker.message import encode_message
 from faststream.broker.publisher.proto import ProducerProto
 from faststream.broker.utils import resolve_custom_func
 from faststream.exceptions import WRONG_PUBLISH_ARGS
 from faststream.nats.parser import NatsParser
-from faststream.types import SendableMessage
 from faststream.utils.functions import timeout_scope
 
 if TYPE_CHECKING:
     from nats.aio.client import Client
     from nats.aio.msg import Msg
     from nats.js import JetStreamContext
 
-    from faststream.broker.message import StreamMessage
     from faststream.broker.types import (
-        AsyncDecoder,
-        AsyncParser,
-        CustomDecoder,
-        CustomParser,
+        AsyncCallable,
+        CustomCallable,
     )
+    from faststream.types import SendableMessage
 
 
 class NatsFastProducer(ProducerProto):
     """A class to represent a NATS producer."""
 
-    _decoder: "AsyncDecoder[StreamMessage[Msg]]"
-    _parser: "AsyncParser[Msg]"
+    _decoder: "AsyncCallable"
+    _parser: "AsyncCallable"
 
     def __init__(
         self,
         *,
         connection: "Client",
-        parser: Optional["CustomParser[Msg]"],
-        decoder: Optional["CustomDecoder[StreamMessage[Msg]]"],
+        parser: Optional["CustomCallable"],
+        decoder: Optional["CustomCallable"],
     ) -> None:
         self._connection = connection
         self._parser = resolve_custom_func(parser, NatsParser.parse_message)
         self._decoder = resolve_custom_func(decoder, NatsParser.decode_message)
 
     @override
     async def publish(  # type: ignore[override]
         self,
-        message: SendableMessage,
+        message: "SendableMessage",
         subject: str,
         *,
         correlation_id: str,
         headers: Optional[Dict[str, str]] = None,
         reply_to: str = "",
         rpc: bool = False,
         rpc_timeout: Optional[float] = 30.0,
@@ -103,23 +100,23 @@
 
         return None
 
 
 class NatsJSFastProducer(ProducerProto):
     """A class to represent a NATS JetStream producer."""
 
-    _decoder: "AsyncDecoder[StreamMessage[Msg]]"
-    _parser: "AsyncParser[Msg]"
+    _decoder: "AsyncCallable"
+    _parser: "AsyncCallable"
 
     def __init__(
         self,
         *,
         connection: "JetStreamContext",
-        parser: Optional["CustomParser[Msg]"],
-        decoder: Optional["CustomDecoder[StreamMessage[Msg]]"],
+        parser: Optional["CustomCallable"],
+        decoder: Optional["CustomCallable"],
     ) -> None:
         self._connection = connection
         self._parser = resolve_custom_func(parser, NatsParser.parse_message)
         self._decoder = resolve_custom_func(decoder, NatsParser.decode_message)
 
     @override
     async def publish(  # type: ignore[override]
```

### Comparing `faststream-0.5.0rc0/faststream/nats/publisher/usecase.py` & `faststream-0.5.0rc1/faststream/nats/publisher/usecase.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,15 @@
             Doc("NATS subject to send message."),
         ] = "",
         *,
         headers: Annotated[
             Optional[Dict[str, str]],
             Doc(
                 "Message headers to store metainformation. "
-                "**content-type** and **correlation_id** will be setted automatically by framework anyway."
+                "**content-type** and **correlation_id** will be set automatically by framework anyway."
             ),
         ] = None,
         reply_to: Annotated[
             str,
             Doc("NATS subject name to send response."),
         ] = "",
         correlation_id: Annotated[
@@ -132,32 +132,24 @@
             "correlation_id": correlation_id or gen_cor_id(),
             # specific args
             "rpc": rpc,
             "rpc_timeout": rpc_timeout,
             "raise_timeout": raise_timeout,
         }
 
-        if (stream := stream or getattr(self.stream, "name", None)):
-            kwargs.update({
-                "stream": stream,
-                "timeout": timeout or self.timeout
-            })
+        if stream := stream or getattr(self.stream, "name", None):
+            kwargs.update({"stream": stream, "timeout": timeout or self.timeout})
 
         async with AsyncExitStack() as stack:
             for m in chain(
                 _extra_middlewares
                 or (m(None).publish_scope for m in self._broker_middlewares),
                 self._middlewares,
             ):
-                message = await stack.enter_async_context(
-                    m(message, **kwargs)
-                )
-
-            return await self._producer.publish(
-                message,
-                **kwargs
-            )
+                message = await stack.enter_async_context(m(message, **kwargs))
+
+            return await self._producer.publish(message, **kwargs)
 
         return None
 
     def add_prefix(self, prefix: str) -> None:
         self.subject = prefix + self.subject
```

### Comparing `faststream-0.5.0rc0/faststream/nats/schemas/js_stream.py` & `faststream-0.5.0rc1/faststream/nats/schemas/js_stream.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/faststream/nats/schemas/pull_sub.py` & `faststream-0.5.0rc1/faststream/nats/schemas/pull_sub.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,17 +16,21 @@
         self,
         batch_size: Annotated[
             int,
             Doc("Consuming messages batch size."),
         ] = 1,
         timeout: Annotated[
             Optional[float],
-            Doc("Wait this time for required batch size will be accumulated in stream."),
+            Doc(
+                "Wait this time for required batch size will be accumulated in stream."
+            ),
         ] = 5.0,
         batch: Annotated[
             bool,
-            Doc("Whether to propagate consuming batch as iterable object to your handler."),
+            Doc(
+                "Whether to propagate consuming batch as iterable object to your handler."
+            ),
         ] = False,
     ) -> None:
         self.batch_size = batch_size
         self.batch = batch
         self.timeout = timeout
```

### Comparing `faststream-0.5.0rc0/faststream/nats/subscriber/asyncapi.py` & `faststream-0.5.0rc1/faststream/nats/subscriber/asyncapi.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-from typing import Any, Dict, Iterable, Optional, Union
+from typing import TYPE_CHECKING, Any, Dict, Iterable, Optional, Union
 
-from fast_depends.dependencies import Depends
 from nats.aio.subscription import (
     DEFAULT_SUB_PENDING_BYTES_LIMIT,
     DEFAULT_SUB_PENDING_MSGS_LIMIT,
 )
-from nats.js import api
 from nats.js.client import (
     DEFAULT_JS_SUB_PENDING_BYTES_LIMIT,
     DEFAULT_JS_SUB_PENDING_MSGS_LIMIT,
 )
 from typing_extensions import override
 
 from faststream.asyncapi.schema import (
@@ -17,24 +15,29 @@
     ChannelBinding,
     CorrelationId,
     Message,
     Operation,
 )
 from faststream.asyncapi.schema.bindings import nats
 from faststream.asyncapi.utils import resolve_payloads
-from faststream.broker.types import BrokerMiddleware
 from faststream.exceptions import SetupError
 from faststream.nats.helpers import stream_builder
-from faststream.nats.schemas import JStream, PullSub
 from faststream.nats.subscriber.usecase import (
     BatchHandler,
     DefaultHandler,
     LogicSubscriber,
 )
-from faststream.types import AnyDict
+
+if TYPE_CHECKING:
+    from fast_depends.dependencies import Depends
+    from nats.js import api
+
+    from faststream.broker.types import BrokerMiddleware
+    from faststream.nats.schemas import JStream, PullSub
+    from faststream.types import AnyDict
 
 
 class AsyncAPISubscriber(LogicSubscriber[Any]):
     """A class to represent a NATS handler."""
 
     def get_name(self) -> str:
         return f"{self.subject}:{self.call_name}"
@@ -87,43 +90,44 @@
         # custom args
         ack_first: bool,
         max_workers: int,
         stream: Union[str, "JStream", None],
         # Subscriber args
         no_ack: bool,
         retry: Union[bool, int],
-        broker_dependencies: Iterable[Depends],
-        broker_middlewares: Iterable[BrokerMiddleware[Any]],
+        broker_dependencies: Iterable["Depends"],
+        broker_middlewares: Iterable["BrokerMiddleware[Any]"],
         # AsyncAPI information
         title_: Optional[str],
         description_: Optional[str],
         include_in_schema: bool,
     ) -> Union[
         "AsyncAPIDefaultSubscriber",
         "AsyncAPIBatchSubscriber",
     ]:
-        if (stream := stream_builder.stream(stream)):
+        if stream := stream_builder.stream(stream):
             stream.add_subject(subject)
 
         if pull_sub is not None and stream is None:
             raise SetupError("Pull subscriber can be used only with a stream")
 
         if stream:
             # TODO: pull & queue warning
             # TODO: push & durable warning
 
-            extra_options: AnyDict  = {
-                "pending_msgs_limit": pending_msgs_limit or DEFAULT_JS_SUB_PENDING_MSGS_LIMIT,
-                "pending_bytes_limit": pending_bytes_limit or DEFAULT_JS_SUB_PENDING_BYTES_LIMIT,
+            extra_options: AnyDict = {
+                "pending_msgs_limit": pending_msgs_limit
+                or DEFAULT_JS_SUB_PENDING_MSGS_LIMIT,
+                "pending_bytes_limit": pending_bytes_limit
+                or DEFAULT_JS_SUB_PENDING_BYTES_LIMIT,
                 "durable": durable,
                 "stream": stream.name,
                 "config": config,
             }
 
-
             if pull_sub is not None:
                 extra_options.update({"inbox_prefix": inbox_prefix})
 
             else:
                 extra_options.update(
                     {
                         "ordered_consumer": ordered_consumer,
@@ -133,16 +137,18 @@
                         "headers_only": headers_only,
                         "manual_ack": not ack_first,
                     }
                 )
 
         else:
             extra_options = {
-                "pending_msgs_limit": pending_msgs_limit or DEFAULT_SUB_PENDING_MSGS_LIMIT,
-                "pending_bytes_limit": pending_bytes_limit or DEFAULT_SUB_PENDING_BYTES_LIMIT,
+                "pending_msgs_limit": pending_msgs_limit
+                or DEFAULT_SUB_PENDING_MSGS_LIMIT,
+                "pending_bytes_limit": pending_bytes_limit
+                or DEFAULT_SUB_PENDING_BYTES_LIMIT,
                 "max_msgs": max_msgs,
             }
 
         if getattr(pull_sub, "batch", False):
             return AsyncAPIBatchSubscriber(
                 extra_options=extra_options,
                 # basic args
```

### Comparing `faststream-0.5.0rc0/faststream/nats/subscriber/usecase.py` & `faststream-0.5.0rc1/faststream/nats/subscriber/usecase.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,33 +19,32 @@
 import anyio
 from fast_depends.dependencies import Depends
 from nats.errors import ConnectionClosedError, TimeoutError
 from typing_extensions import Annotated, Doc, override
 
 from faststream.broker.message import StreamMessage
 from faststream.broker.publisher.fake import FakePublisher
-from faststream.broker.publisher.proto import ProducerProto
 from faststream.broker.subscriber.usecase import SubscriberUsecase
-from faststream.broker.types import CustomDecoder, CustomParser, MsgType
+from faststream.broker.types import CustomCallable, MsgType
 from faststream.exceptions import NOT_CONNECTED_YET, SetupError
 from faststream.nats.parser import BatchParser, JsParser, NatsParser
 from faststream.types import AnyDict, LoggerProto, SendableMessage
 from faststream.utils.path import compile_path
 
 if TYPE_CHECKING:
     from anyio.streams.memory import MemoryObjectReceiveStream, MemoryObjectSendStream
     from nats.aio.client import Client
     from nats.aio.msg import Msg
     from nats.aio.subscription import Subscription
     from nats.js import JetStreamContext
 
     from faststream.broker.message import StreamMessage
+    from faststream.broker.publisher.proto import ProducerProto
     from faststream.broker.types import (
-        AsyncDecoder,
-        AsyncParser,
+        AsyncCallable,
         BrokerMiddleware,
     )
     from faststream.nats.schemas import JStream, PullSub
 
 
 class LogicSubscriber(SubscriberUsecase[MsgType]):
     """A class to represent a NATS handler."""
@@ -64,16 +63,16 @@
         *,
         subject: str,
         extra_options: Optional[AnyDict],
         queue: str,
         stream: Optional["JStream"],
         pull_sub: Optional["PullSub"],
         # Subscriber args
-        default_parser: "AsyncParser[MsgType]",
-        default_decoder: "AsyncDecoder[StreamMessage[MsgType]]",
+        default_parser: "AsyncCallable",
+        default_decoder: "AsyncCallable",
         no_ack: bool,
         retry: Union[bool, int],
         broker_dependencies: Iterable[Depends],
         broker_middlewares: Iterable["BrokerMiddleware[MsgType]"],
         # AsyncAPI args
         title_: Optional[str],
         description_: Optional[str],
@@ -119,16 +118,16 @@
         connection: Union["Client", "JetStreamContext"],
         # basic args
         logger: Optional["LoggerProto"],
         producer: Optional["ProducerProto"],
         graceful_timeout: Optional[float],
         extra_context: Optional["AnyDict"],
         # broker options
-        broker_parser: Optional["CustomParser[MsgType]"],
-        broker_decoder: Optional["CustomDecoder[StreamMessage[MsgType]]"],
+        broker_parser: Optional["CustomCallable"],
+        broker_decoder: Optional["CustomCallable"],
         # dependant args
         apply_types: bool,
         is_validate: bool,
         _get_dependant: Optional[Callable[..., Any]],
     ) -> None:
         self._connection = connection
 
@@ -140,19 +139,17 @@
             broker_parser=broker_parser,
             broker_decoder=broker_decoder,
             apply_types=apply_types,
             is_validate=is_validate,
             _get_dependant=_get_dependant,
         )
 
-    async def start(
-        self
-    ) -> None:
+    async def start(self) -> None:
         """Create NATS subscription and start consume tasks."""
-        assert self._connection, NOT_CONNECTED_YET
+        assert self._connection, NOT_CONNECTED_YET  # nosec B101
         await super().start()
         await self._create_subscription(connection=self._connection)
 
     async def close(self) -> None:
         """Clean up handler subscription, cancel consume task in graceful mode."""
         await super().close()
 
@@ -327,16 +324,15 @@
         else:
             cb = self.consume
 
         if self.pull_sub is not None:
             connection = cast("JetStreamContext", connection)
 
             if self.stream is None:
-                raise SetupError(
-                    "Pull subscriber can be used only with a stream")
+                raise SetupError("Pull subscriber can be used only with a stream")
 
             self.subscription = await connection.pull_subscribe(
                 subject=self.subject,
                 **self.extra_options,
             )
             self.tasks.append(asyncio.create_task(self._consume_pull(cb=cb)))
```

### Comparing `faststream-0.5.0rc0/faststream/rabbit/__init__.py` & `faststream-0.5.0rc1/faststream/rabbit/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/faststream/rabbit/annotations.py` & `faststream-0.5.0rc1/faststream/rabbit/annotations.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/faststream/rabbit/message.py` & `faststream-0.5.0rc1/faststream/rabbit/message.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/faststream/rabbit/parser.py` & `faststream-0.5.0rc1/faststream/rabbit/parser.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/faststream/rabbit/router.py` & `faststream-0.5.0rc1/faststream/rabbit/router.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,52 +1,51 @@
 from typing import TYPE_CHECKING, Any, Callable, Iterable, Optional, Union
 
 from typing_extensions import Annotated, Doc, deprecated
 
 from faststream.broker.router import ArgsContainer, BrokerRouter, SubscriberRoute
 from faststream.broker.utils import default_filter
 from faststream.rabbit.broker.registrator import RabbitRegistrator
-from faststream.rabbit.schemas import (
-    RabbitExchange,
-    RabbitQueue,
-)
 
 if TYPE_CHECKING:
     from aio_pika.abc import DateType, HeadersType, TimeoutType
     from aio_pika.message import IncomingMessage
     from broker.types import PublisherMiddleware
     from fast_depends.dependencies import Depends
 
-    from faststream.broker.message import StreamMessage
     from faststream.broker.types import (
         BrokerMiddleware,
-        CustomDecoder,
-        CustomParser,
+        CustomCallable,
         Filter,
         SubscriberMiddleware,
     )
+    from faststream.rabbit.message import RabbitMessage
+    from faststream.rabbit.schemas import (
+        RabbitExchange,
+        RabbitQueue,
+    )
     from faststream.rabbit.schemas.reply import ReplyConfig
     from faststream.rabbit.types import AioPikaSendableMessage
     from faststream.types import AnyDict
 
 
 class RabbitPublisher(ArgsContainer):
     """Delayed RabbitPublisher registration object.
 
     Just a copy of `RabbitRegistrator.publisher(...)` arguments.
     """
 
     def __init__(
         self,
         queue: Annotated[
-            Union[RabbitQueue, str],
+            Union["RabbitQueue", str],
             Doc("Default message routing key to publish with."),
         ] = "",
         exchange: Annotated[
-            Union[RabbitExchange, str, None],
+            Union["RabbitExchange", str, None],
             Doc("Target exchange to publish message to."),
         ] = None,
         *,
         routing_key: Annotated[
             str,
             Doc(
                 "Default message routing key to publish with. "
@@ -119,15 +118,15 @@
             ),
         ] = None,
         content_type: Annotated[
             Optional[str],
             Doc(
                 "Message **content-type** header. "
                 "Used by application, not core RabbitMQ. "
-                "Will be setted automatically if not specified."
+                "Will be set automatically if not specified."
             ),
         ] = None,
         content_encoding: Annotated[
             Optional[str],
             Doc("Message body content encoding, e.g. **gzip**."),
         ] = None,
         expiration: Annotated[
@@ -181,22 +180,22 @@
             Callable[..., "AioPikaSendableMessage"],
             Doc(
                 "Message handler function "
                 "to wrap the same with `@broker.subscriber(...)` way."
             ),
         ],
         queue: Annotated[
-            Union[str, RabbitQueue],
+            Union[str, "RabbitQueue"],
             Doc(
                 "RabbitMQ queue to listen. "
                 "**FastStream** declares and binds queue object to `exchange` automatically if it is not passive (by default)."
             ),
         ],
         exchange: Annotated[
-            Union[str, RabbitExchange, None],
+            Union[str, "RabbitExchange", None],
             Doc(
                 "RabbitMQ exchange to bind queue to. "
                 "Uses default exchange if not presented. "
                 "**FastStream** declares exchange object automatically if it is not passive (by default)."
             ),
         ] = None,
         *,
@@ -214,27 +213,27 @@
         ] = None,
         # broker arguments
         dependencies: Annotated[
             Iterable["Depends"],
             Doc("Dependencies list (`[Depends(),]`) to apply to the subscriber."),
         ] = (),
         parser: Annotated[
-            Optional["CustomParser[IncomingMessage]"],
+            Optional["CustomCallable"],
             Doc("Parser to map original **IncomingMessage** Msg to FastStream one."),
         ] = None,
         decoder: Annotated[
-            Optional["CustomDecoder[StreamMessage[IncomingMessage]]"],
+            Optional["CustomCallable"],
             Doc("Function to decode FastStream msg bytes body to python objects."),
         ] = None,
         middlewares: Annotated[
             Iterable["SubscriberMiddleware"],
             Doc("Subscriber middlewares to wrap incoming message processing."),
         ] = (),
         filter: Annotated[
-            "Filter[StreamMessage[IncomingMessage]]",
+            "Filter[RabbitMessage]",
             Doc(
                 "Overload subscriber to consume various messages from the same source."
             ),
             deprecated(
                 "Deprecated in **FastStream 0.5.0**. "
                 "Please, create `subscriber` object and use it explicitly instead. "
                 "Argument will be removed in **FastStream 0.6.0**."
@@ -309,19 +308,19 @@
             ),
         ] = (),
         middlewares: Annotated[
             Iterable["BrokerMiddleware[IncomingMessage]"],
             Doc("Router middlewares to apply to all routers' publishers/subscribers."),
         ] = (),
         parser: Annotated[
-            Optional["CustomParser[IncomingMessage]"],
+            Optional["CustomCallable"],
             Doc("Parser to map original **IncomingMessage** Msg to FastStream one."),
         ] = None,
         decoder: Annotated[
-            Optional["CustomDecoder[StreamMessage[IncomingMessage]]"],
+            Optional["CustomCallable"],
             Doc("Function to decode FastStream msg bytes body to python objects."),
         ] = None,
         include_in_schema: Annotated[
             Optional[bool],
             Doc("Whetever to include operation in AsyncAPI schema or not."),
         ] = None,
     ) -> None:
```

### Comparing `faststream-0.5.0rc0/faststream/rabbit/security.py` & `faststream-0.5.0rc1/faststream/rabbit/security.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,37 @@
-from typing import Optional
+from typing import TYPE_CHECKING, Optional
 
 from faststream.security import (
     BaseSecurity,
     SASLPlaintext,
 )
-from faststream.types import AnyDict
 
+if TYPE_CHECKING:
+    from faststream.types import AnyDict
 
-def parse_security(security: Optional[BaseSecurity]) -> AnyDict:
+
+def parse_security(security: Optional[BaseSecurity]) -> "AnyDict":
     """Convert security object to connection arguments."""
     if security is None:
         return {}
     elif isinstance(security, SASLPlaintext):
         return _parse_sasl_plaintext(security)
     elif isinstance(security, BaseSecurity):
         return _parse_base_security(security)
     else:
         raise NotImplementedError(f"RabbitBroker does not support {type(security)}")
 
 
-def _parse_base_security(security: BaseSecurity) -> AnyDict:
+def _parse_base_security(security: BaseSecurity) -> "AnyDict":
     return {
         "ssl": security.use_ssl,
         "ssl_context": security.ssl_context,
     }
 
 
-def _parse_sasl_plaintext(security: SASLPlaintext) -> AnyDict:
+def _parse_sasl_plaintext(security: SASLPlaintext) -> "AnyDict":
     return {
         "ssl": security.use_ssl,
         "ssl_context": security.ssl_context,
         "login": security.username,
         "password": security.password,
     }
```

### Comparing `faststream-0.5.0rc0/faststream/rabbit/testing.py` & `faststream-0.5.0rc1/faststream/rabbit/testing.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,35 @@
-from typing import Any, Optional, Union
+from typing import TYPE_CHECKING, Any, Optional, Union
 from unittest.mock import AsyncMock
 
 import aiormq
-from aio_pika.abc import DateType, HeadersType, TimeoutType
 from aio_pika.message import IncomingMessage
 from pamqp import commands as spec
 from pamqp.header import ContentHeader
 from typing_extensions import override
 
 from faststream.broker.message import gen_cor_id
-from faststream.broker.wrapper.call import HandlerCallWrapper
 from faststream.rabbit.broker.broker import RabbitBroker
 from faststream.rabbit.parser import AioPikaParser
 from faststream.rabbit.publisher.asyncapi import AsyncAPIPublisher
 from faststream.rabbit.publisher.producer import AioPikaFastProducer
 from faststream.rabbit.schemas import (
     ExchangeType,
     RabbitExchange,
     RabbitQueue,
 )
 from faststream.rabbit.subscriber.asyncapi import AsyncAPISubscriber
-from faststream.rabbit.types import AioPikaSendableMessage
 from faststream.testing.broker import TestBroker, call_handler
 
+if TYPE_CHECKING:
+    from aio_pika.abc import DateType, HeadersType, TimeoutType
+
+    from faststream.broker.wrapper.call import HandlerCallWrapper
+    from faststream.rabbit.types import AioPikaSendableMessage
+
 __all__ = ("TestRabbitBroker",)
 
 
 class TestRabbitBroker(TestBroker[RabbitBroker]):
     """A class to test RabbitMQ brokers."""
 
     @classmethod
@@ -39,15 +42,15 @@
     async def _fake_connect(broker: RabbitBroker, *args: Any, **kwargs: Any) -> None:
         broker._producer = FakeProducer(broker)
 
     @staticmethod
     def create_publisher_fake_subscriber(
         broker: RabbitBroker,
         publisher: AsyncAPIPublisher,
-    ) -> HandlerCallWrapper[Any, Any, Any]:
+    ) -> "HandlerCallWrapper[Any, Any, Any]":
         sub = broker.subscriber(
             queue=publisher.queue,
             exchange=publisher.exchange,
         )
 
         if not sub.calls:
 
@@ -89,16 +92,16 @@
 
     async def reject(self, requeue: bool = False) -> None:
         """Rejects a task."""
         pass
 
 
 def build_message(
-    message: AioPikaSendableMessage = "",
-    queue: Union[RabbitQueue, str] = "",
+    message: "AioPikaSendableMessage" = "",
+    queue: Union["RabbitQueue", str] = "",
     exchange: Union["RabbitExchange", str, None] = None,
     *,
     routing_key: str = "",
     persist: bool = False,
     reply_to: Optional[str] = None,
     headers: Optional["HeadersType"] = None,
     content_type: Optional[str] = None,
@@ -163,34 +166,34 @@
 
     def __init__(self, broker: RabbitBroker) -> None:
         self.broker = broker
 
     @override
     async def publish(  # type: ignore[override]
         self,
-        message: AioPikaSendableMessage = "",
-        exchange: Union[RabbitExchange, str, None] = None,
+        message: "AioPikaSendableMessage" = "",
+        exchange: Union["RabbitExchange", str, None] = None,
         *,
         routing_key: str = "",
         mandatory: bool = True,
         immediate: bool = False,
-        timeout: TimeoutType = None,
+        timeout: "TimeoutType" = None,
         rpc: bool = False,
         rpc_timeout: Optional[float] = 30.0,
         raise_timeout: bool = False,
         persist: bool = False,
         reply_to: Optional[str] = None,
-        headers: Optional[HeadersType] = None,
+        headers: Optional["HeadersType"] = None,
         content_type: Optional[str] = None,
         content_encoding: Optional[str] = None,
         priority: Optional[int] = None,
         correlation_id: Optional[str] = None,
-        expiration: Optional[DateType] = None,
+        expiration: Optional["DateType"] = None,
         message_id: Optional[str] = None,
-        timestamp: Optional[DateType] = None,
+        timestamp: Optional["DateType"] = None,
         message_type: Optional[str] = None,
         user_id: Optional[str] = None,
         app_id: Optional[str] = None,
     ) -> Optional[Any]:
         """Publish a message to a RabbitMQ queue or exchange."""
         exch = RabbitExchange.validate(exchange)
```

### Comparing `faststream-0.5.0rc0/faststream/rabbit/utils.py` & `faststream-0.5.0rc1/faststream/rabbit/utils.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/faststream/rabbit/broker/broker.py` & `faststream-0.5.0rc1/faststream/rabbit/broker/broker.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,43 +43,41 @@
     )
     from aio_pika.abc import DateType, HeadersType, SSLOptions, TimeoutType
     from fast_depends.dependencies import Depends
     from pamqp.common import FieldTable
     from yarl import URL
 
     from faststream.asyncapi import schema as asyncapi
-    from faststream.broker.message import StreamMessage
     from faststream.broker.types import (
         BrokerMiddleware,
-        CustomDecoder,
-        CustomParser,
+        CustomCallable,
     )
     from faststream.rabbit.types import AioPikaSendableMessage
     from faststream.security import BaseSecurity
-    from faststream.types import AnyDict
+    from faststream.types import AnyDict, LoggerProto
 
 
 class RabbitBroker(
     RabbitRegistrator,
     RabbitLoggingBroker,
 ):
     """A class to represent a RabbitMQ broker."""
 
     url: str
-    _producer: Optional[AioPikaFastProducer]
+    _producer: Optional["AioPikaFastProducer"]
 
     declarer: Optional[RabbitDeclarer]
     _channel: Optional["RobustChannel"]
 
     def __init__(
         self,
         url: Annotated[
             Union[str, "URL", None],
             Doc("RabbitMQ destination location to connect."),
-        ] = "amqp://guest:guest@localhost:5672/",
+        ] = "amqp://guest:guest@localhost:5672/",  # pragma: allowlist secret
         *,
         # connection args
         host: Annotated[
             Optional[str],
             Doc("Destination host. This option overrides `url` option host."),
         ] = None,
         port: Annotated[
@@ -118,19 +116,19 @@
         graceful_timeout: Annotated[
             Optional[float],
             Doc(
                 "Graceful shutdown timeout. Broker waits for all running subscribers completion before shut down."
             ),
         ] = None,
         decoder: Annotated[
-            Optional["CustomDecoder[StreamMessage[IncomingMessage]]"],
+            Optional["CustomCallable"],
             Doc("Custom decoder object."),
         ] = None,
         parser: Annotated[
-            Optional["CustomParser[IncomingMessage]"],
+            Optional["CustomCallable"],
             Doc("Custom parser object."),
         ] = None,
         dependencies: Annotated[
             Iterable["Depends"],
             Doc("Dependencies to apply to all broker subscribers."),
         ] = (),
         middlewares: Annotated[
@@ -162,15 +160,15 @@
         ] = None,
         tags: Annotated[
             Optional[Iterable[Union["asyncapi.Tag", "asyncapi.TagDict"]]],
             Doc("AsyncAPI server tags."),
         ] = None,
         # logging args
         logger: Annotated[
-            Union[logging.Logger, None, object],
+            Union["LoggerProto", None, object],
             Doc("User specified logger to pass into Context and log service messages."),
         ] = Parameter.empty,
         log_level: Annotated[
             int,
             Doc("Service messages log level."),
         ] = logging.INFO,
         log_fmt: Annotated[
@@ -263,16 +261,15 @@
             "virtual_host": self.virtual_host,
         }
 
     @override
     async def connect(  # type: ignore[override]
         self,
         url: Annotated[
-            Union[str, "URL", object], Doc(
-                "RabbitMQ destination location to connect.")
+            Union[str, "URL", object], Doc("RabbitMQ destination location to connect.")
         ] = Parameter.empty,
         *,
         host: Annotated[
             Optional[str],
             Doc("Destination host. This option overrides `url` option host."),
         ] = None,
         port: Annotated[
@@ -421,19 +418,19 @@
     async def publish(  # type: ignore[override]
         self,
         message: Annotated[
             "AioPikaSendableMessage",
             Doc("Message body to send."),
         ] = None,
         queue: Annotated[
-            Union[RabbitQueue, str],
+            Union["RabbitQueue", str],
             Doc("Message routing key to publish with."),
         ] = "",
         exchange: Annotated[
-            Union[RabbitExchange, str, None],
+            Union["RabbitExchange", str, None],
             Doc("Target exchange to publish message to."),
         ] = None,
         *,
         routing_key: Annotated[
             str,
             Doc(
                 "Message routing key to publish with. "
@@ -496,15 +493,15 @@
             Doc("Message headers to store metainformation."),
         ] = None,
         content_type: Annotated[
             Optional[str],
             Doc(
                 "Message **content-type** header. "
                 "Used by application, not core RabbitMQ. "
-                "Will be setted automatically if not specified."
+                "Will be set automatically if not specified."
             ),
         ] = None,
         content_encoding: Annotated[
             Optional[str],
             Doc("Message body content encoding, e.g. **gzip**."),
         ] = None,
         expiration: Annotated[
@@ -567,25 +564,25 @@
             rpc_timeout=rpc_timeout,
             raise_timeout=raise_timeout,
         )
 
     async def declare_queue(
         self,
         queue: Annotated[
-            RabbitQueue,
+            "RabbitQueue",
             Doc("Queue object to create."),
         ],
     ) -> "RobustQueue":
         """Declares queue object in **RabbitMQ**."""
         assert self.declarer, NOT_CONNECTED_YET  # nosec B101
         return await self.declarer.declare_queue(queue)
 
     async def declare_exchange(
         self,
         exchange: Annotated[
-            RabbitExchange,
+            "RabbitExchange",
             Doc("Exchange object to create."),
         ],
     ) -> "RobustExchange":
         """Declares exchange object in **RabbitMQ**."""
         assert self.declarer, NOT_CONNECTED_YET  # nosec B101
         return await self.declarer.declare_exchange(exchange)
```

### Comparing `faststream-0.5.0rc0/faststream/rabbit/broker/logging.py` & `faststream-0.5.0rc1/faststream/rabbit/broker/logging.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 import logging
 from inspect import Parameter
-from typing import Any, ClassVar, Optional, Union
+from typing import TYPE_CHECKING, Any, ClassVar, Optional, Union
 
 from aio_pika import IncomingMessage, RobustConnection
 
 from faststream.broker.core.usecase import BrokerUsecase
 from faststream.log.logging import get_broker_logger
 
+if TYPE_CHECKING:
+    from faststream.types import LoggerProto
+
 
 class RabbitLoggingBroker(BrokerUsecase[IncomingMessage, RobustConnection]):
     """A class that extends the LoggingMixin class and adds additional functionality for logging RabbitMQ related information."""
 
     _max_queue_len: int
     _max_exchange_len: int
     __max_msg_id_ln: ClassVar[int] = 10
 
     def __init__(
         self,
         *args: Any,
-        logger: Union[logging.Logger, object, None] = Parameter.empty,
+        logger: Union["LoggerProto", object, None] = Parameter.empty,
         log_level: int = logging.INFO,
         log_fmt: Optional[str] = None,
         **kwargs: Any,
     ) -> None:
         super().__init__(
             *args,
             logger=logger,
```

### Comparing `faststream-0.5.0rc0/faststream/rabbit/broker/registrator.py` & `faststream-0.5.0rc1/faststream/redis/router.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,101 +1,163 @@
-from typing import TYPE_CHECKING, Any, Dict, Iterable, Optional, Union, cast
+from typing import TYPE_CHECKING, Any, Callable, Iterable, Optional, Union
 
-from typing_extensions import Annotated, Doc, deprecated, override
+from typing_extensions import Annotated, Doc, deprecated
 
-from faststream.broker.core.abc import ABCBroker
+from faststream.broker.router import ArgsContainer, BrokerRouter, SubscriberRoute
 from faststream.broker.utils import default_filter
-from faststream.rabbit.publisher.asyncapi import AsyncAPIPublisher
-from faststream.rabbit.publisher.usecase import PublishKwargs
-from faststream.rabbit.schemas import (
-    RabbitExchange,
-    RabbitQueue,
-)
-from faststream.rabbit.subscriber.asyncapi import AsyncAPISubscriber
+from faststream.redis.broker.registrator import RedisRegistrator
+from faststream.redis.message import BaseMessage
 
 if TYPE_CHECKING:
-    from aio_pika.abc import DateType, HeadersType, TimeoutType
-    from aio_pika.message import IncomingMessage
     from fast_depends.dependencies import Depends
 
-    from faststream.broker.message import StreamMessage
     from faststream.broker.types import (
-        CustomDecoder,
-        CustomParser,
+        BrokerMiddleware,
+        CustomCallable,
         Filter,
         PublisherMiddleware,
         SubscriberMiddleware,
     )
-    from faststream.rabbit.schemas.reply import ReplyConfig
-    from faststream.types import AnyDict
+    from faststream.redis.message import UnifyRedisMessage
+    from faststream.redis.schemas import ListSub, PubSub, StreamSub
+    from faststream.types import AnyDict, SendableMessage
 
 
-class RabbitRegistrator(ABCBroker["IncomingMessage"]):
-    """Includable to RabbitBroker router."""
+class RedisPublisher(ArgsContainer):
+    """Delayed RedisPublisher registration object.
 
-    _subscribers: Dict[int, AsyncAPISubscriber]
-    _publishers: Dict[int, AsyncAPIPublisher]
+    Just a copy of RedisRegistrator.publisher(...) arguments.
+    """
 
-    @override
-    def subscriber(  # type: ignore[override]
+    def __init__(
         self,
-        queue: Annotated[
-            Union[str, RabbitQueue],
+        channel: Annotated[
+            Union["PubSub", str, None],
+            Doc("Redis PubSub object name to send message."),
+        ] = None,
+        *,
+        list: Annotated[
+            Union["ListSub", str, None],
+            Doc("Redis List object name to send message."),
+        ] = None,
+        stream: Annotated[
+            Union["StreamSub", str, None],
+            Doc("Redis Stream object name to send message."),
+        ] = None,
+        headers: Annotated[
+            Optional["AnyDict"],
             Doc(
-                "RabbitMQ queue to listen. "
-                "**FastStream** declares and binds queue object to `exchange` automatically if it is not passive (by default)."
+                "Message headers to store metainformation. "
+                "Can be overridden by `publish.headers` if specified."
             ),
-        ],
-        exchange: Annotated[
-            Union[str, RabbitExchange, None],
+        ] = None,
+        reply_to: Annotated[
+            str,
+            Doc("Reply message destination PubSub object name."),
+        ] = "",
+        middlewares: Annotated[
+            Iterable["PublisherMiddleware"],
+            Doc("Publisher middlewares to wrap outgoing messages."),
+        ] = (),
+        # AsyncAPI information
+        title: Annotated[
+            Optional[str],
+            Doc("AsyncAPI publisher object title."),
+        ] = None,
+        description: Annotated[
+            Optional[str],
+            Doc("AsyncAPI publisher object description."),
+        ] = None,
+        schema: Annotated[
+            Optional[Any],
             Doc(
-                "RabbitMQ exchange to bind queue to. "
-                "Uses default exchange if not presented. "
-                "**FastStream** declares exchange object automatically if it is not passive (by default)."
+                "AsyncAPI publishing message type. "
+                "Should be any python-native object annotation or `pydantic.BaseModel`."
             ),
         ] = None,
-        *,
-        consume_args: Annotated[
-            Optional["AnyDict"],
-            Doc("Extra consumer arguments to use in `queue.consume(...)` method."),
+        include_in_schema: Annotated[
+            bool,
+            Doc("Whetever to include operation in AsyncAPI schema or not."),
+        ] = True,
+    ) -> None:
+        super().__init__(
+            channel=channel,
+            list=list,
+            stream=stream,
+            headers=headers,
+            reply_to=reply_to,
+            middlewares=middlewares,
+            title=title,
+            description=description,
+            schema=schema,
+            include_in_schema=include_in_schema,
+        )
+
+
+class RedisRoute(SubscriberRoute):
+    """Class to store delayed RedisBroker subscriber registration."""
+
+    def __init__(
+        self,
+        call: Annotated[
+            Callable[..., "SendableMessage"],
+            Doc(
+                "Message handler function "
+                "to wrap the same with `@broker.subscriber(...)` way."
+            ),
+        ],
+        channel: Annotated[
+            Union["PubSub", str, None],
+            Doc("Redis PubSub object name to send message."),
         ] = None,
-        reply_config: Annotated[
-            Optional["ReplyConfig"],
-            Doc("Extra options to use at replies publishing."),
+        *,
+        publishers: Annotated[
+            Iterable["RedisPublisher"],
+            Doc("Redis publishers to broadcast the handler result."),
+        ] = (),
+        list: Annotated[
+            Union["ListSub", str, None],
+            Doc("Redis List object name to send message."),
+        ] = None,
+        stream: Annotated[
+            Union["StreamSub", str, None],
+            Doc("Redis Stream object name to send message."),
         ] = None,
         # broker arguments
         dependencies: Annotated[
             Iterable["Depends"],
             Doc("Dependencies list (`[Depends(),]`) to apply to the subscriber."),
         ] = (),
         parser: Annotated[
-            Optional["CustomParser[IncomingMessage]"],
-            Doc("Parser to map original **IncomingMessage** Msg to FastStream one."),
+            Optional["CustomCallable"],
+            Doc(
+                "Parser to map original **aio_pika.IncomingMessage** Msg to FastStream one."
+            ),
         ] = None,
         decoder: Annotated[
-            Optional["CustomDecoder[StreamMessage[IncomingMessage]]"],
+            Optional["CustomCallable"],
             Doc("Function to decode FastStream msg bytes body to python objects."),
         ] = None,
         middlewares: Annotated[
             Iterable["SubscriberMiddleware"],
             Doc("Subscriber middlewares to wrap incoming message processing."),
         ] = (),
         filter: Annotated[
-            "Filter[StreamMessage[IncomingMessage]]",
+            "Filter[UnifyRedisMessage]",
             Doc(
                 "Overload subscriber to consume various messages from the same source."
             ),
             deprecated(
                 "Deprecated in **FastStream 0.5.0**. "
                 "Please, create `subscriber` object and use it explicitly instead. "
                 "Argument will be removed in **FastStream 0.6.0**."
             ),
         ] = default_filter,
         retry: Annotated[
-            Union[bool, int],
+            bool,
             Doc("Whether to `nack` message at processing exception."),
         ] = False,
         no_ack: Annotated[
             bool,
             Doc("Whether to disable **FastStream** autoacknowledgement logic or not."),
         ] = False,
         # AsyncAPI information
@@ -110,189 +172,77 @@
                 "Uses decorated docstring as default."
             ),
         ] = None,
         include_in_schema: Annotated[
             bool,
             Doc("Whetever to include operation in AsyncAPI schema or not."),
         ] = True,
-    ) -> AsyncAPISubscriber:
-        subscriber = cast(
-            AsyncAPISubscriber,
-            super().subscriber(
-                AsyncAPISubscriber.create(
-                    queue=RabbitQueue.validate(queue),
-                    exchange=RabbitExchange.validate(exchange),
-                    consume_args=consume_args,
-                    reply_config=reply_config,
-                    # subscriber args
-                    no_ack=no_ack,
-                    retry=retry,
-                    broker_middlewares=self._middlewares,
-                    broker_dependencies=self._dependencies,
-                    # AsyncAPI
-                    title_=title,
-                    description_=description,
-                    include_in_schema=self._solve_include_in_schema(include_in_schema),
-                )
-            ),
+    ) -> None:
+        super().__init__(
+            call,
+            channel=channel,
+            publishers=publishers,
+            list=list,
+            stream=stream,
+            dependencies=dependencies,
+            parser=parser,
+            decoder=decoder,
+            middlewares=middlewares,
+            filter=filter,
+            retry=retry,
+            no_ack=no_ack,
+            title=title,
+            description=description,
+            include_in_schema=include_in_schema,
         )
 
-        return subscriber.add_call(
-            filter_=filter,
-            parser_=parser or self._parser,
-            decoder_=decoder or self._decoder,
-            dependencies_=dependencies,
-            middlewares_=middlewares,
-        )
 
-    @override
-    def publisher(  # type: ignore[override]
+class RedisRouter(
+    BrokerRouter[BaseMessage],
+    RedisRegistrator,
+):
+    """Includable to RedisBroker router."""
+
+    def __init__(
         self,
-        queue: Annotated[
-            Union[RabbitQueue, str],
-            Doc("Default message routing key to publish with."),
-        ] = "",
-        exchange: Annotated[
-            Union[RabbitExchange, str, None],
-            Doc("Target exchange to publish message to."),
-        ] = None,
-        *,
-        routing_key: Annotated[
+        prefix: Annotated[
             str,
-            Doc(
-                "Default message routing key to publish with. "
-                "Overrides `queue` option if presented."
-            ),
+            Doc("String prefix to add to all subscribers queues."),
         ] = "",
-        mandatory: Annotated[
-            bool,
-            Doc(
-                "Client waits for confirmation that the message is placed to some queue. "
-                "RabbitMQ returns message to client if there is no suitable queue."
-            ),
-        ] = True,
-        immediate: Annotated[
-            bool,
-            Doc(
-                "Client expects that there is consumer ready to take the message to work. "
-                "RabbitMQ returns message to client if there is no suitable consumer."
-            ),
-        ] = False,
-        timeout: Annotated[
-            "TimeoutType",
-            Doc("Send confirmation time from RabbitMQ."),
-        ] = None,
-        persist: Annotated[
-            bool,
-            Doc("Restore the message on RabbitMQ reboot."),
-        ] = False,
-        reply_to: Annotated[
-            Optional[str],
+        handlers: Annotated[
+            Iterable[RedisRoute],
+            Doc("Route object to include."),
+        ] = (),
+        *,
+        dependencies: Annotated[
+            Iterable["Depends"],
             Doc(
-                "Reply message routing key to send with (always sending to default exchange)."
+                "Dependencies list (`[Depends(),]`) to apply to all routers' publishers/subscribers."
             ),
-        ] = None,
-        priority: Annotated[
-            Optional[int],
-            Doc("The message priority (0 by default)."),
-        ] = None,
-        # specific
+        ] = (),
         middlewares: Annotated[
-            Iterable["PublisherMiddleware"],
-            Doc("Publisher middlewares to wrap outgoing messages."),
+            Iterable["BrokerMiddleware[BaseMessage]"],
+            Doc("Router middlewares to apply to all routers' publishers/subscribers."),
         ] = (),
-        # AsyncAPI information
-        title: Annotated[
-            Optional[str],
-            Doc("AsyncAPI publisher object title."),
-        ] = None,
-        description: Annotated[
-            Optional[str],
-            Doc("AsyncAPI publisher object description."),
+        parser: Annotated[
+            Optional["CustomCallable"],
+            Doc("Parser to map original **IncomingMessage** Msg to FastStream one."),
         ] = None,
-        schema: Annotated[
-            Optional[Any],
-            Doc(
-                "AsyncAPI publishing message type. "
-                "Should be any python-native object annotation or `pydantic.BaseModel`."
-            ),
+        decoder: Annotated[
+            Optional["CustomCallable"],
+            Doc("Function to decode FastStream msg bytes body to python objects."),
         ] = None,
         include_in_schema: Annotated[
-            bool,
+            Optional[bool],
             Doc("Whetever to include operation in AsyncAPI schema or not."),
-        ] = True,
-        # message args
-        headers: Annotated[
-            Optional["HeadersType"],
-            Doc(
-                "Message headers to store metainformation. "
-                "Can be overridden by `publish.headers` if specified."
-            ),
-        ] = None,
-        content_type: Annotated[
-            Optional[str],
-            Doc(
-                "Message **content-type** header. "
-                "Used by application, not core RabbitMQ. "
-                "Will be setted automatically if not specified."
-            ),
         ] = None,
-        content_encoding: Annotated[
-            Optional[str],
-            Doc("Message body content encoding, e.g. **gzip**."),
-        ] = None,
-        expiration: Annotated[
-            Optional["DateType"],
-            Doc("Message expiration (lifetime) in seconds (or datetime or timedelta)."),
-        ] = None,
-        message_type: Annotated[
-            Optional[str],
-            Doc("Application-specific message type, e.g. **orders.created**."),
-        ] = None,
-        user_id: Annotated[
-            Optional[str],
-            Doc("Publisher connection User ID, validated if set."),
-        ] = None,
-    ) -> AsyncAPIPublisher:
-        """Creates long-living and AsyncAPI-documented publisher object.
-
-        You can use it as a handler decorator (handler should be decorated by `@broker.subscriber(...)` too) - `@broker.publisher(...)`.
-        In such case publisher will publish your handler return value.
-
-        Or you can create a publisher object to call it lately - `broker.publisher(...).publish(...)`.
-        """
-        message_kwargs = PublishKwargs(
-            mandatory=mandatory,
-            immediate=immediate,
-            timeout=timeout,
-            persist=persist,
-            reply_to=reply_to,
-            headers=headers,
-            priority=priority,
-            content_type=content_type,
-            content_encoding=content_encoding,
-            message_type=message_type,
-            user_id=user_id,
-            expiration=expiration,
+    ) -> None:
+        super().__init__(
+            handlers=handlers,
+            # basic args
+            prefix=prefix,
+            dependencies=dependencies,
+            middlewares=middlewares,
+            parser=parser,
+            decoder=decoder,
+            include_in_schema=include_in_schema,
         )
-
-        publisher = cast(
-            AsyncAPIPublisher,
-            super().publisher(
-                AsyncAPIPublisher.create(
-                    routing_key=routing_key,
-                    queue=RabbitQueue.validate(queue),
-                    exchange=RabbitExchange.validate(exchange),
-                    message_kwargs=message_kwargs,
-                    # Specific
-                    broker_middlewares=self._middlewares,
-                    middlewares=middlewares,
-                    # AsyncAPI
-                    title_=title,
-                    description_=description,
-                    schema_=schema,
-                    include_in_schema=self._solve_include_in_schema(include_in_schema),
-                )
-            ),
-        )
-
-        return publisher
```

### Comparing `faststream-0.5.0rc0/faststream/rabbit/fastapi/__init__.py` & `faststream-0.5.0rc1/faststream/rabbit/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/faststream/rabbit/fastapi/router.py` & `faststream-0.5.0rc1/faststream/rabbit/fastapi/router.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,40 +41,39 @@
     from fastapi.types import IncEx
     from pamqp.common import FieldTable
     from starlette.responses import Response
     from starlette.types import ASGIApp, Lifespan
     from yarl import URL
 
     from faststream.asyncapi import schema as asyncapi
-    from faststream.broker.message import StreamMessage
     from faststream.broker.types import (
         BrokerMiddleware,
-        CustomDecoder,
-        CustomParser,
+        CustomCallable,
         Filter,
         PublisherMiddleware,
         SubscriberMiddleware,
     )
+    from faststream.rabbit.message import RabbitMessage
     from faststream.rabbit.schemas.reply import ReplyConfig
     from faststream.security import BaseSecurity
-    from faststream.types import AnyDict
+    from faststream.types import AnyDict, LoggerProto
 
 
 class RabbitRouter(StreamRouter["IncomingMessage"]):
     """A class to represent a RabbitMQ router for incoming messages."""
 
     broker_class = RB
     broker: RB
 
     def __init__(
         self,
         url: Annotated[
             Union[str, "URL", None],
             Doc("RabbitMQ destination location to connect."),
-        ] = "amqp://guest:guest@localhost:5672/",
+        ] = "amqp://guest:guest@localhost:5672/",  # pragma: allowlist secret
         *,
         # connection args
         host: Annotated[
             Optional[str],
             Doc("Destination host. This option overrides `url` option host."),
         ] = None,
         port: Annotated[
@@ -113,19 +112,19 @@
         graceful_timeout: Annotated[
             Optional[float],
             Doc(
                 "Graceful shutdown timeout. Broker waits for all running subscribers completion before shut down."
             ),
         ] = 15.0,
         decoder: Annotated[
-            Optional["CustomDecoder[StreamMessage[IncomingMessage]]"],
+            Optional["CustomCallable"],
             Doc("Custom decoder object."),
         ] = None,
         parser: Annotated[
-            Optional["CustomParser[IncomingMessage]"],
+            Optional["CustomCallable"],
             Doc("Custom parser object."),
         ] = None,
         middlewares: Annotated[
             Iterable["BrokerMiddleware[IncomingMessage]"],
             Doc("Middlewares to apply to all broker publishers/subscribers."),
         ] = (),
         # AsyncAPI args
@@ -153,15 +152,15 @@
         ] = None,
         asyncapi_tags: Annotated[
             Optional[Iterable[Union["asyncapi.Tag", "asyncapi.TagDict"]]],
             Doc("AsyncAPI server tags."),
         ] = None,
         # logging args
         logger: Annotated[
-            Union[logging.Logger, None, object],
+            Union["LoggerProto", None, object],
             Doc("User specified logger to pass into Context and log service messages."),
         ] = Parameter.empty,
         log_level: Annotated[
             int,
             Doc("Service messages log level."),
         ] = logging.INFO,
         log_fmt: Annotated[
@@ -470,29 +469,29 @@
         ] = None,
         # broker arguments
         dependencies: Annotated[
             Iterable["params.Depends"],
             Doc("Dependencies list (`[Depends(),]`) to apply to the subscriber."),
         ] = (),
         parser: Annotated[
-            Optional["CustomParser[IncomingMessage]"],
+            Optional["CustomCallable"],
             Doc(
                 "Parser to map original **aio_pika.IncomingMessage** Msg to FastStream one."
             ),
         ] = None,
         decoder: Annotated[
-            Optional["CustomDecoder[StreamMessage[IncomingMessage]]"],
+            Optional["CustomCallable"],
             Doc("Function to decode FastStream msg bytes body to python objects."),
         ] = None,
         middlewares: Annotated[
             Iterable["SubscriberMiddleware"],
             Doc("Subscriber middlewares to wrap incoming message processing."),
         ] = (),
         filter: Annotated[
-            "Filter[StreamMessage[IncomingMessage]]",
+            "Filter[RabbitMessage]",
             Doc(
                 "Overload subscriber to consume various messages from the same source."
             ),
             deprecated(
                 "Deprecated in **FastStream 0.5.0**. "
                 "Please, create `subscriber` object and use it explicitly instead. "
                 "Argument will be removed in **FastStream 0.6.0**."
@@ -761,15 +760,15 @@
             ),
         ] = None,
         content_type: Annotated[
             Optional[str],
             Doc(
                 "Message **content-type** header. "
                 "Used by application, not core RabbitMQ. "
-                "Will be setted automatically if not specified."
+                "Will be set automatically if not specified."
             ),
         ] = None,
         content_encoding: Annotated[
             Optional[str],
             Doc("Message body content encoding, e.g. **gzip**."),
         ] = None,
         expiration: Annotated[
```

### Comparing `faststream-0.5.0rc0/faststream/rabbit/publisher/asyncapi.py` & `faststream-0.5.0rc1/faststream/rabbit/publisher/asyncapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,30 @@
-from typing import Any, Dict, Iterable, Optional
+from typing import TYPE_CHECKING, Any, Dict, Iterable, Optional
 
-from aio_pika import IncomingMessage
 from typing_extensions import override
 
 from faststream.asyncapi.schema import (
     Channel,
     ChannelBinding,
     CorrelationId,
     Message,
     Operation,
     OperationBinding,
 )
 from faststream.asyncapi.schema.bindings import amqp
 from faststream.asyncapi.utils import resolve_payloads
-from faststream.broker.types import BrokerMiddleware, PublisherMiddleware
 from faststream.rabbit.publisher.usecase import LogicPublisher, PublishKwargs
-from faststream.rabbit.schemas import RabbitExchange, RabbitQueue
 from faststream.rabbit.utils import is_routing_exchange
 
+if TYPE_CHECKING:
+    from aio_pika import IncomingMessage
+
+    from faststream.broker.types import BrokerMiddleware, PublisherMiddleware
+    from faststream.rabbit.schemas import RabbitExchange, RabbitQueue
+
 
 class AsyncAPIPublisher(LogicPublisher):
     """AsyncAPI-compatible Rabbit Publisher class.
 
     Creting by
 
     ```python
@@ -102,20 +105,20 @@
 
     @override
     @classmethod
     def create(  # type: ignore[override]
         cls,
         *,
         routing_key: str,
-        queue: RabbitQueue,
-        exchange: Optional[RabbitExchange],
-        message_kwargs: PublishKwargs,
+        queue: "RabbitQueue",
+        exchange: Optional["RabbitExchange"],
+        message_kwargs: "PublishKwargs",
         # Publisher args
-        broker_middlewares: Iterable[BrokerMiddleware[IncomingMessage]],
-        middlewares: Iterable[PublisherMiddleware],
+        broker_middlewares: Iterable["BrokerMiddleware[IncomingMessage]"],
+        middlewares: Iterable["PublisherMiddleware"],
         # AsyncAPI args
         schema_: Optional[Any],
         title_: Optional[str],
         description_: Optional[str],
         include_in_schema: bool,
     ) -> "AsyncAPIPublisher":
         return cls(
```

### Comparing `faststream-0.5.0rc0/faststream/rabbit/publisher/producer.py` & `faststream-0.5.0rc1/faststream/rabbit/publisher/producer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from types import TracebackType
 from typing import (
     TYPE_CHECKING,
     Any,
     AsyncContextManager,
     Optional,
     Type,
     Union,
@@ -17,44 +16,43 @@
 from faststream.broker.utils import resolve_custom_func
 from faststream.exceptions import WRONG_PUBLISH_ARGS
 from faststream.rabbit.parser import AioPikaParser
 from faststream.rabbit.schemas import RABBIT_REPLY, RabbitExchange
 from faststream.utils.functions import fake_context, timeout_scope
 
 if TYPE_CHECKING:
+    from types import TracebackType
+
     import aiormq
     from aio_pika import IncomingMessage, RobustChannel, RobustQueue
     from aio_pika.abc import DateType, HeadersType, TimeoutType
     from anyio.streams.memory import MemoryObjectReceiveStream
 
-    from faststream.broker.message import StreamMessage
     from faststream.broker.types import (
-        AsyncDecoder,
-        AsyncParser,
-        CustomDecoder,
-        CustomParser,
+        AsyncCallable,
+        CustomCallable,
     )
     from faststream.rabbit.types import AioPikaSendableMessage
     from faststream.rabbit.utils import RabbitDeclarer
     from faststream.types import SendableMessage
 
 
 class AioPikaFastProducer(ProducerProto):
     """A class for fast producing messages using aio-pika."""
 
-    _decoder: "AsyncDecoder[StreamMessage[IncomingMessage]]"
-    _parser: "AsyncParser[IncomingMessage]"
+    _decoder: "AsyncCallable"
+    _parser: "AsyncCallable"
 
     def __init__(
         self,
         *,
         channel: "RobustChannel",
         declarer: "RabbitDeclarer",
-        parser: Optional["CustomParser[IncomingMessage]"],
-        decoder: Optional["CustomDecoder[StreamMessage[IncomingMessage]]"],
+        parser: Optional["CustomCallable"],
+        decoder: Optional["CustomCallable"],
     ) -> None:
         self._channel = channel
         self.declarer = declarer
         self._parser = resolve_custom_func(parser, AioPikaParser.parse_message)
         self._decoder = resolve_custom_func(decoder, AioPikaParser.decode_message)
         self._rpc_lock = anyio.Lock()
 
@@ -193,25 +191,25 @@
             timeout=timeout,
         )
 
 
 class _RPCCallback:
     """A class provides an RPC lock."""
 
-    def __init__(
-        self, lock: "anyio.Lock", callback_queue: "RobustQueue"
-    ) -> None:
+    def __init__(self, lock: "anyio.Lock", callback_queue: "RobustQueue") -> None:
         self.lock = lock
         self.queue = callback_queue
 
     async def __aenter__(self) -> "MemoryObjectReceiveStream[IncomingMessage]":
         (
             send_response_stream,
             receive_response_stream,
-        ) = anyio.create_memory_object_stream[AbstractIncomingMessage](max_buffer_size=1)
+        ) = anyio.create_memory_object_stream[AbstractIncomingMessage](
+            max_buffer_size=1
+        )
         await self.lock.acquire()
 
         self.consumer_tag = await self.queue.consume(
             callback=send_response_stream.send,
             no_ack=True,
         )
 
@@ -220,11 +218,11 @@
             receive_response_stream,
         )
 
     async def __aexit__(
         self,
         exc_type: Optional[Type[BaseException]] = None,
         exc_val: Optional[BaseException] = None,
-        exc_tb: Optional[TracebackType] = None,
+        exc_tb: Optional["TracebackType"] = None,
     ) -> None:
         self.lock.release()
         await self.queue.cancel(self.consumer_tag)
```

### Comparing `faststream-0.5.0rc0/faststream/rabbit/publisher/usecase.py` & `faststream-0.5.0rc1/faststream/rabbit/publisher/usecase.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         Doc("Application-specific message type, e.g. **orders.created**."),
     ]
     content_type: Annotated[
         Optional[str],
         Doc(
             "Message **content-type** header. "
             "Used by application, not core RabbitMQ. "
-            "Will be setted automatically if not specified."
+            "Will be set automatically if not specified."
         ),
     ]
     user_id: Annotated[
         Optional[str],
         Doc("Publisher connection User ID, validated if set."),
     ]
     expiration: Annotated[
```

### Comparing `faststream-0.5.0rc0/faststream/rabbit/schemas/constants.py` & `faststream-0.5.0rc1/faststream/rabbit/schemas/constants.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/faststream/rabbit/schemas/exchange.py` & `faststream-0.5.0rc1/faststream/rabbit/schemas/exchange.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/faststream/rabbit/schemas/queue.py` & `faststream-0.5.0rc1/faststream/rabbit/schemas/queue.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from typing import TYPE_CHECKING, Optional
 
 from typing_extensions import Annotated, Doc
 
 from faststream.broker.schemas import NameRequired
-from faststream.types import AnyDict
 from faststream.utils.path import compile_path
 
 if TYPE_CHECKING:
     from aio_pika.abc import TimeoutType
 
+    from faststream.types import AnyDict
+
 
 class RabbitQueue(NameRequired):
     """A class to represent a RabbitMQ queue.
 
     You can find information about all options in the official RabbitMQ documentation:
 
     https://www.rabbitmq.com/docs/queues
@@ -69,30 +70,30 @@
             Doc("Do not create queue automatically."),
         ] = False,
         auto_delete: Annotated[
             bool,
             Doc("The queue will be deleted after connection closed."),
         ] = False,
         arguments: Annotated[
-            Optional[AnyDict],
+            Optional["AnyDict"],
             Doc(
                 "Queue declarationg arguments. "
                 "You can find information about them in the official RabbitMQ documentation: https://www.rabbitmq.com/docs/queues#optional-arguments"
             ),
         ] = None,
         timeout: Annotated[
             "TimeoutType",
             Doc("Send confirmation time from RabbitMQ."),
         ] = None,
         robust: Annotated[
             bool,
             Doc("Whether to declare queue object as restorable."),
         ] = True,
         bind_arguments: Annotated[
-            Optional[AnyDict],
+            Optional["AnyDict"],
             Doc("Queue-exchange binding options."),
         ] = None,
         routing_key: Annotated[
             str,
             Doc("Explicit binding routing key. Uses `name` if not presented."),
         ] = "",
     ) -> None:
```

### Comparing `faststream-0.5.0rc0/faststream/rabbit/schemas/reply.py` & `faststream-0.5.0rc1/faststream/rabbit/schemas/reply.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/faststream/rabbit/subscriber/asyncapi.py` & `faststream-0.5.0rc1/faststream/rabbit/subscriber/asyncapi.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,31 @@
-from typing import Dict, Iterable, Optional, Union
+from typing import TYPE_CHECKING, Dict, Iterable, Optional, Union
 
-from aio_pika import IncomingMessage
-from fast_depends.dependencies import Depends
 from typing_extensions import override
 
 from faststream.asyncapi.schema import (
     Channel,
     ChannelBinding,
     CorrelationId,
     Message,
     Operation,
     OperationBinding,
 )
 from faststream.asyncapi.schema.bindings import amqp
 from faststream.asyncapi.utils import resolve_payloads
-from faststream.broker.types import BrokerMiddleware
 from faststream.rabbit.schemas import RabbitExchange, RabbitQueue, ReplyConfig
 from faststream.rabbit.subscriber.usecase import LogicSubscriber
 from faststream.rabbit.utils import is_routing_exchange
-from faststream.types import AnyDict
+
+if TYPE_CHECKING:
+    from aio_pika import IncomingMessage
+    from fast_depends.dependencies import Depends
+
+    from faststream.broker.types import BrokerMiddleware
+    from faststream.types import AnyDict
 
 
 class AsyncAPISubscriber(LogicSubscriber):
     """AsyncAPI-compatible Rabbit Subscriber class."""
 
     def get_name(self) -> str:
         return (
@@ -83,22 +86,22 @@
 
     @override
     @classmethod
     def create(  # type: ignore[override]
         cls,
         *,
         queue: RabbitQueue,
-        exchange: Optional[RabbitExchange],
-        consume_args: Optional[AnyDict],
-        reply_config: Optional[ReplyConfig],
+        exchange: Optional["RabbitExchange"],
+        consume_args: Optional["AnyDict"],
+        reply_config: Optional["ReplyConfig"],
         # Subscriber args
         no_ack: bool,
         retry: Union[bool, int],
-        broker_dependencies: Iterable[Depends],
-        broker_middlewares: Iterable[BrokerMiddleware[IncomingMessage]],
+        broker_dependencies: Iterable["Depends"],
+        broker_middlewares: Iterable["BrokerMiddleware[IncomingMessage]"],
         # AsyncAPI args
         title_: Optional[str],
         description_: Optional[str],
         include_in_schema: bool,
     ) -> "AsyncAPISubscriber":
         return cls(
             queue=queue,
```

### Comparing `faststream-0.5.0rc0/faststream/rabbit/subscriber/usecase.py` & `faststream-0.5.0rc1/faststream/rabbit/subscriber/usecase.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,63 +1,68 @@
 from copy import deepcopy
 from typing import (
+    TYPE_CHECKING,
     Any,
     Callable,
     Dict,
     Iterable,
     Optional,
     Sequence,
     Union,
 )
 
-from aio_pika import IncomingMessage, RobustQueue
-from fast_depends.dependencies import Depends
 from typing_extensions import override
 
-from faststream.broker.message import StreamMessage
 from faststream.broker.publisher.fake import FakePublisher
 from faststream.broker.subscriber.usecase import SubscriberUsecase
-from faststream.broker.types import BrokerMiddleware, CustomDecoder, CustomParser
 from faststream.exceptions import SetupError
 from faststream.rabbit.parser import AioPikaParser
-from faststream.rabbit.publisher.producer import AioPikaFastProducer
-from faststream.rabbit.schemas import (
-    BaseRMQInformation,
-    RabbitExchange,
-    RabbitQueue,
-    ReplyConfig,
-)
-from faststream.rabbit.utils import RabbitDeclarer
-from faststream.types import AnyDict, LoggerProto
+from faststream.rabbit.schemas import BaseRMQInformation
+
+if TYPE_CHECKING:
+    from aio_pika import IncomingMessage, RobustQueue
+    from fast_depends.dependencies import Depends
+
+    from faststream.broker.message import StreamMessage
+    from faststream.broker.types import BrokerMiddleware, CustomCallable
+    from faststream.rabbit.publisher.producer import AioPikaFastProducer
+    from faststream.rabbit.schemas import (
+        RabbitExchange,
+        RabbitQueue,
+        ReplyConfig,
+    )
+    from faststream.rabbit.utils import RabbitDeclarer
+    from faststream.types import AnyDict, LoggerProto
 
 
 class LogicSubscriber(
-    SubscriberUsecase[IncomingMessage],
+    SubscriberUsecase["IncomingMessage"],
     BaseRMQInformation,
 ):
     """A class to handle logic for RabbitMQ message consumption."""
+
     app_id: Optional[str]
-    declarer: Optional[RabbitDeclarer]
+    declarer: Optional["RabbitDeclarer"]
 
     _consumer_tag: Optional[str]
-    _queue_obj: Optional[RobustQueue]
-    _producer: Optional[AioPikaFastProducer]
+    _queue_obj: Optional["RobustQueue"]
+    _producer: Optional["AioPikaFastProducer"]
 
     def __init__(
         self,
         *,
-        queue: RabbitQueue,
-        exchange: Optional[RabbitExchange],
-        consume_args: Optional[AnyDict],
-        reply_config: Optional[ReplyConfig],
+        queue: "RabbitQueue",
+        exchange: Optional["RabbitExchange"],
+        consume_args: Optional["AnyDict"],
+        reply_config: Optional["ReplyConfig"],
         # Subscriber args
         no_ack: bool,
         retry: Union[bool, int],
-        broker_dependencies: Iterable[Depends],
-        broker_middlewares: Iterable[BrokerMiddleware[IncomingMessage]],
+        broker_dependencies: Iterable["Depends"],
+        broker_middlewares: Iterable["BrokerMiddleware[IncomingMessage]"],
         # AsyncAPI args
         title_: Optional[str],
         description_: Optional[str],
         include_in_schema: bool,
     ) -> None:
         super().__init__(
             default_parser=AioPikaParser.parse_message,
@@ -89,23 +94,23 @@
 
     @override
     def setup(  # type: ignore[override]
         self,
         *,
         app_id: Optional[str],
         virtual_host: str,
-        declarer: RabbitDeclarer,
+        declarer: "RabbitDeclarer",
         # basic args
         logger: Optional["LoggerProto"],
         producer: Optional["AioPikaFastProducer"],
         graceful_timeout: Optional[float],
         extra_context: Optional["AnyDict"],
         # broker options
-        broker_parser: Optional["CustomParser[IncomingMessage]"],
-        broker_decoder: Optional["CustomDecoder[StreamMessage[IncomingMessage]]"],
+        broker_parser: Optional["CustomCallable"],
+        broker_decoder: Optional["CustomCallable"],
         # dependant args
         apply_types: bool,
         is_validate: bool,
         _get_dependant: Optional[Callable[..., Any]],
     ) -> None:
         self.app_id = app_id
         self.virtual_host = virtual_host
@@ -159,16 +164,16 @@
                     await self._queue_obj.cancel(self._consumer_tag)
                 self._consumer_tag = None
 
             self._queue_obj = None
 
     def _make_response_publisher(
         self,
-        message: StreamMessage[Any],
-    ) -> Sequence[FakePublisher]:
+        message: "StreamMessage[Any]",
+    ) -> Sequence["FakePublisher"]:
         if not message.reply_to or self._producer is None:
             return ()
 
         return (
             FakePublisher(
                 self._producer.publish,
                 publish_kwargs={
@@ -180,25 +185,25 @@
         )
 
     def __hash__(self) -> int:
         return self.get_routing_hash(self.queue, self.exchange)
 
     @staticmethod
     def get_routing_hash(
-        queue: RabbitQueue,
-        exchange: Optional[RabbitExchange] = None,
+        queue: "RabbitQueue",
+        exchange: Optional["RabbitExchange"] = None,
     ) -> int:
         """Calculate the routing hash for a RabbitMQ queue and exchange."""
         return hash(queue) + hash(exchange or "")
 
     @staticmethod
     def build_log_context(
         message: Optional["StreamMessage[Any]"],
-        queue: RabbitQueue,
-        exchange: Optional[RabbitExchange] = None,
+        queue: "RabbitQueue",
+        exchange: Optional["RabbitExchange"] = None,
     ) -> Dict[str, str]:
         return {
             "queue": queue.name,
             "exchange": getattr(exchange, "name", ""),
             "message_id": getattr(message, "message_id", ""),
         }
```

### Comparing `faststream-0.5.0rc0/faststream/redis/__init__.py` & `faststream-0.5.0rc1/faststream/redis/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/faststream/redis/annotations.py` & `faststream-0.5.0rc1/faststream/redis/fastapi/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from redis.asyncio.client import Redis as RedisClient
 from typing_extensions import Annotated
 
-from faststream.annotations import ContextRepo, Logger, NoCast
-from faststream.broker.message import StreamMessage as BrokerStreamMessage
+from faststream.broker.fastapi.context import Context, ContextRepo, Logger
 from faststream.redis.broker.broker import RedisBroker as RB
-from faststream.redis.message import BaseMessage as BM
-from faststream.utils.context import Context
+from faststream.redis.fastapi.fastapi import RedisRouter
+from faststream.redis.message import BaseMessage as RM  # noqa: N814
 
 __all__ = (
+    "Context",
     "Logger",
     "ContextRepo",
-    "NoCast",
+    "RedisRouter",
     "RedisMessage",
     "RedisBroker",
     "Redis",
 )
 
-RedisMessage = Annotated[BrokerStreamMessage[BM], Context("message")]
+RedisMessage = Annotated[RM, Context("message")]
 RedisBroker = Annotated[RB, Context("broker")]
 Redis = Annotated[RedisClient, Context("broker._connection")]
```

### Comparing `faststream-0.5.0rc0/faststream/redis/message.py` & `faststream-0.5.0rc1/faststream/redis/message.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     List,
     Literal,
     Optional,
     TypeVar,
     Union,
 )
 
-from typing_extensions import TypeAlias, TypedDict, override
+from typing_extensions import NotRequired, TypeAlias, TypedDict, override
 
 from faststream.broker.message import StreamMessage as BrokerStreamMessage
 
 if TYPE_CHECKING:
     from redis.asyncio import Redis
 
     from faststream.types import DecodedMessage
@@ -23,77 +23,117 @@
     "DefaultListMessage",
     "BatchListMessage",
     "DefaultStreamMessage",
     "BatchStreamMessage",
 ]
 
 
+class UnifyRedisDict(TypedDict):
+    type: Literal[
+        "pmessage",
+        "message",
+        "list",
+        "blist",
+        "stream",
+        "bstream",
+    ]
+    channel: str
+    data: Union[
+        bytes,
+        List[bytes],
+        Dict[bytes, bytes],
+        List[Dict[bytes, bytes]],
+    ]
+    pattern: NotRequired[Optional[bytes]]
+
+
+class UnifyRedisMessage(BrokerStreamMessage[UnifyRedisDict]):
+    pass
+
+
 class PubSubMessage(TypedDict):
     """A class to represent a PubSub message."""
+
     type: Literal["pmessage", "message"]
     channel: str
     data: bytes
     pattern: Optional[bytes]
 
 
 class RedisMessage(BrokerStreamMessage[PubSubMessage]):
     pass
 
+
 class ListMessage(TypedDict):
     """A class to represent an Abstract List message."""
+
     channel: str
 
+
 class DefaultListMessage(ListMessage):
     """A class to represent a single List message."""
+
     type: Literal["list"]
     data: bytes
 
+
 class BatchListMessage(ListMessage):
     """A class to represent a List messages batch."""
+
     type: Literal["blist"]
     data: List[bytes]
 
+
 class RedisListMessage(BrokerStreamMessage[DefaultListMessage]):
     """StreamMessage for single List message."""
+
     pass
 
+
 class RedisBatchListMessage(BrokerStreamMessage[BatchListMessage]):
     """StreamMessage for single List message."""
+
     decoded_body: List["DecodedMessage"]
 
 
 DATA_KEY = "__data__"
 bDATA_KEY = DATA_KEY.encode()  # noqa: N816
 
 
 class StreamMessage(TypedDict):
     channel: str
     message_ids: List[bytes]
 
+
 class DefaultStreamMessage(StreamMessage):
     type: Literal["stream"]
     data: Dict[bytes, bytes]
 
+
 class BatchStreamMessage(StreamMessage):
     type: Literal["bstream"]
     data: List[Dict[bytes, bytes]]
 
+
 _StreamMsgType = TypeVar("_StreamMsgType", bound=StreamMessage)
 
+
 class _RedisStreamMessageMixin(BrokerStreamMessage[_StreamMsgType]):
     @override
     async def ack(
         self,
         redis: Optional["Redis[bytes]"] = None,
         group: Optional[str] = None,
     ) -> None:
         if not self.committed and group is not None and redis is not None:
             ids = self.raw_message["message_ids"]
             channel = self.raw_message["channel"]
             await redis.xack(channel, group, *ids)  # type: ignore[no-untyped-call]
             await super().ack()
 
+
 class RedisStreamMessage(_RedisStreamMessageMixin[DefaultStreamMessage]):
     pass
 
+
 class RedisBatchStreamMessage(_RedisStreamMessageMixin[BatchStreamMessage]):
     decoded_body: List["DecodedMessage"]
```

### Comparing `faststream-0.5.0rc0/faststream/redis/parser.py` & `faststream-0.5.0rc1/faststream/redis/parser.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,46 +1,40 @@
 from typing import (
     TYPE_CHECKING,
     Any,
-    Generic,
     Mapping,
     Optional,
     Sequence,
     Tuple,
     Type,
     TypeVar,
     Union,
     cast,
 )
 
 from faststream._compat import dump_json, json_loads
 from faststream.broker.message import (
-    StreamMessage,
     decode_message,
     encode_message,
     gen_cor_id,
 )
 from faststream.constants import ContentTypes
 from faststream.redis.message import (
-    BatchListMessage,
-    BatchStreamMessage,
-    DefaultListMessage,
-    DefaultStreamMessage,
-    PubSubMessage,
     RedisBatchListMessage,
     RedisBatchStreamMessage,
     RedisListMessage,
     RedisMessage,
     RedisStreamMessage,
     bDATA_KEY,
 )
 from faststream.types import AnyDict, DecodedMessage, SendableMessage
 from faststream.utils.context.repository import context
 
 if TYPE_CHECKING:
+    from faststream.broker.message import StreamMessage
     from faststream.redis.schemas import PubSub
     from faststream.redis.subscriber.usecase import ChannelSubscriber
 
 
 MsgType = TypeVar("MsgType", bound=Mapping[str, Any])
 
 
@@ -60,17 +54,17 @@
         self.data = data
         self.headers = headers or {}
 
     @classmethod
     def build(
         cls,
         *,
-        message: Union[Sequence[SendableMessage], SendableMessage],
+        message: Union[Sequence["SendableMessage"], "SendableMessage"],
         reply_to: Optional[str],
-        headers: Optional[AnyDict],
+        headers: Optional["AnyDict"],
         correlation_id: str,
     ) -> "RawMessage":
         payload, content_type = encode_message(message)
 
         headers_to_send = {
             "correlation_id": correlation_id,
         }
@@ -89,34 +83,36 @@
             headers=headers_to_send,
         )
 
     @classmethod
     def encode(
         cls,
         *,
-        message: Union[Sequence[SendableMessage], SendableMessage],
+        message: Union[Sequence["SendableMessage"], "SendableMessage"],
         reply_to: Optional[str],
-        headers: Optional[AnyDict],
+        headers: Optional["AnyDict"],
         correlation_id: str,
     ) -> bytes:
         msg = cls.build(
             message=message,
             reply_to=reply_to,
             headers=headers,
             correlation_id=correlation_id,
         )
 
-        return dump_json({
-            "data": msg.data,
-            "headers": msg.headers,
-        })
+        return dump_json(
+            {
+                "data": msg.data,
+                "headers": msg.headers,
+            }
+        )
 
     @staticmethod
-    def parse(data: bytes) -> Tuple[bytes, AnyDict]:
-        headers: AnyDict
+    def parse(data: bytes) -> Tuple[bytes, "AnyDict"]:
+        headers: "AnyDict"
 
         try:
             # FastStream message format
             parsed_data = json_loads(data)
             data = parsed_data["data"].encode()
             headers = parsed_data["headers"]
 
@@ -124,99 +120,96 @@
             # Raw Redis message format
             data = data
             headers = {}
 
         return data, headers
 
 
-class SimpleParser(Generic[MsgType]):
-    msg_class: Type[StreamMessage[MsgType]]
+class SimpleParser:
+    msg_class: Type["StreamMessage[Any]"]
 
     @classmethod
-    async def parse_message(cls, message: MsgType) -> StreamMessage[MsgType]:
+    async def parse_message(
+        cls, message: Mapping[str, Any]
+    ) -> "StreamMessage[Mapping[str, Any]]":
         data, headers = cls._parse_data(message)
         id_ = gen_cor_id()
         return cls.msg_class(
             raw_message=message,
             body=data,
             path=cls.get_path(message),
             headers=headers,
             reply_to=headers.get("reply_to", ""),
             content_type=headers.get("content-type"),
             message_id=headers.get("message_id", id_),
             correlation_id=headers.get("correlation_id", id_),
         )
 
     @staticmethod
-    def _parse_data(message: MsgType) -> Tuple[bytes, AnyDict]:
+    def _parse_data(message: Mapping[str, Any]) -> Tuple[bytes, "AnyDict"]:
         return RawMessage.parse(message["data"])
 
     @staticmethod
-    def get_path(message: MsgType) -> AnyDict:
+    def get_path(message: Mapping[str, Any]) -> "AnyDict":
         return {}
 
     @staticmethod
     async def decode_message(
-        msg: StreamMessage[MsgType],
+        msg: "StreamMessage[MsgType]",
     ) -> DecodedMessage:
         return decode_message(msg)
 
 
-class RedisPubSubParser(SimpleParser[PubSubMessage]):
+class RedisPubSubParser(SimpleParser):
     msg_class = RedisMessage
 
     @staticmethod
-    def get_path(message: PubSubMessage) -> AnyDict:
+    def get_path(message: Mapping[str, Any]) -> "AnyDict":
         if (
             message.get("pattern")
             and (handler := cast("ChannelSubscriber", context.get_local("handler_")))
             and (channel := cast(Optional["PubSub"], getattr(handler, "channel", None)))
             and (path_re := channel.path_regex)
             and (match := path_re.match(message["channel"]))
         ):
             return match.groupdict()
 
         else:
             return {}
 
 
-class RedisListParser(SimpleParser[DefaultListMessage]):
+class RedisListParser(SimpleParser):
     msg_class = RedisListMessage
 
 
-class RedisBatchListParser(SimpleParser[BatchListMessage]):
+class RedisBatchListParser(SimpleParser):
     msg_class = RedisBatchListMessage
 
     @staticmethod
-    def _parse_data(message: BatchListMessage) -> Tuple[bytes, AnyDict]:
+    def _parse_data(message: Mapping[str, Any]) -> Tuple[bytes, "AnyDict"]:
         return (
-            dump_json(
-                RawMessage.parse(x)[0]
-                for x in message["data"]
-            ),
+            dump_json(RawMessage.parse(x)[0] for x in message["data"]),
             {"content-type": ContentTypes.json},
         )
 
 
-class RedisStreamParser(SimpleParser[DefaultStreamMessage]):
+class RedisStreamParser(SimpleParser):
     msg_class = RedisStreamMessage
 
     @classmethod
-    def _parse_data(cls, message: DefaultStreamMessage) -> Tuple[bytes, AnyDict]:
+    def _parse_data(cls, message: Mapping[str, Any]) -> Tuple[bytes, "AnyDict"]:
         data = message["data"]
         return RawMessage.parse(data.get(bDATA_KEY) or dump_json(data))
 
 
-class RedisBatchStreamParser(SimpleParser[BatchStreamMessage]):
+class RedisBatchStreamParser(SimpleParser):
     msg_class = RedisBatchStreamMessage
 
     @staticmethod
-    def _parse_data(message: BatchStreamMessage) -> Tuple[bytes, AnyDict]:
+    def _parse_data(message: Mapping[str, Any]) -> Tuple[bytes, "AnyDict"]:
         return (
             dump_json(
-                RawMessage.parse(data)[0]
-                if (data := x.get(bDATA_KEY))
-                else x
+                RawMessage.parse(data)[0] if (data := x.get(bDATA_KEY)) else x
                 for x in message["data"]
             ),
             {"content-type": ContentTypes.json},
         )
```

### Comparing `faststream-0.5.0rc0/faststream/redis/router.py` & `faststream-0.5.0rc1/faststream/redis/broker/registrator.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,155 +1,76 @@
-from typing import TYPE_CHECKING, Any, Callable, Iterable, Optional, Union
+from typing import TYPE_CHECKING, Any, Dict, Iterable, Optional, Union, cast
 
-from typing_extensions import Annotated, Doc, deprecated
+from typing_extensions import Annotated, Doc, deprecated, override
 
-from faststream.broker.router import ArgsContainer, BrokerRouter, SubscriberRoute
+from faststream.broker.core.abc import ABCBroker
 from faststream.broker.utils import default_filter
-from faststream.redis.broker.registrator import RedisRegistrator
-from faststream.redis.message import BaseMessage
-from faststream.redis.schemas import ListSub, PubSub, StreamSub
-from faststream.types import SendableMessage
+from faststream.redis.message import UnifyRedisDict
+from faststream.redis.publisher.asyncapi import AsyncAPIPublisher
+from faststream.redis.subscriber.asyncapi import AsyncAPISubscriber
 
 if TYPE_CHECKING:
-    from aio_pika.message import IncomingMessage
     from fast_depends.dependencies import Depends
 
-    from faststream.broker.message import StreamMessage
     from faststream.broker.types import (
-        BrokerMiddleware,
-        CustomDecoder,
-        CustomParser,
+        CustomCallable,
         Filter,
         PublisherMiddleware,
         SubscriberMiddleware,
     )
+    from faststream.redis.message import UnifyRedisMessage
+    from faststream.redis.publisher.asyncapi import PublisherType
+    from faststream.redis.schemas import ListSub, PubSub, StreamSub
+    from faststream.redis.subscriber.asyncapi import SubsciberType
     from faststream.types import AnyDict
 
 
-class RedisPublisher(ArgsContainer):
-    """Delayed RedisPublisher registration object.
+class RedisRegistrator(ABCBroker[UnifyRedisDict]):
+    """Includable to RabbitBroker router."""
 
-    Just a copy of RedisRegistrator.publisher(...) arguments.
-    """
+    _subscribers: Dict[int, "SubsciberType"]
+    _publishers: Dict[int, "PublisherType"]
 
-    def __init__(
+    @override
+    def subscriber(  # type: ignore[override]
         self,
         channel: Annotated[
-            Union[PubSub, str, None],
+            Union["PubSub", str, None],
             Doc("Redis PubSub object name to send message."),
         ] = None,
         *,
         list: Annotated[
-            Union[ListSub, str, None],
+            Union["ListSub", str, None],
             Doc("Redis List object name to send message."),
         ] = None,
         stream: Annotated[
-            Union[StreamSub, str, None],
-            Doc("Redis Stream object name to send message."),
-        ] = None,
-        headers: Annotated[
-            Optional["AnyDict"],
-            Doc(
-                "Message headers to store metainformation. "
-                "Can be overridden by `publish.headers` if specified."
-            ),
-        ] = None,
-        reply_to: Annotated[
-            str,
-            Doc("Reply message destination PubSub object name."),
-        ] = "",
-        middlewares: Annotated[
-            Iterable["PublisherMiddleware"],
-            Doc("Publisher middlewares to wrap outgoing messages."),
-        ] = (),
-        # AsyncAPI information
-        title: Annotated[
-            Optional[str],
-            Doc("AsyncAPI publisher object title."),
-        ] = None,
-        description: Annotated[
-            Optional[str],
-            Doc("AsyncAPI publisher object description."),
-        ] = None,
-        schema: Annotated[
-            Optional[Any],
-            Doc(
-                "AsyncAPI publishing message type. "
-                "Should be any python-native object annotation or `pydantic.BaseModel`."
-            ),
-        ] = None,
-        include_in_schema: Annotated[
-            bool,
-            Doc("Whetever to include operation in AsyncAPI schema or not."),
-        ] = True,
-    ) -> None:
-        super().__init__(
-            channel=channel,
-            list=list,
-            stream=stream,
-            headers=headers,
-            reply_to=reply_to,
-            middlewares=middlewares,
-            title=title,
-            description=description,
-            schema=schema,
-            include_in_schema=include_in_schema,
-        )
-
-
-class RedisRoute(SubscriberRoute):
-    """Class to store delayed RedisBroker subscriber registration."""
-
-    def __init__(
-        self,
-        call: Annotated[
-            Callable[..., SendableMessage],
-            Doc(
-                "Message handler function "
-                "to wrap the same with `@broker.subscriber(...)` way."
-            ),
-        ],
-        channel: Annotated[
-            Union[PubSub, str, None],
-            Doc("Redis PubSub object name to send message."),
-        ] = None,
-        *,
-        publishers: Annotated[
-            Iterable[RedisPublisher],
-            Doc("Redis publishers to broadcast the handler result."),
-        ] = (),
-        list: Annotated[
-            Union[ListSub, str, None],
-            Doc("Redis List object name to send message."),
-        ] = None,
-        stream: Annotated[
-            Union[StreamSub, str, None],
+            Union["StreamSub", str, None],
             Doc("Redis Stream object name to send message."),
         ] = None,
         # broker arguments
         dependencies: Annotated[
             Iterable["Depends"],
             Doc("Dependencies list (`[Depends(),]`) to apply to the subscriber."),
         ] = (),
         parser: Annotated[
-            Optional["CustomParser[BaseMessage]"],
+            Optional["CustomCallable"],
             Doc(
                 "Parser to map original **aio_pika.IncomingMessage** Msg to FastStream one."
             ),
         ] = None,
         decoder: Annotated[
-            Optional["CustomDecoder[StreamMessage[BaseMessage]]"],
+            Optional["CustomCallable"],
             Doc("Function to decode FastStream msg bytes body to python objects."),
         ] = None,
         middlewares: Annotated[
             Iterable["SubscriberMiddleware"],
             Doc("Subscriber middlewares to wrap incoming message processing."),
         ] = (),
         filter: Annotated[
-            "Filter[StreamMessage[BaseMessage]]",
+            "Filter[UnifyRedisMessage]",
             Doc(
                 "Overload subscriber to consume various messages from the same source."
             ),
             deprecated(
                 "Deprecated in **FastStream 0.5.0**. "
                 "Please, create `subscriber` object and use it explicitly instead. "
                 "Argument will be removed in **FastStream 0.6.0**."
@@ -175,77 +96,115 @@
                 "Uses decorated docstring as default."
             ),
         ] = None,
         include_in_schema: Annotated[
             bool,
             Doc("Whetever to include operation in AsyncAPI schema or not."),
         ] = True,
-    ) -> None:
-        super().__init__(
-            call,
-            channel=channel,
-            publishers=publishers,
-            list=list,
-            stream=stream,
-            dependencies=dependencies,
-            parser=parser,
-            decoder=decoder,
-            middlewares=middlewares,
-            filter=filter,
-            retry=retry,
-            no_ack=no_ack,
-            title=title,
-            description=description,
-            include_in_schema=include_in_schema,
+    ) -> AsyncAPISubscriber:
+        subscriber = cast(
+            AsyncAPISubscriber,
+            super().subscriber(
+                AsyncAPISubscriber.create(
+                    channel=channel,
+                    list=list,
+                    stream=stream,
+                    # subscriber args
+                    no_ack=no_ack,
+                    retry=retry,
+                    broker_middlewares=self._middlewares,
+                    broker_dependencies=self._dependencies,
+                    # AsyncAPI
+                    title_=title,
+                    description_=description,
+                    include_in_schema=self._solve_include_in_schema(include_in_schema),
+                )
+            ),
         )
 
+        return subscriber.add_call(
+            filter_=filter,
+            parser_=parser or self._parser,
+            decoder_=decoder or self._decoder,
+            dependencies_=dependencies,
+            middlewares_=middlewares,
+        )
 
-class RedisRouter(
-    BrokerRouter[BaseMessage],
-    RedisRegistrator,
-):
-    """Includable to RedisBroker router."""
-
-    def __init__(
+    @override
+    def publisher(  # type: ignore[override]
         self,
-        prefix: Annotated[
-            str,
-            Doc("String prefix to add to all subscribers queues."),
-        ] = "",
-        handlers: Annotated[
-            Iterable[RedisRoute],
-            Doc("Route object to include."),
-        ] = (),
+        channel: Annotated[
+            Union["PubSub", str, None],
+            Doc("Redis PubSub object name to send message."),
+        ] = None,
         *,
-        dependencies: Annotated[
-            Iterable["Depends"],
+        list: Annotated[
+            Union["ListSub", str, None],
+            Doc("Redis List object name to send message."),
+        ] = None,
+        stream: Annotated[
+            Union["StreamSub", str, None],
+            Doc("Redis Stream object name to send message."),
+        ] = None,
+        headers: Annotated[
+            Optional["AnyDict"],
             Doc(
-                "Dependencies list (`[Depends(),]`) to apply to all routers' publishers/subscribers."
+                "Message headers to store metainformation. "
+                "Can be overridden by `publish.headers` if specified."
             ),
-        ] = (),
+        ] = None,
+        reply_to: Annotated[
+            str,
+            Doc("Reply message destination PubSub object name."),
+        ] = "",
         middlewares: Annotated[
-            Iterable["BrokerMiddleware[IncomingMessage]"],
-            Doc("Router middlewares to apply to all routers' publishers/subscribers."),
+            Iterable["PublisherMiddleware"],
+            Doc("Publisher middlewares to wrap outgoing messages."),
         ] = (),
-        parser: Annotated[
-            Optional["CustomParser[IncomingMessage]"],
-            Doc("Parser to map original **IncomingMessage** Msg to FastStream one."),
+        # AsyncAPI information
+        title: Annotated[
+            Optional[str],
+            Doc("AsyncAPI publisher object title."),
         ] = None,
-        decoder: Annotated[
-            Optional["CustomDecoder[StreamMessage[IncomingMessage]]"],
-            Doc("Function to decode FastStream msg bytes body to python objects."),
+        description: Annotated[
+            Optional[str],
+            Doc("AsyncAPI publisher object description."),
+        ] = None,
+        schema: Annotated[
+            Optional[Any],
+            Doc(
+                "AsyncAPI publishing message type. "
+                "Should be any python-native object annotation or `pydantic.BaseModel`."
+            ),
         ] = None,
         include_in_schema: Annotated[
-            Optional[bool],
+            bool,
             Doc("Whetever to include operation in AsyncAPI schema or not."),
-        ] = None,
-    ) -> None:
-        super().__init__(
-            handlers=handlers,
-            # basic args
-            prefix=prefix,
-            dependencies=dependencies,
-            middlewares=middlewares,
-            parser=parser,
-            decoder=decoder,
-            include_in_schema=include_in_schema,
+        ] = True,
+    ) -> AsyncAPIPublisher:
+        """Creates long-living and AsyncAPI-documented publisher object.
+
+        You can use it as a handler decorator (handler should be decorated by `@broker.subscriber(...)` too) - `@broker.publisher(...)`.
+        In such case publisher will publish your handler return value.
+
+        Or you can create a publisher object to call it lately - `broker.publisher(...).publish(...)`.
+        """
+        return cast(
+            AsyncAPIPublisher,
+            super().publisher(
+                AsyncAPIPublisher.create(
+                    channel=channel,
+                    list=list,
+                    stream=stream,
+                    headers=headers,
+                    reply_to=reply_to,
+                    # Specific
+                    broker_middlewares=self._middlewares,
+                    middlewares=middlewares,
+                    # AsyncAPI
+                    title_=title,
+                    description_=description,
+                    schema_=schema,
+                    include_in_schema=self._solve_include_in_schema(include_in_schema),
+                )
+            ),
         )
```

### Comparing `faststream-0.5.0rc0/faststream/redis/security.py` & `faststream-0.5.0rc1/faststream/redis/security.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,50 @@
-from typing import Any, Optional
+from typing import TYPE_CHECKING, Any, Optional
 
 from redis.asyncio.connection import Connection
 
 from faststream.security import BaseSecurity, SASLPlaintext
-from faststream.types import AnyDict
 
+if TYPE_CHECKING:
+    from faststream.types import AnyDict
 
-def parse_security(security: Optional[BaseSecurity]) -> AnyDict:
+
+def parse_security(security: Optional[BaseSecurity]) -> "AnyDict":
     if security is None:
         return {}
     elif isinstance(security, SASLPlaintext):
         return _parse_sasl_plaintext(security)
     elif isinstance(security, BaseSecurity):
         return _parse_base_security(security)
     else:
         raise NotImplementedError(f"RedisBroker does not support {type(security)}")
 
 
-def _parse_base_security(security: BaseSecurity) -> AnyDict:
+def _parse_base_security(security: BaseSecurity) -> "AnyDict":
     if security.use_ssl:
 
         class SSLConnection(Connection):
             def __init__(
                 self,
                 _security: BaseSecurity = security,
                 **kwargs: Any,
             ) -> None:
                 self._security = _security
                 super().__init__(**kwargs)
 
             def _connection_arguments(self) -> Any:
                 return {
                     **super()._connection_arguments(),  # type: ignore[misc]
-                    "ssl": self._security.ssl_context
+                    "ssl": self._security.ssl_context,
                 }
 
         return {"connection_class": SSLConnection}
     else:
         return {}
 
 
-def _parse_sasl_plaintext(security: SASLPlaintext) -> AnyDict:
+def _parse_sasl_plaintext(security: SASLPlaintext) -> "AnyDict":
     return {
         **_parse_base_security(security),
         "username": security.username,
         "password": security.password,
     }
```

### Comparing `faststream-0.5.0rc0/faststream/redis/testing.py` & `faststream-0.5.0rc1/faststream/redis/testing.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,46 +1,49 @@
 import re
-from typing import Any, Optional, Sequence, Union
+from typing import TYPE_CHECKING, Any, Optional, Sequence, Union
 
 from typing_extensions import override
 
 from faststream.broker.message import gen_cor_id
-from faststream.broker.wrapper.call import HandlerCallWrapper
 from faststream.exceptions import SetupError
 from faststream.redis.broker.broker import RedisBroker
 from faststream.redis.message import (
     BatchListMessage,
     BatchStreamMessage,
     DefaultListMessage,
     DefaultStreamMessage,
     PubSubMessage,
     bDATA_KEY,
 )
 from faststream.redis.parser import RawMessage
-from faststream.redis.publisher.asyncapi import AsyncAPIPublisher
 from faststream.redis.publisher.producer import RedisFastProducer
 from faststream.redis.schemas import INCORRECT_SETUP_MSG
 from faststream.redis.subscriber.asyncapi import AsyncAPISubscriber
 from faststream.testing.broker import TestBroker, call_handler
-from faststream.types import AnyDict, SendableMessage
+
+if TYPE_CHECKING:
+    from faststream.broker.wrapper.call import HandlerCallWrapper
+    from faststream.redis.publisher.asyncapi import AsyncAPIPublisher
+    from faststream.types import AnyDict, SendableMessage
 
 __all__ = ("TestRedisBroker",)
 
 
 class TestRedisBroker(TestBroker[RedisBroker]):
     """A class to test Redis brokers."""
 
     @staticmethod
     def create_publisher_fake_subscriber(
         broker: RedisBroker,
-        publisher: AsyncAPIPublisher,
-    ) -> HandlerCallWrapper[Any, Any, Any]:
+        publisher: "AsyncAPIPublisher",
+    ) -> "HandlerCallWrapper[Any, Any, Any]":
         sub = broker.subscriber(**publisher.subscriber_property)
 
         if not sub.calls:
+
             @sub
             def f(msg: Any) -> None:
                 pass
 
             broker.setup_subscriber(sub)
 
         return sub.calls[0].handler
@@ -52,46 +55,50 @@
         **kwargs: Any,
     ) -> None:
         broker._producer = FakeProducer(broker)  # type: ignore[assignment]
 
     @staticmethod
     def remove_publisher_fake_subscriber(
         broker: RedisBroker,
-        publisher: AsyncAPIPublisher,
+        publisher: "AsyncAPIPublisher",
     ) -> None:
         broker._subscribers.pop(
             hash(AsyncAPISubscriber.create(**publisher.subscriber_property)),
             None,
         )
 
 
 class FakeProducer(RedisFastProducer):
     def __init__(self, broker: RedisBroker) -> None:
         self.broker = broker
 
     @override
     async def publish(  # type: ignore[override]
         self,
-        message: SendableMessage,
+        message: "SendableMessage",
         *,
         channel: Optional[str] = None,
         list: Optional[str] = None,
         stream: Optional[str] = None,
         maxlen: Optional[int] = None,
-        headers: Optional[AnyDict] = None,
+        headers: Optional["AnyDict"] = None,
         reply_to: str = "",
         correlation_id: Optional[str] = None,
         rpc: bool = False,
         rpc_timeout: Optional[float] = 30.0,
         raise_timeout: bool = False,
     ) -> Optional[Any]:
         correlation_id = correlation_id or gen_cor_id()
 
-        body = build_message(message=message, reply_to=reply_to,
-                             correlation_id=correlation_id, headers=headers,)
+        body = build_message(
+            message=message,
+            reply_to=reply_to,
+            correlation_id=correlation_id,
+            headers=headers,
+        )
 
         any_of = channel or list or stream
         if any_of is None:
             raise SetupError(INCORRECT_SETUP_MSG)
 
         msg: Any = None
         for handler in self.broker._subscribers.values():  # pragma: no branch
@@ -135,22 +142,22 @@
 
             elif stream and (st := getattr(handler, "stream_sub", None)) is not None:
                 if st.batch:
                     msg = BatchStreamMessage(
                         type="bstream",
                         channel=stream,
                         data=[{bDATA_KEY: body}],
-                        message_ids=[]
+                        message_ids=[],
                     )
                 else:
                     msg = DefaultStreamMessage(
                         type="stream",
                         channel=stream,
                         data={bDATA_KEY: body},
-                        message_ids=[]
+                        message_ids=[],
                     )
 
                 call = stream == st.name
 
             if call:
                 r = await call_handler(
                     handler=handler,
@@ -163,41 +170,48 @@
                 if rpc:  # pragma: no branch
                     return r
 
         return None
 
     async def publish_batch(
         self,
-        *msgs: SendableMessage,
+        *msgs: "SendableMessage",
         list: str,
         correlation_id: Optional[str] = None,
     ) -> None:
         correlation_id = correlation_id or gen_cor_id()
 
         for handler in self.broker._subscribers.values():  # pragma: no branch
-            if (list_sub := getattr(handler, "list_sub", None)) and list_sub.name == list:
+            if (
+                list_sub := getattr(handler, "list_sub", None)
+            ) and list_sub.name == list:
                 await call_handler(
                     handler=handler,
                     message=BatchListMessage(
                         type="blist",
                         channel=list,
-                        data=[build_message(
-                            m, correlation_id=correlation_id,) for m in msgs],
-                    )
+                        data=[
+                            build_message(
+                                m,
+                                correlation_id=correlation_id,
+                            )
+                            for m in msgs
+                        ],
+                    ),
                 )
 
         return None
 
 
 def build_message(
-    message: Union[Sequence[SendableMessage], SendableMessage],
+    message: Union[Sequence["SendableMessage"], "SendableMessage"],
     *,
     correlation_id: str,
     reply_to: str = "",
-    headers: Optional[AnyDict] = None,
+    headers: Optional["AnyDict"] = None,
 ) -> bytes:
     data = RawMessage.encode(
         message=message,
         reply_to=reply_to,
         headers=headers,
         correlation_id=correlation_id,
     )
```

### Comparing `faststream-0.5.0rc0/faststream/redis/broker/broker.py` & `faststream-0.5.0rc1/faststream/redis/broker/broker.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,35 +25,32 @@
 from typing_extensions import Annotated, Doc, TypeAlias, override
 
 from faststream.__about__ import __version__
 from faststream.broker.message import gen_cor_id
 from faststream.exceptions import NOT_CONNECTED_YET
 from faststream.redis.broker.logging import RedisLoggingBroker
 from faststream.redis.broker.registrator import RedisRegistrator
-from faststream.redis.message import BaseMessage
 from faststream.redis.publisher.producer import RedisFastProducer
 from faststream.redis.security import parse_security
-from faststream.types import AnyDict
 
 if TYPE_CHECKING:
     from types import TracebackType
 
     from fast_depends.dependencies import Depends
     from redis.asyncio.connection import BaseParser
     from typing_extensions import TypedDict, Unpack
 
     from faststream.asyncapi import schema as asyncapi
-    from faststream.broker.message import StreamMessage
     from faststream.broker.types import (
         BrokerMiddleware,
-        CustomDecoder,
-        CustomParser,
+        CustomCallable,
     )
+    from faststream.redis.message import BaseMessage
     from faststream.security import BaseSecurity
-    from faststream.types import AnyDict, DecodedMessage, SendableMessage
+    from faststream.types import AnyDict, DecodedMessage, LoggerProto, SendableMessage
 
     class RedisInitKwargs(TypedDict, total=False):
         host: Optional[str]
         port: Union[str, int, None]
         db: Union[str, int, None]
         client_name: Optional[str]
         health_check_interval: Optional[float]
@@ -96,16 +93,15 @@
         client_name: Optional[str] = None,
         health_check_interval: float = 0,
         max_connections: Optional[int] = None,
         socket_timeout: Optional[float] = None,
         socket_connect_timeout: Optional[float] = None,
         socket_read_size: int = 65536,
         socket_keepalive: bool = False,
-        socket_keepalive_options: Optional[Mapping[int,
-                                                   Union[int, bytes]]] = None,
+        socket_keepalive_options: Optional[Mapping[int, Union[int, bytes]]] = None,
         socket_type: int = 0,
         retry_on_timeout: bool = False,
         encoding: str = "utf-8",
         encoding_errors: str = "strict",
         decode_responses: bool = False,
         parser_class: Type["BaseParser"] = DefaultParser,
         connection_class: Type["Connection"] = Connection,
@@ -114,19 +110,19 @@
         graceful_timeout: Annotated[
             Optional[float],
             Doc(
                 "Graceful shutdown timeout. Broker waits for all running subscribers completion before shut down."
             ),
         ] = 15.0,
         decoder: Annotated[
-            Optional["CustomDecoder[StreamMessage[BaseMessage]]"],
+            Optional["CustomCallable"],
             Doc("Custom decoder object."),
         ] = None,
         parser: Annotated[
-            Optional["CustomParser[BaseMessage]"],
+            Optional["CustomCallable"],
             Doc("Custom parser object."),
         ] = None,
         dependencies: Annotated[
             Iterable["Depends"],
             Doc("Dependencies to apply to all broker subscribers."),
         ] = (),
         middlewares: Annotated[
@@ -158,15 +154,15 @@
         ] = None,
         tags: Annotated[
             Optional[Iterable[Union["asyncapi.Tag", "asyncapi.TagDict"]]],
             Doc("AsyncAPI server tags."),
         ] = None,
         # logging args
         logger: Annotated[
-            Union[logging.Logger, None, object],
+            Union["LoggerProto", None, object],
             Doc("User specified logger to pass into Context and log service messages."),
         ] = Parameter.empty,
         log_level: Annotated[
             int,
             Doc("Service messages log level."),
         ] = logging.INFO,
         log_fmt: Annotated[
@@ -311,16 +307,15 @@
         url_options.update(parse_security(self.security))
         pool = ConnectionPool(
             **url_options,
             lib_name="faststream",
             lib_version=__version__,
         )
 
-        client: Redis[bytes] = Redis.from_pool(
-            pool)  # type: ignore[attr-defined]
+        client: Redis[bytes] = Redis.from_pool(pool)  # type: ignore[attr-defined]
         self._producer = RedisFastProducer(
             connection=client,
             parser=self._parser,
             decoder=self._decoder,
         )
         return client
 
@@ -342,15 +337,15 @@
             self._log(
                 f"`{handler.call_name}` waiting for messages",
                 extra=handler.get_log_context(None),
             )
             await handler.start()
 
     @property
-    def _subscriber_setup_extra(self) -> AnyDict:
+    def _subscriber_setup_extra(self) -> "AnyDict":
         return {
             "connection": self._connection,
         }
 
     @override
     async def publish(  # type: ignore[override]
         self,
@@ -456,16 +451,23 @@
 
         correlation_id = correlation_id or gen_cor_id()
 
         async with AsyncExitStack() as stack:
             wrapped_messages = [
                 await stack.enter_async_context(
                     middleware(None).publish_scope(
-                        msg, list=list, correlation_id=correlation_id,)
+                        msg,
+                        list=list,
+                        correlation_id=correlation_id,
+                    )
                 )
                 for msg in messages
                 for middleware in self._middlewares
             ] or messages
 
-            return await self._producer.publish_batch(*wrapped_messages, list=list, correlation_id=correlation_id,)
+            return await self._producer.publish_batch(
+                *wrapped_messages,
+                list=list,
+                correlation_id=correlation_id,
+            )
 
         return None
```

### Comparing `faststream-0.5.0rc0/faststream/redis/broker/logging.py` & `faststream-0.5.0rc1/faststream/redis/broker/logging.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 import logging
 from inspect import Parameter
-from typing import Any, ClassVar, Optional, Union
+from typing import TYPE_CHECKING, Any, ClassVar, Optional, Union
 
 from faststream.broker.core.usecase import BrokerUsecase
 from faststream.log.logging import get_broker_logger
-from faststream.redis.message import BaseMessage
+from faststream.redis.message import UnifyRedisDict
 
+if TYPE_CHECKING:
+    from redis.asyncio.client import Redis  # noqa: F401
 
-class RedisLoggingBroker(BrokerUsecase[BaseMessage, "Redis[bytes]"]):
+    from faststream.types import LoggerProto
+
+
+class RedisLoggingBroker(BrokerUsecase[UnifyRedisDict, "Redis[bytes]"]):
     """A class that extends the LoggingMixin class and adds additional functionality for logging Redis related information."""
 
     _max_channel_name: int
     __max_msg_id_ln: ClassVar[int] = 10
 
     def __init__(
         self,
         *args: Any,
-        logger: Union[logging.Logger, object, None] = Parameter.empty,
+        logger: Union["LoggerProto", object, None] = Parameter.empty,
         log_level: int = logging.INFO,
         log_fmt: Optional[str] = None,
         **kwargs: Any,
     ) -> None:
         super().__init__(
             *args,
             logger=logger,
```

### Comparing `faststream-0.5.0rc0/faststream/redis/publisher/asyncapi.py` & `faststream-0.5.0rc1/faststream/redis/publisher/asyncapi.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,44 @@
-from typing import Any, Dict, Iterable, Optional, Union
+from typing import TYPE_CHECKING, Any, Dict, Iterable, Optional, Union
 
 from typing_extensions import TypeAlias, override
 
 from faststream.asyncapi.schema import (
     Channel,
     ChannelBinding,
     CorrelationId,
     Message,
     Operation,
 )
 from faststream.asyncapi.schema.bindings import redis
 from faststream.asyncapi.utils import resolve_payloads
-from faststream.broker.types import BrokerMiddleware, PublisherMiddleware
 from faststream.exceptions import SetupError
-from faststream.redis.message import BaseMessage
 from faststream.redis.publisher.usecase import (
     ChannelPublisher,
     ListBatchPublisher,
     ListPublisher,
     LogicPublisher,
     StreamPublisher,
 )
 from faststream.redis.schemas import INCORRECT_SETUP_MSG, ListSub, PubSub, StreamSub
 from faststream.redis.schemas.proto import RedisAsyncAPIProtocol, validate_options
-from faststream.types import AnyDict
+
+if TYPE_CHECKING:
+    from faststream.broker.types import BrokerMiddleware, PublisherMiddleware
+    from faststream.redis.message import UnifyRedisDict
+    from faststream.types import AnyDict
 
 PublisherType: TypeAlias = Union[
     "AsyncAPIChannelPublisher",
     "AsyncAPIStreamPublisher",
     "AsyncAPIListPublisher",
     "AsyncAPIListBatchPublisher",
 ]
 
+
 class AsyncAPIPublisher(LogicPublisher, RedisAsyncAPIProtocol):
     """A class to represent a Redis publisher."""
 
     def get_schema(self) -> Dict[str, Channel]:
         payloads = self.get_payloads()
 
         return {
@@ -56,21 +59,21 @@
             )
         }
 
     @override
     @staticmethod
     def create(  # type: ignore[override]
         *,
-        channel: Union[PubSub, str, None],
-        list: Union[ListSub, str, None],
-        stream: Union[StreamSub, str, None],
-        headers: Optional[AnyDict],
+        channel: Union["PubSub", str, None],
+        list: Union["ListSub", str, None],
+        stream: Union["StreamSub", str, None],
+        headers: Optional["AnyDict"],
         reply_to: str,
-        broker_middlewares: Iterable[BrokerMiddleware[BaseMessage]],
-        middlewares: Iterable[PublisherMiddleware],
+        broker_middlewares: Iterable["BrokerMiddleware[UnifyRedisDict]"],
+        middlewares: Iterable["PublisherMiddleware"],
         # AsyncAPI args
         title_: Optional[str],
         description_: Optional[str],
         schema_: Optional[Any],
         include_in_schema: bool,
     ) -> PublisherType:
         validate_options(channel=channel, list=list, stream=stream)
@@ -140,29 +143,29 @@
 
 
 class AsyncAPIChannelPublisher(ChannelPublisher, AsyncAPIPublisher):
     def get_name(self) -> str:
         return f"{self.channel.name}:Publisher"
 
     @property
-    def channel_binding(self) -> redis.ChannelBinding:
+    def channel_binding(self) -> "redis.ChannelBinding":
         return redis.ChannelBinding(
             channel=self.channel.name,
             method="publish",
         )
 
 
 class _ListPublisherMixin(AsyncAPIPublisher):
     list: "ListSub"
 
     def get_name(self) -> str:
         return f"{self.list.name}:Publisher"
 
     @property
-    def channel_binding(self) -> redis.ChannelBinding:
+    def channel_binding(self) -> "redis.ChannelBinding":
         return redis.ChannelBinding(
             channel=self.list.name,
             method="rpush",
         )
 
 
 class AsyncAPIListPublisher(ListPublisher, _ListPublisherMixin):
@@ -174,12 +177,12 @@
 
 
 class AsyncAPIStreamPublisher(StreamPublisher, AsyncAPIPublisher):
     def get_name(self) -> str:
         return f"{self.stream.name}:Publisher"
 
     @property
-    def channel_binding(self) -> redis.ChannelBinding:
+    def channel_binding(self) -> "redis.ChannelBinding":
         return redis.ChannelBinding(
             channel=self.stream.name,
             method="xadd",
         )
```

### Comparing `faststream-0.5.0rc0/faststream/redis/publisher/producer.py` & `faststream-0.5.0rc1/faststream/redis/publisher/producer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,62 +1,64 @@
-from typing import Any, Optional
+from typing import TYPE_CHECKING, Any, Optional
 from uuid import uuid4
 
-from redis.asyncio.client import PubSub, Redis
 from typing_extensions import override
 
-from faststream.broker.message import StreamMessage
 from faststream.broker.publisher.proto import ProducerProto
-from faststream.broker.types import (
-    AsyncDecoder,
-    AsyncParser,
-    CustomDecoder,
-    CustomParser,
-)
 from faststream.broker.utils import resolve_custom_func
 from faststream.exceptions import WRONG_PUBLISH_ARGS, SetupError
-from faststream.redis.message import DATA_KEY, PubSubMessage
+from faststream.redis.message import DATA_KEY
 from faststream.redis.parser import RawMessage, RedisPubSubParser
 from faststream.redis.schemas import INCORRECT_SETUP_MSG
-from faststream.types import AnyDict, SendableMessage
 from faststream.utils.functions import timeout_scope
 
+if TYPE_CHECKING:
+    from redis.asyncio.client import PubSub, Redis
+
+    from faststream.broker.types import (
+        AsyncCallable,
+        CustomCallable,
+    )
+    from faststream.types import AnyDict, SendableMessage
+
 
 class RedisFastProducer(ProducerProto):
     """A class to represent a Redis producer."""
 
     _connection: "Redis[bytes]"
-    _decoder: AsyncDecoder[StreamMessage[PubSubMessage]]
-    _parser: AsyncParser[PubSubMessage]
+    _decoder: "AsyncCallable"
+    _parser: "AsyncCallable"
 
     def __init__(
         self,
         connection: "Redis[bytes]",
-        parser: Optional[CustomParser[PubSubMessage]],
-        decoder: Optional[CustomDecoder[StreamMessage[PubSubMessage]]],
+        parser: Optional["CustomCallable"],
+        decoder: Optional["CustomCallable"],
     ) -> None:
         self._connection = connection
         self._parser = resolve_custom_func(
-            parser,  # type: ignore[arg-type,assignment]
+            parser,
             RedisPubSubParser.parse_message,
         )
         self._decoder = resolve_custom_func(
-            decoder, RedisPubSubParser.decode_message)
+            decoder,
+            RedisPubSubParser.decode_message,
+        )
 
     @override
     async def publish(  # type: ignore[override]
         self,
-        message: SendableMessage,
+        message: "SendableMessage",
         *,
         correlation_id: str,
         channel: Optional[str] = None,
         list: Optional[str] = None,
         stream: Optional[str] = None,
         maxlen: Optional[int] = None,
-        headers: Optional[AnyDict] = None,
+        headers: Optional["AnyDict"] = None,
         reply_to: str = "",
         rpc: bool = False,
         rpc_timeout: Optional[float] = 30.0,
         raise_timeout: bool = False,
     ) -> Optional[Any]:
         if not any((channel, list, stream)):
             raise SetupError(INCORRECT_SETUP_MSG)
@@ -117,14 +119,21 @@
                 else:
                     return None
             else:
                 return await self._decoder(await self._parser(m))
 
     async def publish_batch(
         self,
-        *msgs: SendableMessage,
+        *msgs: "SendableMessage",
         list: str,
         correlation_id: str,
     ) -> None:
-        batch = (RawMessage.encode(message=msg, correlation_id=correlation_id,
-                 reply_to=None, headers=None,) for msg in msgs)
+        batch = (
+            RawMessage.encode(
+                message=msg,
+                correlation_id=correlation_id,
+                reply_to=None,
+                headers=None,
+            )
+            for msg in msgs
+        )
         await self._connection.rpush(list, *batch)
```

### Comparing `faststream-0.5.0rc0/faststream/redis/publisher/usecase.py` & `faststream-0.5.0rc1/faststream/redis/publisher/usecase.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,34 +5,35 @@
 from typing import TYPE_CHECKING, Any, Iterable, Optional
 
 from typing_extensions import Annotated, Doc, override
 
 from faststream.broker.message import gen_cor_id
 from faststream.broker.publisher.usecase import PublisherUsecase
 from faststream.exceptions import NOT_CONNECTED_YET
-from faststream.redis.message import BaseMessage
+from faststream.redis.message import UnifyRedisDict
 from faststream.redis.schemas import ListSub, PubSub, StreamSub
 
 if TYPE_CHECKING:
     from faststream.broker.types import BrokerMiddleware, PublisherMiddleware
     from faststream.redis.publisher.producer import RedisFastProducer
     from faststream.types import AnyDict, SendableMessage
 
 
-class LogicPublisher(PublisherUsecase[BaseMessage]):
+class LogicPublisher(PublisherUsecase[UnifyRedisDict]):
     """A class to represent a Redis publisher."""
+
     _producer: Optional["RedisFastProducer"]
 
     def __init__(
         self,
         *,
         reply_to: str,
         headers: Optional["AnyDict"],
         # Publisher args
-        broker_middlewares: Iterable["BrokerMiddleware[BaseMessage]"],
+        broker_middlewares: Iterable["BrokerMiddleware[UnifyRedisDict]"],
         middlewares: Iterable["PublisherMiddleware"],
         # AsyncAPI args
         schema_: Optional[Any],
         title_: Optional[str],
         description_: Optional[str],
         include_in_schema: bool,
     ) -> None:
@@ -57,19 +58,19 @@
         raise NotImplementedError()
 
 
 class ChannelPublisher(LogicPublisher):
     def __init__(
         self,
         *,
-        channel: PubSub,
+        channel: "PubSub",
         reply_to: str,
         headers: Optional["AnyDict"],
         # Regular publisher options
-        broker_middlewares: Iterable["BrokerMiddleware[BaseMessage]"],
+        broker_middlewares: Iterable["BrokerMiddleware[UnifyRedisDict]"],
         middlewares: Iterable["PublisherMiddleware"],
         # AsyncAPI options
         schema_: Optional[Any],
         title_: Optional[str],
         description_: Optional[str],
         include_in_schema: bool,
     ) -> None:
@@ -195,19 +196,19 @@
         return None
 
 
 class ListPublisher(LogicPublisher):
     def __init__(
         self,
         *,
-        list: ListSub,
+        list: "ListSub",
         reply_to: str,
         headers: Optional["AnyDict"],
         # Regular publisher options
-        broker_middlewares: Iterable["BrokerMiddleware[BaseMessage]"],
+        broker_middlewares: Iterable["BrokerMiddleware[UnifyRedisDict]"],
         middlewares: Iterable["PublisherMiddleware"],
         # AsyncAPI options
         schema_: Optional[Any],
         title_: Optional[str],
         description_: Optional[str],
         include_in_schema: bool,
     ) -> None:
@@ -344,17 +345,15 @@
         list: Annotated[
             Optional[str],
             Doc("Redis List object name to send message."),
         ] = None,
         *,
         correlation_id: Annotated[
             Optional[str],
-            Doc(
-                "Has no real effect. Option to be compatible with original protocol."
-            ),
+            Doc("Has no real effect. Option to be compatible with original protocol."),
         ] = None,
         # publisher specific
         _extra_middlewares: Annotated[
             Iterable["PublisherMiddleware"],
             Doc("Extra middlewares to wrap publishing process."),
         ] = (),
     ) -> None:
@@ -362,15 +361,19 @@
 
         list_sub = ListSub.validate(list or self.list)
         correlation_id = correlation_id or gen_cor_id()
 
         async with AsyncExitStack() as stack:
             wrapped_messages = [
                 await stack.enter_async_context(
-                    middleware(msg, list=list_sub, correlation_id=correlation_id,)
+                    middleware(
+                        msg,
+                        list=list_sub,
+                        correlation_id=correlation_id,
+                    )
                 )
                 for msg in message
                 for middleware in chain(
                     _extra_middlewares
                     or (m(None).publish_scope for m in self._broker_middlewares),
                     self._middlewares,
                 )
@@ -385,19 +388,19 @@
         return None
 
 
 class StreamPublisher(LogicPublisher):
     def __init__(
         self,
         *,
-        stream: StreamSub,
+        stream: "StreamSub",
         reply_to: str,
         headers: Optional["AnyDict"],
         # Regular publisher options
-        broker_middlewares: Iterable["BrokerMiddleware[BaseMessage]"],
+        broker_middlewares: Iterable["BrokerMiddleware[UnifyRedisDict]"],
         middlewares: Iterable["PublisherMiddleware"],
         # AsyncAPI options
         schema_: Optional[Any],
         title_: Optional[str],
         description_: Optional[str],
         include_in_schema: bool,
     ) -> None:
@@ -415,19 +418,15 @@
         self.stream = stream
 
     def __hash__(self) -> int:
         return hash(f"publisher:stream:{self.stream.name}")
 
     @property
     def subscriber_property(self) -> "AnyDict":
-        return {
-            "channel": None,
-            "list": None,
-            "stream": self.stream
-        }
+        return {"channel": None, "list": None, "stream": self.stream}
 
     def add_prefix(self, prefix: str) -> None:
         stream_sub = deepcopy(self.stream)
         stream_sub.name = "".join((prefix, stream_sub.name))
         self.stream = stream_sub
 
     @override
```

### Comparing `faststream-0.5.0rc0/faststream/redis/schemas/list_sub.py` & `faststream-0.5.0rc1/faststream/redis/schemas/list_sub.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/faststream/redis/schemas/proto.py` & `faststream-0.5.0rc1/faststream/redis/schemas/proto.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,25 +8,22 @@
     from faststream.asyncapi.schema.bindings import redis
     from faststream.redis.schemas import ListSub, PubSub, StreamSub
 
 
 class RedisAsyncAPIProtocol(AsyncAPIOperation):
     @property
     @abstractmethod
-    def channel_binding(self) -> "redis.ChannelBinding":
-        ...
+    def channel_binding(self) -> "redis.ChannelBinding": ...
 
     @abstractmethod
-    def get_payloads(self) -> Any:
-        ...
+    def get_payloads(self) -> Any: ...
 
     @staticmethod
     @abstractmethod
-    def create() -> Any:
-        ...
+    def create() -> Any: ...
 
 
 def validate_options(
     *,
     channel: Union["PubSub", str, None],
     list: Union["ListSub", str, None],
     stream: Union["StreamSub", str, None],
```

### Comparing `faststream-0.5.0rc0/faststream/redis/schemas/pub_sub.py` & `faststream-0.5.0rc1/faststream/redis/schemas/pub_sub.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/faststream/redis/schemas/stream_sub.py` & `faststream-0.5.0rc1/faststream/redis/schemas/stream_sub.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/faststream/redis/subscriber/asyncapi.py` & `faststream-0.5.0rc1/faststream/redis/subscriber/asyncapi.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,47 +1,48 @@
-from typing import Dict, Iterable, Optional, Union
+from typing import TYPE_CHECKING, Dict, Iterable, Optional, Union
 
-from fast_depends.dependencies import Depends
 from typing_extensions import TypeAlias, override
 
 from faststream.asyncapi.schema import (
     Channel,
     ChannelBinding,
     CorrelationId,
     Message,
     Operation,
 )
 from faststream.asyncapi.schema.bindings import redis
 from faststream.asyncapi.utils import resolve_payloads
-from faststream.broker.types import (
-    BrokerMiddleware,
-)
 from faststream.exceptions import SetupError
-from faststream.redis.message import BaseMessage
 from faststream.redis.schemas import INCORRECT_SETUP_MSG, ListSub, PubSub, StreamSub
 from faststream.redis.schemas.proto import RedisAsyncAPIProtocol, validate_options
 from faststream.redis.subscriber.usecase import (
     BatchListSubscriber,
     BatchStreamSubscriber,
     ChannelSubscriber,
     ListSubscriber,
     LogicSubscriber,
     StreamSubscriber,
 )
 
-HandlerType: TypeAlias = Union[
+if TYPE_CHECKING:
+    from fast_depends.dependencies import Depends
+
+    from faststream.broker.types import BrokerMiddleware
+    from faststream.redis.message import UnifyRedisDict
+
+SubsciberType: TypeAlias = Union[
     "AsyncAPIChannelSubscriber",
     "AsyncAPIStreamBatchSubscriber",
     "AsyncAPIStreamSubscriber",
     "AsyncAPIListBatchSubscriber",
     "AsyncAPIListSubscriber",
 ]
 
 
-class AsyncAPISubscriber(LogicSubscriber[BaseMessage], RedisAsyncAPIProtocol):
+class AsyncAPISubscriber(LogicSubscriber, RedisAsyncAPIProtocol):
     """A class to represent a Redis handler."""
 
     def get_schema(self) -> Dict[str, Channel]:
         payloads = self.get_payloads()
 
         return {
             self.name: Channel(
@@ -61,27 +62,27 @@
             )
         }
 
     @override
     @staticmethod
     def create(  # type: ignore[override]
         *,
-        channel: Union[PubSub, str, None],
-        list: Union[ListSub, str, None],
-        stream: Union[StreamSub, str, None],
+        channel: Union["PubSub", str, None],
+        list: Union["ListSub", str, None],
+        stream: Union["StreamSub", str, None],
         # Subscriber args
         no_ack: bool = False,
         retry: bool = False,
-        broker_dependencies: Iterable[Depends] = (),
-        broker_middlewares: Iterable[BrokerMiddleware[BaseMessage]] = (),
+        broker_dependencies: Iterable["Depends"] = (),
+        broker_middlewares: Iterable["BrokerMiddleware[UnifyRedisDict]"] = (),
         # AsyncAPI args
         title_: Optional[str] = None,
         description_: Optional[str] = None,
         include_in_schema: bool = True,
-    ) -> HandlerType:
+    ) -> SubsciberType:
         validate_options(channel=channel, list=list, stream=stream)
 
         if (channel_sub := PubSub.validate(channel)) is not None:
             return AsyncAPIChannelSubscriber(
                 channel=channel_sub,
                 # basic args
                 no_ack=no_ack,
@@ -155,29 +156,29 @@
 
 
 class AsyncAPIChannelSubscriber(ChannelSubscriber, AsyncAPISubscriber):
     def get_name(self) -> str:
         return f"{self.channel.name}:{self.call_name}"
 
     @property
-    def channel_binding(self) -> redis.ChannelBinding:
+    def channel_binding(self) -> "redis.ChannelBinding":
         return redis.ChannelBinding(
             channel=self.channel.name,
             method="psubscribe" if self.channel.pattern else "subscribe",
         )
 
 
 class _StreamSubscriberMixin(AsyncAPISubscriber):
     stream_sub: StreamSub
 
     def get_name(self) -> str:
         return f"{self.stream_sub.name}:{self.call_name}"
 
     @property
-    def channel_binding(self) -> redis.ChannelBinding:
+    def channel_binding(self) -> "redis.ChannelBinding":
         return redis.ChannelBinding(
             channel=self.stream_sub.name,
             group_name=self.stream_sub.group,
             consumer_name=self.stream_sub.consumer,
             method="xreadgroup" if self.stream_sub.group else "xread",
         )
 
@@ -193,15 +194,15 @@
 class _ListSubscriberMixin(AsyncAPISubscriber):
     list_sub: ListSub
 
     def get_name(self) -> str:
         return f"{self.list_sub.name}:{self.call_name}"
 
     @property
-    def channel_binding(self) -> redis.ChannelBinding:
+    def channel_binding(self) -> "redis.ChannelBinding":
         return redis.ChannelBinding(
             channel=self.list_sub.name,
             method="lpop",
         )
 
 
 class AsyncAPIListSubscriber(ListSubscriber, _ListSubscriberMixin):
```

### Comparing `faststream-0.5.0rc0/faststream/redis/subscriber/usecase.py` & `faststream-0.5.0rc1/faststream/redis/subscriber/usecase.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,82 +6,77 @@
     TYPE_CHECKING,
     Any,
     Awaitable,
     Callable,
     Dict,
     Iterable,
     List,
-    Mapping,
     Optional,
     Sequence,
     Tuple,
-    TypeVar,
 )
 
 import anyio
-from fast_depends.dependencies import Depends
 from redis.asyncio.client import PubSub as RPubSub
 from redis.asyncio.client import Redis
 from redis.exceptions import ResponseError
-from typing_extensions import override
+from typing_extensions import TypeAlias, override
 
 from faststream.broker.publisher.fake import FakePublisher
-from faststream.broker.publisher.proto import ProducerProto
 from faststream.broker.subscriber.usecase import SubscriberUsecase
-from faststream.broker.types import (
-    AsyncDecoder,
-    AsyncParser,
-    BrokerMiddleware,
-    CustomDecoder,
-    CustomParser,
-)
 from faststream.redis.message import (
     BatchListMessage,
     BatchStreamMessage,
     DefaultListMessage,
     DefaultStreamMessage,
-    ListMessage,
     PubSubMessage,
-    StreamMessage,
+    UnifyRedisDict,
 )
 from faststream.redis.parser import (
     RedisBatchListParser,
     RedisBatchStreamParser,
     RedisListParser,
     RedisPubSubParser,
     RedisStreamParser,
 )
 from faststream.redis.schemas import ListSub, PubSub, StreamSub
-from faststream.types import AnyDict, LoggerProto
 
 if TYPE_CHECKING:
     from fast_depends.dependencies import Depends
 
     from faststream.broker.message import StreamMessage as BrokerStreamMessage
+    from faststream.broker.publisher.proto import ProducerProto
+    from faststream.broker.types import (
+        AsyncCallable,
+        BrokerMiddleware,
+        CustomCallable,
+    )
+    from faststream.types import AnyDict, LoggerProto
 
 
-MsgType = TypeVar("MsgType", bound=Mapping[str, Any])
+TopicName: TypeAlias = bytes
+Offset: TypeAlias = bytes
 
 
-class LogicSubscriber(ABC, SubscriberUsecase[MsgType]):
+class LogicSubscriber(ABC, SubscriberUsecase[UnifyRedisDict]):
     """A class to represent a Redis handler."""
 
     _client: Optional["Redis[bytes]"]
 
     def __init__(
         self,
         *,
-        default_parser: "AsyncParser[MsgType]",
-        default_decoder: "AsyncDecoder[BrokerStreamMessage[MsgType]]",
+        default_parser: "AsyncCallable",
+        default_decoder: "AsyncCallable",
         # Subscriber args
         no_ack: bool,
         retry: bool,
-        broker_dependencies: Iterable[Depends],
-        broker_middlewares: Iterable[BrokerMiddleware[MsgType]],
-        # AsyncAPI MsgType
+        broker_dependencies: Iterable["Depends"],
+        broker_middlewares: Iterable["BrokerMiddleware[UnifyRedisDict]"],
+        # AsyncAPI args
         title_: Optional[str],
         description_: Optional[str],
         include_in_schema: bool,
     ) -> None:
         super().__init__(
             default_parser=default_parser,
             default_decoder=default_decoder,
@@ -106,16 +101,16 @@
         connection: Optional["Redis[bytes]"],
         # basic args
         logger: Optional["LoggerProto"],
         producer: Optional["ProducerProto"],
         graceful_timeout: Optional[float],
         extra_context: Optional["AnyDict"],
         # broker options
-        broker_parser: Optional["CustomParser[MsgType]"],
-        broker_decoder: Optional["CustomDecoder[BrokerStreamMessage[MsgType]]"],
+        broker_parser: Optional["CustomCallable"],
+        broker_decoder: Optional["CustomCallable"],
         # dependant args
         apply_types: bool,
         is_validate: bool,
         _get_dependant: Optional[Callable[..., Any]],
     ) -> None:
         self._client = connection
 
@@ -128,15 +123,15 @@
             broker_decoder=broker_decoder,
             apply_types=apply_types,
             is_validate=is_validate,
             _get_dependant=_get_dependant,
         )
 
     def _make_response_publisher(
-        self, message: "BrokerStreamMessage[MsgType]"
+        self, message: "BrokerStreamMessage[UnifyRedisDict]"
     ) -> Sequence[FakePublisher]:
         if not message.reply_to or self._producer is None:
             return ()
 
         return (
             FakePublisher(
                 self._producer.publish,
@@ -197,27 +192,27 @@
     ) -> Dict[str, str]:
         return {
             "channel": channel,
             "message_id": getattr(message, "message_id", ""),
         }
 
 
-class ChannelSubscriber(LogicSubscriber[PubSubMessage]):
+class ChannelSubscriber(LogicSubscriber):
     subscription: Optional[RPubSub]
 
     def __init__(
         self,
         *,
-        channel: PubSub,
+        channel: "PubSub",
         # Subscriber args
         no_ack: bool,
         retry: bool,
-        broker_dependencies: Iterable[Depends],
-        broker_middlewares: Iterable[BrokerMiddleware[PubSubMessage]],
-        # AsyncAPI MsgType
+        broker_dependencies: Iterable["Depends"],
+        broker_middlewares: Iterable["BrokerMiddleware[UnifyRedisDict]"],
+        # AsyncAPI args
         title_: Optional[str],
         description_: Optional[str],
         include_in_schema: bool,
     ) -> None:
         super().__init__(
             default_parser=RedisPubSubParser.parse_message,
             default_decoder=RedisPubSubParser.decode_message,
@@ -277,38 +272,35 @@
         if raw_msg:
             msg = PubSubMessage(
                 type=raw_msg["type"],
                 data=raw_msg["data"],
                 channel=raw_msg["channel"].decode(),
                 pattern=raw_msg["pattern"],
             )
-            await self.consume(msg)
+            await self.consume(msg)  # type: ignore[arg-type]
 
     def add_prefix(self, prefix: str) -> None:
         new_ch = deepcopy(self.channel)
         new_ch.name = "".join((prefix, new_ch.name))
         self.channel = new_ch
 
 
-ListMsgType = TypeVar("ListMsgType", bound=ListMessage)
-
-
-class _ListHandlerMixin(LogicSubscriber[ListMsgType]):
+class _ListHandlerMixin(LogicSubscriber):
     def __init__(
         self,
         *,
         list: ListSub,
-        default_parser: "AsyncParser[ListMsgType]",
-        default_decoder: "AsyncDecoder[BrokerStreamMessage[ListMsgType]]",
+        default_parser: "AsyncCallable",
+        default_decoder: "AsyncCallable",
         # Subscriber args
         no_ack: bool,
         retry: bool,
-        broker_dependencies: Iterable[Depends],
-        broker_middlewares: Iterable[BrokerMiddleware[ListMsgType]],
-        # AsyncAPI MsgType
+        broker_dependencies: Iterable["Depends"],
+        broker_middlewares: Iterable["BrokerMiddleware[UnifyRedisDict]"],
+        # AsyncAPI args
         title_: Optional[str],
         description_: Optional[str],
         include_in_schema: bool,
     ) -> None:
         super().__init__(
             default_parser=default_parser,
             default_decoder=default_decoder,
@@ -338,15 +330,15 @@
         )
 
     @override
     async def _consume(  # type: ignore[override]
         self,
         client: "Redis[bytes]",
         *,
-        start_signal: anyio.Event,
+        start_signal: "anyio.Event",
     ) -> None:
         start_signal.set()
         await super()._consume(client, start_signal=start_signal)
 
     @override
     async def start(self) -> None:
         assert self._client, "You should setup subscriber at first."  # nosec B101
@@ -354,25 +346,25 @@
 
     def add_prefix(self, prefix: str) -> None:
         new_list = deepcopy(self.list_sub)
         new_list.name = "".join((prefix, new_list.name))
         self.list_sub = new_list
 
 
-class ListSubscriber(_ListHandlerMixin[DefaultListMessage]):
+class ListSubscriber(_ListHandlerMixin):
     def __init__(
         self,
         *,
         list: ListSub,
         # Subscriber args
         no_ack: bool,
         retry: bool,
-        broker_dependencies: Iterable[Depends],
-        broker_middlewares: Iterable[BrokerMiddleware[DefaultListMessage]],
-        # AsyncAPI MsgType
+        broker_dependencies: Iterable["Depends"],
+        broker_middlewares: Iterable["BrokerMiddleware[UnifyRedisDict]"],
+        # AsyncAPI args
         title_: Optional[str],
         description_: Optional[str],
         include_in_schema: bool,
     ) -> None:
         super().__init__(
             list=list,
             default_parser=RedisListParser.parse_message,
@@ -394,31 +386,31 @@
         if raw_msg:
             message = DefaultListMessage(
                 type="list",
                 data=raw_msg,
                 channel=self.list_sub.name,
             )
 
-            await self.consume(message)
+            await self.consume(message)  # type: ignore[arg-type]
 
         else:
             await anyio.sleep(self.list_sub.polling_interval)
 
 
-class BatchListSubscriber(_ListHandlerMixin[BatchListMessage]):
+class BatchListSubscriber(_ListHandlerMixin):
     def __init__(
         self,
         *,
         list: ListSub,
         # Subscriber args
         no_ack: bool,
         retry: bool,
-        broker_dependencies: Iterable[Depends],
-        broker_middlewares: Iterable[BrokerMiddleware[BatchListMessage]],
-        # AsyncAPI MsgType
+        broker_dependencies: Iterable["Depends"],
+        broker_middlewares: Iterable["BrokerMiddleware[UnifyRedisDict]"],
+        # AsyncAPI args
         title_: Optional[str],
         description_: Optional[str],
         include_in_schema: bool,
     ) -> None:
         super().__init__(
             list=list,
             default_parser=RedisBatchListParser.parse_message,
@@ -443,36 +435,33 @@
         if raw_msgs:
             msg = BatchListMessage(
                 type="blist",
                 channel=self.list_sub.name,
                 data=raw_msgs,
             )
 
-            await self.consume(msg)
+            await self.consume(msg)  # type: ignore[arg-type]
 
         else:
             await anyio.sleep(self.list_sub.polling_interval)
 
 
-StreamMsgType = TypeVar("StreamMsgType", bound=StreamMessage)
-
-
-class _StreamHandlerMixin(LogicSubscriber[StreamMsgType]):
+class _StreamHandlerMixin(LogicSubscriber):
     def __init__(
         self,
         *,
         stream: StreamSub,
-        default_parser: "AsyncParser[StreamMsgType]",
-        default_decoder: "AsyncDecoder[BrokerStreamMessage[StreamMsgType]]",
+        default_parser: "AsyncCallable",
+        default_decoder: "AsyncCallable",
         # Subscriber args
         no_ack: bool,
         retry: bool,
-        broker_dependencies: Iterable[Depends],
-        broker_middlewares: Iterable[BrokerMiddleware[StreamMsgType]],
-        # AsyncAPI MsgType
+        broker_dependencies: Iterable["Depends"],
+        broker_middlewares: Iterable["BrokerMiddleware[UnifyRedisDict]"],
+        # AsyncAPI args
         title_: Optional[str],
         description_: Optional[str],
         include_in_schema: bool,
     ) -> None:
         super().__init__(
             default_parser=default_parser,
             default_decoder=default_decoder,
@@ -510,61 +499,115 @@
         self.extra_watcher_options.update(
             redis=client,
             group=self.stream_sub.group,
         )
 
         stream = self.stream_sub
 
+        read: Callable[
+            [str],
+            Awaitable[
+                Tuple[
+                    Tuple[
+                        TopicName,
+                        Tuple[
+                            Tuple[
+                                Offset,
+                                Dict[bytes, bytes],
+                            ],
+                            ...,
+                        ],
+                    ],
+                    ...,
+                ],
+            ],
+        ]
+
         if stream.group and stream.consumer:
             try:
                 await client.xgroup_create(
                     name=stream.name,
                     id=self.last_id,
                     groupname=stream.group,
                     mkstream=True,
                 )
             except ResponseError as e:
                 if "already exists" not in str(e):
                     raise e
 
-            read = lambda _: client.xreadgroup(
-                groupname=stream.group,
-                consumername=stream.consumer,
-                streams={stream.name: ">"},
-                count=stream.max_records,
-                block=stream.polling_interval,
-                noack=stream.no_ack,
-            )
+            def read(
+                _: str,
+            ) -> Awaitable[
+                Tuple[
+                    Tuple[
+                        TopicName,
+                        Tuple[
+                            Tuple[
+                                Offset,
+                                Dict[bytes, bytes],
+                            ],
+                            ...,
+                        ],
+                    ],
+                    ...,
+                ],
+            ]:
+                return client.xreadgroup(
+                    groupname=stream.group,
+                    consumername=stream.consumer,
+                    streams={stream.name: ">"},
+                    count=stream.max_records,
+                    block=stream.polling_interval,
+                    noack=stream.no_ack,
+                )
 
         else:
-            read = lambda last_id: client.xread(
-                {stream.name: last_id},
-                block=stream.polling_interval,
-                count=stream.max_records,
-            )
+
+            def read(
+                last_id: str,
+            ) -> Awaitable[
+                Tuple[
+                    Tuple[
+                        TopicName,
+                        Tuple[
+                            Tuple[
+                                Offset,
+                                Dict[bytes, bytes],
+                            ],
+                            ...,
+                        ],
+                    ],
+                    ...,
+                ],
+            ]:
+                return client.xread(
+                    {stream.name: last_id},
+                    block=stream.polling_interval,
+                    count=stream.max_records,
+                )
 
         await super().start(read)
 
     def add_prefix(self, prefix: str) -> None:
         new_stream = deepcopy(self.stream_sub)
         new_stream.name = "".join((prefix, new_stream.name))
         self.stream_sub = new_stream
 
 
-class StreamSubscriber(_StreamHandlerMixin[DefaultStreamMessage]):
+class StreamSubscriber(_StreamHandlerMixin):
     def __init__(
         self,
         *,
         stream: StreamSub,
         # Subscriber args
         no_ack: bool,
         retry: bool,
-        broker_dependencies: Iterable[Depends],
-        broker_middlewares: Iterable[BrokerMiddleware[DefaultStreamMessage]],
-        # AsyncAPI MsgType
+        broker_dependencies: Iterable["Depends"],
+        broker_middlewares: Iterable["BrokerMiddleware[UnifyRedisDict]"],
+        # AsyncAPI args
         title_: Optional[str],
         description_: Optional[str],
         include_in_schema: bool,
     ) -> None:
         super().__init__(
             stream=stream,
             default_parser=RedisStreamParser.parse_message,
@@ -581,15 +624,27 @@
         )
 
     async def _get_msgs(
         self,
         read: Callable[
             [str],
             Awaitable[
-                Tuple[Tuple[bytes, Tuple[Tuple[bytes, Dict[bytes, bytes]], ...]], ...],
+                Tuple[
+                    Tuple[
+                        TopicName,
+                        Tuple[
+                            Tuple[
+                                Offset,
+                                Dict[bytes, bytes],
+                            ],
+                            ...,
+                        ],
+                    ],
+                    ...,
+                ],
             ],
         ],
     ) -> None:
         for stream_name, msgs in await read(self.last_id):
             if msgs:
                 self.last_id = msgs[-1][0].decode()
 
@@ -597,28 +652,28 @@
                     msg = DefaultStreamMessage(
                         type="stream",
                         channel=stream_name.decode(),
                         message_ids=[message_id],
                         data=raw_msg,
                     )
 
-                    await self.consume(msg)
+                    await self.consume(msg)  # type: ignore[arg-type]
 
 
-class BatchStreamSubscriber(_StreamHandlerMixin[BatchStreamMessage]):
+class BatchStreamSubscriber(_StreamHandlerMixin):
     def __init__(
         self,
         *,
         stream: StreamSub,
         # Subscriber args
         no_ack: bool,
         retry: bool,
-        broker_dependencies: Iterable[Depends],
-        broker_middlewares: Iterable[BrokerMiddleware[BatchStreamMessage]],
-        # AsyncAPI MsgType
+        broker_dependencies: Iterable["Depends"],
+        broker_middlewares: Iterable["BrokerMiddleware[UnifyRedisDict]"],
+        # AsyncAPI args
         title_: Optional[str],
         description_: Optional[str],
         include_in_schema: bool,
     ) -> None:
         super().__init__(
             stream=stream,
             default_parser=RedisBatchStreamParser.parse_message,
@@ -656,8 +711,8 @@
                 msg = BatchStreamMessage(
                     type="bstream",
                     channel=stream_name.decode(),
                     data=data,
                     message_ids=ids,
                 )
 
-                await self.consume(msg)
+                await self.consume(msg)  # type: ignore[arg-type]
```

### Comparing `faststream-0.5.0rc0/faststream/testing/app.py` & `faststream-0.5.0rc1/faststream/testing/app.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 from contextlib import ExitStack
 from functools import partial
-from types import TracebackType
-from typing import Any, Dict, Optional, Type, TypeVar
+from typing import TYPE_CHECKING, Any, Dict, Optional, Type, TypeVar
 
 from anyio.from_thread import start_blocking_portal
 
-from faststream.app import FastStream
 from faststream.broker.core.usecase import BrokerUsecase
-from faststream.types import SettingField
+
+if TYPE_CHECKING:
+    from types import TracebackType
+
+    from faststream.app import FastStream
+    from faststream.types import SettingField
 
 Broker = TypeVar("Broker", bound=BrokerUsecase[Any, Any])
 
 
 class TestApp:
     """A class to represent a test application."""
 
     __test__ = False
 
-    app: FastStream
-    _extra_options: Dict[str, SettingField]
+    app: "FastStream"
+    _extra_options: Dict[str, "SettingField"]
 
     def __init__(
         self,
-        app: FastStream,
-        run_extra_options: Optional[Dict[str, SettingField]] = None,
+        app: "FastStream",
+        run_extra_options: Optional[Dict[str, "SettingField"]] = None,
     ) -> None:
         self.app = app
         self._extra_options = run_extra_options or {}
 
-    def __enter__(self) -> FastStream:
+    def __enter__(self) -> "FastStream":
         with ExitStack() as stack:
             portal = stack.enter_context(start_blocking_portal())
 
             lifespan_context = self.app.lifespan_context(**self._extra_options)
             stack.enter_context(portal.wrap_async_context_manager(lifespan_context))
             portal.call(partial(self.app.start, **self._extra_options))
 
@@ -44,26 +47,26 @@
 
         return self.app
 
     def __exit__(
         self,
         exc_type: Optional[Type[BaseException]] = None,
         exc_val: Optional[BaseException] = None,
-        exc_tb: Optional[TracebackType] = None,
+        exc_tb: Optional["TracebackType"] = None,
     ) -> None:
         self.exit_stack.close()
 
-    async def __aenter__(self) -> FastStream:
+    async def __aenter__(self) -> "FastStream":
         self.lifespan_scope = self.app.lifespan_context(**self._extra_options)
         await self.lifespan_scope.__aenter__()
         await self.app.start(**self._extra_options)
         return self.app
 
     async def __aexit__(
         self,
         exc_type: Optional[Type[BaseException]] = None,
         exc_val: Optional[BaseException] = None,
-        exc_tb: Optional[TracebackType] = None,
+        exc_tb: Optional["TracebackType"] = None,
     ) -> None:
         """Exit the asynchronous context manager."""
         await self.app.stop()
         await self.lifespan_scope.__aexit__(exc_type, exc_val, exc_tb)
```

### Comparing `faststream-0.5.0rc0/faststream/testing/broker.py` & `faststream-0.5.0rc1/faststream/testing/broker.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,38 @@
 import warnings
 from abc import abstractmethod
 from contextlib import asynccontextmanager
 from functools import partial
-from types import MethodType, TracebackType
-from typing import Any, AsyncGenerator, Generic, Optional, Type, TypeVar
+from types import MethodType
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    AsyncGenerator,
+    Generic,
+    Optional,
+    Tuple,
+    Type,
+    TypeVar,
+)
 from unittest.mock import AsyncMock, MagicMock
 
 from faststream.broker.core.usecase import BrokerUsecase
 from faststream.broker.middlewares.logging import CriticalLogMiddleware
-from faststream.broker.subscriber.proto import SubscriberProto
 from faststream.broker.wrapper.call import HandlerCallWrapper
 from faststream.testing.app import TestApp
 from faststream.utils.ast import is_contains_context_name
 from faststream.utils.functions import timeout_scope
 
+if TYPE_CHECKING:
+    from types import TracebackType
+
+    from faststream.broker.subscriber.proto import SubscriberProto
+    from faststream.broker.types import BrokerMiddleware
+
+
 Broker = TypeVar("Broker", bound=BrokerUsecase[Any, Any])
 
 
 class TestBroker(Generic[Broker]):
     """A class to represent a test broker."""
 
     # This is set so pytest ignores this class
@@ -38,15 +53,15 @@
                     self.__class__.__name__,
                     TestApp.__name__,
                 )
             except Exception:  # pragma: no cover
                 warnings.warn(
                     (
                         "\nError `{e!r}` occurred at `{self.__class__.__name__}` AST parsing."
-                        "\n`connect_only` is setted to `False` by default."
+                        "\n`connect_only` is set to `False` by default."
                     ),
                     category=RuntimeWarning,
                     stacklevel=1,
                 )
 
                 connect_only = False
 
@@ -70,16 +85,16 @@
 
         self._ctx = self._create_ctx()
         return await self._ctx.__aenter__()
 
     async def __aexit__(self, *args: Any) -> None:
         await self._ctx.__aexit__(*args)
 
-        middlewares = (
-            CriticalLogMiddleware(
+        middlewares: Tuple["BrokerMiddleware[Any]", ...] = (
+            CriticalLogMiddleware(  # type: ignore[arg-type]
                 logger=self.broker.logger,
                 log_level=self.broker._msg_log_level,
             ),
             *self.broker._middlewares,
         )
 
         self.broker._middlewares = middlewares
@@ -114,47 +129,47 @@
     @classmethod
     def _fake_start(cls, broker: Broker, *args: Any, **kwargs: Any) -> None:
         broker.setup()
 
         patch_broker_calls(broker)
 
         for key, p in broker._publishers.items():
-            if p._fake_handler:
+            if getattr(p, "_fake_handler", None):
                 continue
 
             handler = broker._subscribers.get(key)
 
             if handler is not None:
                 mock = MagicMock()
-                p.set_test(mock=mock, with_fake=False)
+                p.set_test(mock=mock, with_fake=False)  # type: ignore[attr-defined]
                 for h in handler.calls:
                     h.handler.set_test()
                     assert h.handler.mock  # nosec B101
                     h.handler.mock.side_effect = mock
 
             else:
                 f = cls.create_publisher_fake_subscriber(broker, p)
                 f.set_test()
                 assert f.mock  # nosec B101
-                p.set_test(mock=f.mock, with_fake=True)
+                p.set_test(mock=f.mock, with_fake=True)  # type: ignore[attr-defined]
 
         for handler in broker._subscribers.values():
             handler.running = True
 
     @classmethod
     def _fake_close(
         cls,
         broker: Broker,
         exc_type: Optional[Type[BaseException]] = None,
         exc_val: Optional[BaseException] = None,
-        exc_tb: Optional[TracebackType] = None,
+        exc_tb: Optional["TracebackType"] = None,
     ) -> None:
         for p in broker._publishers.values():
-            if p._fake_handler:
-                p.reset_test()
+            if getattr(p, "_fake_handler", None):
+                p.reset_test()  # type: ignore[attr-defined]
                 cls.remove_publisher_fake_subscriber(broker, p)
 
         for h in broker._subscribers.values():
             h.running = False
             for call in h.calls:
                 call.handler.reset_test()
 
@@ -172,25 +187,25 @@
 
     @staticmethod
     @abstractmethod
     async def _fake_connect(broker: Broker, *args: Any, **kwargs: Any) -> None:
         raise NotImplementedError()
 
 
-def patch_broker_calls(broker: BrokerUsecase[Any, Any]) -> None:
+def patch_broker_calls(broker: "BrokerUsecase[Any, Any]") -> None:
     """Patch broker calls."""
     broker._abc_start()
 
     for handler in broker._subscribers.values():
         for h in handler.calls:
             h.handler.set_test()
 
 
 async def call_handler(
-    handler: SubscriberProto[Any],
+    handler: "SubscriberProto[Any]",
     message: Any,
     rpc: bool = False,
     rpc_timeout: Optional[float] = 30.0,
     raise_timeout: bool = False,
 ) -> Any:
     """Asynchronously call a handler function."""
     with timeout_scope(rpc_timeout, raise_timeout):
```

### Comparing `faststream-0.5.0rc0/faststream/utils/ast.py` & `faststream-0.5.0rc1/faststream/utils/ast.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/faststream/utils/classes.py` & `faststream-0.5.0rc1/faststream/utils/classes.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/faststream/utils/data.py` & `faststream-0.5.0rc1/faststream/utils/data.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/faststream/utils/functions.py` & `faststream-0.5.0rc1/faststream/utils/functions.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,21 +26,21 @@
     "drop_response_type",
 )
 
 
 @overload
 def to_async(
     func: Callable[F_Spec, Awaitable[F_Return]],
-) -> Callable[F_Spec, Awaitable[F_Return]]:
-    ...
+) -> Callable[F_Spec, Awaitable[F_Return]]: ...
 
 
 @overload
-def to_async(func: Callable[F_Spec, F_Return]) -> Callable[F_Spec, Awaitable[F_Return]]:
-    ...
+def to_async(
+    func: Callable[F_Spec, F_Return],
+) -> Callable[F_Spec, Awaitable[F_Return]]: ...
 
 
 def to_async(
     func: Union[
         Callable[F_Spec, F_Return],
         Callable[F_Spec, Awaitable[F_Return]],
     ],
```

### Comparing `faststream-0.5.0rc0/faststream/utils/no_cast.py` & `faststream-0.5.0rc1/faststream/utils/no_cast.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/faststream/utils/path.py` & `faststream-0.5.0rc1/faststream/utils/path.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/faststream/utils/context/builders.py` & `faststream-0.5.0rc1/faststream/utils/context/builders.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/faststream/utils/context/repository.py` & `faststream-0.5.0rc1/faststream/utils/context/repository.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/faststream/utils/context/types.py` & `faststream-0.5.0rc1/faststream/utils/context/types.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/scripts/build-docs-pre-commit.sh` & `faststream-0.5.0rc1/scripts/build-docs-pre-commit.sh`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/scripts/lint-pre-commit.sh` & `faststream-0.5.0rc1/scripts/lint-pre-commit.sh`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/scripts/set_variables.sh` & `faststream-0.5.0rc1/scripts/set_variables.sh`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/scripts/static-pre-commit.sh` & `faststream-0.5.0rc1/scripts/static-pre-commit.sh`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/LICENSE` & `faststream-0.5.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/README.md` & `faststream-0.5.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `faststream-0.5.0rc0/pyproject.toml` & `faststream-0.5.0rc1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -65,50 +65,53 @@
 # public distributions
 rabbit = ["aio-pika>=9,<10"]
 
 kafka = ["aiokafka>=0.9,<0.11"]
 
 confluent = ["confluent-kafka>=2,<3"]
 
-nats = [
-    "nats-py>=2.3.1,<=3.0.0"
-]
+nats = ["nats-py>=2.3.1,<=3.0.0"]
 
 redis = ["redis>=5.0.0,<6.0.0"]
 
 # dev dependencies
 devdocs = [
-    "mkdocs-material==9.5.13",
-    "mkdocs-static-i18n==1.2.0",
+    "mkdocs-material==9.5.16",
+    "mkdocs-static-i18n==1.2.2",
     "mdx-include==1.4.2",
     "mkdocstrings[python]==0.24.1",
     "mkdocs-literate-nav==0.6.1",
     "mkdocs-git-revision-date-localized-plugin==1.2.4",
-    "mike==2.0.0",  # versioning
+    "mike==2.0.0",                                      # versioning
     "mkdocs-minify-plugin==0.8.0",
-    "mkdocs-macros-plugin==1.0.5",  # includes with variables
-    "mkdocs-glightbox==0.3.7",  # img zoom
-    "pillow==10.2.0",  # required for mkdocs-glightbo
-    "cairosvg==2.7.1",  # required for mkdocs-glightbo
-    "requests",  # using in CI, do not pin it
+    "mkdocs-macros-plugin==1.0.5",                      # includes with variables
+    "mkdocs-glightbox==0.3.7",                          # img zoom
+    "pillow==10.2.0",                                   # required for mkdocs-glightbo
+    "cairosvg==2.7.1",                                  # required for mkdocs-glightbo
+    "requests",                                         # using in CI, do not pin it
 ]
 
-lint = [
+types = [
+    "faststream[rabbit,confluent,kafka,nats,redis]",
+    "mypy==1.9.0",
     # mypy extensions
     "types-PyYAML",
     "types-setuptools",
     "types-ujson",
     "types-redis",
     "types-Pygments",
     "types-docutils",
     "confluent-kafka-stubs; python_version >= '3.11'",
-    "mypy==1.9.0",
-    "ruff==0.3.0",
+]
+
+lint = [
+    "faststream[types]",
+    "ruff==0.3.4",
     "bandit==1.7.8",
-    "semgrep==1.66.0",
+    "semgrep==1.67.0",
     "codespell==2.2.6",
 ]
 
 test-core = [
     "coverage[toml]==7.4.4",
     "pytest==8.1.1",
     "pytest-asyncio==0.23.5.post1",
@@ -146,14 +149,15 @@
 path = "faststream/__about__.py"
 
 [tool.hatch.build]
 skip-excluded-dirs = true
 exclude = ["/tests", "/docs"]
 
 [tool.mypy]
+files = ["faststream", "tests/mypy"]
 strict = true
 python_version = "3.8"
 ignore_missing_imports = true
 install_types = true
 non_interactive = true
 plugins = ["pydantic.mypy"]
 
@@ -212,29 +216,39 @@
     # todo pep8-naming
     "N817", # CamelCase `*` imported as acronym `*`
     "N815", # Variable `*` in class scope should not be mixedCase
     "N803", # Argument name `expandMessageExamples` should be lowercase
 
     # todo pydocstyle
     "D100", # missing docstring in public module
+    "D101",
+    "D102",
+    "D103",
     "D104", # missing docstring in public package
     "D105", # missing docstring in magic methods
     "D106", # missing docstring in public nested class
     "D107", # missing docstring in __init__
 ]
 
 [tool.ruff.lint.per-file-ignores]
 "tests/**" = [
-    "D101",       # docstrings
+    "D101",    # docstrings
     "D102",
     "D103",
-    "PLR2004", # magic-value-comparison 
+    "PLR2004", # magic-value-comparison
     "S101",    # use assert
 ]
 
+"docs/*.py" = [
+    "D101", # docstrings
+    "D102",
+    "D103",
+]
+
+
 [tool.ruff.lint.isort]
 case-sensitive = true
 
 [tool.ruff.format]
 docstring-code-format = true
 
 [tool.ruff.lint.pydocstyle]
```

### Comparing `faststream-0.5.0rc0/PKG-INFO` & `faststream-0.5.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: faststream
-Version: 0.5.0rc0
+Version: 0.5.0rc1
 Summary: FastStream: the simplest way to work with a messaging queues
 Project-URL: Homepage, https://faststream.airt.ai/latest/
 Project-URL: Documentation, https://faststream.airt.ai/latest/getting-started/
 Project-URL: Tracker, https://github.com/airtai/FastStream/issues
 Project-URL: Source, https://github.com/airtai/FastStream
 Project-URL: Discord, https://discord.gg/qFm6aSqq59
 Author-email: airt <info@airt.ai>, Nikita Pastukhov <nikita@pastukhov-dev.ru>
@@ -53,35 +53,28 @@
 Requires-Dist: cairosvg==2.7.1; extra == 'devdocs'
 Requires-Dist: mdx-include==1.4.2; extra == 'devdocs'
 Requires-Dist: mike==2.0.0; extra == 'devdocs'
 Requires-Dist: mkdocs-git-revision-date-localized-plugin==1.2.4; extra == 'devdocs'
 Requires-Dist: mkdocs-glightbox==0.3.7; extra == 'devdocs'
 Requires-Dist: mkdocs-literate-nav==0.6.1; extra == 'devdocs'
 Requires-Dist: mkdocs-macros-plugin==1.0.5; extra == 'devdocs'
-Requires-Dist: mkdocs-material==9.5.13; extra == 'devdocs'
+Requires-Dist: mkdocs-material==9.5.16; extra == 'devdocs'
 Requires-Dist: mkdocs-minify-plugin==0.8.0; extra == 'devdocs'
-Requires-Dist: mkdocs-static-i18n==1.2.0; extra == 'devdocs'
+Requires-Dist: mkdocs-static-i18n==1.2.2; extra == 'devdocs'
 Requires-Dist: mkdocstrings[python]==0.24.1; extra == 'devdocs'
 Requires-Dist: pillow==10.2.0; extra == 'devdocs'
 Requires-Dist: requests; extra == 'devdocs'
 Provides-Extra: kafka
 Requires-Dist: aiokafka<0.11,>=0.9; extra == 'kafka'
 Provides-Extra: lint
 Requires-Dist: bandit==1.7.8; extra == 'lint'
 Requires-Dist: codespell==2.2.6; extra == 'lint'
-Requires-Dist: confluent-kafka-stubs; (python_version >= '3.11') and extra == 'lint'
-Requires-Dist: mypy==1.9.0; extra == 'lint'
-Requires-Dist: ruff==0.3.0; extra == 'lint'
-Requires-Dist: semgrep==1.66.0; extra == 'lint'
-Requires-Dist: types-docutils; extra == 'lint'
-Requires-Dist: types-pygments; extra == 'lint'
-Requires-Dist: types-pyyaml; extra == 'lint'
-Requires-Dist: types-redis; extra == 'lint'
-Requires-Dist: types-setuptools; extra == 'lint'
-Requires-Dist: types-ujson; extra == 'lint'
+Requires-Dist: faststream[types]; extra == 'lint'
+Requires-Dist: ruff==0.3.4; extra == 'lint'
+Requires-Dist: semgrep==1.67.0; extra == 'lint'
 Provides-Extra: nats
 Requires-Dist: nats-py<=3.0.0,>=2.3.1; extra == 'nats'
 Provides-Extra: rabbit
 Requires-Dist: aio-pika<10,>=9; extra == 'rabbit'
 Provides-Extra: redis
 Requires-Dist: redis<6.0.0,>=5.0.0; extra == 'redis'
 Provides-Extra: test-core
@@ -93,14 +86,24 @@
 Requires-Dist: email-validator==2.1.1; extra == 'testing'
 Requires-Dist: fastapi==0.109.2; extra == 'testing'
 Requires-Dist: faststream[test-core]; extra == 'testing'
 Requires-Dist: httpx==0.27.0; extra == 'testing'
 Requires-Dist: pydantic-settings<3.0.0,>=2.0.0; extra == 'testing'
 Requires-Dist: pyyaml==6.0.1; extra == 'testing'
 Requires-Dist: watchfiles==0.21.0; extra == 'testing'
+Provides-Extra: types
+Requires-Dist: confluent-kafka-stubs; (python_version >= '3.11') and extra == 'types'
+Requires-Dist: faststream[confluent,kafka,nats,rabbit,redis]; extra == 'types'
+Requires-Dist: mypy==1.9.0; extra == 'types'
+Requires-Dist: types-docutils; extra == 'types'
+Requires-Dist: types-pygments; extra == 'types'
+Requires-Dist: types-pyyaml; extra == 'types'
+Requires-Dist: types-redis; extra == 'types'
+Requires-Dist: types-setuptools; extra == 'types'
+Requires-Dist: types-ujson; extra == 'types'
 Description-Content-Type: text/markdown
 
 # FastStream
 
 <b>Effortless event stream integration for your services</b>
 
 ---
```

