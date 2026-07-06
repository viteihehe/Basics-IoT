# IoT World

**Current Problems**: In modern days, we have more and more complex problems. These are associated, in most cases, with a lack of communication between electronic devices. But since 1999, the world has stepped into the next level: the level of IoT, where your toaster connects to your TV and smartphone. Irrigation systems can be activated with the press of a button—this is the world of IoT. And now, you are going to enter this field of technology.

## Introduction to IoT

* **IoT**: Internet of Things. This acronym describes the network of hardware embedded with sensors, software, and other technologies with the objective of connecting and exchanging data with other devices and network systems over the internet.

* **Pillars**:
    * Sensors
    * Actuators
    * Network
    * Autonomous systems
    * AI (Artificial Intelligence)
    * Computer Vision

## Communication Protocols and Security for IoT

* **Communication protocols**: Are conventions that control and enable communication and data exchange between two or more computational devices. The most famous protocol is the OSI model.

### Universal Properties

* Node detection
* Handshaking (establishing a connection)
* Characteristics negotiation
* How to initiate messaging
* How to format a message
* What to do with a corrupted message
* How to detect a lost connection and what to do afterward
* End of session/connection

### Introduction to IoT Communication Layers

**IoT Protocols**: The most common protocols are:
1. Wi-Fi
2. Insteon
3. Bluetooth
4. Z-Wave
5. Zigbee
6. Thread Group

* These protocols need to be optimized, lightweight, and cheap to implement, operating with low traffic in unstable networks because the only use of this communication is exchanging small amounts of data.
* These devices establish connections through brokers, following the publisher-subscriber model. The broker only sends and receives data for specific topics.

The two emerging protocols for IoT are MQTT and REST.

#### Physical Layer:

Ethernet protocol IEEE 802.3: Is a connection protocols that needs a cable to acess the internet.

    Advantage: Speed and cheap internet connection.
    Disavantage: Needs a cable.

Wi-fi protocol IEEE 802.11: Internet wireless connection.

LPWA - Low Power Wide Area: Low power consumption network, allowing high distance communication.

    Advantage: Long range and low power consumption.
    Disavantage: Low data traffic, and strict message limit.

#### Transport Layer

This layer is inspired by the OSI model.

TCP/UDP:

    TCP is connection-oriented, this protocol holds a connection between two points, to terminate the link , both sides must signal their intent to disconnect.
    UDP isn't connection-oriented, the connection is simple, they only send and has no control over the package.

#### Aplication Layer

* MQTT: is based on TCP with SSL security. When two or more devices connected, they can exchange data, that data can be used for these devices for they function.

* CoAP: is a lightweight protocol, based in UDP with DTLS security, it can find other devices in coap network and send messages for a specifc ID. It controls which message read or not. Low payload.

* AMQP: is based on TCP with TLS security. It has incredible flexibility, can be used for (pub/sub) with brokers, direct messaging, and broadcast, and is highly secure. However, it lacks backward compatibility. 

* XMPP: is based on TCP with TLS and SASL security. It only works in client-server communication (servers can communicate with each other). It is used when you want to know about the endpoint and monitor the state of the devices, but can be used for instant messaging. It features a decentralized architecture, and big payload messages. However, it needs a high footprint device for the implementation. 

* DDS: is based on TCP with TLS and DDS security, but also use UDP with DTLS security. Communication is P2P, but need more network band.

* HTTP: Web protocol based on TCP with TLS security.