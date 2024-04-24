### what is amqp?
AMQP stands for Advanced Message Queuing Protocol. It is an open standard application layer protocol for message-oriented middleware. The defining features of AMQP are message orientation, queuing, routing, reliability and security. AMQP is a binary protocol and is designed to efficiently support a wide variety of messaging applications and communication patterns.

### what it means? guest:guest@localhost:5672 , what is the first quest, and what is the second guest, and what is localhost:5672 is for?

The first guest is the username and the second guest is the password. The localhost:5672 is the host and port number. The default port number for AMQP is 5672.

### Slow subscriber
![slow](./image/Screenshot%202024-04-24%20200200.png)

the queue number in the queued messages is around 50. This happens because the subscriber is slow to receive the data from the message broker. The subscriber is slow because it sleep for 1 seconds before receiving the data from the message broker.

### 3 subscriber 1 publisher
![3sub1pub](./image/Screenshot%202024-04-24%20201148.png)

the queue messages is below 50 now. This happens because there are 3 subscribers that receive the data from the message broker. The data is distributed to the 3 subscribers.