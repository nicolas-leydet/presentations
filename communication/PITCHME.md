# Communication between services

---

## HTTP

@ul[spaced-list-items]
 * Hypertext Transfer Protocol
 * Simple / easy to implement
 * Very well known and supported
 * Client -> server communication
 * Examples
   * Allsports API
   * Mapping / Matching services
@ulend

---

## RabbitMQ

@ul[spaced-list-items]
 * Message broker
 * Reliable
 * Easy Scalability
 * Support for Pub-sub / Remote Procedure Call (RPC)
 * Examples
   * SD Data BUS
   * Stat service (nameko)
@ulend

---

## WAMP / Websocket

@ul[spaced-list-items]
 * Web Application Messaging Protocol
 * Bidirectional
 * Pubsub / rpc easy to implement
 * Example
   * Autobeast (Wamp)
@ulend
