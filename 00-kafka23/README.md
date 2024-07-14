Installing Apache Kafka server on MacOS
---------------------------------------
+ Open your web browser and go to the Apache Kafka download page: https://kafka.apache.org/downloads

+ Download the latest version of Kafka.

+ Navigate to the directory where you downloaded Kafka and extract and Unzip the downloaded kafka.


## Start ZooKeeper
+ Open a new terminal and navigate to the Kafka directory.
+ Type `bin/zookeeper-server-start.sh config/zookeeper.properties` in terminal.


## Start Kafka server
+ Open a new terminal and navigate to the Kafka directory.
+ Type `bin/kafka-server-start.sh config/server.properties` in terminal.

This will start the Kafka broker, and it will be ready to receive and process messages.

## Create Topic
+ Open a new terminal and navigate to the Kafka directory.
+ Type `bin/kafka-topics.sh --create --topic cities --bootstrap-server localhost:9092` in terminal.

## To List all the Topics
+ Open a new terminal and navigate to the Kafka directory.
+ Type `bin/kafka-topics.sh --list --bootstrap-server localhost:9092` in terminal.

## To stop the Kafka server
+ Open a new terminal and navigate to the Kafka directory.
+ Type `bin/kafka-server-stop.sh` in terminal.



References
----------

1. https://medium.com/@bectorhimanshu/setting-up-installing-and-starting-the-kafka-server-on-macos-7d505e32039a
