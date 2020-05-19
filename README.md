# kafka
Apache Kafka is an open-source stream-processing software platform developed by LinkedIn and donated to the Apache Software Foundation, written in Scala and Java. The project aims to provide a unified, high-throughput, low-latency platform for handling real-time data feeds.
# kafka-commands
#### .\bin\windows\zookeeper-server-start.bat .\config\zookeeper.properties
This command is used to start the zookeeper.Zookeeper is distrubuted management tool which will manage all the kafka brokers.
#### .\bin\windows\kafka-server-start.bat .\config\server.properties
This command is used to run the kafka service by using the properities file.
#### .\bin\windows\kafka-topics.bat --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --create --topic book-authors
This command is used to create topic called book-authors. Topic is a place where kafka will store all the content.
#### .\bin\windows\kafka-console-producer.bat --broker-list localhost:9092 --topic book-authors
This will start producer in which we can produce different book authors.
#### .\bin\windows\kafka-console-consumer.bat --bootstrap-server localhost:9092 --topic book-authors
This is a consumer who wants to consume all the data produced by producer.

