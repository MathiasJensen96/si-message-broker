# si-message-broker

## Quick Start ##
### Download Kafka latest ###
https://www.apache.org/dyn/closer.cgi?path=/kafka/3.6.0/kafka_2.13-3.6.0.tgz

Click this Http link:
https://dlcdn.apache.org/kafka/3.6.0/kafka_2.13-3.6.0.tgz

And put it in the Downloads folder.

Open the CMD / terminal and cd to the kafka file.
```
$ cd Downloads
$ cd kafka_2.13-3.6.0
```
#### Kafka with ZooKeeper ####
Run the following commands in order to start all services in the correct order:

```
$ bin/zookeeper-server-start.sh config/zookeeper.properties
```

In a new CMD / Terminal run this command:

```
$ bin/kafka-server-start.sh config/server.properties
```
Once all services have successfully launched, you will have a basic Kafka environment running and ready to use.

You will now see that your Kafka env is running on port :9092

## Read Event ##
Run in a new CMD / Terminal this command:
```
$ bin/kafka-console-consumer.sh --topic ["NameOfTopic"] --from-beginning --bootstrap-server localhost:9092
```

##

### for a Food Delivery Application: ###
#### Order Processing: ####

Use message brokers and data streaming for real-time order processing, tracking, and updates.
#### Inventory Management: ####

Implement communication channels for real-time updates on inventory levels and item availability.
#### Delivery Tracking: ####

Utilize data streaming for real-time tracking of delivery status, location updates, and estimated delivery times.
#### Customer Notifications: ####

Use message brokers to trigger notifications to customers about order confirmations, delays, or other relevant updates.


We intend to use kafka as a message broker between our microservices for our exam project. This will allow our customer service to communicate with our restaurant service and from there to our courier service.

## 

### Accessibility:

#### Simple Integration:

Kafka integrates easily with various applications using client libraries in popular programming languages.
#### RESTful Interface:

Offers a user-friendly RESTful interface accessible through simple HTTP requests.
#### Scalability:

Scales horizontally to handle growing workloads, ensuring quick access for both suppliers and employees.
### Reliability:

#### Fault Tolerance:

Designed to be fault-tolerant, with data replication to prevent disruptions in communication.
#### Durability:

Persists messages to disk, providing data durability and preventing message loss during system failures.
### Benefits:

#### Real-time Updates:

Suppliers receive instant updates on orders, enabling quick adjustments to inventory and production.
#### Efficient Communication:

Enables seamless communication within the company, keeping everyone informed of critical updates.
#### Streamlined Processing:

Facilitates streamlined order processing with real-time tracking for both suppliers and employees.
#### Improved Decision-Making:

Empowers informed decision-making by providing timely and reliable information.
#### Cost-effective Scaling:

Scales cost-effectively, accommodating increased communication needs as the company grows.

In essence, Kafka ensures quick, reliable, and cost-effective communication, benefiting both suppliers and employees in a food delivery company.
