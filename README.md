# rabbitmq-manager-solution

## About
[RabbitMQ](https://www.rabbitmq.com) is an open source message broker: it accepts and forwards messages. It implements the Advanced Message Queuing Protocol (AMQP).

[RabbitMQ Management Plugin](https://www.rabbitmq.com/management.html) allows you to monitor and manage your RabbitMQ server along with a browser-based UI and a command line too.

**Here we run this plugin in one command with [Containerum](https://containerum.com).**

## How to deploy on Containerum

**1.** Sign Up at [containerum.com](https://containerum.com)

**2.** Install CLI Containerum `chkit` following [instruction](https://containerum.com/documentation/Installing-Containerum-CLI-from-binaries).

**3.** Open Terminal and run `chkit login`

```
$ chkit login
Enter your email: test@gmail.com
Password:
********
Chosen namespace: mynamespace
Successful login
Token changed to:  QA0u64rOkTtCxxxxxxxxxxliUAnBnPlCbGQfpCQpzqM=
```
**4.** Use command `run solution`
