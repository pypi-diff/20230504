# Comparing `tmp/py_volley-0.23.4.tar.gz` & `tmp/py_volley-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_volley-0.23.4.tar", max compression
+gzip compressed data, was "py_volley-1.0.0.tar", max compression
```

## Comparing `py_volley-0.23.4.tar` & `py_volley-1.0.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1068 2023-04-10 13:14:36.547374 py_volley-0.23.4/LICENSE.md
--rw-r--r--   0        0        0     8734 2023-04-10 13:14:36.547374 py_volley-0.23.4/README.md
--rw-r--r--   0        0        0     2752 2023-04-10 13:14:36.559375 py_volley-0.23.4/pyproject.toml
--rw-r--r--   0        0        0      132 2023-04-10 13:14:36.563376 py_volley-0.23.4/volley/__init__.py
--rw-r--r--   0        0        0     1922 2023-04-10 13:14:36.563376 py_volley-0.23.4/volley/concurrency.py
--rw-r--r--   0        0        0     4897 2023-04-10 13:14:36.563376 py_volley-0.23.4/volley/config.py
--rw-r--r--   0        0        0        0 2023-04-10 13:14:36.563376 py_volley-0.23.4/volley/connectors/__init__.py
--rw-r--r--   0        0        0     2361 2023-04-10 13:14:36.563376 py_volley-0.23.4/volley/connectors/base.py
--rw-r--r--   0        0        0    15131 2023-04-10 13:14:36.563376 py_volley-0.23.4/volley/connectors/confluent.py
--rw-r--r--   0        0        0     7372 2023-04-10 13:14:36.563376 py_volley-0.23.4/volley/connectors/rsmq.py
--rw-r--r--   0        0        0     3018 2023-04-10 13:14:36.563376 py_volley-0.23.4/volley/connectors/zmq.py
--rw-r--r--   0        0        0      393 2023-04-10 13:14:36.563376 py_volley-0.23.4/volley/data_models.py
--rw-r--r--   0        0        0    12250 2023-04-10 13:14:36.563376 py_volley-0.23.4/volley/engine.py
--rw-r--r--   0        0        0     3150 2023-04-10 13:14:36.563376 py_volley-0.23.4/volley/global.yml
--rw-r--r--   0        0        0       53 2023-04-10 13:14:36.563376 py_volley-0.23.4/volley/logging.py
--rw-r--r--   0        0        0     1686 2023-04-10 13:14:36.563376 py_volley-0.23.4/volley/metrics.py
--rw-r--r--   0        0        0      253 2023-04-10 13:14:36.563376 py_volley-0.23.4/volley/models/__init__.py
--rw-r--r--   0        0        0     4858 2023-04-10 13:14:36.563376 py_volley-0.23.4/volley/models/base.py
--rw-r--r--   0        0        0     2113 2023-04-10 13:14:36.563376 py_volley-0.23.4/volley/models/pydantic_model.py
--rw-r--r--   0        0        0     4271 2023-04-10 13:14:36.563376 py_volley-0.23.4/volley/profiles.py
--rw-r--r--   0        0        0     4078 2023-04-10 13:14:36.563376 py_volley-0.23.4/volley/queues.py
--rw-r--r--   0        0        0      285 2023-04-10 13:14:36.563376 py_volley-0.23.4/volley/serializers/__init__.py
--rw-r--r--   0        0        0      537 2023-04-10 13:14:36.563376 py_volley-0.23.4/volley/serializers/base.py
--rw-r--r--   0        0        0      453 2023-04-10 13:14:36.563376 py_volley-0.23.4/volley/serializers/json_serializer.py
--rw-r--r--   0        0        0      439 2023-04-10 13:14:36.563376 py_volley-0.23.4/volley/serializers/msgpack_serializer.py
--rw-r--r--   0        0        0      475 2023-04-10 13:14:36.563376 py_volley-0.23.4/volley/serializers/orjson_serializer.py
--rw-r--r--   0        0        0     4663 2023-04-10 13:14:36.563376 py_volley-0.23.4/volley/transport.py
--rw-r--r--   0        0        0     1742 2023-04-10 13:14:36.571376 py_volley-0.23.4/volley/util.py
--rw-r--r--   0        0        0    10191 1970-01-01 00:00:00.000000 py_volley-0.23.4/setup.py
--rw-r--r--   0        0        0    10103 1970-01-01 00:00:00.000000 py_volley-0.23.4/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-05-04 20:51:04.032201 py_volley-1.0.0/LICENSE.md
+-rw-r--r--   0        0        0     8734 2023-05-04 20:51:04.032201 py_volley-1.0.0/README.md
+-rw-r--r--   0        0        0     2751 2023-05-04 20:51:04.036201 py_volley-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      132 2023-05-04 20:51:04.036201 py_volley-1.0.0/volley/__init__.py
+-rw-r--r--   0        0        0     1922 2023-05-04 20:51:04.036201 py_volley-1.0.0/volley/concurrency.py
+-rw-r--r--   0        0        0     4897 2023-05-04 20:51:04.036201 py_volley-1.0.0/volley/config.py
+-rw-r--r--   0        0        0        0 2023-05-04 20:51:04.036201 py_volley-1.0.0/volley/connectors/__init__.py
+-rw-r--r--   0        0        0     2361 2023-05-04 20:51:04.036201 py_volley-1.0.0/volley/connectors/base.py
+-rw-r--r--   0        0        0    16383 2023-05-04 20:51:04.036201 py_volley-1.0.0/volley/connectors/confluent.py
+-rw-r--r--   0        0        0     7372 2023-05-04 20:51:04.036201 py_volley-1.0.0/volley/connectors/rsmq.py
+-rw-r--r--   0        0        0     3018 2023-05-04 20:51:04.036201 py_volley-1.0.0/volley/connectors/zmq.py
+-rw-r--r--   0        0        0      393 2023-05-04 20:51:04.036201 py_volley-1.0.0/volley/data_models.py
+-rw-r--r--   0        0        0    12250 2023-05-04 20:51:04.036201 py_volley-1.0.0/volley/engine.py
+-rw-r--r--   0        0        0     3150 2023-05-04 20:51:04.036201 py_volley-1.0.0/volley/global.yml
+-rw-r--r--   0        0        0       53 2023-05-04 20:51:04.036201 py_volley-1.0.0/volley/logging.py
+-rw-r--r--   0        0        0     1686 2023-05-04 20:51:04.036201 py_volley-1.0.0/volley/metrics.py
+-rw-r--r--   0        0        0      253 2023-05-04 20:51:04.036201 py_volley-1.0.0/volley/models/__init__.py
+-rw-r--r--   0        0        0     4858 2023-05-04 20:51:04.036201 py_volley-1.0.0/volley/models/base.py
+-rw-r--r--   0        0        0     2113 2023-05-04 20:51:04.036201 py_volley-1.0.0/volley/models/pydantic_model.py
+-rw-r--r--   0        0        0     4271 2023-05-04 20:51:04.036201 py_volley-1.0.0/volley/profiles.py
+-rw-r--r--   0        0        0     4078 2023-05-04 20:51:04.036201 py_volley-1.0.0/volley/queues.py
+-rw-r--r--   0        0        0      285 2023-05-04 20:51:04.036201 py_volley-1.0.0/volley/serializers/__init__.py
+-rw-r--r--   0        0        0      537 2023-05-04 20:51:04.036201 py_volley-1.0.0/volley/serializers/base.py
+-rw-r--r--   0        0        0      453 2023-05-04 20:51:04.036201 py_volley-1.0.0/volley/serializers/json_serializer.py
+-rw-r--r--   0        0        0      439 2023-05-04 20:51:04.036201 py_volley-1.0.0/volley/serializers/msgpack_serializer.py
+-rw-r--r--   0        0        0      475 2023-05-04 20:51:04.036201 py_volley-1.0.0/volley/serializers/orjson_serializer.py
+-rw-r--r--   0        0        0     4663 2023-05-04 20:51:04.036201 py_volley-1.0.0/volley/transport.py
+-rw-r--r--   0        0        0     1742 2023-05-04 20:51:04.036201 py_volley-1.0.0/volley/util.py
+-rw-r--r--   0        0        0    10190 1970-01-01 00:00:00.000000 py_volley-1.0.0/setup.py
+-rw-r--r--   0        0        0    10102 1970-01-01 00:00:00.000000 py_volley-1.0.0/PKG-INFO
```

### Comparing `py_volley-0.23.4/LICENSE.md` & `py_volley-1.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `py_volley-0.23.4/README.md` & `py_volley-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `py_volley-0.23.4/pyproject.toml` & `py_volley-1.0.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py_volley"
-version = "0.23.4"
+version = "1.0.0"
 description = "Pluggable message queueing for Python"
 authors = ["ask-machine-learning <shipt@shipt.com>"]
 readme = "README.md"
 
 packages = [
     { include = "volley" },
 ]
