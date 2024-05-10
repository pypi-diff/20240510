# Comparing `tmp/ebb_events-0.1.0.tar.gz` & `tmp/ebb_events-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebb_events-0.1.0.tar", max compression
+gzip compressed data, was "ebb_events-0.2.0.tar", max compression
```

## Comparing `ebb_events-0.1.0.tar` & `ebb_events-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     1071 2024-05-06 17:17:20.374070 ebb_events-0.1.0/LICENSE
--rw-r--r--   0        0        0     7681 2024-05-06 17:17:21.775844 ebb_events-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-04-19 21:49:16.587650 ebb_events-0.1.0/ebb_events/__init__.py
--rw-r--r--   0        0        0     5705 2024-05-06 17:17:21.776054 ebb_events-0.1.0/ebb_events/builders/event_builder.py
--rw-r--r--   0        0        0      231 2024-05-06 17:16:47.745004 ebb_events-0.1.0/ebb_events/constants.py
--rw-r--r--   0        0        0     8533 2024-05-06 17:17:21.776493 ebb_events-0.1.0/ebb_events/consumers/event_consumer.py
--rw-r--r--   0        0        0      174 2024-04-22 19:12:51.110543 ebb_events-0.1.0/ebb_events/enums.py
--rw-r--r--   0        0        0     2066 2024-05-06 17:16:47.745815 ebb_events-0.1.0/ebb_events/event_schema.py
--rw-r--r--   0        0        0      383 2024-05-06 17:16:47.746622 ebb_events-0.1.0/ebb_events/exceptions.py
--rw-r--r--   0        0        0      571 2024-05-02 21:01:50.974720 ebb_events-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     8179 1970-01-01 00:00:00.000000 ebb_events-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-05-06 20:14:00.489414 ebb_events-0.2.0/LICENSE
+-rw-r--r--   0        0        0     8800 2024-05-10 21:40:45.942475 ebb_events-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-19 21:49:16.587650 ebb_events-0.2.0/ebb_events/__init__.py
+-rw-r--r--   0        0        0     7572 2024-05-10 21:40:45.943169 ebb_events-0.2.0/ebb_events/builders/event_builder.py
+-rw-r--r--   0        0        0      231 2024-05-06 17:16:47.745004 ebb_events-0.2.0/ebb_events/constants.py
+-rw-r--r--   0        0        0     8523 2024-05-10 21:40:45.943550 ebb_events-0.2.0/ebb_events/consumers/event_consumer.py
+-rw-r--r--   0        0        0      174 2024-04-22 19:12:51.110543 ebb_events-0.2.0/ebb_events/enums.py
+-rw-r--r--   0        0        0      414 2024-05-10 21:40:45.943826 ebb_events-0.2.0/ebb_events/event_payload_utils.py
+-rw-r--r--   0        0        0     2668 2024-05-10 21:40:45.944168 ebb_events-0.2.0/ebb_events/event_schema.py
+-rw-r--r--   0        0        0      383 2024-05-06 17:16:47.746622 ebb_events-0.2.0/ebb_events/exceptions.py
+-rw-r--r--   0        0        0      571 2024-05-10 21:40:45.944486 ebb_events-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     9298 1970-01-01 00:00:00.000000 ebb_events-0.2.0/PKG-INFO
```

### Comparing `ebb_events-0.1.0/LICENSE` & `ebb_events-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ebb_events-0.1.0/README.md` & `ebb_events-0.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 # ebb-events:
-EbbCarbon package to standardize MQTT event message structures. For environmental and industrial automation montioring, we are using many physical sensors to read/gather data about our systems and the environment. In order to communicate this information across systems, we utilize the MQTT messaging protocol to publish and subscribe to various messages and topics. In an attempt to standardize the MQTT event message structure, this package works to define a standard topic hierarchy, standard event types to use, and a standard payload structure that can be replicated and re-used throughout the industry. This structure will be consistent with the CloudEvent structure defined [here] (https://cloudevents.io/) while implementing some additional standards and best practices so that these events can be consumed and used by CloudEvent users as well.
+EbbCarbon package to standardize event message structures. For environmental and industrial automation montioring, we are using many physical sensors to read/gather data about our systems and the environment. In order to communicate this information across systems, we are utilizing the MQTT messaging protocol to publish and subscribe to various messages and topics (however, this structure can be used to publish events across various other protocols as well). In an attempt to standardize the event message structure, this package works to define a standard topic hierarchy, standard event types to use, and a standard payload structure that can be replicated and re-used throughout the industry. This structure will be consistent with the CloudEvent structure defined [here] (https://cloudevents.io/) while implementing some additional standards and best practices so that these events can be consumed and used by CloudEvent users as well.
 
 # Use:
-Install the ebb-events package from pip installer and use it to format your MQTT event messages and topics.
+Install the ebb-events package from pip installer via: `pip install ebb-events`.
+Use ebb-events to format your event messages and topics.
 ```python
 from ebb_events.builders.event_builder import EventEnvelope
 
 event_envelope = EventEnvelope(
     organization="test-org",
     system_id="test-system",
     event_type="data",
     subsystem_id="test-subsystem",
     device_id="test-device-01",
 )
 
 event_topic = event_envelope.build_event_topic()
-event_payload = event_envelope.build_event_payload(message={...}, metadata={...})  # Builds a payload of the expected ebb-events structure
+event_payload = event_envelope.build_event_payload_json(message={...}, metadata={...})  # Builds a payload of the expected ebb-events structure
 ```
 
 Use ebb-events package to consume events published with this expected ebb-events structure
 ```python
 from ebb_events.consumers.event_consumer import EventConsumer
 
-my_payload = {...}
-event_consumer = EventConsumer(payload=my_payload)
+my_event_payload = {...}
+event_consumer = EventConsumer(payload=my_event_payload)
 
-event_consumer.get_event_message()  # Retrieves the json message found in the payload's `data` field
+event_consumer.get_event_message()  # Retrieves the dict message found in the payload's `data` field
 event_consumer.get_event_time()
 event_conumser.get_event_system_id()
 ```
 
 # Topic Structure:
 One thing that this package enforces is a topic structure for publishing MQTT messages to a broker. Well defined topics help Our topic structure is as follows:
 * _\<organization\>/\<system-id\>/\<event-type\>/\<subsystem-id\>/\<device-id\>_
@@ -73,23 +74,39 @@
     "source": str,  # same as topic string
     "type": str,
     "data": {
         "metadata": {
             "serial_number": str,  # Example of potential metadata, this is not a required metadata field
             ...
         },
-        ...  # unique nested json dependent on event-type
+        ...  # unique nested JSON dependent on event-type
     }
 }
 ```
 
+### Suggested `data` Event Message Structure:
+The ebb-events package allows users to publish payloads of any structure (as long as they are JSON serializable) so that it can be helpful for publishing all types of events.  However, we have a recommened message structure that we encourage all to adopt when publishing sensor data events that will allow consumers to process the readings smoothly and accurately. Each variable that is measured by a sensor should named following the convention outlined [here](https://cfconventions.org/Data/cf-standard-names/current/build/cf-standard-name-table.html) whenever possible, and should have a corresponding `value` and `units` attached to it and should be formatted in the `message` argument of `build_event_payload_json/dict(message={})` like so:
+```python
+message = {
+    "variable_name_1": {
+        "value": ____,
+        "units": str
+    },
+    "variable_name_2": {
+        "value": ____,
+        "units": str
+    },
+    ...
+}
+```
+
 ### EventEnvelope Class:
 The EventEnvelope class is used to consolidate all of the pieces of aa event payload and build the expected structure for a user so that users don't have to worry about constructing the properly formatted topic or payload. The `EventEnvelope` class expects to be provided with certain fields that are then used to build the topic and payload via class methods. These methods handle all the validation and formatting needed to ensure that your events follow the ebb-events standards.
 
 Required fields: `organization`, `system_id`, `event_type`, `subsystem_id`, `device_id`
 Useful methods: `EventEnvelope().build_event_topic()`, `EventEnvelope().build_event_payload()`
 
 # Event Consumer:
-This package defines an event consumer that can be used to process incoming events that follow this ebb-events structure. To use this consumer, initialize the class with a given json payload: `EventConsumer(payload=my_payload)`. Then, you can use the various getters present on the class in order to retrieve different pieces of the payload depending on your needs (e.g. system_id, message, metadata, etc.). If you need all the parts of the payload that go into building it (e.g. an entire `EventEnvelope` wrapper for the payload) you may also use the `get_event_envelope()` method to do so.
+This package defines an event consumer that can be used to process incoming events that follow this ebb-events structure. To use this consumer, initialize the class with a given JSON payload: `EventConsumer(payload=my_payload)`. Then, you can use the various getters present on the class in order to retrieve different pieces of the payload depending on your needs (e.g. system_id, message, metadata, etc.). If you need all the parts of the payload that go into building it (e.g. an entire `EventEnvelope` wrapper for the payload) you may also use the `get_event_envelope()` method to do so.
 
 ### Exception Handling
-If you attempt to consume an event that _DOES NOT_ match the ebb-events structure, you can still initialize an `EventConsumer(payload=my_payload)` object and the payload will live as `EventConsumer().raw_payload`. However, all of the getter methods will raise `PayloadFormatExceptions` because the payload does not match the expected format. Therefore, for a payload that does not match the ebb-events structure, you must process the payload as a raw json/dict object instead.
+If you attempt to consume an event that _DOES NOT_ match the ebb-events structure, you can still initialize an `EventConsumer(payload=my_payload)` object and the payload will live as `EventConsumer().raw_payload`. However, all of the getter methods will raise `PayloadFormatExceptions` because the payload does not match the expected format. Therefore, for a payload that does not match the ebb-events structure, you must process the payload as a raw JSON/dict object instead.
```

### Comparing `ebb_events-0.1.0/ebb_events/builders/event_builder.py` & `ebb_events-0.2.0/ebb_events/builders/event_builder.py`

 * *Files 18% similar despite different names*

```diff
@@ -82,36 +82,41 @@
         """
         topic = f"{self.organization}/{self.system_id}/{self.event_type}/{self.subsystem_id}/{self.device_id}"
         # This should be enforced by the ._validate() call and the EventEnvelopeSchema too
         if len(topic) > 256:
             raise TopicFormatException("Topic length cannot exceed 256 characters.")
         return topic
 
-    def build_event_payload(
+    def build_event_payload_dict(
         self,
         message: dict,
         metadata: dict = {},
         datetime_obj: Optional[datetime] = None,
+        remove_nones: bool = False,
     ) -> dict:
         """
         Method validates the message structure, builds and returns the expected
-        event payload to be used in the MQTT payload as a json serializable dictionary
+        event payload to be used in the MQTT payload as a json serializable dictionary.
+        NOTE: Returned object is a python dictionary, not a json object. In order to publish this,
+        one must either `json.dumps()` this result or use `build_event_payload_json()` method.
 
         Args:
             message (dict): Dictionary containing the message information that is being published
             metadata (dict): Dictionary containing metadata information to be included in the data
             datetime_obj (Optional[datetime]): datetime obj to use as event time
+            remove_nones (bool): If set to True, all key:value pairs where value=None or NaN will
+                                    be removed/omitted from the resulting payload dict
 
         Returns:
             dict: Dictionary of the expected MQTT event message format
 
         Exceptions:
             Raises 'PayloadFormatException' if the topic or message does not meet the expected format
         """
-        payload_schema = EventPayloadSchema()
+        payload_schema = EventPayloadSchema(context={"remove_nones": remove_nones})
         if datetime_obj is not None and type(datetime_obj) is not datetime:
             raise PayloadFormatException(
                 "datetime_obj must be a valid datetime object."
             )
         try:
             event_payload = {
                 ID: uuid4(),
@@ -138,7 +143,41 @@
             )
         except TypeError:
             # Exception raised by json.dumps() if not valid json serializable object
             raise PayloadFormatException(
                 "Payload message and metadata must be JSON serializable dictionaries."
             )
         return payload_schema.dump(deserialized_payload)
+
+    def build_event_payload_json(
+        self,
+        message: dict,
+        metadata: dict = {},
+        datetime_obj: Optional[datetime] = None,
+        remove_nones: bool = False,
+    ):
+        """
+        Method validates the message structure, builds and returns the expected
+        event payload to be used in the MQTT payload as a JSON formatted str.
+
+        This returned value can be immediately placed in an MQTT publish call as it's a json string
+
+        Args:
+            message (dict): Dictionary containing the message information that is being published
+            metadata (dict): Dictionary containing metadata information to be included in the data
+            datetime_obj (Optional[datetime]): datetime obj to use as event time
+            remove_nones (bool): If set to True, all key:value pairs where value=None or NaN will
+                                    be removed/omitted from the resulting payload json
+
+        Returns:
+            dict: Dictionary of the expected MQTT event message format
+
+        Exceptions:
+            Raises 'PayloadFormatException' if the topic or message does not meet the expected format
+        """
+        payload_dict = self.build_event_payload_dict(
+            message=message,
+            metadata=metadata,
+            datetime_obj=datetime_obj,
+            remove_nones=remove_nones,
+        )
+        return json.dumps(payload_dict)
```

### Comparing `ebb_events-0.1.0/ebb_events/consumers/event_consumer.py` & `ebb_events-0.2.0/ebb_events/consumers/event_consumer.py`

 * *Files 1% similar despite different names*

```diff
@@ -200,16 +200,16 @@
                 subsystem_id=self.get_event_subsystem_id(),
                 device_id=self.get_event_device_id(),
             )
         raise PayloadFormatException()
 
     def get_event_message(self, metadata_included=True) -> dict:
         """
-        Helper fetches and returns message json from payload
-        Metadata field in the message json is included by default but can be parsed out
+        Helper fetches and returns message dict from payload
+        Metadata field in the message dict is included by default but can be parsed out
 
         Args:
             metadata_included (bool, optional): If set to False, returned dict will remove the `metadata` portion of the message.
                                                 Defaults to True.
 
         Raises:
             PayloadFormatException: Raised if event does not match ebb_event structure
@@ -223,18 +223,18 @@
             if not metadata_included:
                 message.pop(METADATA, {})
             return message
         raise PayloadFormatException()
 
     def get_event_message_metadata(self) -> dict:
         """
-        Helper to fetch and return the metadata dictionary within the payload's event message json
+        Helper to fetch and return the metadata dictionary within the payload's event message
 
         Raises:
             PayloadFormatException: Raised if event does not match ebb_event structure
 
         Returns:
-            dict: Metadata included in event message json
+            dict: Metadata included in event message
         """
         if self.is_ebb_event_structure:
             return self.raw_payload.get(DATA, {}).get(METADATA, {})
         raise PayloadFormatException()
```

### Comparing `ebb_events-0.1.0/ebb_events/event_schema.py` & `ebb_events-0.2.0/ebb_events/event_schema.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from marshmallow import Schema, fields, validate
 
 from ebb_events.enums import EventType
+from ebb_events.event_payload_utils import remove_nones_helper
 
 
 TOPIC_MAX_LENGTH = 50
 TOPIC_REGEX = r"^[a-z0-9-]+$"
 SOURCE_REGEX = r"^([a-z0-9-]+\/){4}[a-z0-9-]+$"
 SOURCE_MAX_LENGTH = 256
 
@@ -50,14 +51,30 @@
     that id as a string value e.g. (str(id))
     """
 
     def _serialize(self, value, attr, obj, **kwargs):
         return str(value)
 
 
+class DictConditionallyRemoveInvalid(fields.Dict):
+    """
+    Class for EventPayloadSchema data field to conditionally
+    remove invalid fields: None, NaN
+    """
+
+    def _serialize(self, value, attr, obj, **kwargs):
+        remove_nones = self.context.get("remove_nones", False)
+        if remove_nones:
+            # Filter out None values from the dictionary for top and second levels
+            filtered_dict = remove_nones_helper(value)
+            return filtered_dict
+        else:
+            return value
+
+
 class EventPayloadSchema(Schema):
     """Schema for event payload json to validate fields follow requirements"""
 
     # id field could be uuid but doesn't have to be (could be string(int))
     id = RawToStringField(required=True)
     time = fields.DateTime(required=True, format="iso")
     source = fields.Str(
@@ -69,8 +86,8 @@
     )
     type = fields.Str(
         required=True,
         validate=[
             validate.OneOf([e.value for e in EventType]),
         ],
     )
-    data = fields.Dict(required=True)
+    data = DictConditionallyRemoveInvalid(required=True)
```

### Comparing `ebb_events-0.1.0/pyproject.toml` & `ebb_events-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ebb-events"
-version = "0.1.0"
+version = "0.2.0"
 description = "Package for building and standardizing MQTT event messages."
 authors = ["Ryan Bloom <ryan.bloom@ebbcarbon.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 marshmallow = "^3.21.1"
```

### Comparing `ebb_events-0.1.0/PKG-INFO` & `ebb_events-0.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,49 +1,50 @@
 Metadata-Version: 2.1
 Name: ebb-events
-Version: 0.1.0
+Version: 0.2.0
 Summary: Package for building and standardizing MQTT event messages.
 Author: Ryan Bloom
 Author-email: ryan.bloom@ebbcarbon.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: marshmallow (>=3.21.1,<4.0.0)
 Description-Content-Type: text/markdown
 
 # ebb-events:
-EbbCarbon package to standardize MQTT event message structures. For environmental and industrial automation montioring, we are using many physical sensors to read/gather data about our systems and the environment. In order to communicate this information across systems, we utilize the MQTT messaging protocol to publish and subscribe to various messages and topics. In an attempt to standardize the MQTT event message structure, this package works to define a standard topic hierarchy, standard event types to use, and a standard payload structure that can be replicated and re-used throughout the industry. This structure will be consistent with the CloudEvent structure defined [here] (https://cloudevents.io/) while implementing some additional standards and best practices so that these events can be consumed and used by CloudEvent users as well.
+EbbCarbon package to standardize event message structures. For environmental and industrial automation montioring, we are using many physical sensors to read/gather data about our systems and the environment. In order to communicate this information across systems, we are utilizing the MQTT messaging protocol to publish and subscribe to various messages and topics (however, this structure can be used to publish events across various other protocols as well). In an attempt to standardize the event message structure, this package works to define a standard topic hierarchy, standard event types to use, and a standard payload structure that can be replicated and re-used throughout the industry. This structure will be consistent with the CloudEvent structure defined [here] (https://cloudevents.io/) while implementing some additional standards and best practices so that these events can be consumed and used by CloudEvent users as well.
 
 # Use:
-Install the ebb-events package from pip installer and use it to format your MQTT event messages and topics.
+Install the ebb-events package from pip installer via: `pip install ebb-events`.
+Use ebb-events to format your event messages and topics.
 ```python
 from ebb_events.builders.event_builder import EventEnvelope
 
 event_envelope = EventEnvelope(
     organization="test-org",
     system_id="test-system",
     event_type="data",
     subsystem_id="test-subsystem",
     device_id="test-device-01",
 )
 
 event_topic = event_envelope.build_event_topic()
-event_payload = event_envelope.build_event_payload(message={...}, metadata={...})  # Builds a payload of the expected ebb-events structure
+event_payload = event_envelope.build_event_payload_json(message={...}, metadata={...})  # Builds a payload of the expected ebb-events structure
 ```
 
 Use ebb-events package to consume events published with this expected ebb-events structure
 ```python
 from ebb_events.consumers.event_consumer import EventConsumer
 
-my_payload = {...}
-event_consumer = EventConsumer(payload=my_payload)
+my_event_payload = {...}
+event_consumer = EventConsumer(payload=my_event_payload)
 
-event_consumer.get_event_message()  # Retrieves the json message found in the payload's `data` field
+event_consumer.get_event_message()  # Retrieves the dict message found in the payload's `data` field
 event_consumer.get_event_time()
 event_conumser.get_event_system_id()
 ```
 
 # Topic Structure:
 One thing that this package enforces is a topic structure for publishing MQTT messages to a broker. Well defined topics help Our topic structure is as follows:
 * _\<organization\>/\<system-id\>/\<event-type\>/\<subsystem-id\>/\<device-id\>_
@@ -87,24 +88,40 @@
     "source": str,  # same as topic string
     "type": str,
     "data": {
         "metadata": {
             "serial_number": str,  # Example of potential metadata, this is not a required metadata field
             ...
         },
-        ...  # unique nested json dependent on event-type
+        ...  # unique nested JSON dependent on event-type
     }
 }
 ```
 
+### Suggested `data` Event Message Structure:
+The ebb-events package allows users to publish payloads of any structure (as long as they are JSON serializable) so that it can be helpful for publishing all types of events.  However, we have a recommened message structure that we encourage all to adopt when publishing sensor data events that will allow consumers to process the readings smoothly and accurately. Each variable that is measured by a sensor should named following the convention outlined [here](https://cfconventions.org/Data/cf-standard-names/current/build/cf-standard-name-table.html) whenever possible, and should have a corresponding `value` and `units` attached to it and should be formatted in the `message` argument of `build_event_payload_json/dict(message={})` like so:
+```python
+message = {
+    "variable_name_1": {
+        "value": ____,
+        "units": str
+    },
+    "variable_name_2": {
+        "value": ____,
+        "units": str
+    },
+    ...
+}
+```
+
 ### EventEnvelope Class:
 The EventEnvelope class is used to consolidate all of the pieces of aa event payload and build the expected structure for a user so that users don't have to worry about constructing the properly formatted topic or payload. The `EventEnvelope` class expects to be provided with certain fields that are then used to build the topic and payload via class methods. These methods handle all the validation and formatting needed to ensure that your events follow the ebb-events standards.
 
 Required fields: `organization`, `system_id`, `event_type`, `subsystem_id`, `device_id`
 Useful methods: `EventEnvelope().build_event_topic()`, `EventEnvelope().build_event_payload()`
 
 # Event Consumer:
-This package defines an event consumer that can be used to process incoming events that follow this ebb-events structure. To use this consumer, initialize the class with a given json payload: `EventConsumer(payload=my_payload)`. Then, you can use the various getters present on the class in order to retrieve different pieces of the payload depending on your needs (e.g. system_id, message, metadata, etc.). If you need all the parts of the payload that go into building it (e.g. an entire `EventEnvelope` wrapper for the payload) you may also use the `get_event_envelope()` method to do so.
+This package defines an event consumer that can be used to process incoming events that follow this ebb-events structure. To use this consumer, initialize the class with a given JSON payload: `EventConsumer(payload=my_payload)`. Then, you can use the various getters present on the class in order to retrieve different pieces of the payload depending on your needs (e.g. system_id, message, metadata, etc.). If you need all the parts of the payload that go into building it (e.g. an entire `EventEnvelope` wrapper for the payload) you may also use the `get_event_envelope()` method to do so.
 
 ### Exception Handling
-If you attempt to consume an event that _DOES NOT_ match the ebb-events structure, you can still initialize an `EventConsumer(payload=my_payload)` object and the payload will live as `EventConsumer().raw_payload`. However, all of the getter methods will raise `PayloadFormatExceptions` because the payload does not match the expected format. Therefore, for a payload that does not match the ebb-events structure, you must process the payload as a raw json/dict object instead.
+If you attempt to consume an event that _DOES NOT_ match the ebb-events structure, you can still initialize an `EventConsumer(payload=my_payload)` object and the payload will live as `EventConsumer().raw_payload`. However, all of the getter methods will raise `PayloadFormatExceptions` because the payload does not match the expected format. Therefore, for a payload that does not match the ebb-events structure, you must process the payload as a raw JSON/dict object instead.
```

