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
(data travels though the transmission media/link as electrical signals which are then interpreted as bits and so on...)
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

Q. Explain why OSI model didn't replace TCP/IP model (aka internet model)?  
The OSI stack is a rather theoretical/abstract _model_ (and standard) for networking layers, but it has little practical relevance and mainly survives as a subject of CS classes.  
TCP/IP is a suite of concrete networking protocols that have seen overwhelming adoption on the internet. It roughly maps to the layers 3 and 4 in the OSI model.  

TCI/IP is not **conceptual** but it is a concrete implementation of the OSI.

![[TCP-IP as implementation of OSI.png]]

---

# Signals

data travels though the transmission media/link as electrical signals which are then interpreted as bits and so on...

## Types 
- Analog
- Digital

## Analog signals 

### Can take 2 forms
- Periodic
	- simple → a single sine wave
	- composite → composed of multiple sine waves
- Non-periodic (aperiodic)

![insert image....]
### Parameters of a simple periodic signal
- Peak amplitude - absolute value of highest intensity (measured in volts)
- Phase - (measured in radians degree)
- Period & Frequency
	- Period - (measured in s)
	- Frequency - (measured in $s^{-1}$)
- Wavelength → $\lambda = c/f = c \times T$

### Parameters of composite periodic signal
- Bandwidth → we measure bandwidth in composite signals
	- Bandwidth = difference b/w highest and lowest frequencies contained in that signal

## Digital Signals

A digital signal can have multiple levels.

number of bits transmitted per level = $\log_{2}L$

![](Pasted%20image%2020230912133626.png)

### Bit rate
- Number of bits transmitted per second

### Bit Length
- $= 1/bitrate$

>[!Problems]  
>Q1. Assume we need to download text documents at the rate of 100 pages per second. What is the required bit rate of the channel? A page is an average of 24 lines with 80 characters in each line. What is the bit rate and bit length?
>
>Ans: 
>
>Assuming each character in the page takes 8 bits.
>
>Bit rate = no. of pages x no. of lines x avg. no of characters x no. of bits per character  
>Bit rate = 100 x 24 x 80 x 8  
>Bit rate = 1536000 bits/s = 1.536Mbps
>
Bit length = 1/1536000 = 0.651 $\micro s$

---

