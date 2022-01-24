# IPv4 Subnetting Basics

A quick rundown of IP addressesing and how this ties into binary at it's core. 

To understand subnetting, you should first understand the decimal and binary structure of an IP address.

Let's start with the basics. Here's what an IP address looks like: **192.168.1.20**

An IPv4 address is a 32-bit number. To make addresses more straightforward, they are divided into four 8-bit numbers — or octets — separated by a decimal point. **These octets range in number from 0 to 255.**

Why do octets only go up to 255? Because they're binary.

The biggest IP address possible is **255.255.255.255**

In binary, this IP address looks like this: **11111111.11111111.11111111.11111111**

Note that there are eight numbers between the decimal points. Each number represents a bit. Hence the term octet or the 8-bit number grouping.

Binary corresponds to the following table of numbers:
```
128	64	32	16	8	4	2	1
```

Every 1 in a binary number "turns on" the number in its position. So, 1 in the first and last positions "turn on" 128 and 1.

## How to define the network portion of a subnet IP address

There are two parts to an IP address: The network portion and the host portion.
It's like the address for a house. The network portion is like the city, state, and zip code. The host portion is like the house and street number.

A subnet defines the number of bits, out of 32, used for the "network portion" of the address. Subnet masks can also be defined in a more common 'slash' representation, known as CIDR notation. In the following table, the red digits represent the bits used for the network. The black digits will be used for device IP addresses. Note that the 255.0.0.0 mask can also be represented as a '/8' because it reserves 8 bits of the overall 32 bits used to describe an IPv4 address as the network portion.

The first 3 octets of an IP address is considered the **network portion**. The last octet will be the **host portion**.

## What are IP address classes?

To complicate things further, IP addresses have five classes, but only three are applicable to subnetting — A, B, C.

Here are the IP address ranges by class:

Class A = 1.0.0.0 to 127.0.0.0

Class B = 128.0.0.0 to 191.255.0.0

Class C = 192.0.0.0 to 223.255.255.0
