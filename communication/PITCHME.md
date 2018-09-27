# Communication between services

---

## HTTP

@ul[spaced-list-items]

* Hypertext Transfer Protocol
* Simple / fast to implement
* Very well known and supported
* Limited to client -> server communication
* Examples
  + Allsports API
  + Mapping / Matching services
  + Most data provider APIs

@ulend

---

## RabbitMQ

@ul[spaced-list-items]

* Message broker
* Reliable
* Easy Scalability
* Support for pub-sub / Remote Procedure Call (RPC)
* Examples
  + SD Data BUS
  + Stat service (Nameko)
  + Opta (Celery)

@ulend

---

## WAMP / Websocket

@ul[spaced-list-items]

* Web Application Messaging Protocol
* Based on Websocket (Bidirectional communication)
* Pub-sub / rpc easy to implement
* Example
  + Autobeast (Wamp)

@ulend
