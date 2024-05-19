# Comparing `tmp/faststream-0.5.6.tar.gz` & `tmp/faststream-0.5.7.tar.gz`

## Comparing `faststream-0.5.6.tar` & `faststream-0.5.7.tar`

### file list

```diff
@@ -1,322 +1,341 @@
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 faststream-0.5.6/.codespell-whitelist.txt
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 faststream-0.5.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0     3861 2020-02-02 00:00:00.000000 faststream-0.5.6/.secrets.baseline
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 faststream-0.5.6/.semgrepignore
--rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 faststream-0.5.6/CITATION.cff
--rw-r--r--   0        0        0     5480 2020-02-02 00:00:00.000000 faststream-0.5.6/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     2630 2020-02-02 00:00:00.000000 faststream-0.5.6/CONTRIBUTING.md
--rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 faststream-0.5.6/SECURITY.md
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 faststream-0.5.6/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 faststream-0.5.6/.github/dependabot.yml
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 faststream-0.5.6/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 faststream-0.5.6/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 faststream-0.5.6/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 faststream-0.5.6/.github/workflows/check-broken-links-in-docs.yaml
--rw-r--r--   0        0        0     3520 2020-02-02 00:00:00.000000 faststream-0.5.6/.github/workflows/codeql.yml
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 faststream-0.5.6/.github/workflows/dependency-review.yaml
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 faststream-0.5.6/.github/workflows/deploy-docs.yaml
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 faststream-0.5.6/.github/workflows/publish_coverage.yml
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 faststream-0.5.6/.github/workflows/publish_pypi.yml
--rw-r--r--   0        0        0    16399 2020-02-02 00:00:00.000000 faststream-0.5.6/.github/workflows/test.yaml
--rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 faststream-0.5.6/.github/workflows/update_release_notes.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/__init__.py
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/e01_basic_consume.py
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/e02_1_basic_publisher.py
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/e02_2_basic_publisher.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/e02_3_basic_publisher.py
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/e03_miltiple_pubsub.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/e04_msg_filter.py
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/e05_rpc_request.py
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/e06_manual_ack.py
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/e07_ack_immediately.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/e08_testing.py
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/e09_testing_mocks.py
--rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/e10_middlewares.py
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/e11_settings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/fastapi_integration/__init__.py
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/fastapi_integration/app.py
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/fastapi_integration/testing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/howto/__init__.py
--rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/howto/structlogs.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/kafka/__init__.py
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/kafka/ack_after_process.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/kafka/batch_consume.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/kafka/batch_publish_1.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/kafka/batch_publish_2.py
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/kafka/batch_publish_3.py
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/kafka/testing.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/nats/__init__.py
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/nats/e01_basic.py
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/nats/e02_basic_rpc.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/nats/e03_publisher.py
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/nats/e04_js_basic.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/nats/e05_basic_and_js.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/nats/e06_key_value.py
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/nats/e07_object_storage.py
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/nats/e08_wildcards.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/nats/e09_pull_sub.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/rabbit/__init__.py
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/rabbit/direct.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/rabbit/fanout.py
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/rabbit/header.py
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/rabbit/stream.py
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/rabbit/topic.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/redis/__init__.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/redis/channel_sub.py
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/redis/channel_sub_pattern.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/redis/list_sub.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/redis/list_sub_batch.py
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/redis/rpc.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/redis/stream_sub.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/redis/stream_sub_batch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/router/__init__.py
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/router/basic_consume.py
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/router/basic_publish.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/router/delay_registration.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/serialization/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/serialization/avro/__init__.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/serialization/avro/avro.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/serialization/avro/person.avsc
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/serialization/avro/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/serialization/msgpack/__init__.py
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/serialization/msgpack/pack.py
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/serialization/msgpack/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/serialization/protobuf/__init__.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/serialization/protobuf/message.proto
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/serialization/protobuf/protobuf.py
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 faststream-0.5.6/examples/serialization/protobuf/requirements.txt
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/__about__.py
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/__init__.py
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/__main__.py
--rw-r--r--   0        0        0     5562 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/_compat.py
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/annotations.py
--rw-r--r--   0        0        0     7313 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/app.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/constants.py
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/py.typed
--rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/security.py
--rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/types.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/asyncapi/__init__.py
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/asyncapi/abc.py
--rw-r--r--   0        0        0     5963 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/asyncapi/generate.py
--rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/asyncapi/message.py
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/asyncapi/proto.py
--rw-r--r--   0        0        0     4742 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/asyncapi/site.py
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/asyncapi/utils.py
--rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/asyncapi/schema/__init__.py
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/asyncapi/schema/channels.py
--rw-r--r--   0        0        0     5067 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/asyncapi/schema/info.py
--rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/asyncapi/schema/main.py
--rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/asyncapi/schema/message.py
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/asyncapi/schema/operations.py
--rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/asyncapi/schema/security.py
--rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/asyncapi/schema/servers.py
--rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/asyncapi/schema/utils.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/asyncapi/schema/bindings/__init__.py
--rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/asyncapi/schema/bindings/amqp.py
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/asyncapi/schema/bindings/kafka.py
--rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/asyncapi/schema/bindings/main.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/asyncapi/schema/bindings/nats.py
--rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/asyncapi/schema/bindings/redis.py
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/asyncapi/schema/bindings/sqs.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/broker/__init__.py
--rw-r--r--   0        0        0     6619 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/broker/acknowledgement_watcher.py
--rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/broker/message.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/broker/proto.py
--rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/broker/router.py
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/broker/schemas.py
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/broker/types.py
--rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/broker/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/broker/core/__init__.py
--rw-r--r--   0        0        0     4729 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/broker/core/abc.py
--rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/broker/core/logging.py
--rw-r--r--   0        0        0    10503 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/broker/core/usecase.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/broker/fastapi/__init__.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/broker/fastapi/context.py
--rw-r--r--   0        0        0     4309 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/broker/fastapi/get_dependant.py
--rw-r--r--   0        0        0     9644 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/broker/fastapi/route.py
--rw-r--r--   0        0        0    18036 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/broker/fastapi/router.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/broker/middlewares/__init__.py
--rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/broker/middlewares/base.py
--rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/broker/middlewares/logging.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/broker/publisher/__init__.py
--rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/broker/publisher/fake.py
--rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/broker/publisher/proto.py
--rw-r--r--   0        0        0     5206 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/broker/publisher/usecase.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/broker/subscriber/__init__.py
--rw-r--r--   0        0        0     5197 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/broker/subscriber/call_item.py
--rw-r--r--   0        0        0     2847 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/broker/subscriber/proto.py
--rw-r--r--   0        0        0    13242 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/broker/subscriber/usecase.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/broker/wrapper/__init__.py
--rw-r--r--   0        0        0     5992 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/broker/wrapper/call.py
--rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/broker/wrapper/proto.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/cli/__init__.py
--rw-r--r--   0        0        0     7507 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/cli/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/cli/docs/__init__.py
--rw-r--r--   0        0        0     5273 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/cli/docs/app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/cli/supervisors/__init__.py
--rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/cli/supervisors/basereload.py
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/cli/supervisors/multiprocess.py
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/cli/supervisors/utils.py
--rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/cli/supervisors/watchfiles.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/cli/utils/__init__.py
--rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/cli/utils/imports.py
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/cli/utils/logs.py
--rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/cli/utils/parser.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/confluent/__init__.py
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/confluent/annotations.py
--rw-r--r--   0        0        0    14880 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/confluent/client.py
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/confluent/message.py
--rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/confluent/parser.py
--rw-r--r--   0        0        0    20008 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/confluent/router.py
--rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/confluent/security.py
--rw-r--r--   0        0        0     7570 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/confluent/testing.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/confluent/broker/__init__.py
--rw-r--r--   0        0        0    18973 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/confluent/broker/broker.py
--rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/confluent/broker/logging.py
--rw-r--r--   0        0        0    65013 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/confluent/broker/registrator.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/confluent/fastapi/__init__.py
--rw-r--r--   0        0        0    99735 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/confluent/fastapi/fastapi.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/confluent/publisher/__init__.py
--rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/confluent/publisher/asyncapi.py
--rw-r--r--   0        0        0     3274 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/confluent/publisher/producer.py
--rw-r--r--   0        0        0     5840 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/confluent/publisher/usecase.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/confluent/schemas/__init__.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/confluent/schemas/params.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/confluent/subscriber/__init__.py
--rw-r--r--   0        0        0     6028 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/confluent/subscriber/asyncapi.py
--rw-r--r--   0        0        0    10552 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/confluent/subscriber/usecase.py
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/kafka/__init__.py
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/kafka/annotations.py
--rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/kafka/message.py
--rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/kafka/parser.py
--rw-r--r--   0        0        0    22297 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/kafka/router.py
--rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/kafka/security.py
--rwxr-xr-x   0        0        0     6854 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/kafka/testing.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/kafka/broker/__init__.py
--rw-r--r--   0        0        0    29045 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/kafka/broker/broker.py
--rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/kafka/broker/logging.py
--rw-r--r--   0        0        0    72613 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/kafka/broker/registrator.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/kafka/fastapi/__init__.py
--rw-r--r--   0        0        0   118913 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/kafka/fastapi/fastapi.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/kafka/publisher/__init__.py
--rw-r--r--   0        0        0     5520 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/kafka/publisher/asyncapi.py
--rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/kafka/publisher/producer.py
--rw-r--r--   0        0        0     8807 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/kafka/publisher/usecase.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/kafka/schemas/__init__.py
--rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/kafka/schemas/params.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/kafka/subscriber/__init__.py
--rw-r--r--   0        0        0     7564 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/kafka/subscriber/asyncapi.py
--rw-r--r--   0        0        0    11865 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/kafka/subscriber/usecase.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/log/__init__.py
--rw-r--r--   0        0        0     2424 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/log/formatter.py
--rw-r--r--   0        0        0     1975 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/log/logging.py
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/nats/__init__.py
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/nats/annotations.py
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/nats/helpers.py
--rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/nats/message.py
--rw-r--r--   0        0        0     3789 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/nats/parser.py
--rw-r--r--   0        0        0    12274 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/nats/router.py
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/nats/security.py
--rw-r--r--   0        0        0     4606 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/nats/testing.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/nats/broker/__init__.py
--rw-r--r--   0        0        0    27057 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/nats/broker/broker.py
--rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/nats/broker/logging.py
--rw-r--r--   0        0        0    11868 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/nats/broker/registrator.py
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/nats/fastapi/__init__.py
--rw-r--r--   0        0        0    36228 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/nats/fastapi/fastapi.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/nats/publisher/__init__.py
--rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/nats/publisher/asyncapi.py
--rw-r--r--   0        0        0     5595 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/nats/publisher/producer.py
--rw-r--r--   0        0        0     5125 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/nats/publisher/usecase.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/nats/schemas/__init__.py
--rw-r--r--   0        0        0     9645 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/nats/schemas/js_stream.py
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/nats/schemas/pull_sub.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/nats/subscriber/__init__.py
--rw-r--r--   0        0        0     6406 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/nats/subscriber/asyncapi.py
--rw-r--r--   0        0        0    14807 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/nats/subscriber/usecase.py
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/rabbit/__init__.py
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/rabbit/annotations.py
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/rabbit/message.py
--rw-r--r--   0        0        0     3247 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/rabbit/parser.py
--rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/rabbit/router.py
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/rabbit/security.py
--rw-r--r--   0        0        0    10191 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/rabbit/testing.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/rabbit/types.py
--rw-r--r--   0        0        0     4125 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/rabbit/utils.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/rabbit/broker/__init__.py
--rw-r--r--   0        0        0    21801 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/rabbit/broker/broker.py
--rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/rabbit/broker/logging.py
--rw-r--r--   0        0        0    10794 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/rabbit/broker/registrator.py
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/rabbit/fastapi/__init__.py
--rw-r--r--   0        0        0    31096 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/rabbit/fastapi/router.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/rabbit/publisher/__init__.py
--rw-r--r--   0        0        0     5063 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/rabbit/publisher/asyncapi.py
--rw-r--r--   0        0        0     7466 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/rabbit/publisher/producer.py
--rw-r--r--   0        0        0     8209 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/rabbit/publisher/usecase.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/rabbit/schemas/__init__.py
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/rabbit/schemas/constants.py
--rw-r--r--   0        0        0     3919 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/rabbit/schemas/exchange.py
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/rabbit/schemas/proto.py
--rw-r--r--   0        0        0     3585 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/rabbit/schemas/queue.py
--rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/rabbit/schemas/reply.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/rabbit/subscriber/__init__.py
--rw-r--r--   0        0        0     4383 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/rabbit/subscriber/asyncapi.py
--rw-r--r--   0        0        0     7082 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/rabbit/subscriber/usecase.py
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/redis/__init__.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/redis/annotations.py
--rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/redis/message.py
--rw-r--r--   0        0        0     6414 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/redis/parser.py
--rw-r--r--   0        0        0     8211 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/redis/router.py
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/redis/security.py
--rw-r--r--   0        0        0     6909 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/redis/testing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/redis/broker/__init__.py
--rw-r--r--   0        0        0    15909 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/redis/broker/broker.py
--rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/redis/broker/logging.py
--rw-r--r--   0        0        0     7576 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/redis/broker/registrator.py
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/redis/fastapi/__init__.py
--rw-r--r--   0        0        0    27638 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/redis/fastapi/fastapi.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/redis/publisher/__init__.py
--rw-r--r--   0        0        0     6019 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/redis/publisher/asyncapi.py
--rw-r--r--   0        0        0     4143 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/redis/publisher/producer.py
--rw-r--r--   0        0        0    14932 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/redis/publisher/usecase.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/redis/schemas/__init__.py
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/redis/schemas/list_sub.py
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/redis/schemas/proto.py
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/redis/schemas/pub_sub.py
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/redis/schemas/stream_sub.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/redis/subscriber/__init__.py
--rw-r--r--   0        0        0     7044 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/redis/subscriber/asyncapi.py
--rw-r--r--   0        0        0    21352 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/redis/subscriber/usecase.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/testing/__init__.py
--rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/testing/app.py
--rw-r--r--   0        0        0     6746 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/testing/broker.py
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/utils/__init__.py
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/utils/ast.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/utils/classes.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/utils/data.py
--rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/utils/functions.py
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/utils/no_cast.py
--rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/utils/path.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/utils/context/__init__.py
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/utils/context/builders.py
--rw-r--r--   0        0        0     5117 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/utils/context/repository.py
--rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 faststream-0.5.6/faststream/utils/context/types.py
--rwxr-xr-x   0        0        0      915 2020-02-02 00:00:00.000000 faststream-0.5.6/scripts/build-docs-pre-commit.sh
--rwxr-xr-x   0        0        0       66 2020-02-02 00:00:00.000000 faststream-0.5.6/scripts/build-docs.sh
--rwxr-xr-x   0        0        0      909 2020-02-02 00:00:00.000000 faststream-0.5.6/scripts/lint-pre-commit.sh
--rwxr-xr-x   0        0        0      247 2020-02-02 00:00:00.000000 faststream-0.5.6/scripts/lint.sh
--rwxr-xr-x   0        0        0       51 2020-02-02 00:00:00.000000 faststream-0.5.6/scripts/publish.sh
--rwxr-xr-x   0        0        0       70 2020-02-02 00:00:00.000000 faststream-0.5.6/scripts/serve-docs.sh
--rwxr-xr-x   0        0        0      522 2020-02-02 00:00:00.000000 faststream-0.5.6/scripts/set_variables.sh
--rwxr-xr-x   0        0        0      147 2020-02-02 00:00:00.000000 faststream-0.5.6/scripts/start_test_env.sh
--rwxr-xr-x   0        0        0      175 2020-02-02 00:00:00.000000 faststream-0.5.6/scripts/static-analysis.sh
--rwxr-xr-x   0        0        0      926 2020-02-02 00:00:00.000000 faststream-0.5.6/scripts/static-pre-commit.sh
--rwxr-xr-x   0        0        0      132 2020-02-02 00:00:00.000000 faststream-0.5.6/scripts/stop_test_env.sh
--rwxr-xr-x   0        0        0      154 2020-02-02 00:00:00.000000 faststream-0.5.6/scripts/test-cov.sh
--rwxr-xr-x   0        0        0      131 2020-02-02 00:00:00.000000 faststream-0.5.6/scripts/test.sh
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 faststream-0.5.6/.gitignore
--rw-r--r--   0        0        0    11363 2020-02-02 00:00:00.000000 faststream-0.5.6/LICENSE
--rw-r--r--   0        0        0    14865 2020-02-02 00:00:00.000000 faststream-0.5.6/README.md
--rw-r--r--   0        0        0    10331 2020-02-02 00:00:00.000000 faststream-0.5.6/pyproject.toml
--rw-r--r--   0        0        0    22991 2020-02-02 00:00:00.000000 faststream-0.5.6/PKG-INFO
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 faststream-0.5.7/.codespell-whitelist.txt
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 faststream-0.5.7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     3861 2020-02-02 00:00:00.000000 faststream-0.5.7/.secrets.baseline
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 faststream-0.5.7/.semgrepignore
+-rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 faststream-0.5.7/CITATION.cff
+-rw-r--r--   0        0        0     5480 2020-02-02 00:00:00.000000 faststream-0.5.7/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     2630 2020-02-02 00:00:00.000000 faststream-0.5.7/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 faststream-0.5.7/SECURITY.md
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 faststream-0.5.7/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 faststream-0.5.7/.github/dependabot.yml
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 faststream-0.5.7/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 faststream-0.5.7/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 faststream-0.5.7/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 faststream-0.5.7/.github/workflows/check-broken-links-in-docs.yaml
+-rw-r--r--   0        0        0     3520 2020-02-02 00:00:00.000000 faststream-0.5.7/.github/workflows/codeql.yml
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 faststream-0.5.7/.github/workflows/dependency-review.yaml
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 faststream-0.5.7/.github/workflows/deploy-docs.yaml
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 faststream-0.5.7/.github/workflows/publish_coverage.yml
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 faststream-0.5.7/.github/workflows/publish_pypi.yml
+-rw-r--r--   0        0        0    16183 2020-02-02 00:00:00.000000 faststream-0.5.7/.github/workflows/test.yaml
+-rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 faststream-0.5.7/.github/workflows/update_release_notes.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/__init__.py
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/e01_basic_consume.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/e02_1_basic_publisher.py
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/e02_2_basic_publisher.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/e02_3_basic_publisher.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/e03_miltiple_pubsub.py
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/e04_msg_filter.py
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/e05_rpc_request.py
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/e06_manual_ack.py
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/e07_ack_immediately.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/e08_testing.py
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/e09_testing_mocks.py
+-rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/e10_middlewares.py
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/e11_settings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/fastapi_integration/__init__.py
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/fastapi_integration/app.py
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/fastapi_integration/testing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/howto/__init__.py
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/howto/structlogs.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/kafka/__init__.py
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/kafka/ack_after_process.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/kafka/batch_consume.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/kafka/batch_publish_1.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/kafka/batch_publish_2.py
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/kafka/batch_publish_3.py
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/kafka/testing.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/nats/__init__.py
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/nats/e01_basic.py
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/nats/e02_basic_rpc.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/nats/e03_publisher.py
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/nats/e04_js_basic.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/nats/e05_basic_and_js.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/nats/e06_key_value.py
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/nats/e07_object_storage.py
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/nats/e08_wildcards.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/nats/e09_pull_sub.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/rabbit/__init__.py
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/rabbit/direct.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/rabbit/fanout.py
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/rabbit/header.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/rabbit/stream.py
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/rabbit/topic.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/redis/__init__.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/redis/channel_sub.py
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/redis/channel_sub_pattern.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/redis/list_sub.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/redis/list_sub_batch.py
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/redis/rpc.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/redis/stream_sub.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/redis/stream_sub_batch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/router/__init__.py
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/router/basic_consume.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/router/basic_publish.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/router/delay_registration.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/serialization/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/serialization/avro/__init__.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/serialization/avro/avro.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/serialization/avro/person.avsc
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/serialization/avro/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/serialization/msgpack/__init__.py
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/serialization/msgpack/pack.py
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/serialization/msgpack/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/serialization/protobuf/__init__.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/serialization/protobuf/message.proto
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/serialization/protobuf/protobuf.py
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 faststream-0.5.7/examples/serialization/protobuf/requirements.txt
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/__about__.py
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/__init__.py
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/__main__.py
+-rw-r--r--   0        0        0     5562 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/_compat.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/annotations.py
+-rw-r--r--   0        0        0     7313 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/app.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/constants.py
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/py.typed
+-rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/security.py
+-rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/types.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/asyncapi/__init__.py
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/asyncapi/abc.py
+-rw-r--r--   0        0        0     5963 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/asyncapi/generate.py
+-rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/asyncapi/message.py
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/asyncapi/proto.py
+-rw-r--r--   0        0        0     4742 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/asyncapi/site.py
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/asyncapi/utils.py
+-rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/asyncapi/schema/__init__.py
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/asyncapi/schema/channels.py
+-rw-r--r--   0        0        0     5067 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/asyncapi/schema/info.py
+-rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/asyncapi/schema/main.py
+-rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/asyncapi/schema/message.py
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/asyncapi/schema/operations.py
+-rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/asyncapi/schema/security.py
+-rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/asyncapi/schema/servers.py
+-rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/asyncapi/schema/utils.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/asyncapi/schema/bindings/__init__.py
+-rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/asyncapi/schema/bindings/amqp.py
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/asyncapi/schema/bindings/kafka.py
+-rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/asyncapi/schema/bindings/main.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/asyncapi/schema/bindings/nats.py
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/asyncapi/schema/bindings/redis.py
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/asyncapi/schema/bindings/sqs.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/broker/__init__.py
+-rw-r--r--   0        0        0     6619 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/broker/acknowledgement_watcher.py
+-rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/broker/message.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/broker/proto.py
+-rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/broker/router.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/broker/schemas.py
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/broker/types.py
+-rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/broker/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/broker/core/__init__.py
+-rw-r--r--   0        0        0     4731 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/broker/core/abc.py
+-rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/broker/core/logging.py
+-rw-r--r--   0        0        0    10550 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/broker/core/usecase.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/broker/fastapi/__init__.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/broker/fastapi/context.py
+-rw-r--r--   0        0        0     4309 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/broker/fastapi/get_dependant.py
+-rw-r--r--   0        0        0     9644 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/broker/fastapi/route.py
+-rw-r--r--   0        0        0    18036 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/broker/fastapi/router.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/broker/middlewares/__init__.py
+-rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/broker/middlewares/base.py
+-rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/broker/middlewares/logging.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/broker/publisher/__init__.py
+-rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/broker/publisher/fake.py
+-rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/broker/publisher/proto.py
+-rw-r--r--   0        0        0     5206 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/broker/publisher/usecase.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/broker/subscriber/__init__.py
+-rw-r--r--   0        0        0     5197 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/broker/subscriber/call_item.py
+-rw-r--r--   0        0        0     2848 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/broker/subscriber/proto.py
+-rw-r--r--   0        0        0    13229 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/broker/subscriber/usecase.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/broker/wrapper/__init__.py
+-rw-r--r--   0        0        0     5992 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/broker/wrapper/call.py
+-rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/broker/wrapper/proto.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/cli/__init__.py
+-rw-r--r--   0        0        0     7507 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/cli/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/cli/docs/__init__.py
+-rw-r--r--   0        0        0     5273 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/cli/docs/app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/cli/supervisors/__init__.py
+-rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/cli/supervisors/basereload.py
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/cli/supervisors/multiprocess.py
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/cli/supervisors/utils.py
+-rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/cli/supervisors/watchfiles.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/cli/utils/__init__.py
+-rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/cli/utils/imports.py
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/cli/utils/logs.py
+-rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/cli/utils/parser.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/confluent/__init__.py
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/confluent/annotations.py
+-rw-r--r--   0        0        0    14880 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/confluent/client.py
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/confluent/message.py
+-rw-r--r--   0        0        0     3294 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/confluent/parser.py
+-rw-r--r--   0        0        0    20122 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/confluent/router.py
+-rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/confluent/security.py
+-rw-r--r--   0        0        0     7570 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/confluent/testing.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/confluent/broker/__init__.py
+-rw-r--r--   0        0        0    19020 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/confluent/broker/broker.py
+-rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/confluent/broker/logging.py
+-rw-r--r--   0        0        0    65013 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/confluent/broker/registrator.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/confluent/fastapi/__init__.py
+-rw-r--r--   0        0        0    99735 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/confluent/fastapi/fastapi.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/confluent/opentelemetry/__init__.py
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/confluent/opentelemetry/middleware.py
+-rw-r--r--   0        0        0     4008 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/confluent/opentelemetry/provider.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/confluent/publisher/__init__.py
+-rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/confluent/publisher/asyncapi.py
+-rw-r--r--   0        0        0     3274 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/confluent/publisher/producer.py
+-rw-r--r--   0        0        0     5840 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/confluent/publisher/usecase.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/confluent/schemas/__init__.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/confluent/schemas/params.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/confluent/subscriber/__init__.py
+-rw-r--r--   0        0        0     6028 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/confluent/subscriber/asyncapi.py
+-rw-r--r--   0        0        0    10542 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/confluent/subscriber/usecase.py
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/kafka/__init__.py
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/kafka/annotations.py
+-rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/kafka/message.py
+-rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/kafka/parser.py
+-rw-r--r--   0        0        0    22411 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/kafka/router.py
+-rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/kafka/security.py
+-rwxr-xr-x   0        0        0     6854 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/kafka/testing.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/kafka/broker/__init__.py
+-rw-r--r--   0        0        0    29093 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/kafka/broker/broker.py
+-rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/kafka/broker/logging.py
+-rw-r--r--   0        0        0    72613 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/kafka/broker/registrator.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/kafka/fastapi/__init__.py
+-rw-r--r--   0        0        0   118913 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/kafka/fastapi/fastapi.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/kafka/opentelemetry/__init__.py
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/kafka/opentelemetry/middleware.py
+-rw-r--r--   0        0        0     4020 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/kafka/opentelemetry/provider.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/kafka/publisher/__init__.py
+-rw-r--r--   0        0        0     5520 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/kafka/publisher/asyncapi.py
+-rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/kafka/publisher/producer.py
+-rw-r--r--   0        0        0     8807 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/kafka/publisher/usecase.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/kafka/schemas/__init__.py
+-rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/kafka/schemas/params.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/kafka/subscriber/__init__.py
+-rw-r--r--   0        0        0     7564 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/kafka/subscriber/asyncapi.py
+-rw-r--r--   0        0        0    11855 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/kafka/subscriber/usecase.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/log/__init__.py
+-rw-r--r--   0        0        0     2424 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/log/formatter.py
+-rw-r--r--   0        0        0     1975 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/log/logging.py
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/nats/__init__.py
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/nats/annotations.py
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/nats/helpers.py
+-rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/nats/message.py
+-rw-r--r--   0        0        0     3789 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/nats/parser.py
+-rw-r--r--   0        0        0    12421 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/nats/router.py
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/nats/security.py
+-rw-r--r--   0        0        0     4606 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/nats/testing.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/nats/broker/__init__.py
+-rw-r--r--   0        0        0    27010 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/nats/broker/broker.py
+-rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/nats/broker/logging.py
+-rw-r--r--   0        0        0    11894 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/nats/broker/registrator.py
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/nats/fastapi/__init__.py
+-rw-r--r--   0        0        0    36228 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/nats/fastapi/fastapi.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/nats/opentelemetry/__init__.py
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/nats/opentelemetry/middleware.py
+-rw-r--r--   0        0        0     3583 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/nats/opentelemetry/provider.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/nats/publisher/__init__.py
+-rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/nats/publisher/asyncapi.py
+-rw-r--r--   0        0        0     5595 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/nats/publisher/producer.py
+-rw-r--r--   0        0        0     5125 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/nats/publisher/usecase.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/nats/schemas/__init__.py
+-rw-r--r--   0        0        0     9645 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/nats/schemas/js_stream.py
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/nats/schemas/pull_sub.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/nats/subscriber/__init__.py
+-rw-r--r--   0        0        0     6406 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/nats/subscriber/asyncapi.py
+-rw-r--r--   0        0        0    14797 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/nats/subscriber/usecase.py
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/opentelemetry/__init__.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/opentelemetry/consts.py
+-rw-r--r--   0        0        0    10165 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/opentelemetry/middleware.py
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/opentelemetry/provider.py
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/rabbit/__init__.py
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/rabbit/annotations.py
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/rabbit/message.py
+-rw-r--r--   0        0        0     3247 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/rabbit/parser.py
+-rw-r--r--   0        0        0    11614 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/rabbit/router.py
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/rabbit/security.py
+-rw-r--r--   0        0        0    10191 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/rabbit/testing.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/rabbit/types.py
+-rw-r--r--   0        0        0     4125 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/rabbit/utils.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/rabbit/broker/__init__.py
+-rw-r--r--   0        0        0    21894 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/rabbit/broker/broker.py
+-rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/rabbit/broker/logging.py
+-rw-r--r--   0        0        0    10794 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/rabbit/broker/registrator.py
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/rabbit/fastapi/__init__.py
+-rw-r--r--   0        0        0    31096 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/rabbit/fastapi/router.py
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/rabbit/opentelemetry/__init__.py
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/rabbit/opentelemetry/middleware.py
+-rw-r--r--   0        0        0     2305 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/rabbit/opentelemetry/provider.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/rabbit/publisher/__init__.py
+-rw-r--r--   0        0        0     5063 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/rabbit/publisher/asyncapi.py
+-rw-r--r--   0        0        0     7466 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/rabbit/publisher/producer.py
+-rw-r--r--   0        0        0     8210 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/rabbit/publisher/usecase.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/rabbit/schemas/__init__.py
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/rabbit/schemas/constants.py
+-rw-r--r--   0        0        0     3919 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/rabbit/schemas/exchange.py
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/rabbit/schemas/proto.py
+-rw-r--r--   0        0        0     3585 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/rabbit/schemas/queue.py
+-rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/rabbit/schemas/reply.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/rabbit/subscriber/__init__.py
+-rw-r--r--   0        0        0     4383 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/rabbit/subscriber/asyncapi.py
+-rw-r--r--   0        0        0     7072 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/rabbit/subscriber/usecase.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/redis/__init__.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/redis/annotations.py
+-rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/redis/message.py
+-rw-r--r--   0        0        0     6414 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/redis/parser.py
+-rw-r--r--   0        0        0     8321 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/redis/router.py
+-rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/redis/security.py
+-rw-r--r--   0        0        0     7003 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/redis/testing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/redis/broker/__init__.py
+-rw-r--r--   0        0        0    15965 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/redis/broker/broker.py
+-rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/redis/broker/logging.py
+-rw-r--r--   0        0        0     7576 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/redis/broker/registrator.py
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/redis/fastapi/__init__.py
+-rw-r--r--   0        0        0    27638 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/redis/fastapi/fastapi.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/redis/opentelemetry/__init__.py
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/redis/opentelemetry/middleware.py
+-rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/redis/opentelemetry/provider.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/redis/publisher/__init__.py
+-rw-r--r--   0        0        0     6019 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/redis/publisher/asyncapi.py
+-rw-r--r--   0        0        0     4191 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/redis/publisher/producer.py
+-rw-r--r--   0        0        0    14932 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/redis/publisher/usecase.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/redis/schemas/__init__.py
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/redis/schemas/list_sub.py
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/redis/schemas/proto.py
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/redis/schemas/pub_sub.py
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/redis/schemas/stream_sub.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/redis/subscriber/__init__.py
+-rw-r--r--   0        0        0     7044 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/redis/subscriber/asyncapi.py
+-rw-r--r--   0        0        0    21342 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/redis/subscriber/usecase.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/testing/__init__.py
+-rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/testing/app.py
+-rw-r--r--   0        0        0     7097 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/testing/broker.py
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/utils/__init__.py
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/utils/ast.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/utils/classes.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/utils/data.py
+-rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/utils/functions.py
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/utils/no_cast.py
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/utils/path.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/utils/context/__init__.py
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/utils/context/builders.py
+-rw-r--r--   0        0        0     5117 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/utils/context/repository.py
+-rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 faststream-0.5.7/faststream/utils/context/types.py
+-rwxr-xr-x   0        0        0      915 2020-02-02 00:00:00.000000 faststream-0.5.7/scripts/build-docs-pre-commit.sh
+-rwxr-xr-x   0        0        0       66 2020-02-02 00:00:00.000000 faststream-0.5.7/scripts/build-docs.sh
+-rwxr-xr-x   0        0        0      909 2020-02-02 00:00:00.000000 faststream-0.5.7/scripts/lint-pre-commit.sh
+-rwxr-xr-x   0        0        0      247 2020-02-02 00:00:00.000000 faststream-0.5.7/scripts/lint.sh
+-rwxr-xr-x   0        0        0       51 2020-02-02 00:00:00.000000 faststream-0.5.7/scripts/publish.sh
+-rwxr-xr-x   0        0        0       70 2020-02-02 00:00:00.000000 faststream-0.5.7/scripts/serve-docs.sh
+-rwxr-xr-x   0        0        0      522 2020-02-02 00:00:00.000000 faststream-0.5.7/scripts/set_variables.sh
+-rwxr-xr-x   0        0        0      147 2020-02-02 00:00:00.000000 faststream-0.5.7/scripts/start_test_env.sh
+-rwxr-xr-x   0        0        0      175 2020-02-02 00:00:00.000000 faststream-0.5.7/scripts/static-analysis.sh
+-rwxr-xr-x   0        0        0      926 2020-02-02 00:00:00.000000 faststream-0.5.7/scripts/static-pre-commit.sh
+-rwxr-xr-x   0        0        0      132 2020-02-02 00:00:00.000000 faststream-0.5.7/scripts/stop_test_env.sh
+-rwxr-xr-x   0        0        0      154 2020-02-02 00:00:00.000000 faststream-0.5.7/scripts/test-cov.sh
+-rwxr-xr-x   0        0        0      131 2020-02-02 00:00:00.000000 faststream-0.5.7/scripts/test.sh
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 faststream-0.5.7/.gitignore
+-rw-r--r--   0        0        0    11363 2020-02-02 00:00:00.000000 faststream-0.5.7/LICENSE
+-rw-r--r--   0        0        0    14865 2020-02-02 00:00:00.000000 faststream-0.5.7/README.md
+-rw-r--r--   0        0        0    10396 2020-02-02 00:00:00.000000 faststream-0.5.7/pyproject.toml
+-rw-r--r--   0        0        0    23654 2020-02-02 00:00:00.000000 faststream-0.5.7/PKG-INFO
```

