# Chat Application
Scalable Real-Time Chat Application with Java & Spring Boot backend leveraging Kafka

## Before Running the Project 

*Start Zookeeper*
```shell script
zookeeper-server-start .\config\zookeeper.properties
```

*Start Kafka*
```shell script
kafka-server-start .\config\server.properties
```

*Create a Topic*
```
kafka-topics --create --topic kafka-chat --zookeeper localhost:2181 --replication-factor 1 --partitions 1
```

*Start Backend*
```
mvn spring-boot:run
```

*Start Frontend*
```
npm start
```



