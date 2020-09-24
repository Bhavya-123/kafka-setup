# kAFKA-SETUP

### Below are the command to:
- Start the Zookeeper service:
.\bin\windows\zookeeper-server-start.bat .\config\zookeeper.properties

- Start the kafka Service:
.\bin\windows\kafka-server-start.bat .\config\server.properties

- Create a topic in Kafka:
.\bin\windows\kafka-topics.bat --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --create --topic shopping-orders

- List all the topics:
.\bin\windows\kafka-topics.bat --zookeeper localhost:2181 --list

- Run Producer to record messages:
.\bin\windows\kafka-console-producer.bat --broker-list localhost:9092 --topic shopping-orders

- Run Consumer to retrieve the messages from the beginning:
.\bin\windows\kafka-console-consumer.bat --bootstrap-server localhost:9092 --topic bearcat-messages --from-beginning