### Comparing `faststream-0.5.6/.pre-commit-config.yaml` & `faststream-0.5.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/.secrets.baseline` & `faststream-0.5.7/.secrets.baseline`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/CITATION.cff` & `faststream-0.5.7/CITATION.cff`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/CODE_OF_CONDUCT.md` & `faststream-0.5.7/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/CONTRIBUTING.md` & `faststream-0.5.7/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/SECURITY.md` & `faststream-0.5.7/SECURITY.md`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/.github/PULL_REQUEST_TEMPLATE.md` & `faststream-0.5.7/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files 0% similar despite different names*

```diff
@@ -18,9 +18,9 @@
 
 - [ ] My code adheres to the style guidelines of this project (`scripts/lint.sh` shows no errors)
 - [ ] I have conducted a self-review of my own code
 - [ ] I have made the necessary changes to the documentation
 - [ ] My changes do not generate any new warnings
 - [ ] I have added tests to validate the effectiveness of my fix or the functionality of my new feature
 - [ ] Both new and existing unit tests pass successfully on my local environment by running `scripts/test-cov.sh`
-- [ ] I have ensured that static analysis tests are passing by running `scripts/static-anaylysis.sh`
+- [ ] I have ensured that static analysis tests are passing by running `scripts/static-analysis.sh`
 - [ ] I have included code examples to illustrate the modifications
```

