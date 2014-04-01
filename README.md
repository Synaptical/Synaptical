# Synaptical


A typical Synaptical system has two levels: Ambient and Cosmos

## Ambient

Ambient is all devices physically within the border of, or close to your home. They communicate to each others via WiFi, Bluetooth LTE, XBEE or other close range techologies.

At this level security is not first priority, low energy consumption and seamless integration between devices are more important.

For smart devices, protocal of choice is ZeroMQ, the second one is RESTful json based Web API

For dumb devices, there will be proxies who talk their low level protocal like XBEE, then proxies will use ZeroMQ and RESTful API like other smart devices


http://docs.saltstack.com/en/latest/topics/topology/proxyminion/index.html


## Cosmos

Or in other word, the Internet

 * Web Hooks (HTTPS/JSON/PUBSUBHUBBUB)
 * XMPP (firewall peneration, long live connection, SASL secured)

## Gatekeeper

The one sit between Ambient and Cosmos
