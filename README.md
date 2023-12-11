# Test_Kafka_Cluster

## Using Apache JMeter to Test Kafka Cluster

Apache JMeter is a popular open-source tool used for load testing and performance measurement. Although it is primarily designed for web applications, in our case we will use it to test Apache Kafka clusters.
This document will guide you through the process of using JMeter to test a Kafka cluster.

## Prerequisites:

Apache JMeter: Download and install Apache JMeter from the official website [Apache JMeter Download](https://jmeter.apache.org/download_jmeter.cgi)
Follow the link > Source > Download the ZIP file.

## Install JMeter plugins to run the test for a KAFKA Cluster:
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
- follow these Steps [How to build a JAR file from the Maven project Using IntelliJ](https://github.com/Fahad-Alsubaihi/Test_Kafka_Cluster/edit/main/README.md#:~:text=How%20to%20build%20a%20JAR%20file%20from%20the%20Maven%20project%20Using%20IntelliJ)
- Copy the JAR file to your JMeter lib/ext folder.
  
Once installed you have a couple of Config Elements and a Sampler and it

#### 2- KLoadgen:
is a plugin designed to work with AVRO Schema Registries.
- Build the pepper-box JAR file from the source found [Here](https://github.com/sngular/kloadgen)
- follow these Steps [How to build a JAR file from the Maven project Using IntelliJ](https://github.com/Fahad-Alsubaihi/Test_Kafka_Cluster/edit/main/README.md#:~:text=How%20to%20build%20a%20JAR%20file%20from%20the%20Maven%20project%20Using%20IntelliJ)
- Copy the JAR file to your JMeter lib/ext folder.
- You can follow the steps [How to run a test plan](https://github.com/sngular/kloadgen/wiki/how-to-run#how-to-run-a-test-plan) to start the Test.
  
-------------------
## How to build a JAR file from the Maven project Using IntelliJ:
- open IntelliJ on the right-hand side and click on Maven
  
![IntelliJ](https://github.com/Fahad-Alsubaihi/Test_Kafka_Cluster/blob/main/step1.png?raw=true)

- click on LifeCycle
  
![IntelliJ](https://github.com/Fahad-Alsubaihi/Test_Kafka_Cluster/blob/main/step2.png?raw=true)

- Double-click on the clean to run the command and clean the project.
  
![IntelliJ](https://github.com/Fahad-Alsubaihi/Test_Kafka_Cluster/blob/main/step3.png?raw=true)

- After the cleaning is done Double-click on the package command and wait...  

![IntelliJ](https://github.com/Fahad-Alsubaihi/Test_Kafka_Cluster/blob/main/step4.png?raw=true)

- After the Build is done you can see your JAR file under the Target directory like the image below.

![IntelliJ](https://github.com/Fahad-Alsubaihi/Test_Kafka_Cluster/blob/main/final.png?raw=true)

#### Now your JAR file is ready to use 