### Comparing `faststream-0.5.6/.github/dependabot.yml` & `faststream-0.5.7/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/.github/ISSUE_TEMPLATE/bug_report.md` & `faststream-0.5.7/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/.github/ISSUE_TEMPLATE/feature_request.md` & `faststream-0.5.7/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/.github/workflows/check-broken-links-in-docs.yaml` & `faststream-0.5.7/.github/workflows/check-broken-links-in-docs.yaml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/.github/workflows/codeql.yml` & `faststream-0.5.7/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/.github/workflows/dependency-review.yaml` & `faststream-0.5.7/.github/workflows/dependency-review.yaml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/.github/workflows/deploy-docs.yaml` & `faststream-0.5.7/.github/workflows/deploy-docs.yaml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/.github/workflows/publish_coverage.yml` & `faststream-0.5.7/.github/workflows/publish_coverage.yml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/.github/workflows/publish_pypi.yml` & `faststream-0.5.7/.github/workflows/publish_pypi.yml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/.github/workflows/test.yaml` & `faststream-0.5.7/.github/workflows/test.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -80,15 +80,15 @@
       - uses: actions/cache@v4
         id: cache
         with:
           path: ${{ env.pythonLocation }}
           key: ${{ runner.os }}-python-${{ env.pythonLocation }}-${{ hashFiles('pyproject.toml') }}-test-v03
       - name: Install Dependencies
         if: steps.cache.outputs.cache-hit != 'true'