```

### Comparing `py_volley-0.23.4/volley/concurrency.py` & `py_volley-1.0.0/volley/concurrency.py`

 * *Files identical despite different names*

### Comparing `py_volley-0.23.4/volley/config.py` & `py_volley-1.0.0/volley/config.py`

 * *Files identical despite different names*

### Comparing `py_volley-0.23.4/volley/connectors/base.py` & `py_volley-1.0.0/volley/connectors/base.py`

 * *Files identical despite different names*

### Comparing `py_volley-0.23.4/volley/connectors/confluent.py` & `py_volley-1.0.0/volley/connectors/confluent.py`

 * *Files 11% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     auto_offset_reset: str = "earliest"
     auto_commit_interval_ms: int = 3000
     stop_on_failure: bool = True
     # mapping of topic -> partition/offset of the last stored commit
     last_offset: Dict[str, Dict[int, int]] = field(init=False)
 
     def __post_init__(self) -> None:  # noqa: C901
-        self.config = handle_creds(self.config)
+        self.config = _handle_creds(self.config, True)
 
         if "auto.offset.reset" not in self.config:
             logger.info("Assigning auto.offset.reset default: %s", self.auto_offset_reset)
             self.config["auto.offset.reset"] = self.auto_offset_reset
 
         if "auto.commit.interval.ms" not in self.config:
             logger.info("Assigning auto.commit.interval.ms default: %s", self.auto_commit_interval_ms)
@@ -179,15 +179,15 @@
 class ConfluentKafkaProducer(BaseProducer):
     compression_type: str = "gzip"
     thread: bool = False
     poll_thread_timeout: float = 1.0
 
     def __post_init__(self) -> None:  # noqa: C901
         self.callback_delivery = True
-        self.config = handle_creds(self.config)
+        self.config = _handle_creds(self.config, False)
         if "compression.type" not in self.config:
             logger.info("Assigning compression.type default: %s", self.compression_type)
             self.config["compression.type"] = self.compression_type
 
         self.p = Producer(self.config, logger=logger)
 
         # producer poll thread
@@ -243,28 +243,50 @@
     def shutdown(self) -> None:
         self.p.flush()
         if self.thread:
             self.kill_poll_thread = True
             self.poll_thread.join(self.poll_thread_timeout)
 
 
-def handle_creds(config_dict: Dict[str, Any]) -> Dict[str, Any]:
-    if "bootstrap.servers" in config_dict:
-        pass
-    else:
-        try:
+def _handle_creds(config_dict: Dict[str, Any], is_consumer: bool) -> Dict[str, Any]:
+    """Populates credential related kafka configuration values based on well
+    known environment variables.
+
+    Environment variable mappings:
+        * KAFKA_BROKERS maps to bootstrap.servers
+        * KAFKA_CONSUMER_BROKERS maps to bootstrap.servers for consumers only,
+          falling back to KAFKA_BROKERS.
+        * KAFKA_PRODUCER_BROKERS maps to bootstrap.servers for producers only,
+          falling back to KAFKA_BROKERS.
+        * KAFKA_KEY maps to sasl.username
+        * KAFKA_SECRET maps to sasl.password
+
+    Note that environment variables will only be used when previous config
+    values do not exist.
+    """
+
+    if "bootstrap.servers" not in config_dict:
+        # Attempt to set consumer / producer specific overrides first
+        if is_consumer and os.getenv("KAFKA_CONSUMER_BROKERS") is not None:
+            config_dict["bootstrap.servers"] = os.environ["KAFKA_CONSUMER_BROKERS"]
+
+        if not is_consumer and os.getenv("KAFKA_PRODUCER_BROKERS") is not None:
+            config_dict["bootstrap.servers"] = os.environ["KAFKA_PRODUCER_BROKERS"]
+
+    # Fall back to "KAFKA_BROKERS" for both consumers and producers if still not set
+    if "bootstrap.servers" not in config_dict:
+        if os.getenv("KAFKA_BROKERS") is not None:
             config_dict["bootstrap.servers"] = os.environ["KAFKA_BROKERS"]
-        except KeyError:
-            logger.exception("Kafka brokers not specified, set in config dict or env var KAFKA_BROKERS")
-            raise
+
+    if "bootstrap.servers" not in config_dict:
+        logger.error("Kafka brokers not specified, set in config dict or env var KAFKA_BROKERS")
+        raise ValueError("bootstrap.servers is required")
 
     # No key == dev mode
-    if config_dict.get("sasl.username") and config_dict.get("sasl.password"):
-        pass
-    else:
+    if "sasl.username" not in config_dict and "sasl.passsword" not in config_dict:
         sasl_username = os.getenv("KAFKA_KEY")
         sasl_password = os.getenv("KAFKA_SECRET")
         if (sasl_username is not None) and (sasl_password is not None):
             logger.info(
                 "KAFKA_KEY and KAFKA_SECRET found in environment. Assigning security.protocol and sasl.mechanism"
             )
             config_dict["sasl.username"] = sasl_username
```

