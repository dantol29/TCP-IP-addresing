# TCP/IP addresing

## Network

<b>How to determine the range of usable IP addresses?</b>

1. Identify the Subnet Mask.
2. Identify the Network Address
3. Identify the Broadcast Address
4. Determine the Range of Usable IP Addresses
5. Identify Special Addresses

## 1. Identify the Subnet Mask
The subnet mask is <b>used to divide IP address</b> into network and host portions. The network portion ensures that data packets reach the right network, while the host portion identifies a specific device on that network.

An example: `255.255.255.0`

## 2. Identify the Network Address
The network address is obtained by performing a <b>bitwise AND operation</b> between the IP address and the subnet mask.

For example, if the IP address is `192.168.1.100` and the subnet mask is `255.255.255.0`, the network address would be `192.168.1.0`.

## 3. Identify the Broadcast Address
The broadcast address is the highest address in the subnet. It's obtained by <b>setting all host bits to 1</b> within the network portion of the IP address. 

For example, if the subnet mask is `255.255.255.0`, the broadcast address for the network `192.168.1.0` would be `192.168.1.255`.

## 4. Determine the Range of Usable IP Addresses

These are the addresses between the network and broadcast addresses, excluding those addresses. 

For example, if the network address is `192.168.1.0` and the broadcast address is `192.168.1.255`, the usable IP addresses in this subnet would be from `192.168.1.1` to `192.168.1.254`.

## 5. Identify Special Addresses
Some special addresses are reserved within each subnet. These include the <b>network address</b> (the first address in the subnet) and the <b>broadcast address</b> (the last address in the subnet). 

Additionally, there might be other addresses reserved for specific purposes, such as the default gateway and DNS servers.


## 6. Special IP-ranges
The following special address-ranges are reserved for Private Networks:

`10.0.0.0` – `10.255.255.255`

`172.16.0.0` – `172.31.255.255`

`192.168.0.0` – `192.168.255.255`


The following address-range is reserved for so called loopback addresses:

`127.0.0.0 – 127.255.255.255`

## IP addresses

An IP address is a <b>32-bit number</b>. It identifies a host on a TCP/IP network.

IP addresses are normally expressed in dotted-decimal format, with four numbers separated by periods, such as _192.168.123.132_.

An IP address <b>has two parts</b>:

1. The first part is a _network adress_ (`192.168.123.0`)

2. The second part is a _host address_ (`000.000.000.132`)

To understand how subnet masks are used, examine an IP address in binary notation.

IP address `192.168.123.132` in binary notation is `11000000.10101000.01111011.10000100`.