-        run: pip install .[rabbit,kafka,confluent,nats,redis,testing]
+        run: pip install .[optionals,testing]
       - name: Install Pydantic v1
         if: matrix.pydantic-version == 'pydantic-v1'
         run: pip install "pydantic>=1.10.0,<2.0.0"
       - name: Install Pydantic v2
         if: matrix.pydantic-version == 'pydantic-v2'
         run: pip install --pre "pydantic>=2.0.0b2,<3.0.0"
       - run: mkdir coverage
@@ -113,15 +113,15 @@
         uses: actions/setup-python@v5
         with:
           python-version: "3.12"
           cache: "pip"
           cache-dependency-path: pyproject.toml
       - name: Install Dependencies
         if: steps.cache.outputs.cache-hit != 'true'
-        run: pip install .[nats,kafka,confluent,rabbit,redis,testing] orjson
+        run: pip install .[optionals,testing] orjson
       - run: mkdir coverage
       - name: Test
         run: bash scripts/test.sh -m"(slow and (not nats and not kafka and not confluent and not rabbit and not redis)) or (not nats and not kafka and not confluent and not rabbit and not redis)"
         env:
           COVERAGE_FILE: coverage/.coverage.orjson
           CONTEXT: orjson
       - name: Store coverage files
@@ -140,15 +140,15 @@
         uses: actions/setup-python@v5
         with:
           python-version: "3.12"
           cache: "pip"
           cache-dependency-path: pyproject.toml
       - name: Install Dependencies
         if: steps.cache.outputs.cache-hit != 'true'
-        run: pip install .[rabbit,kafka,confluent,nats,redis,testing]
+        run: pip install .[optionals,testing]
       - name: Test
         run: bash scripts/test.sh -m "(slow and (not nats and not kafka and not confluent and not rabbit and not redis)) or (not nats and not kafka and not confluent and not rabbit and not redis)"
 
   test-windows-latest:
     if: github.event.pull_request.draft == false
     runs-on: windows-latest
     steps:
@@ -157,15 +157,15 @@
         uses: actions/setup-python@v5
         with:
           python-version: "3.12"
           cache: "pip"
           cache-dependency-path: pyproject.toml
       - name: Install Dependencies
         if: steps.cache.outputs.cache-hit != 'true'
-        run: pip install .[rabbit,kafka,confluent,nats,redis,testing]
+        run: pip install .[optionals,testing]
       - name: Test
         run: bash scripts/test.sh -m "(slow and (not nats and not kafka and not confluent and not rabbit and not redis)) or (not nats and not kafka and not confluent and not rabbit and not redis)"
 
   test-kafka-real:
     if: github.event.pull_request.draft == false
     runs-on: ubuntu-latest
     services:
@@ -190,15 +190,15 @@
         uses: actions/setup-python@v5
         with:
           python-version: "3.12"
           cache: "pip"
           cache-dependency-path: pyproject.toml
       - name: Install Dependencies
         if: steps.cache.outputs.cache-hit != 'true'
-        run: pip install .[nats,kafka,confluent,rabbit,redis,testing]
+        run: pip install .[optionals,testing]
       - run: mkdir coverage
       - name: Test
         run: bash scripts/test.sh -m "(slow and kafka) or kafka"
         env:
           COVERAGE_FILE: coverage/.coverage.kafka-py
           CONTEXT: kafka-py
       - name: Store coverage files
@@ -250,15 +250,15 @@
         uses: actions/setup-python@v5
         with:
           python-version: "3.12"
           cache: "pip"
           cache-dependency-path: pyproject.toml
       - name: Install Dependencies
         if: steps.cache.outputs.cache-hit != 'true'
-        run: pip install .[nats,kafka,confluent,rabbit,redis,testing]
+        run: pip install .[optionals,testing]
       - run: mkdir coverage
       - name: Test
         run: bash scripts/test.sh -m "(slow and confluent) or confluent"
         env:
           COVERAGE_FILE: coverage/.coverage.confluent-py
           CONTEXT: confluent-py
       - name: Store coverage files
@@ -299,15 +299,15 @@
         uses: actions/setup-python@v5
         with:
           python-version: "3.12"
           cache: "pip"
           cache-dependency-path: pyproject.toml
       - name: Install Dependencies
         if: steps.cache.outputs.cache-hit != 'true'
-        run: pip install .[nats,kafka,confluent,rabbit,redis,testing]
+        run: pip install .[optionals,testing]
       - run: mkdir coverage
       - name: Test
         run: bash scripts/test.sh -m "(slow and rabbit) or rabbit"
         env:
           COVERAGE_FILE: coverage/.coverage.rabbit-py
           CONTEXT: rabbit-py
       - name: Store coverage files
@@ -348,15 +348,15 @@
         uses: actions/setup-python@v5
         with:
           python-version: "3.12"
           cache: "pip"
           cache-dependency-path: pyproject.toml
       - name: Install Dependencies
         if: steps.cache.outputs.cache-hit != 'true'
-        run: pip install .[nats,kafka,confluent,rabbit,redis,testing]
+        run: pip install .[optionals,testing]
       - run: mkdir coverage
       - name: Test
         run: bash scripts/test.sh -m "(slow and nats) or nats"
         env:
           COVERAGE_FILE: coverage/.coverage.nats-py
           CONTEXT: nats-py
       - name: Store coverage files
@@ -397,15 +397,15 @@
         uses: actions/setup-python@v5
         with:
           python-version: "3.12"
           cache: "pip"
           cache-dependency-path: pyproject.toml
       - name: Install Dependencies
         if: steps.cache.outputs.cache-hit != 'true'
-        run: pip install .[nats,kafka,confluent,rabbit,redis,testing]
+        run: pip install .[optionals,testing]
       - run: mkdir coverage
       - name: Test
         run: bash scripts/test.sh -m "(slow and redis) or redis"
         env:
           COVERAGE_FILE: coverage/.coverage.redis-py
           CONTEXT: redis-py
       - name: Store coverage files
```

### Comparing `faststream-0.5.6/.github/workflows/update_release_notes.yaml` & `faststream-0.5.7/.github/workflows/update_release_notes.yaml`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/examples/e02_1_basic_publisher.py` & `faststream-0.5.7/examples/e02_1_basic_publisher.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/examples/e02_2_basic_publisher.py` & `faststream-0.5.7/examples/e02_2_basic_publisher.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/examples/e02_3_basic_publisher.py` & `faststream-0.5.7/examples/e02_3_basic_publisher.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/examples/e03_miltiple_pubsub.py` & `faststream-0.5.7/examples/e03_miltiple_pubsub.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/examples/e04_msg_filter.py` & `faststream-0.5.7/examples/e04_msg_filter.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/examples/e07_ack_immediately.py` & `faststream-0.5.7/examples/e07_ack_immediately.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/examples/e09_testing_mocks.py` & `faststream-0.5.7/examples/e09_testing_mocks.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/examples/e10_middlewares.py` & `faststream-0.5.7/examples/e10_middlewares.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/examples/e11_settings.py` & `faststream-0.5.7/examples/e11_settings.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/examples/fastapi_integration/testing.py` & `faststream-0.5.7/examples/fastapi_integration/testing.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/examples/howto/structlogs.py` & `faststream-0.5.7/examples/howto/structlogs.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/examples/kafka/testing.py` & `faststream-0.5.7/examples/kafka/testing.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/examples/nats/e03_publisher.py` & `faststream-0.5.7/examples/nats/e03_publisher.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/examples/nats/e04_js_basic.py` & `faststream-0.5.7/examples/nats/e04_js_basic.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/examples/nats/e05_basic_and_js.py` & `faststream-0.5.7/examples/nats/e05_basic_and_js.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/examples/nats/e06_key_value.py` & `faststream-0.5.7/examples/nats/e06_key_value.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/examples/nats/e07_object_storage.py` & `faststream-0.5.7/examples/nats/e07_object_storage.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/examples/rabbit/direct.py` & `faststream-0.5.7/examples/rabbit/direct.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/examples/rabbit/fanout.py` & `faststream-0.5.7/examples/rabbit/fanout.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/examples/rabbit/header.py` & `faststream-0.5.7/examples/rabbit/header.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/examples/rabbit/topic.py` & `faststream-0.5.7/examples/rabbit/topic.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/examples/redis/channel_sub_pattern.py` & `faststream-0.5.7/examples/redis/channel_sub_pattern.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/examples/redis/rpc.py` & `faststream-0.5.7/examples/redis/rpc.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/examples/router/basic_publish.py` & `faststream-0.5.7/examples/router/basic_publish.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/examples/serialization/avro/avro.py` & `faststream-0.5.7/examples/serialization/avro/avro.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/examples/serialization/msgpack/pack.py` & `faststream-0.5.7/examples/serialization/msgpack/pack.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/examples/serialization/protobuf/protobuf.py` & `faststream-0.5.7/examples/serialization/protobuf/protobuf.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/__init__.py` & `faststream-0.5.7/faststream/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/_compat.py` & `faststream-0.5.7/faststream/_compat.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/app.py` & `faststream-0.5.7/faststream/app.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/exceptions.py` & `faststream-0.5.7/faststream/exceptions.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/security.py` & `faststream-0.5.7/faststream/security.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/types.py` & `faststream-0.5.7/faststream/types.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/asyncapi/abc.py` & `faststream-0.5.7/faststream/asyncapi/abc.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/asyncapi/generate.py` & `faststream-0.5.7/faststream/asyncapi/generate.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/asyncapi/message.py` & `faststream-0.5.7/faststream/asyncapi/message.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/asyncapi/proto.py` & `faststream-0.5.7/faststream/asyncapi/proto.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/asyncapi/site.py` & `faststream-0.5.7/faststream/asyncapi/site.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/asyncapi/utils.py` & `faststream-0.5.7/faststream/asyncapi/utils.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/asyncapi/schema/__init__.py` & `faststream-0.5.7/faststream/asyncapi/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/asyncapi/schema/channels.py` & `faststream-0.5.7/faststream/asyncapi/schema/channels.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/asyncapi/schema/info.py` & `faststream-0.5.7/faststream/asyncapi/schema/info.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/asyncapi/schema/main.py` & `faststream-0.5.7/faststream/asyncapi/schema/main.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/asyncapi/schema/message.py` & `faststream-0.5.7/faststream/asyncapi/schema/message.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/asyncapi/schema/operations.py` & `faststream-0.5.7/faststream/asyncapi/schema/operations.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/asyncapi/schema/security.py` & `faststream-0.5.7/faststream/asyncapi/schema/security.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/asyncapi/schema/servers.py` & `faststream-0.5.7/faststream/asyncapi/schema/servers.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/asyncapi/schema/utils.py` & `faststream-0.5.7/faststream/asyncapi/schema/utils.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/asyncapi/schema/bindings/amqp.py` & `faststream-0.5.7/faststream/asyncapi/schema/bindings/amqp.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/asyncapi/schema/bindings/kafka.py` & `faststream-0.5.7/faststream/asyncapi/schema/bindings/kafka.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/asyncapi/schema/bindings/main.py` & `faststream-0.5.7/faststream/asyncapi/schema/bindings/main.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/asyncapi/schema/bindings/nats.py` & `faststream-0.5.7/faststream/asyncapi/schema/bindings/nats.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/asyncapi/schema/bindings/redis.py` & `faststream-0.5.7/faststream/asyncapi/schema/bindings/redis.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/asyncapi/schema/bindings/sqs.py` & `faststream-0.5.7/faststream/asyncapi/schema/bindings/sqs.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/broker/acknowledgement_watcher.py` & `faststream-0.5.7/faststream/broker/acknowledgement_watcher.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/broker/message.py` & `faststream-0.5.7/faststream/broker/message.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/broker/router.py` & `faststream-0.5.7/faststream/broker/router.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/broker/schemas.py` & `faststream-0.5.7/faststream/broker/schemas.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/broker/types.py` & `faststream-0.5.7/faststream/broker/types.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/broker/utils.py` & `faststream-0.5.7/faststream/broker/utils.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/broker/core/abc.py` & `faststream-0.5.7/faststream/broker/core/abc.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,18 +103,18 @@
                     h.include_in_schema = include_in_schema
 
                 h._broker_middlewares = (
                     *self._middlewares,
                     *middlewares,
                     *h._broker_middlewares,
                 )
-                h._broker_dependecies = (
+                h._broker_dependencies = (
                     *self._dependencies,
                     *dependencies,
-                    *h._broker_dependecies,
+                    *h._broker_dependencies,
                 )
                 self._subscribers = {**self._subscribers, key: h}
 
         for p in router._publishers.values():
             p.add_prefix(self.prefix)
 
             if (key := hash(p)) not in self._publishers:
```

