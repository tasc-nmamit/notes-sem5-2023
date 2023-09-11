---
aliases:
  - networking
---
# Unit 1

## Data Communication

<dl> 
<dt>Data Communication :</dt>
<dd>Exchange of data b/w 2 devices</dd>
</dl>

---

## Protocol Layering

Examples 
<dl> 
<dt>Single Layer Protocol : </dt>
<dt>Three Layer Protocol : </dt>
</dl>
### Principles of protocol layering {#imp}

- First Principle: Bidirectional communication - we need to make each layer so that it is able to perform two opposite tasks.
- Second Principle: (There should be equal number of layers in both sender and receiver side and the identical tasks should be performed in either sides.)

---

# TCP/IP Protocol Suite

Q. Explain TCP/IP protocol suite  
Q. Explain internet protocol suite

TCP/IP is a set of hierarchical protocol suite used in the Internet today.

![Insert diagram from ppt]  
which shows different devices at different layers
- switch → dl layer
- router → network layer
- sender/receiver → application layer

PDU are referred by different names across different layers of the OSI Model: 
- Physical Layer - bits/electrical signals
- Data Link Layer - frame (called datagram in TCP/IP model)
- Network Layer - packet
- Transport Layer - segment (TCP), datagram (UDP)
- Session Layer - message or data 
- Presentation Layer - data unit
- Application Layer - request/response or data

End to end communication/communication → Transport layer

---

# The OSI Model

<dl>
<dt>ISO - International Organization for Standardization </dt>
<dd>It is a multinational body dedicated to worldwide agreement on international standards</dd>
<dt>OSI - Open Systems Interconnect</dt>
<dd>Provides 7 layers</dd>
</dl>

The TCP/IP model came before the OSI model.

Q. Explain why OSI model didn't replace TCP/IP model?  
The OSI stack is a rather theoretical/abstract _model_ (and standard) for networking layers, but it has little practical relevance and mainly survives as a subject of CS classes.  
TCP/IP is a suite of concrete networking protocols that have seen overwhelming adoption on the internet. It roughly maps to the layers 3 and 4 in the OSI model.  

TCI/IP is not **conceptual** but it is a concrete implementation of the OSI.

![[TCP-IP as implementation of OSI.png]]

---







