
## Assignment Questions:
## How ride Scheduling can be implemented in ride hailing app:

![flow](https://github.com/vansh123456/assignment/blob/b5404134cb6cb550b557aafcb4c1670fff6688bc/Image%201-3-25%20at%205.46%E2%80%AFPM.png)



## Abstract
we are first assuming that we have a /schedule endpoint that we will be hitting to create a schedule for the ride

## Request body
```
body{
    latitude:
    longitude:
    time:
    Fare:
    isScheduled:
}
```
## Choices

## Message Queues

Can use RabbitMQ or Amazon SQS

### Advantages
Scalable, reliable, decouples components

## Cache-Based
Redis with Bulls

### Advantages
can be easily cached and memory safe better for scalability and  supports retries and delays.

Though we will have to setup a message broker

## Serverless Based Solutions
### AWS lambda and CloudFlare workers
Server designed to accepts requests and hits the /schedule at the desired time and scheduling done via above methods so for scalability it can handle more requests 


