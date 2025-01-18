# RabbitMQDemo

A demo project demonstrating the use of RabbitMQ for message queuing and handling in a distributed system. This repository serves as a starting point for learning and experimenting with RabbitMQ integration in .NET applications.

---

## Features

- **Message Queuing:** Utilizes RabbitMQ for reliable message delivery.
- **Publisher-Subscriber Pattern:** Implements a basic pub-sub model.
- **Scalable Architecture:** Designed for distributed systems.
- **.NET Integration:** Built using C# and .NET.

---

docker run -d --hostname rmq --name rabbit-server -p 8080:15672 -p 5672:5672 rabbitmq:3-management
