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
