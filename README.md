# Test_Kafka_Cluster

## Using Apache JMeter to Test Kafka Cluster

Apache JMeter is a popular open-source tool used for load testing and performance measurement. Although it is primarily designed for web applications, in our case we will use it to test Apache Kafka clusters.
This document will guide you through the process of using JMeter to test a Kafka cluster.

## Prerequisites:

Apache JMeter: Download and install Apache JMeter from the official website [Apache JMeter Download](https://jmeter.apache.org/download_jmeter.cgi)
Follow the link > Source > Download the ZIP file.

## Now JMeter plugins to run the test for a KAFKA Cluster:
In Apache JMeter, you can manage plugins using the JMeter Plugins Manager. The Plugins Manager is a convenient tool that allows you to install, uninstall, and update JMeter plugins more easily.
### To Download the Plugins Manage follow the link [here](https://jmeter-plugins.org/install/Install/) 
Download the JAR file and move it to this path 
```
apache-jmeter-x.x.x / lib / ext
```
First, download the Plugins Manager  From this link (https://jmeter-plugins.org/install/Install/)
The easiest way to get the plugins is to install Plugins Manager. 
#### 1- pepper-box:
- Build the pepper-box JAR file from the source found [here](https://github.com/GSLabDev/pepper-box)
- Copy the JAR file to your JMeter lib/ext folder.
  
Once installed you have a couple of Config Elements and a Sampler and it

#### 2- KLoadgen:
is a plugin designed to work with AVRO Schema Registries.
- Build the pepper-box JAR file from the source found [Here](https://github.com/sngular/kloadgen)
- Copy the JAR file to your JMeter lib/ext folder.
- You can follow the steps [How to run a test plan](https://github.com/sngular/kloadgen/wiki/how-to-run#how-to-run-a-test-plan) to start the Test.
  
-------------------
## How to build a JAR file from the Maven project:


Kafka JMeter Plugin: Download the Kafka JMeter plugin from the following GitHub repository (https://github.com/Blazemeter/kafka-jmeter) ↗) and place it in the JMeter's "lib/ext" directory.

Kafka Cluster: Set up a Kafka cluster with one or more brokers. Ensure that you have the necessary connection details (bootstrap servers, topics, etc.) for testing.