### Comparing `faststream-0.5.6/faststream/broker/core/logging.py` & `faststream-0.5.7/faststream/broker/core/logging.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/broker/core/usecase.py` & `faststream-0.5.7/faststream/broker/core/usecase.py`

 * *Files 15% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     from types import TracebackType
 
     from fast_depends.dependencies import Depends
 
     from faststream.asyncapi.schema import Tag, TagDict
     from faststream.broker.publisher.proto import ProducerProto, PublisherProto
     from faststream.security import BaseSecurity
-    from faststream.types import AnyDict, AsyncFunc, Decorator, LoggerProto
+    from faststream.types import AnyDict, Decorator, LoggerProto
 
 
 class BrokerUsecase(
     LoggingBroker[MsgType],
     SetupAble,
     Generic[MsgType, ConnectionType],
 ):
@@ -238,50 +238,50 @@
 
     def setup_subscriber(
         self,
         subscriber: SubscriberProto[MsgType],
         **kwargs: Any,
     ) -> None:
         """Setup the Subscriber to prepare it to starting."""
-        subscriber.setup(
-            logger=self.logger,
-            producer=self._producer,
-            graceful_timeout=self.graceful_timeout,
-            extra_context={},
-            # broker options
-            broker_parser=self._parser,
-            broker_decoder=self._decoder,
-            # dependant args
-            apply_types=self._is_apply_types,
-            is_validate=self._is_validate,
-            _get_dependant=self._get_dependant,
-            _call_decorators=self._call_decorators,
-            **self._subscriber_setup_extra,
-            **kwargs,
-        )
+        data = self._subscriber_setup_extra.copy()
+        data.update(kwargs)
+        subscriber.setup(**data)
 
     def setup_publisher(
         self,
         publisher: "PublisherProto[MsgType]",
         **kwargs: Any,
     ) -> None:
         """Setup the Publisher to prepare it to starting."""
-        publisher.setup(
-            producer=self._producer,
-            **self._publisher_setup_extra,
-            **kwargs,
-        )
+        data = self._publisher_setup_extra.copy()
+        data.update(kwargs)
+        publisher.setup(**data)
 
     @property
     def _subscriber_setup_extra(self) -> "AnyDict":
-        return {}
+        return {
+            "logger": self.logger,
+            "producer": self._producer,
+            "graceful_timeout": self.graceful_timeout,
+            "extra_context": {},
+            # broker options
+            "broker_parser": self._parser,
+            "broker_decoder": self._decoder,
+            # dependant args
+            "apply_types": self._is_apply_types,
+            "is_validate": self._is_validate,
+            "_get_dependant": self._get_dependant,
+            "_call_decorators": self._call_decorators,
+        }
 
     @property
     def _publisher_setup_extra(self) -> "AnyDict":
-        return {}
+        return {
+            "producer": self._producer,
+        }
 
     def publisher(self, *args: Any, **kwargs: Any) -> "PublisherProto[MsgType]":
         pub = super().publisher(*args, **kwargs)
         if self.running:
             self.setup_publisher(pub)
         return pub
 
@@ -329,14 +329,15 @@
         self,
         msg: Any,
         *,
         producer: Optional["ProducerProto"],
         **kwargs: Any,
     ) -> Optional[Any]:
         """Publish message directly."""
-        assert producer, NOT_CONNECTED_YET  # nosec B101)
+        assert producer, NOT_CONNECTED_YET  # nosec B101
+
+        publish = producer.publish
 
-        publish: "AsyncFunc" = producer.publish
         for m in self._middlewares:
             publish = partial(m(None).publish_scope, publish)
 
         return await publish(msg, **kwargs)
```

### Comparing `faststream-0.5.6/faststream/broker/fastapi/context.py` & `faststream-0.5.7/faststream/broker/fastapi/context.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/broker/fastapi/get_dependant.py` & `faststream-0.5.7/faststream/broker/fastapi/get_dependant.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/broker/fastapi/route.py` & `faststream-0.5.7/faststream/broker/fastapi/route.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/broker/fastapi/router.py` & `faststream-0.5.7/faststream/broker/fastapi/router.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/broker/middlewares/base.py` & `faststream-0.5.7/faststream/broker/middlewares/base.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/broker/middlewares/logging.py` & `faststream-0.5.7/faststream/broker/middlewares/logging.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/broker/publisher/fake.py` & `faststream-0.5.7/faststream/broker/publisher/fake.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/broker/publisher/proto.py` & `faststream-0.5.7/faststream/broker/publisher/proto.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/broker/publisher/usecase.py` & `faststream-0.5.7/faststream/broker/publisher/usecase.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/broker/subscriber/call_item.py` & `faststream-0.5.7/faststream/broker/subscriber/call_item.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/broker/subscriber/proto.py` & `faststream-0.5.7/faststream/broker/subscriber/proto.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     AsyncAPIProto,
     EndpointProto,
     WrapperProto[MsgType],
 ):
     calls: List["HandlerItem[MsgType]"]
     running: bool
 
-    _broker_dependecies: Iterable["Depends"]
+    _broker_dependencies: Iterable["Depends"]
     _broker_middlewares: Iterable["BrokerMiddleware[MsgType]"]
     _producer: Optional["ProducerProto"]
 
     @abstractmethod
     def add_middleware(self, middleware: "BrokerMiddleware[MsgType]") -> None: ...
 
     @staticmethod
```

### Comparing `faststream-0.5.6/faststream/broker/subscriber/usecase.py` & `faststream-0.5.7/faststream/broker/subscriber/usecase.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,15 @@
     """A class representing an asynchronous handler."""
 
     lock: ContextManager[Any]
     extra_watcher_options: "AnyDict"
     extra_context: "AnyDict"
     graceful_timeout: Optional[float]
 
