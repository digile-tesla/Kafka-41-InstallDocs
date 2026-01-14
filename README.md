# Kafka-41-InstallDocs
Installation docs for Kafka in Windows 11 Pro
# Pre-Requisities
1.Kafka to be downloaded and extracted
https://kafka.apache.org/41/getting-started/quickstart/
2. set the path of kafka to extracted bin folder
3.Docker to be installed 
https://docs.docker.com/desktop/setup/install/windows-install/
4. Get a guid from powershell using the below command
New-Guid | Set-Clipboard
5. Create a folder in your localdesktop.
6. Execute the following commands from your local desktop folder
7.kafka-storage.sh format --standalone -t $KAFKA_CLUSTER_ID -c config/server.properties
8.kafka-server-start.sh config/server.properties
9.docker pull apache/kafka:4.1.1
10. docker run -p 9092:9092 apache/kafka:4.1.1
11. kafka-topics.sh --create --topic quickstart-events --bootstrap-server localhost:9092
12.kafka-topics.sh --describe --topic quickstart-events --bootstrap-server localhost:9092
  .kafka-console-producer.sh --topic quickstart-events --bootstrap-server localhost:9092
>This is my first event
13. kafka-console-consumer.sh --topic quickstart-events --from-beginning --bootstrap-server localhost:9092
This is my first event
This is my second event
14.
>This is my second event