### Comparing `py_volley-0.23.4/volley/connectors/rsmq.py` & `py_volley-1.0.0/volley/connectors/rsmq.py`

 * *Files identical despite different names*

### Comparing `py_volley-0.23.4/volley/connectors/zmq.py` & `py_volley-1.0.0/volley/connectors/zmq.py`

 * *Files identical despite different names*

### Comparing `py_volley-0.23.4/volley/engine.py` & `py_volley-1.0.0/volley/engine.py`

 * *Files identical despite different names*

### Comparing `py_volley-0.23.4/volley/global.yml` & `py_volley-1.0.0/volley/global.yml`

 * *Files identical despite different names*

### Comparing `py_volley-0.23.4/volley/metrics.py` & `py_volley-1.0.0/volley/metrics.py`

 * *Files identical despite different names*

### Comparing `py_volley-0.23.4/volley/models/base.py` & `py_volley-1.0.0/volley/models/base.py`

 * *Files identical despite different names*

### Comparing `py_volley-0.23.4/volley/models/pydantic_model.py` & `py_volley-1.0.0/volley/models/pydantic_model.py`

 * *Files identical despite different names*

### Comparing `py_volley-0.23.4/volley/profiles.py` & `py_volley-1.0.0/volley/profiles.py`

 * *Files identical despite different names*

