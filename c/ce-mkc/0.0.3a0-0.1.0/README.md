# Comparing `tmp/ce_mkc-0.0.3a0.tar.gz` & `tmp/ce_mkc-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ce_mkc-0.0.3a0.tar", max compression
+gzip compressed data, was "ce_mkc-0.1.0.tar", max compression
```

## Comparing `ce_mkc-0.0.3a0.tar` & `ce_mkc-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,4 @@
--rw-r--r--   0        0        0    15263 2024-05-10 14:59:58.510746 ce_mkc-0.0.3a0/README.md
--rw-r--r--   0        0        0       33 2024-05-10 14:59:58.510746 ce_mkc-0.0.3a0/ce_mkc/__init__.py
--rw-r--r--   0        0        0      163 2024-05-10 14:59:58.510746 ce_mkc-0.0.3a0/ce_mkc/__main__.py
--rw-r--r--   0        0        0        0 2024-05-10 14:59:58.510746 ce_mkc-0.0.3a0/ce_mkc/main/__init__.py
--rw-r--r--   0        0        0    30339 2024-05-10 14:59:58.510746 ce_mkc-0.0.3a0/ce_mkc/main/ce_mkc.py
--rw-r--r--   0        0        0        0 2024-05-10 14:59:58.510746 ce_mkc-0.0.3a0/ce_mkc/templates/__init__.py
--rw-r--r--   0        0        0      547 2024-05-10 14:59:58.510746 ce_mkc-0.0.3a0/ce_mkc/templates/akhq/akhq.template
--rw-r--r--   0        0        0     5286 2024-05-10 14:59:58.510746 ce_mkc-0.0.3a0/ce_mkc/templates/docker-compose.template
--rw-r--r--   0        0        0     4397 2024-05-10 14:59:58.510746 ce_mkc-0.0.3a0/ce_mkc/templates/docker-compose.template.reference
--rw-r--r--   0        0        0     2104 2024-05-10 14:59:58.510746 ce_mkc-0.0.3a0/ce_mkc/templates/kafka/kafka.template
--rw-r--r--   0        0        0      183 2024-05-10 14:59:58.510746 ce_mkc-0.0.3a0/ce_mkc/templates/kafka/kafka_server_jaas.conf.template
--rw-r--r--   0        0        0      313 2024-05-10 14:59:58.510746 ce_mkc-0.0.3a0/ce_mkc/templates/kafka/zookeeper.template
--rw-r--r--   0        0        0     2251 2024-05-10 14:59:58.510746 ce_mkc-0.0.3a0/ce_mkc/templates/kafkaconnect/kafkaconnect.template
--rw-r--r--   0        0        0      112 2024-05-10 14:59:58.514746 ce_mkc-0.0.3a0/ce_mkc/templates/mongod/mongod.conf.template
--rw-r--r--   0        0        0      372 2024-05-10 14:59:58.514746 ce_mkc-0.0.3a0/ce_mkc/templates/mongod/mongod.template
--rw-r--r--   0        0        0      335 2024-05-10 14:59:58.514746 ce_mkc-0.0.3a0/ce_mkc/templates/schemaregistry/schemaregistry.template
--rw-r--r--   0        0        0      420 2024-05-10 14:59:58.518746 ce_mkc-0.0.3a0/pyproject.toml
--rw-r--r--   0        0        0    15794 1970-01-01 00:00:00.000000 ce_mkc-0.0.3a0/PKG-INFO
+-rw-r--r--   0        0        0    15263 2024-03-20 07:03:50.879186 ce_mkc-0.1.0/README.md
+-rw-r--r--   0        0        0    24186 2024-03-20 07:03:50.886024 ce_mkc-0.1.0/ce_mkc.py
+-rw-r--r--   0        0        0      595 2024-05-06 13:09:49.902413 ce_mkc-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0    16090 1970-01-01 00:00:00.000000 ce_mkc-0.1.0/PKG-INFO
```

### Comparing `ce_mkc-0.0.3a0/README.md` & `ce_mkc-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `ce_mkc-0.0.3a0/ce_mkc/main/ce_mkc.py` & `ce_mkc-0.1.0/ce_mkc.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,27 +8,21 @@
 import time
 from pymongo import MongoClient
 from zipfile import ZipFile
 
 import docker
 import requests
 
-#import templates
-from importlib import resources as impresources
-from ce_mkc import templates
-
 ########################################################################################################################
 # Constants
 ########################################################################################################################
 
 DEFAULT_CONFIG_DATA = {
         "zookeeperVersion" : "6.2.0",
-        "kafka" : {
-            "version" : "6.2.0"
-        },
+        "kafkaVersion" : "6.2.0",
         "schemaRegistryVersion" : "6.2.0",
         "kafkaConnectVersion" : "6.2.0",
         "kafkaCatVersion" : "1.6.0",
         "mongodbVersion" : "5.2.0",
         "zookeeperVersion" : "6.2.0",
         "akhqVersion" : "0.24.0"
     }
@@ -37,36 +31,27 @@
 KAFKA_CONNECT_CONTAINER_NAME = "kafkaConnectContainer-mkc"
 SCHEMA_REGISTRY_CONTAINER_NAME = "schemaRegistryContainer-mkc"
 KAFKA_BROKER_CONTAINER_NAME = "kafkaBrokerContainer-mkc"
 ZOOKEEPER_CONTAINER_NAME = "zookeeperContainer-mkc"
 MONGODB_SERVER_CONTAINER_NAME = "mongodContainer-mkc"
 AKHQ_SERVER_CONTAINER_NAME = "akhqContainer-mkc"
 
-KAFKA_DEFAULT_DOCKER_INTERNAL_PORT="29092"
-KAFKA_DEFAULT_HOST_INTERNAL_PORT="9092"
-KAFKA_DEFAULT_HOST_INTERNAL_HOSTNAME="localhost"
-KAFKA_DEFAULT_HOST_INTERNAL_SECURITY_PROTOCOL="PLAINTEXT"
-
 CONTAINERS = [
     KAFKA_CONNECT_CONTAINER_NAME,
     SCHEMA_REGISTRY_CONTAINER_NAME,
     KAFKA_BROKER_CONTAINER_NAME,
     ZOOKEEPER_CONTAINER_NAME
 ]
 
-CONTAINER_TEMPLATE_PATH_AKHQ = "akhq/akhq.template"
-CONTAINER_TEMPLATE_PATH_KAFKA = "kafka/kafka.template"
-KAFKA_SERVER_JAAS_TEMPLATE_PATH = "kafka/kafka_server_jaas.conf.template"
-CONTAINER_TEMPLATE_PATH_ZOOKEEPER = "kafka/zookeeper.template"
-CONTAINER_TEMPLATE_PATH_MONGOD = "mongod/mongod.template"
-CONTAINER_TEMPLATE_PATH_KAFKA_CONNECT = "kafkaconnect/kafkaconnect.template"
-CONTAINER_TEMPLATE_PATH_SCHEMA_REGISTRY = "schemaregistry/schemaregistry.template"
-
-DOCKER_COMPOSE_TEMPLATE_PATH = "docker-compose.template"
-MONGODB_CONF_TEMPLATE_PATH = "mongod/mongod.conf.template"
+CONTAINER_TEMPLATE_PATH_AKHQ = "templates/akhq/akhq.template"
+CONTAINER_TEMPLATE_PATH_KAFKA = "templates/kafka/kafka.template"
+CONTAINER_TEMPLATE_PATH_ZOOKEEPER = "templates/kafka/zookeeper.template"
+CONTAINER_TEMPLATE_PATH_MONGOD = "templates/mongod/mongod.template"
+CONTAINER_TEMPLATE_PATH_KAFKA_CONNECT = "templates/kafkaconnect/kafkaconnect.template"
+CONTAINER_TEMPLATE_PATH_SCHEMA_REGISTRY = "templates/schemaregistry/schemaregistry.template"
 
 
 CONNECTOR_DOWNLOADS_PATH = "connector-downloads"
 MDB_KAFKA_CONNECTOR_VERSIONS = [
     "0.1",
     "0.2",
     "1.0.0",
@@ -120,29 +105,34 @@
     },
     "confluent-datagen-connector" : {
         "downloadURL" : "https://d1i4a15mxbxib1.cloudfront.net/api/plugins/confluentinc/kafka-connect-datagen/versions/{version}/confluentinc-kafka-connect-datagen-{version}.zip",
         "versions" : CONFLUENT_DATAGEN_CONNECTORS_VERSIONS
     }
 }
 
+
+DOCKER_COMPOSE_TEMPLATE_PATH = "templates/docker-compose.template"
+MONGODB_CONF_TEMPLATE_PATH = "templates/mongod/mongod.conf.template"
+
 MONGODB_CONN_STR = "localhost:27017"
 KAFKA_CONNECT_CONFIG_URL = "http://localhost:8083"
 SCHEMA_REGISTRY_CONFIG_URL = "http://localhost:8081"
 
 ########################################################################################################################
 # Helper Methods
 ########################################################################################################################
 
 def createMongoDBConfFromTemplate(config):
     """
     Create MongoDB Conf From Template
 
     :return:
     """
-    templateData = readTemplate(MONGODB_CONF_TEMPLATE_PATH)
+    with open(MONGODB_CONF_TEMPLATE_PATH, 'r') as f:
+        templateData = f.read()
 
     mongodbConfFile = templateData.format()
     logging.debug("Created docker-compose file data {}".format(mongodbConfFile))
 
     return mongodbConfFile
 
 def downloadConnectorJar(connectorName, downloadUrl, connectorVersion="latest", forceDownload=False):
@@ -183,127 +173,27 @@
     with requests.get(url, stream=True) as r:
         r.raise_for_status()
         with open(localFileName, "wb") as f:
             for chunk in r.iter_content(chunk_size=8192):
                 f.write(chunk)
     return localFileName, fileName
 
-def buildHostInternalConfig(config):
-
-    result = {
-        "hostname" : KAFKA_DEFAULT_HOST_INTERNAL_HOSTNAME,
-        "port" : KAFKA_DEFAULT_HOST_INTERNAL_PORT,
-        "securityProtocol" : KAFKA_DEFAULT_HOST_INTERNAL_SECURITY_PROTOCOL
-    }
-        
-    if "listeners" in config["kafka"] and "host" in config["kafka"]["listeners"]:
-        hostInternalConfig = config["kafka"]["listeners"]["host"]
-
-        if hostInternalConfig is not None:
-            if "port" in hostInternalConfig:
-                result["port"] = str(hostInternalConfig["port"])
-            
-            if "hostname" in hostInternalConfig:
-                result["hostname"] = hostInternalConfig["hostname"]
-
-            if "securityProtocol" in hostInternalConfig:
-                result["securityProtocol"] = hostInternalConfig["securityProtocol"]
-        
-    return result
-
-def buildHostExternalConfig(config):
-    if "listeners" in config["kafka"] and "external" in config["kafka"]["listeners"]:
-        hostExternalConfig = config["kafka"]["listeners"]["external"]
-        result = { }
-        if hostExternalConfig is not None:
-            if "port" in hostExternalConfig:
-                result["port"] = str(hostExternalConfig["port"])
-            else:
-                errorMessage = f"'port' is required when defining an external interface"
-                logging.error(errorMessage)
-                raise Exception(errorMessage)
-            
-            if "hostname" in hostExternalConfig:
-                result["hostname"] = hostExternalConfig["hostname"]
-            else:
-                errorMessage = f"'hostname' is required when defining an external interface"
-                logging.error(errorMessage)
-                raise Exception(errorMessage)
-
-            if "securityProtocol" in hostExternalConfig:
-                result["securityProtocol"] = hostExternalConfig["securityProtocol"]
-            else:
-                errorMessage = f"'securityProtocol' is required when defining an external interface"
-                logging.error(errorMessage)
-                raise Exception(errorMessage)
-        
-        return result
-    else:
-        return None
-
-
 def createDockerComposeFileFromTemplate(config):
     """
     Create Docker Compose Template
 
     :return:
     """
-
-    currentPID = os.getpid()
-    dockerFile = f"docker-compose.{currentPID}.yml"
-    logging.info(f"Generating docker-compose file at {dockerFile} ...")
-    kafka_server_jaas_File = f"kafka_server_jaas.{currentPID}.conf"
-
     dockerComposeBase = "---\nversion: '2'\nservices:\n"
-    if "kafka" in config:
+    if "kafkaVersion" in config:
         zookeeperContainerConfig = readTemplate(CONTAINER_TEMPLATE_PATH_ZOOKEEPER)
         zookeeperContainerConfig = zookeeperContainerConfig.format(zookeeper_version=config["zookeeperVersion"], zookeeper_container_name=ZOOKEEPER_CONTAINER_NAME)
         dockerComposeBase += "\n{}\n".format(zookeeperContainerConfig)
         kafkaContainerConfig = readTemplate(CONTAINER_TEMPLATE_PATH_KAFKA)
-        
-        #build advertised_listeners and advertised_listeners_security_protocol
-        #create docker internal interface
-        advertised_listeners = "DOCKER_INTERNAL://broker:" + KAFKA_DEFAULT_DOCKER_INTERNAL_PORT
-        advertised_listeners_security_protocol = "DOCKER_INTERNAL:PLAINTEXT"
-        
-        #create host internal interface
-        hostInternalConfig = buildHostInternalConfig(config)
-        advertised_listeners += ",HOST_INTERNAL://" + hostInternalConfig["hostname"] + ":" + hostInternalConfig["port"]
-        advertised_listeners_security_protocol += ",HOST_INTERNAL:" + hostInternalConfig["securityProtocol"]
-
-        #create host external interface
-        external_port_mapping = ""
-        hostExternalConfig = buildHostExternalConfig(config)
-        if hostExternalConfig is not None:
-            advertised_listeners += ",HOST_EXTERNAL://" + hostExternalConfig["hostname"] + ":" + hostExternalConfig["port"]
-            advertised_listeners_security_protocol += ",HOST_EXTERNAL:" + hostExternalConfig["securityProtocol"]
-            external_port_mapping = "- " + hostExternalConfig["port"] + ":" + hostExternalConfig["port"]
-        
-        logging.info(f"{advertised_listeners}")
-        logging.info(f"{advertised_listeners_security_protocol}")
-        logging.info(f"{external_port_mapping}")
-
-        #create jaas file
-        kafkaServerJaasTemplate = readTemplate(KAFKA_SERVER_JAAS_TEMPLATE_PATH)
-        additional_users = ""
-        if "credentials" in config["kafka"]:
-            credentials = config["kafka"]["credentials"]
-            for c in credentials:
-                additional_users += "user_" + c["username"] + "=\"" + c["password"] + "\"" + "\n"
-        kafkaServerJaasContent = kafkaServerJaasTemplate.format(additional_users = additional_users)
-
-        kafkaContainerConfig = kafkaContainerConfig.format(
-            kafka_version=config["kafka"]["version"], 
-            kafka_broker_container_name=KAFKA_BROKER_CONTAINER_NAME,
-            external_port_mapping=external_port_mapping,
-            kafka_server_jaas=kafka_server_jaas_File,
-            advertised_listeners=advertised_listeners,
-            advertised_listeners_security_protocol=advertised_listeners_security_protocol,
-            inter_broker_listener="DOCKER_INTERNAL"
-            )
+        kafkaContainerConfig = kafkaContainerConfig.format(kafka_version=config["kafkaVersion"], kafka_broker_container_name=KAFKA_BROKER_CONTAINER_NAME)
         dockerComposeBase += "\n{}\n".format(kafkaContainerConfig)
 
     if "schemaRegistryVersion" in config:
         schemaRegistryContainerConfig = readTemplate(CONTAINER_TEMPLATE_PATH_SCHEMA_REGISTRY)
         schemaRegistryContainerConfig = schemaRegistryContainerConfig.format(schema_registry_version=config["schemaRegistryVersion"], schema_registry_container_name=SCHEMA_REGISTRY_CONTAINER_NAME)
         dockerComposeBase += "\n{}\n".format(schemaRegistryContainerConfig)
 
@@ -320,31 +210,27 @@
     if "akhqVersion" in config:
         akhqContainerConfig = readTemplate(CONTAINER_TEMPLATE_PATH_AKHQ)
         akhqContainerConfig = akhqContainerConfig.format(akhq_version=config["akhqVersion"], akhq_container_name=AKHQ_SERVER_CONTAINER_NAME)
         dockerComposeBase += "\n{}\n".format(akhqContainerConfig)
 
     logging.debug("Created docker-compose file data {}".format(dockerComposeBase))
 
-    
+    currentPID = os.getpid()
+    dockerFile = f"docker-compose.{currentPID}.yml"
     with open(dockerFile, "w") as f:
         f.write(dockerComposeBase)
-
-    with open(kafka_server_jaas_File, "w") as f:
-        f.write(kafkaServerJaasContent)
-
     return dockerFile
 
 def readTemplate(templatePath):
     """
     Read Template
     :param templatePath:
     :return:
     """
-    inp_file = impresources.files(templates) / templatePath
-    with inp_file.open("rt") as f:
+    with open(templatePath, 'r') as f:
         templateData = f.read()
     return templateData
 
 
 def parseConfigFile(configFile, launchFullStack=False):
     """
     Parse Config File
@@ -362,35 +248,14 @@
         configFileData = json.loads(configFileData)
 
     # Override any default with the config.json values from the file
     if launchFullStack:
         fullConfigData = { **DEFAULT_CONFIG_DATA, **configFileData }
     else:
         fullConfigData = configFileData
-    return validateKafkaConfigVersions(fullConfigData)
-
-
-def validateKafkaConfigVersions(fullConfigData):
-    if "kafkaVersion" in fullConfigData: 
-        #we need to replace with the kafka structure
-
-        #first we check if kafka already exists, if it does we use what's provided iff kafkaVersion == kafka.version
-        if "kafka" in fullConfigData:
-            if "version" not in fullConfigData["kafka"]:
-                fullConfigData["kafka"]["version"] = fullConfigData["kafkaVersion"]
-            elif "version" in fullConfigData["kafka"] and fullConfigData["kafkaVersion"] != fullConfigData["kafka"]["version"]:
-                kafkaVersionValue = fullConfigData["kafkaVersion"]
-                kafkaDotVersionValue = fullConfigData["kafka"]["version"]
-                errorMessage = f"Incompatible 'kafkaVersion' {kafkaVersionValue} and 'kafka.version' {kafkaDotVersionValue} provided in the config file. These should be equal. Alternatively remove 'kafkaVersion' as not required when 'kafka' is defined."
-                logging.error(errorMessage)
-                raise Exception(errorMessage)
-        #now use the default instead
-        else:
-            fullConfigData["kafka"] = DEFAULT_CONFIG_DATA["kafka"]
-
     return fullConfigData
 
 
 def installStackViaDocker(dockerFilePath):
     """
     Install Kafka Stack Via Docker
 
@@ -501,19 +366,18 @@
             connectorName,
             connectorInstanceName
         ))
 
         numConnectorInstances = 1
         if "num" in connectorConfig:
             numConnectorInstances = int(connectorConfig["num"])
-
-        connectorEndpoint = f"{kafkaConnectAPIUrl}/connectors"
         for i in range(0, numConnectorInstances):
             connectorInstanceNameNumbered = "{}-{}".format(connectorInstanceName, i)
             connectorConfig["name"] = connectorInstanceName if numConnectorInstances == 1 else connectorInstanceNameNumbered
+            connectorEndpoint = f"{kafkaConnectAPIUrl}/connectors"
             headers = {
                 'Content-Type': 'application/json'
             }
             result = requests.post(url=connectorEndpoint, json=connectorConfig, headers=headers)
             logging.debug("Got status code {} result {}".format(result.status_code, json.dumps(result.json())))
 
     logging.info("Done installing connectors")
@@ -778,20 +642,18 @@
 def _configureLogger(logLevel):
     format = '%(message)s'
     if logLevel != 'INFO':
         format = '%(levelname)s: %(message)s'
     logging.basicConfig(format=format, level=logLevel.upper())
 
 def main():
-    print(__name__)
-    
     args = setupArgs()
     _configureLogger(args.logLevel.upper())
     createAndDeployStack(args)
 
-# if __name__ == "__main__":
-#     main()
+if __name__ == "__main__":
+    main()
 
 
 # TODO
 # Get schema registry to work
 # Get the data gen connector to work
```

