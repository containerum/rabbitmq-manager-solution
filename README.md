# Rabbit MQ

RabbitMQ is a message broker. Its main purpose is to receive and send messages. RabbitMQ uses AMQP protocol.

### How it works

The server is launched on containerum.com and RabbitMQ provides a web UI for management and monitoring of your RabbitMQ server.

Using the RabbitMQ management interface, you can handle, create, delete and list queues. You can also monitor queue length, check message rate, change and add users permissions, etc.

### It consists of:

* RabbitMQ  


To launch this solution on Containerum.com sign up with the service, download and use [Containerum CLI](https://github.com/containerum/chkit) `chkit`.

1. Run the Solution with `chkit solution`:
```
chkit solution run containerum/rabbitmq-manager-solution -e NAME=rabbit -e USER=admin -e PASSWORD=12345678
```

2. Make sure that the Solution is running:

```
$ chkit get deploy
+--------------+------+-------------+------+-------+-----+
|     NAME     | PODS | PODS ACTIVE | CPU  |  RAM  | AGE |
+--------------+------+-------------+------+-------+-----+
| rabbit-nzdd6 |    1 |           1 | 500m | 500Mi | 9s  |
+--------------+------+-------------+------+-------+-----+
```
3. Using `chkit get` get the address and the port to access the running Solution:
```
$ chkit get svc
+--------------+----------------+----------+-------------------+-----------------+-----+
|     NAME     |   CLUSTER-IP   | EXTERNAL |       HOST        |      PORTS      | AGE |
+--------------+----------------+----------+-------------------+-----------------+-----+
| rabbit-nzdd6 | 10.105.101.228 | true     | x2.containerum.io | 28553:15672/TCP | 36s |
+--------------+----------------+----------+-------------------+-----------------+-----+
```
4. Go to `x2.containerum.io:28553`and create queues using UI.

![](/gif/rabbitsln.gif)
