# What we are building

Whenever a package is published to the NPM registry, you receive an event with information about the newly published package on a registered webhook. You can create an HTTP server that receives the event and uses KafkaJS to publish a message to Kafka to let you know that a new version of the package has been released.

You are also going to create a KafkaJS consumer that consumes the Kafka topic and sends a message to a Slack channel to notify users that there is a new package version available.

![alt text](https://cdn.confluent.io/wp-content/uploads/npm-to-slack-process-e1612135098854-2048x262.png)

# Prerequisites

- [Node.js](https://nodejs.org/en/).
- A Kafka cluster.
- [Docker]() & [Docker Compose]() if you decide to run Kafka locally.

Credit: Based on Tommy Brun's [tutorial](https://www.confluent.io/en-gb/blog/getting-started-with-kafkajs/)

The original code is written in JavaScript. I opted to use TypeScript as I do with most things lately.




