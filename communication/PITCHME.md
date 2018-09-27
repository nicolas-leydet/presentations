## Communication between services

---

## HTTP

@ul[spaced-list-items]

* Hypertext Transfer Protocol
* Simple / fast to implement
* Very well known and supported
* Examples
  + Allsports API
  + Mapping / Matching services
  + Most data provider APIs

@ulend

```
Client ---> Server
```

---

## RabbitMQ (AMQP)

@ul[spaced-list-items]

* Message broker
* Robust against peers/broker failure and restart
* Easy Scalability
* Support for pub-sub / Remote Procedure Call (RPC)
* Examples
  + SD Data BUS
  + Stat service (Nameko)
  + Opta worker cluster (Celery)

@ulend


```
Service ---> Queues <--- Service

```

---

## WAMP (Websocket)

@ul[spaced-list-items]

* Web Application Messaging Protocol
* Based on Websocket
* Pub-sub / rpc easy to implement
* Example
  + Autobeast

@ulend

```
Caller --> Broker --> Callee

Publisher --> Brocker --> Subscriber

```
