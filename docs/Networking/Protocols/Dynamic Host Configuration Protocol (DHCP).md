# Dynamic Host Configuration Protocol 

## Description

Dynamic Host Configuration Protocol (DHCP) is a service that runs on a server to assign hosts an IP address based on centralized settings. It makes running a TCP/IP environment a breeze.

## Ports/Protocols

DHCP runs on TCP/UDP Port 67.

## Different Types

DHCP can be run as DHCPv4 for IPv4 as well as DHCPv6 for IPv6

## Behavior

A DHCP request begins with a machine **broadcasting** it's request to every other machine in the same broadcast domain. Every DHCP server on the network will respond to the request and the first DHCP offer to reach the client is accepted. 

It is recommended that you only run **one** DHCP server in a given broadcast domain. Multiple DHCP servers can obviously wreak havoc on your network.

DHCP is normally ran on either the router in a home networking environment or on a server/layer 3 switch in an enterprise environment. It is important to understand and plan your network capacity and DHCP uses when setting up/engineering a network. 

