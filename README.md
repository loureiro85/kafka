# kafka
Repo for researching and practing data streaming through Apache Kafka

**Wikipedia Definition of Apache Kafka** 
[[source]](https://en.wikipedia.org/wiki/Apache_Kafka)

Apache Kafka is a distributed event store and stream-processing platform. 
It is an open-source system developed by the Apache Software Foundation written in Java and Scala. 
The project aims to provide a unified, high-throughput, low-latency platform for handling real-time data feeds.

From this definition, the following questions emerge:
- What is a distributed event store?
- What is stream-processing?
- What defines high-throughput?
- What defines low-latency?

These questions are guiding this research.
I hope to answer them during my practice with Apache Kafka.


Curiosity: The name derives from the author Franz Kafka.

**Publish-Subscribe pattern**
- Kafka is based on the Publish-Subscribe pattern in which publishers (senders) and subscribers (recievers) are connected asynchronously. Asynchronously reffering to a latency on the order of 100 miliseconds. See more at [[Pub/Sub Google Cloud definition]](https://cloud.google.com/pubsub/docs/overview).
-  Here`s a definition of the [pub-sub pattern](https://en.wikipedia.org/wiki/Publish%E2%80%93subscribe_pattern): "In software architecture, publish–subscribe is a messaging pattern where senders of messages, called publishers, do not program the messages to be sent directly to specific receivers, called subscribers, but instead categorize published messages into classes without knowledge of which subscribers, if any, there may be. Similarly, subscribers express interest in one or more classes and only receive messages that are of interest, without knowledge of which publishers, if any, there are."

Here's a well though video playlist from [Google Cloud about Pub/Sub](https://www.youtube.com/watch?v=cvu53CnZmGI&list=PLIivdWyY5sqKwVLe4BLJ-vlh9r9zCdOse)

Asynchronous integration, to react to messages (events). Reduces dependency. Facilitates new services integration.

- Connects to event sources and event sinks (postgres, AWS S3 and more)

Offical Kafka site
https://kafka.apache.org/intro