-    _broker_dependecies: Iterable["Depends"]
+    _broker_dependencies: Iterable["Depends"]
     _call_options: Optional["_CallOptions"]
 
     def __init__(
         self,
         *,
         no_ack: bool,
         retry: Union[bool, int],
@@ -113,15 +113,15 @@
         self._retry = retry
 
         self._call_options = None
         self.running = False
         self.lock = sync_fake_context()
 
         # Setup in include
-        self._broker_dependecies = broker_dependencies
+        self._broker_dependencies = broker_dependencies
         self._broker_middlewares = broker_middlewares
 
         # register in setup later
         self._producer = None
         self.graceful_timeout = None
         self.extra_context = {}
         self.extra_watcher_options = {}
@@ -137,29 +137,29 @@
     @override
     def setup(  # type: ignore[override]
         self,
         *,
         logger: Optional["LoggerProto"],
         producer: Optional[ProducerProto],
         graceful_timeout: Optional[float],
-        extra_context: Optional["AnyDict"],
+        extra_context: "AnyDict",
         # broker options
         broker_parser: Optional["CustomCallable"],
         broker_decoder: Optional["CustomCallable"],
         # dependant args
         apply_types: bool,
         is_validate: bool,
         _get_dependant: Optional[Callable[..., Any]],
         _call_decorators: Iterable["Decorator"],
     ) -> None:
         self.lock = MultiLock()
 
         self._producer = producer
         self.graceful_timeout = graceful_timeout
-        self.extra_context = extra_context or {}
+        self.extra_context = extra_context
 
         self.watcher = get_watcher_context(logger, self._no_ack, self._retry)
 
         for call in self.calls:
             if parser := call.item_parser or broker_parser:
                 async_parser = resolve_custom_func(
                     to_async(parser), self._default_parser
@@ -177,15 +177,15 @@
             call.setup(
                 parser=async_parser,
                 decoder=async_decoder,
                 apply_types=apply_types,
                 is_validate=is_validate,
                 _get_dependant=_get_dependant,
                 _call_decorators=_call_decorators,
-                broker_dependencies=self._broker_dependecies,
+                broker_dependencies=self._broker_dependencies,
             )
 
             call.handler.refresh(with_mock=False)
 
     @abstractmethod
     async def start(self) -> None:
         """Start the handler."""
```

### Comparing `faststream-0.5.6/faststream/broker/wrapper/call.py` & `faststream-0.5.7/faststream/broker/wrapper/call.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/broker/wrapper/proto.py` & `faststream-0.5.7/faststream/broker/wrapper/proto.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/cli/main.py` & `faststream-0.5.7/faststream/cli/main.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/cli/docs/app.py` & `faststream-0.5.7/faststream/cli/docs/app.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/cli/supervisors/basereload.py` & `faststream-0.5.7/faststream/cli/supervisors/basereload.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/cli/supervisors/multiprocess.py` & `faststream-0.5.7/faststream/cli/supervisors/multiprocess.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/cli/supervisors/utils.py` & `faststream-0.5.7/faststream/cli/supervisors/utils.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/cli/supervisors/watchfiles.py` & `faststream-0.5.7/faststream/cli/supervisors/watchfiles.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/cli/utils/imports.py` & `faststream-0.5.7/faststream/cli/utils/imports.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/cli/utils/logs.py` & `faststream-0.5.7/faststream/cli/utils/logs.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/cli/utils/parser.py` & `faststream-0.5.7/faststream/cli/utils/parser.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/confluent/annotations.py` & `faststream-0.5.7/faststream/confluent/annotations.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/confluent/client.py` & `faststream-0.5.7/faststream/confluent/client.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/confluent/message.py` & `faststream-0.5.7/faststream/confluent/message.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/confluent/parser.py` & `faststream-0.5.7/faststream/confluent/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         body: List[Any] = []
         batch_headers: List[Dict[str, str]] = []
 
         first = message[0]
         last = message[-1]
 
         for m in message:
-            body.append(m.value)
+            body.append(m.value())
             batch_headers.append(_parse_msg_headers(m.headers()))
 
         headers = next(iter(batch_headers), {})
 
         _, first_timestamp = first.timestamp()
 
         handler: Optional["LogicSubscriber[Any]"] = context.get_local("handler_")
```

### Comparing `faststream-0.5.6/faststream/confluent/router.py` & `faststream-0.5.7/faststream/confluent/router.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import (
     TYPE_CHECKING,
     Any,
+    Awaitable,
     Callable,
     Dict,
     Iterable,
     Literal,
     Optional,
     Sequence,
     Tuple,
@@ -125,15 +126,18 @@
 
 class KafkaRoute(SubscriberRoute):
     """Class to store delaied KafkaBroker subscriber registration."""
 
     def __init__(
         self,
         call: Annotated[
-            Callable[..., "SendableMessage"],
+            Union[
+                Callable[..., "SendableMessage"],
+                Callable[..., Awaitable["SendableMessage"]],
+            ],
             Doc("Message handler function."),
         ],
         *topics: Annotated[
             str,
             Doc("Kafka topics to consume messages from."),
         ],
         publishers: Annotated[
```

### Comparing `faststream-0.5.6/faststream/confluent/security.py` & `faststream-0.5.7/faststream/confluent/security.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/confluent/testing.py` & `faststream-0.5.7/faststream/confluent/testing.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/confluent/broker/broker.py` & `faststream-0.5.7/faststream/confluent/broker/broker.py`

 * *Files 1% similar despite different names*

```diff
@@ -468,14 +468,15 @@
                 extra=handler.get_log_context(None),
             )
             await handler.start()
 
     @property
     def _subscriber_setup_extra(self) -> "AnyDict":
         return {
+            **super()._subscriber_setup_extra,
             "client_id": self.client_id,
             "builder": self._connection,
         }
 
     @override
     async def publish(  # type: ignore[override]
         self,
```

### Comparing `faststream-0.5.6/faststream/confluent/broker/logging.py` & `faststream-0.5.7/faststream/confluent/broker/logging.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/confluent/broker/registrator.py` & `faststream-0.5.7/faststream/confluent/broker/registrator.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/confluent/fastapi/__init__.py` & `faststream-0.5.7/faststream/confluent/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/confluent/fastapi/fastapi.py` & `faststream-0.5.7/faststream/confluent/fastapi/fastapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/confluent/publisher/asyncapi.py` & `faststream-0.5.7/faststream/confluent/publisher/asyncapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/confluent/publisher/producer.py` & `faststream-0.5.7/faststream/confluent/publisher/producer.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/confluent/publisher/usecase.py` & `faststream-0.5.7/faststream/confluent/publisher/usecase.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/confluent/schemas/params.py` & `faststream-0.5.7/faststream/confluent/schemas/params.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/confluent/subscriber/asyncapi.py` & `faststream-0.5.7/faststream/confluent/subscriber/asyncapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/confluent/subscriber/usecase.py` & `faststream-0.5.7/faststream/confluent/subscriber/usecase.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
         *,
         client_id: Optional[str],
         builder: Callable[..., "AsyncConfluentConsumer"],
         # basic args
         logger: Optional["LoggerProto"],
         producer: Optional["ProducerProto"],
         graceful_timeout: Optional[float],
-        extra_context: Optional["AnyDict"],
+        extra_context: "AnyDict",
         # broker options
         broker_parser: Optional["CustomCallable"],
         broker_decoder: Optional["CustomCallable"],
         # dependant args
         apply_types: bool,
         is_validate: bool,
         _get_dependant: Optional[Callable[..., Any]],
```

### Comparing `faststream-0.5.6/faststream/kafka/annotations.py` & `faststream-0.5.7/faststream/kafka/annotations.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/kafka/message.py` & `faststream-0.5.7/faststream/kafka/message.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/kafka/parser.py` & `faststream-0.5.7/faststream/kafka/parser.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/kafka/router.py` & `faststream-0.5.7/faststream/kafka/router.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import (
     TYPE_CHECKING,
     Any,
+    Awaitable,
     Callable,
     Dict,
     Iterable,
     Literal,
     Optional,
     Sequence,
     Tuple,
@@ -128,15 +129,18 @@
 
 class KafkaRoute(SubscriberRoute):
     """Class to store delayed KafkaBroker subscriber registration."""
 
     def __init__(
         self,
         call: Annotated[
-            Callable[..., "SendableMessage"],
+            Union[
+                Callable[..., "SendableMessage"],
+                Callable[..., Awaitable["SendableMessage"]],
+            ],
             Doc(
                 "Message handler function "
                 "to wrap the same with `@broker.subscriber(...)` way."
             ),
         ],
         *topics: Annotated[
             str,
```

### Comparing `faststream-0.5.6/faststream/kafka/security.py` & `faststream-0.5.7/faststream/kafka/security.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/kafka/testing.py` & `faststream-0.5.7/faststream/kafka/testing.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/kafka/broker/broker.py` & `faststream-0.5.7/faststream/kafka/broker/broker.py`

 * *Files 0% similar despite different names*

```diff
@@ -530,14 +530,15 @@
             log_fmt=log_fmt,
             # FastDepends args
             _get_dependant=_get_dependant,
             _call_decorators=_call_decorators,
             apply_types=apply_types,
             validate=validate,
         )
+
         self.client_id = client_id
         self._producer = None
 
     async def _close(
         self,
         exc_type: Optional[Type[BaseException]] = None,
         exc_val: Optional[BaseException] = None,
@@ -608,14 +609,15 @@
                 extra=handler.get_log_context(None),
             )
             await handler.start()
 
     @property
     def _subscriber_setup_extra(self) -> "AnyDict":
         return {
+            **super()._subscriber_setup_extra,
             "client_id": self.client_id,
             "builder": self._connection,
         }
 
     @override
     async def publish(  # type: ignore[override]
         self,
```

### Comparing `faststream-0.5.6/faststream/kafka/broker/logging.py` & `faststream-0.5.7/faststream/kafka/broker/logging.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/kafka/broker/registrator.py` & `faststream-0.5.7/faststream/kafka/broker/registrator.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/kafka/fastapi/__init__.py` & `faststream-0.5.7/faststream/kafka/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/kafka/fastapi/fastapi.py` & `faststream-0.5.7/faststream/kafka/fastapi/fastapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/kafka/publisher/asyncapi.py` & `faststream-0.5.7/faststream/kafka/publisher/asyncapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/kafka/publisher/producer.py` & `faststream-0.5.7/faststream/kafka/publisher/producer.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/kafka/publisher/usecase.py` & `faststream-0.5.7/faststream/kafka/publisher/usecase.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/kafka/schemas/params.py` & `faststream-0.5.7/faststream/kafka/schemas/params.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/kafka/subscriber/asyncapi.py` & `faststream-0.5.7/faststream/kafka/subscriber/asyncapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/kafka/subscriber/usecase.py` & `faststream-0.5.7/faststream/kafka/subscriber/usecase.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,15 @@
         *,
         client_id: Optional[str],
         builder: Callable[..., "AIOKafkaConsumer"],
         # basic args
         logger: Optional["LoggerProto"],
         producer: Optional["ProducerProto"],
         graceful_timeout: Optional[float],
-        extra_context: Optional["AnyDict"],
+        extra_context: "AnyDict",
         # broker options
         broker_parser: Optional["CustomCallable"],
         broker_decoder: Optional["CustomCallable"],
         # dependant args
         apply_types: bool,
         is_validate: bool,
         _get_dependant: Optional[Callable[..., Any]],
```

### Comparing `faststream-0.5.6/faststream/log/formatter.py` & `faststream-0.5.7/faststream/log/formatter.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/log/logging.py` & `faststream-0.5.7/faststream/log/logging.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/nats/__init__.py` & `faststream-0.5.7/faststream/nats/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/nats/annotations.py` & `faststream-0.5.7/faststream/nats/annotations.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/nats/helpers.py` & `faststream-0.5.7/faststream/nats/helpers.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/nats/message.py` & `faststream-0.5.7/faststream/nats/message.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/nats/parser.py` & `faststream-0.5.7/faststream/nats/parser.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/nats/router.py` & `faststream-0.5.7/faststream/nats/router.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,17 @@
-from typing import TYPE_CHECKING, Any, Callable, Dict, Iterable, Optional, Union
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Awaitable,
+    Callable,
+    Dict,
+    Iterable,
+    Optional,
+    Union,
+)
 
 from nats.js import api
 from typing_extensions import Annotated, Doc, deprecated
 
 from faststream.broker.router import ArgsContainer, BrokerRouter, SubscriberRoute
 from faststream.broker.utils import default_filter
 from faststream.nats.broker.registrator import NatsRegistrator
@@ -102,15 +111,18 @@
 
 class NatsRoute(SubscriberRoute):
     """Class to store delayed NatsBroker subscriber registration."""
 
     def __init__(
         self,
         call: Annotated[
-            Callable[..., "SendableMessage"],
+            Union[
+                Callable[..., "SendableMessage"],
+                Callable[..., Awaitable["SendableMessage"]],
+            ],
             Doc(
                 "Message handler function "
                 "to wrap the same with `@broker.subscriber(...)` way."
             ),
         ],
         subject: Annotated[
             str,
```

### Comparing `faststream-0.5.6/faststream/nats/security.py` & `faststream-0.5.7/faststream/nats/security.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/nats/testing.py` & `faststream-0.5.7/faststream/nats/testing.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/nats/broker/broker.py` & `faststream-0.5.7/faststream/nats/broker/broker.py`

 * *Files 2% similar despite different names*

```diff
@@ -713,40 +713,40 @@
         """Publish message directly.
 
         This method allows you to publish message in not AsyncAPI-documented way. You can use it in another frameworks
         applications or to publish messages from time to time.
 
         Please, use `@broker.publisher(...)` or `broker.publisher(...).publish(...)` instead in a regular way.
         """
-        publihs_kwargs = {
+        publish_kwargs = {
             "subject": subject,
             "headers": headers,
             "reply_to": reply_to,
             "correlation_id": correlation_id or gen_cor_id(),
             "rpc": rpc,
             "rpc_timeout": rpc_timeout,
             "raise_timeout": raise_timeout,
         }
 
         producer: Optional[ProducerProto]
         if stream is None:
             producer = self._producer
         else:
             producer = self._js_producer
-            publihs_kwargs.update(
+            publish_kwargs.update(
                 {
                     "stream": stream,
                     "timeout": timeout,
                 }
             )
 
         return await super().publish(
             message,
             producer=producer,
-            **publihs_kwargs,
+            **publish_kwargs,
         )
 
     @override
     def setup_subscriber(  # type: ignore[override]
         self,
         subscriber: "AsyncAPISubscriber",
     ) -> None:
@@ -766,18 +766,15 @@
         if publisher.stream is not None:
             if self._js_producer is not None:
                 producer = self._js_producer
 
         elif self._producer is not None:
             producer = self._producer
 
-        publisher.setup(
-            producer=producer,
-            **self._publisher_setup_extra,
-        )
+        super().setup_publisher(publisher, producer=producer)
 
     def _log_connection_broken(
         self,
         error_cb: Optional["ErrorCallback"] = None,
     ) -> "ErrorCallback":
         c = AsyncAPISubscriber.build_log_context(None, "")
```

### Comparing `faststream-0.5.6/faststream/nats/broker/logging.py` & `faststream-0.5.7/faststream/nats/broker/logging.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/nats/broker/registrator.py` & `faststream-0.5.7/faststream/nats/broker/registrator.py`

 * *Files 2% similar despite different names*

```diff
@@ -186,15 +186,15 @@
         """Creates NATS subscriber object.
 
         You can use it as a handler decorator `@broker.subscriber(...)`.
         """
         subscriber = cast(
             AsyncAPISubscriber,
             super().subscriber(
-                AsyncAPISubscriber.create(
+                AsyncAPISubscriber.create(  # type: ignore[arg-type]
                     subject=subject,
                     queue=queue,
                     stream=stream,
                     pull_sub=pull_sub,
                     max_workers=max_workers,
                     # extra args
                     pending_msgs_limit=pending_msgs_limit,
```

### Comparing `faststream-0.5.6/faststream/nats/fastapi/__init__.py` & `faststream-0.5.7/faststream/nats/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/nats/fastapi/fastapi.py` & `faststream-0.5.7/faststream/nats/fastapi/fastapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/nats/publisher/asyncapi.py` & `faststream-0.5.7/faststream/nats/publisher/asyncapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/nats/publisher/producer.py` & `faststream-0.5.7/faststream/nats/publisher/producer.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/nats/publisher/usecase.py` & `faststream-0.5.7/faststream/nats/publisher/usecase.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/nats/schemas/js_stream.py` & `faststream-0.5.7/faststream/nats/schemas/js_stream.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/nats/schemas/pull_sub.py` & `faststream-0.5.7/faststream/nats/schemas/pull_sub.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/nats/subscriber/asyncapi.py` & `faststream-0.5.7/faststream/nats/subscriber/asyncapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -184,13 +184,13 @@
                 # AsyncAPI information
                 title_=title_,
                 description_=description_,
                 include_in_schema=include_in_schema,
             )
 
 
-class AsyncAPIDefaultSubscriber(AsyncAPISubscriber, DefaultHandler):
+class AsyncAPIDefaultSubscriber(DefaultHandler, AsyncAPISubscriber):
     """One-message consumer with AsyncAPI methods."""
 
 
-class AsyncAPIBatchSubscriber(AsyncAPISubscriber, BatchHandler):
+class AsyncAPIBatchSubscriber(BatchHandler, AsyncAPISubscriber):
     """Batch-message consumer with AsyncAPI methods."""
```

### Comparing `faststream-0.5.6/faststream/nats/subscriber/usecase.py` & `faststream-0.5.7/faststream/nats/subscriber/usecase.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,15 @@
         self,
         *,
         connection: Union["Client", "JetStreamContext"],
         # basic args
         logger: Optional["LoggerProto"],
         producer: Optional["ProducerProto"],
         graceful_timeout: Optional[float],
-        extra_context: Optional["AnyDict"],
+        extra_context: "AnyDict",
         # broker options
         broker_parser: Optional["CustomCallable"],
         broker_decoder: Optional["CustomCallable"],
         # dependant args
         apply_types: bool,
         is_validate: bool,
         _get_dependant: Optional[Callable[..., Any]],
```

### Comparing `faststream-0.5.6/faststream/rabbit/__init__.py` & `faststream-0.5.7/faststream/rabbit/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/rabbit/annotations.py` & `faststream-0.5.7/faststream/rabbit/annotations.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/rabbit/message.py` & `faststream-0.5.7/faststream/rabbit/message.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/rabbit/parser.py` & `faststream-0.5.7/faststream/rabbit/parser.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/rabbit/router.py` & `faststream-0.5.7/faststream/rabbit/router.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TYPE_CHECKING, Any, Callable, Iterable, Optional, Union
+from typing import TYPE_CHECKING, Any, Awaitable, Callable, Iterable, Optional, Union
 
 from typing_extensions import Annotated, Doc, deprecated
 
 from faststream.broker.router import ArgsContainer, BrokerRouter, SubscriberRoute
 from faststream.broker.utils import default_filter
 from faststream.rabbit.broker.registrator import RabbitRegistrator
 
@@ -173,15 +173,18 @@
 
     Just a copy of `RabbitRegistrator.subscriber(...)` arguments.
     """
 
     def __init__(
         self,
         call: Annotated[
-            Callable[..., "AioPikaSendableMessage"],
+            Union[
+                Callable[..., "AioPikaSendableMessage"],
+                Callable[..., Awaitable["AioPikaSendableMessage"]],
+            ],
             Doc(
                 "Message handler function "
                 "to wrap the same with `@broker.subscriber(...)` way."
             ),
         ],
         queue: Annotated[
             Union[str, "RabbitQueue"],
```

### Comparing `faststream-0.5.6/faststream/rabbit/security.py` & `faststream-0.5.7/faststream/rabbit/security.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/rabbit/testing.py` & `faststream-0.5.7/faststream/rabbit/testing.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/rabbit/utils.py` & `faststream-0.5.7/faststream/rabbit/utils.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/rabbit/broker/broker.py` & `faststream-0.5.7/faststream/rabbit/broker/broker.py`

 * *Files 1% similar despite different names*

```diff
@@ -274,22 +274,24 @@
 
         self._channel = None
         self.declarer = None
 
     @property
     def _subscriber_setup_extra(self) -> "AnyDict":
         return {
+            **super()._subscriber_setup_extra,
             "app_id": self.app_id,
             "virtual_host": self.virtual_host,
             "declarer": self.declarer,
         }
 
     @property
     def _publisher_setup_extra(self) -> "AnyDict":
         return {
+            **super()._publisher_setup_extra,
             "app_id": self.app_id,
             "virtual_host": self.virtual_host,
         }
 
     @override
     async def connect(  # type: ignore[override]
         self,
```

### Comparing `faststream-0.5.6/faststream/rabbit/broker/logging.py` & `faststream-0.5.7/faststream/rabbit/broker/logging.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/rabbit/broker/registrator.py` & `faststream-0.5.7/faststream/rabbit/broker/registrator.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/rabbit/fastapi/__init__.py` & `faststream-0.5.7/faststream/rabbit/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/rabbit/fastapi/router.py` & `faststream-0.5.7/faststream/rabbit/fastapi/router.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/rabbit/publisher/asyncapi.py` & `faststream-0.5.7/faststream/rabbit/publisher/asyncapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/rabbit/publisher/producer.py` & `faststream-0.5.7/faststream/rabbit/publisher/producer.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/rabbit/publisher/usecase.py` & `faststream-0.5.7/faststream/rabbit/publisher/usecase.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,17 +93,18 @@
 
 class LogicPublisher(
     PublisherUsecase[IncomingMessage],
     BaseRMQInformation,
 ):
     """A class to represent a RabbitMQ publisher."""
 
-    _producer: Optional["AioPikaFastProducer"]
     app_id: Optional[str]
 
+    _producer: Optional["AioPikaFastProducer"]
+
     def __init__(
         self,
         *,
         routing_key: str,
         queue: "RabbitQueue",
         exchange: Optional["RabbitExchange"],
         message_kwargs: "PublishKwargs",
```

### Comparing `faststream-0.5.6/faststream/rabbit/schemas/constants.py` & `faststream-0.5.7/faststream/rabbit/schemas/constants.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/rabbit/schemas/exchange.py` & `faststream-0.5.7/faststream/rabbit/schemas/exchange.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/rabbit/schemas/queue.py` & `faststream-0.5.7/faststream/rabbit/schemas/queue.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/rabbit/schemas/reply.py` & `faststream-0.5.7/faststream/rabbit/schemas/reply.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/rabbit/subscriber/asyncapi.py` & `faststream-0.5.7/faststream/rabbit/subscriber/asyncapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/rabbit/subscriber/usecase.py` & `faststream-0.5.7/faststream/rabbit/subscriber/usecase.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,15 +100,15 @@
         app_id: Optional[str],
         virtual_host: str,
         declarer: "RabbitDeclarer",
         # basic args
         logger: Optional["LoggerProto"],
         producer: Optional["AioPikaFastProducer"],
         graceful_timeout: Optional[float],
-        extra_context: Optional["AnyDict"],
+        extra_context: "AnyDict",
         # broker options
         broker_parser: Optional["CustomCallable"],
         broker_decoder: Optional["CustomCallable"],
         # dependant args
         apply_types: bool,
         is_validate: bool,
         _get_dependant: Optional[Callable[..., Any]],
```

### Comparing `faststream-0.5.6/faststream/redis/__init__.py` & `faststream-0.5.7/faststream/redis/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/redis/annotations.py` & `faststream-0.5.7/faststream/redis/annotations.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/redis/message.py` & `faststream-0.5.7/faststream/redis/message.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/redis/parser.py` & `faststream-0.5.7/faststream/redis/parser.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/redis/router.py` & `faststream-0.5.7/faststream/redis/router.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TYPE_CHECKING, Any, Callable, Iterable, Optional, Union
+from typing import TYPE_CHECKING, Any, Awaitable, Callable, Iterable, Optional, Union
 
 from typing_extensions import Annotated, Doc, deprecated
 
 from faststream.broker.router import ArgsContainer, BrokerRouter, SubscriberRoute
 from faststream.broker.utils import default_filter
 from faststream.redis.broker.registrator import RedisRegistrator
 from faststream.redis.message import BaseMessage
@@ -95,15 +95,18 @@
 
 class RedisRoute(SubscriberRoute):
     """Class to store delayed RedisBroker subscriber registration."""
 
     def __init__(
         self,
         call: Annotated[
-            Callable[..., "SendableMessage"],
+            Union[
+                Callable[..., "SendableMessage"],
+                Callable[..., Awaitable["SendableMessage"]],
+            ],
             Doc(
                 "Message handler function "
                 "to wrap the same with `@broker.subscriber(...)` way."
             ),
         ],
         channel: Annotated[
             Union["PubSub", str, None],
```

### Comparing `faststream-0.5.6/faststream/redis/security.py` & `faststream-0.5.7/faststream/redis/security.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/redis/testing.py` & `faststream-0.5.7/faststream/redis/testing.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,14 +179,15 @@
 
         return None
 
     async def publish_batch(
         self,
         *msgs: "SendableMessage",
         list: str,
+        headers: Optional["AnyDict"] = None,
         correlation_id: Optional[str] = None,
     ) -> None:
         correlation_id = correlation_id or gen_cor_id()
 
         for handler in self.broker._subscribers.values():  # pragma: no branch
             if (
                 list_sub := getattr(handler, "list_sub", None)
@@ -196,14 +197,15 @@
                     message=BatchListMessage(
                         type="blist",
                         channel=list,
                         data=[
                             build_message(
                                 m,
                                 correlation_id=correlation_id,
+                                headers=headers,
                             )
                             for m in msgs
                         ],
                     ),
                 )
 
         return None
```

### Comparing `faststream-0.5.6/faststream/redis/broker/broker.py` & `faststream-0.5.7/faststream/redis/broker/broker.py`

 * *Files 2% similar despite different names*

```diff
@@ -259,15 +259,15 @@
         """Connect to the Redis server."""
         if url is not Parameter.empty:
             connect_kwargs: "AnyDict" = {
                 "url": url,
                 **kwargs,
             }
         else:
-            connect_kwargs = {**kwargs}
+            connect_kwargs = dict(kwargs).copy()
 
         return await super().connect(**connect_kwargs)
 
     @override
     async def _connect(  # type: ignore[override]
         self,
         url: str,
@@ -355,14 +355,15 @@
                 extra=handler.get_log_context(None),
             )
             await handler.start()
 
     @property
     def _subscriber_setup_extra(self) -> "AnyDict":
         return {
+            **super()._subscriber_setup_extra,
             "connection": self._connection,
         }
 
     @override
     async def publish(  # type: ignore[override]
         self,
         message: Annotated[
```

### Comparing `faststream-0.5.6/faststream/redis/broker/logging.py` & `faststream-0.5.7/faststream/redis/broker/logging.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/redis/broker/registrator.py` & `faststream-0.5.7/faststream/redis/broker/registrator.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/redis/fastapi/__init__.py` & `faststream-0.5.7/faststream/redis/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/redis/fastapi/fastapi.py` & `faststream-0.5.7/faststream/redis/fastapi/fastapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/redis/publisher/asyncapi.py` & `faststream-0.5.7/faststream/redis/publisher/asyncapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/redis/publisher/producer.py` & `faststream-0.5.7/faststream/redis/publisher/producer.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,18 +122,19 @@
                 return await self._decoder(await self._parser(m))
 
     async def publish_batch(
         self,
         *msgs: "SendableMessage",
         list: str,
         correlation_id: str,
+        headers: Optional["AnyDict"] = None,
     ) -> None:
         batch = (
             RawMessage.encode(
                 message=msg,
                 correlation_id=correlation_id,
                 reply_to=None,
-                headers=None,
+                headers=headers,
             )
             for msg in msgs
         )
         await self._connection.rpush(list, *batch)
```

### Comparing `faststream-0.5.6/faststream/redis/publisher/usecase.py` & `faststream-0.5.7/faststream/redis/publisher/usecase.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/redis/schemas/list_sub.py` & `faststream-0.5.7/faststream/redis/schemas/list_sub.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/redis/schemas/proto.py` & `faststream-0.5.7/faststream/redis/schemas/proto.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/redis/schemas/pub_sub.py` & `faststream-0.5.7/faststream/redis/schemas/pub_sub.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/redis/schemas/stream_sub.py` & `faststream-0.5.7/faststream/redis/schemas/stream_sub.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/redis/subscriber/asyncapi.py` & `faststream-0.5.7/faststream/redis/subscriber/asyncapi.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/redis/subscriber/usecase.py` & `faststream-0.5.7/faststream/redis/subscriber/usecase.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,15 @@
         self,
         *,
         connection: Optional["Redis[bytes]"],
         # basic args
         logger: Optional["LoggerProto"],
         producer: Optional["ProducerProto"],
         graceful_timeout: Optional[float],
-        extra_context: Optional["AnyDict"],
+        extra_context: "AnyDict",
         # broker options
         broker_parser: Optional["CustomCallable"],
         broker_decoder: Optional["CustomCallable"],
         # dependant args
         apply_types: bool,
         is_validate: bool,
         _get_dependant: Optional[Callable[..., Any]],
```

### Comparing `faststream-0.5.6/faststream/testing/app.py` & `faststream-0.5.7/faststream/testing/app.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/testing/broker.py` & `faststream-0.5.7/faststream/testing/broker.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     Tuple,
     Type,
     TypeVar,
 )
 from unittest.mock import AsyncMock, MagicMock
 
 from faststream.broker.core.usecase import BrokerUsecase
+from faststream.broker.message import StreamMessage, decode_message, encode_message
 from faststream.broker.middlewares.logging import CriticalLogMiddleware
 from faststream.broker.wrapper.call import HandlerCallWrapper
 from faststream.testing.app import TestApp
 from faststream.utils.ast import is_contains_context_name
 from faststream.utils.functions import timeout_scope
 
 if TYPE_CHECKING:
@@ -208,10 +209,15 @@
     raise_timeout: bool = False,
 ) -> Any:
     """Asynchronously call a handler function."""
     with timeout_scope(rpc_timeout, raise_timeout):
         result = await handler.consume(message)
 
         if rpc:
-            return result
+            message_body, content_type = encode_message(result)
+            msg_to_publish = StreamMessage(
+                raw_message=None, body=message_body, content_type=content_type
+            )
+            consumed_data = decode_message(msg_to_publish)
+            return consumed_data
 
     return None
```

### Comparing `faststream-0.5.6/faststream/utils/ast.py` & `faststream-0.5.7/faststream/utils/ast.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/utils/classes.py` & `faststream-0.5.7/faststream/utils/classes.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/utils/data.py` & `faststream-0.5.7/faststream/utils/data.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/utils/functions.py` & `faststream-0.5.7/faststream/utils/functions.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/utils/no_cast.py` & `faststream-0.5.7/faststream/utils/no_cast.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/utils/path.py` & `faststream-0.5.7/faststream/utils/path.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/utils/context/builders.py` & `faststream-0.5.7/faststream/utils/context/builders.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/utils/context/repository.py` & `faststream-0.5.7/faststream/utils/context/repository.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/faststream/utils/context/types.py` & `faststream-0.5.7/faststream/utils/context/types.py`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/scripts/build-docs-pre-commit.sh` & `faststream-0.5.7/scripts/build-docs-pre-commit.sh`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/scripts/lint-pre-commit.sh` & `faststream-0.5.7/scripts/lint-pre-commit.sh`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/scripts/set_variables.sh` & `faststream-0.5.7/scripts/set_variables.sh`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/scripts/static-pre-commit.sh` & `faststream-0.5.7/scripts/static-pre-commit.sh`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/LICENSE` & `faststream-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/README.md` & `faststream-0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `faststream-0.5.6/pyproject.toml` & `faststream-0.5.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,19 @@
 
 confluent = ["confluent-kafka>=2,<3"]
 
 nats = ["nats-py>=2.3.1,<=3.0.0"]
 
 redis = ["redis>=5.0.0,<6.0.0"]
 
+otel = ["opentelemetry-sdk>=1.24.0,<2.0.0"]
+
 # dev dependencies
+optionals = ["faststream[rabbit,kafka,confluent,nats,redis,otel]"]
+
 devdocs = [
     "mkdocs-material==9.5.21",
     "mkdocs-static-i18n==1.2.3",
     "mdx-include==1.4.2",
     "mkdocstrings[python]==0.25.1",
     "mkdocs-literate-nav==0.6.1",
     "mkdocs-git-revision-date-localized-plugin==1.2.5",
@@ -88,15 +92,15 @@
     "pillow",                                           # required for mkdocs-glightbo
     "cairosvg",                                         # required for mkdocs-glightbo
     "requests",                                         # using in CI, do not pin it
     "griffe-typingdoc==0.2.5",                          # Annotated[..., Doc("")] support
 ]
 
 types = [
-    "faststream[rabbit,confluent,kafka,nats,redis]",
+    "faststream[optionals]",
     "mypy==1.10.0",
     # mypy extensions
     "types-PyYAML",
     "types-setuptools",
     "types-ujson",
     "types-redis",
     "types-Pygments",
@@ -126,15 +130,15 @@
     "httpx==0.27.0",
     "PyYAML==6.0.1",
     "watchfiles==0.21.0",
     "email-validator==2.1.1",
 ]
 
 dev = [
-    "faststream[rabbit,kafka,confluent,nats,redis,lint,testing,devdocs]",
+    "faststream[optionals,lint,testing,devdocs]",
     "pre-commit==3.5.0; python_version < '3.9'",
     "pre-commit==3.7.0; python_version >= '3.9'",
     "detect-secrets==1.5.0",
 ]
 
 [project.urls]
 Homepage = "https://faststream.airt.ai/latest/"
```

### Comparing `faststream-0.5.6/PKG-INFO` & `faststream-0.5.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: faststream
-Version: 0.5.6
+Version: 0.5.7
 Summary: FastStream: the simplest way to work with a messaging queues
 Project-URL: Homepage, https://faststream.airt.ai/latest/
 Project-URL: Documentation, https://faststream.airt.ai/latest/getting-started/
 Project-URL: Tracker, https://github.com/airtai/FastStream/issues
 Project-URL: Source, https://github.com/airtai/FastStream
 Project-URL: Discord, https://discord.gg/qFm6aSqq59
 Author-email: airt <info@airt.ai>, Nikita Pastukhov <nikita@pastukhov-dev.ru>
@@ -67,14 +67,15 @@
 Requires-Dist: mkdocs-macros-plugin==1.0.5; extra == 'dev'
 Requires-Dist: mkdocs-material==9.5.21; extra == 'dev'
 Requires-Dist: mkdocs-minify-plugin==0.8.0; extra == 'dev'
 Requires-Dist: mkdocs-static-i18n==1.2.3; extra == 'dev'
 Requires-Dist: mkdocstrings[python]==0.25.1; extra == 'dev'
 Requires-Dist: mypy==1.10.0; extra == 'dev'
 Requires-Dist: nats-py<=3.0.0,>=2.3.1; extra == 'dev'
+Requires-Dist: opentelemetry-sdk<2.0.0,>=1.24.0; extra == 'dev'
 Requires-Dist: pillow; extra == 'dev'
 Requires-Dist: pre-commit==3.5.0; (python_version < '3.9') and extra == 'dev'
 Requires-Dist: pre-commit==3.7.0; (python_version >= '3.9') and extra == 'dev'
 Requires-Dist: pydantic-settings<3.0.0,>=2.0.0; extra == 'dev'
 Requires-Dist: pytest-asyncio==0.23.6; extra == 'dev'
 Requires-Dist: pytest==8.2.0; extra == 'dev'
 Requires-Dist: pyyaml==6.0.1; extra == 'dev'
@@ -111,25 +112,35 @@
 Requires-Dist: aiokafka<0.11,>=0.9; extra == 'lint'
 Requires-Dist: bandit==1.7.8; extra == 'lint'
 Requires-Dist: codespell==2.2.6; extra == 'lint'
 Requires-Dist: confluent-kafka-stubs; (python_version >= '3.11') and extra == 'lint'
 Requires-Dist: confluent-kafka<3,>=2; extra == 'lint'
 Requires-Dist: mypy==1.10.0; extra == 'lint'
 Requires-Dist: nats-py<=3.0.0,>=2.3.1; extra == 'lint'
+Requires-Dist: opentelemetry-sdk<2.0.0,>=1.24.0; extra == 'lint'
 Requires-Dist: redis<6.0.0,>=5.0.0; extra == 'lint'
 Requires-Dist: ruff==0.4.4; extra == 'lint'
 Requires-Dist: semgrep==1.70.0; extra == 'lint'
 Requires-Dist: types-docutils; extra == 'lint'
 Requires-Dist: types-pygments; extra == 'lint'
 Requires-Dist: types-pyyaml; extra == 'lint'
 Requires-Dist: types-redis; extra == 'lint'
 Requires-Dist: types-setuptools; extra == 'lint'
 Requires-Dist: types-ujson; extra == 'lint'
 Provides-Extra: nats
 Requires-Dist: nats-py<=3.0.0,>=2.3.1; extra == 'nats'
+Provides-Extra: optionals
+Requires-Dist: aio-pika<10,>=9; extra == 'optionals'
+Requires-Dist: aiokafka<0.11,>=0.9; extra == 'optionals'
+Requires-Dist: confluent-kafka<3,>=2; extra == 'optionals'
+Requires-Dist: nats-py<=3.0.0,>=2.3.1; extra == 'optionals'
+Requires-Dist: opentelemetry-sdk<2.0.0,>=1.24.0; extra == 'optionals'
+Requires-Dist: redis<6.0.0,>=5.0.0; extra == 'optionals'
+Provides-Extra: otel
+Requires-Dist: opentelemetry-sdk<2.0.0,>=1.24.0; extra == 'otel'
 Provides-Extra: rabbit
 Requires-Dist: aio-pika<10,>=9; extra == 'rabbit'
 Provides-Extra: redis
 Requires-Dist: redis<6.0.0,>=5.0.0; extra == 'redis'
 Provides-Extra: test-core
 Requires-Dist: coverage[toml]==7.5.1; extra == 'test-core'
 Requires-Dist: dirty-equals==0.7.1.post0; extra == 'test-core'
@@ -149,14 +160,15 @@
 Provides-Extra: types
 Requires-Dist: aio-pika<10,>=9; extra == 'types'
 Requires-Dist: aiokafka<0.11,>=0.9; extra == 'types'
 Requires-Dist: confluent-kafka-stubs; (python_version >= '3.11') and extra == 'types'
 Requires-Dist: confluent-kafka<3,>=2; extra == 'types'
 Requires-Dist: mypy==1.10.0; extra == 'types'
 Requires-Dist: nats-py<=3.0.0,>=2.3.1; extra == 'types'
+Requires-Dist: opentelemetry-sdk<2.0.0,>=1.24.0; extra == 'types'
 Requires-Dist: redis<6.0.0,>=5.0.0; extra == 'types'
 Requires-Dist: types-docutils; extra == 'types'
 Requires-Dist: types-pygments; extra == 'types'
 Requires-Dist: types-pyyaml; extra == 'types'
 Requires-Dist: types-redis; extra == 'types'
 Requires-Dist: types-setuptools; extra == 'types'
 Requires-Dist: types-ujson; extra == 'types'
```