### Comparing `py_volley-0.23.4/volley/queues.py` & `py_volley-1.0.0/volley/queues.py`

 * *Files identical despite different names*

### Comparing `py_volley-0.23.4/volley/serializers/base.py` & `py_volley-1.0.0/volley/serializers/base.py`

 * *Files identical despite different names*

### Comparing `py_volley-0.23.4/volley/transport.py` & `py_volley-1.0.0/volley/transport.py`

 * *Files identical despite different names*

### Comparing `py_volley-0.23.4/volley/util.py` & `py_volley-1.0.0/volley/util.py`

 * *Files identical despite different names*

### Comparing `py_volley-0.23.4/setup.py` & `py_volley-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
  'rsmq': ['PyRSMQ>=0.4.5,<0.5.0',
           'hiredis>=2.0,<3.0',
           'tenacity>=8.0.1,<9.0.0'],
  'zmq': ['pyzmq>=22.3.0']}
 
 setup_kwargs = {
     'name': 'py-volley',
-    'version': '0.23.4',
+    'version': '1.0.0',
     'description': 'Pluggable message queueing for Python',
     'long_description': '![VolleyFull-Horizontal](https://user-images.githubusercontent.com/81711984/149005139-f0441dcf-c76e-4112-baf1-998d0a6abdbb.png)\n\nDocumentation: https://shipt.github.io/py-volley/\n\nVolley makes building event stream applications easier and more accessible. Use Volley if you need to quickly develop an application to consume messages, processes them (and do other things), then publish results to one or many places. Volley was inspired ease of use and developer experience provided by the [Flask](https://github.com/pallets/flask) and [FastAPI](https://github.com/tiangolo/fastapi) projects, and aims to make working with queue based and event driven system as accessible as REST APIs.\n\nVolley handles a number of operations that need to happen before and after processing a message. Reading the data, serialization, data validation, all need to happen before data reaches your application. If these fail, Volley can route the message to a dead-letter-queue. After processing, Volley again handles data validation, serialization, and the writing/publishing of data to any number of output queues. Finally, upon successfully delivery of that message to the target queue, Volley handles marking it as read or deleting it from the input queue.\n\nAll of Volley\'s major operations (connectors, serializers, data validation/model handling) can be extended with plugins, and comes with built in support for queues-like technologies [Apache Kafka](https://kafka.apache.org/) and [RSMQ](https://github.com/mlasevich/PyRSMQ) (Redis Simple Message Queue). There is a plugin built for a Postgres queue in our [examples](./example/plugins/my_plugin.py).\n\n\n[![Build Status](https://drone.shipt.com/api/badges/shipt/py-volley/status.svg?ref=refs/heads/main)](https://drone.shipt.com/shipt/py-volley)\n[![Coverage](https://sonarqube.shipt.com/api/project_badges/measure?project=shipt_py-volley_AYImTs5MsYUjTdFQ7Awt&metric=coverage&token=squ_e98968a6b1bce0281e001fd0e70e538f6228b47f)](https://sonarqube.shipt.com/dashboard?id=shipt_py-volley_AYImTs5MsYUjTdFQ7Awt)\n\n# Installation\n\nRequires Python >= 3.8\n\n```bash\npip install py-volley[all]\n```\n\nYou can also limit the dependencies by:\n```bash\npip install py-volley[kafka]  # Kafka dependencies\npip install py-volley[rsmq]  # RSMQ dependencies\npip install py-volley[zmq]  # ZeroMQ dependencies\n```\n\n## Features\n- Built in support for [Apache Kafka](https://kafka.apache.org/), [RSMQ](https://github.com/smrchy/rsmq), [ZeroMQ](https://zeromq.org/)\n- [Prometheus](https://prometheus.io/) metrics for all operations such as function processing time, and consumption and production count.\n- Serialization in JSON and [MessagePack](https://msgpack.org/index.html)\n- Data validation via [Pydantic](https://pydantic-docs.helpmanual.io/)\n- Optionally configured integration with dead-letter-queues\n- Extendible connectors (consumer/producers), serializers, model handlers, and model handlers via plugins.\n\n## Getting started\n\nVolley handles the process of consuming/producing by providing developers with extendible interfaces and handlers:\n- connectors - consumer and producer interfaces which define how the application should read messages, write messages, and what actions to take when a message is successfully or fails processing.\n- serializers - handlers and interface which describe the behavior for reading an byte objects from connectors. For example, Json or MessagePack serializers.\n- model_handler - handler and interface which works very closely with serializers. Typically used to turn serialized data into a structured Python data model. Pydantic is Volley\'s most supported data_model and can handler serialization itself.\n- data_model - When your application receives data from a queue, what schema and object do you expect it in? The data_model is provided by the user. And the `model_handler` describes how to construct your `data_model`.\n\n\nTo demonstrate, let\'s create an application with two worker nodes. One consumes from Kafka, finds the maximum value in a list then publishes it to Redis. The other consumes the message from Redis - if the max value is > 10, it logs to console otherwise it constructs a new list and publishes to the same Kafka topic. \n\n```mermaid\nflowchart LR\nA[(Kafka)] --> |consume| B[Worker 1]\nB --> |publish| C[(Redis)]\nC --> |consume| D[Worker 2]\nD --> E{>10}\nE --> | no | A\nE --> | yes | F[Log to Console]\n```\n\nYou can skip the details and just run `make intro.start`, which runs this example through `./example/intro/docker-compose.yml`\n\n1. start Kafka and Redis instance\n\n```\ndocker run -d -p 6379:6379 redis:5.0.0\ndocker run -d -p 9092:9092 bashj79/kafka-kraft\n```\n\n2. Configure the queues and data models. Let\'s put this in `./my_config.py`.\n\n```python\n# ./my_config.py\nfrom typing import List, Tuple\nfrom pydantic import BaseModel\n\nfrom volley import Engine, QueueConfig\n\n# define the schemas for the first and second worker nodes.\nclass InputMessage(BaseModel):\n  my_values: List[float]\n\nclass OutputMessage(BaseModel):\n  the_max: float\n\n# define the configurations for the two queues, one in Kafka and the other in Redis.\nqueue_config = [\n  QueueConfig(\n    name="my-kafka-input",\n    value="my.kafka.topic.name",\n    profile="confluent",\n    data_model=InputMessage,\n    config={\n      "group.id": "my.consumer.group",\n      "bootstrap.servers": "localhost:9092",\n    }\n  ),\n  QueueConfig(\n    name="my-redis-output",\n    value="my.redis.output.queue.name",\n    profile="rsmq",\n    data_model=OutputMessage,\n    config={\n      "host": "localhost",\n      "port": 6379,\n    }\n  )\n]\n```\n\n3. Build the first worker node - consume from Kafka, find the max value, publish to Redis\n\n```python\n# ./app_0.py\nfrom typing import List, Tuple\nfrom volley import Engine\n\nfrom my_config import queue_config, InputMessage, OutputMessage\n# the first node - reads from kafka and writes to redis\napp_0 = Engine(\n  app_name="app_0",\n  input_queue="my-kafka-input",  # one input\n  output_queues=["my-redis-output"],  # zero to many outputs\n  queue_config=queue_config\n)\n\n@app_0.stream_app\ndef kafka_to_redis(msg: InputMessage) -> List[Tuple[str, OutputMessage]]:\n  print(f"Received {msg.json()}")\n  max_val = max(msg.my_values)\n  out = OutputMessage(the_max=max_val)\n  print(out)\n  return [("my-redis-output", out)]  # a list of one or many output targets and messages\n\nif __name__ == "__main__":\n  kafka_to_redis()\n\n```\n\n4. Run the first application in a terminal\n```bash\npython app_0.py\n```\n\n\n5. Build the second worker node - consume from Redis, determine if we log to console or recycle the message as a new list.\n```python\n# ./app_1.py\nfrom typing import List, Tuple, Union\nfrom volley import Engine\n\nfrom my_config import OutputMessage, queue_config, InputMessage\n\n# the second node\napp_1 = Engine(\n  app_name="app_1",\n  input_queue="my-redis-output",\n  output_queues=["my-kafka-input"],\n  queue_config=queue_config,\n  metrics_port=None\n)\n\n@app_1.stream_app\ndef redis_to_kafka(msg: OutputMessage) -> Union[bool, List[Tuple[str, InputMessage]]]:\n  print(f"The maximum: {msg.the_max}")\n  if msg.the_max > 10:\n    print("That\'s it, we are done!")\n    return True\n  else:\n    out = InputMessage(my_values=[msg.the_max, msg.the_max+1, msg.the_max+2])\n    return [("my-kafka-input", out)]  # a list of one or many output targets and messages\n\nif __name__ == "__main__":\n    redis_to_kafka()\n```\n\n6. Run the second worker node in another terminal\n```bash\npython app_1.py\n```\n\n7. Finally, let\'s manually publish a message to the input kafka topic:\n```python\nfrom confluent_kafka import Producer\nimport json\nproducer = Producer({"bootstrap.servers": "localhost:9092"})\nproducer.produce(topic="my.kafka.topic.name", value=json.dumps({"my_values":[1,2,3]}))\nproducer.flush(5)\n```\n\nYou should see the following in your two terminals\n\n__./app_0.py__\n```\nReceived {"my_values": [1.0, 2.0, 3.0]}\nthe_max=3.0\nReceived {"my_values": [3.0, 4.0, 5.0]}\nthe_max=5.0\nReceived {"my_values": [5.0, 6.0, 7.0]}\nthe_max=7.0\nReceived {"my_values": [7.0, 8.0, 9.0]}\nthe_max=9.0\nReceived {"my_values": [9.0, 10.0, 11.0]}\nthe_max=11.0\n```\n\n__./app_1.py__\n```\nThe maximum: 3.0\nThe maximum: 5.0\nThe maximum: 7.0\nThe maximum: 9.0\nThe maximum: 11.0\nThat\'s it, we are done!\n```\n\n# Complete example\n\nClone this repo and `make run.example` to see a complete example of:\n- consuming a message from a Kafka topic\n- producing to RSMQ\n- consuming from RSMQ and publishing to Kafka and Postgres using custom plugin for Postgres.\n\n# Contributing\n\nSee our [contributing guide](./CONTRIBUTING.md).\n\nThanks goes to great [projects](./ATTRIBUTIONS.md) and these incredible people.\n\n<a href="https://github.com/shipt/py-volley/graphs/contributors">\n  <img src="https://contrib.rocks/image?repo=shipt/py-volley" />\n</a>\n',
     'author': 'ask-machine-learning',
     'author_email': 'shipt@shipt.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `py_volley-0.23.4/PKG-INFO` & `py_volley-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-volley
-Version: 0.23.4
+Version: 1.0.0
 Summary: Pluggable message queueing for Python
 Author: ask-machine-learning
 Author-email: shipt@shipt.com
 Requires-Python: >=3.8,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

