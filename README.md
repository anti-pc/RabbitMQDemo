# RabbitMQDemo

A demo project demonstrating the use of RabbitMQ for message queuing and handling in a distributed system. This repository serves as a starting point for learning and experimenting with RabbitMQ integration in .NET applications.

---

## Features

- **Message Queuing:** Utilizes RabbitMQ for reliable message delivery.
- **Publisher-Subscriber Pattern:** Implements a basic pub-sub model.
- **Scalable Architecture:** Designed for distributed systems.
- **.NET Integration:** Built using C# and .NET.

---

## Prerequisites

Before running the project, ensure you have the following installed:

- **RabbitMQ Server:** Install and configure RabbitMQ on your local machine or use a hosted solution.
- **.NET SDK:** Version 6.0 or higher.
- **Docker:** Optional, for containerizing the RabbitMQ server.

---

## Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/anti-pc/RabbitMQDemo.git
cd RabbitMQDemo
```

### 2. Install Dependencies

Navigate to the project directory and restore the dependencies:

```bash
dotnet restore
```

### 3. Configure RabbitMQ

1. **Default Setup:** Ensure RabbitMQ is running locally on its default port (5672).
2. **Custom Setup:** Update the connection details in the `appsettings.json` file:

```json
{
  "RabbitMQ": {
    "HostName": "localhost",
    "UserName": "guest",
    "Password": "guest"
  }
}

```

### 4. Run the Application

To start the application, use the following command:

```bash
dotnet run
```

---

## Project Structure

```
RabbitMQDemo/
├── Publisher/
│   ├── Program.cs
│   ├── Publisher.cs
├── Subscriber/
│   ├── Program.cs
│   ├── Subscriber.cs
├── appsettings.json
└── README.md
```

- **Publisher:** Sends messages to the RabbitMQ queue.
- **Subscriber:** Listens to the queue and processes messages.


docker run -d --hostname rmq --name rabbit-server -p 8080:15672 -p 5672:5672 rabbitmq:3-management