### Comparing `ce_mkc-0.0.3a0/PKG-INFO` & `ce_mkc-0.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 Metadata-Version: 2.1
 Name: ce-mkc
-Version: 0.0.3a0
+Version: 0.1.0
 Summary: A command line utility to set up Kafka, MongoDB, and MongoDB Kafka Connector environments.
 License: MIT
 Author: Your Name
 Author-email: you@example.com
-Requires-Python: >=3.9,<3.10
+Requires-Python: >=3.10,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Dist: certifi (==2023.7.22)
+Requires-Dist: charset-normalizer (==3.2.0)
+Requires-Dist: confluent-kafka (==2.2.0)
+Requires-Dist: dnspython (==2.3.0)
 Requires-Dist: docker (==6.1.3)
+Requires-Dist: idna (==3.4)
+Requires-Dist: packaging (==23.1)
 Requires-Dist: pymongo (==4.5.0)
-Requires-Dist: requests (>=2.26)
+Requires-Dist: requests (>=1.26.6)
+Requires-Dist: urllib3 (==2.0.4)
+Requires-Dist: websocket-client (==1.6.1)
 Description-Content-Type: text/markdown
 
 # mkc 
 #### A command line utility to set up Kafka, MongoDB, and MongoDB Kafka Connector environments.
 
 mkc is a python script to create small stacks that pertain to MongoDB and the kafka connector. It uses docker-compose (specifically [this compose file](https://github.com/confluentinc/cp-all-in-one/blob/7.5.0-post/cp-all-in-one/docker-compose.yml) maintained by confluent) to achieve this. You can configure which pieces of the stack you want to deploy, which connectors (if applicable), and which schemas to register (if applicable).
```

