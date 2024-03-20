# TCP/IP addresing

## 1. Network

How do I know if two devices are part of the same network?

For this you need to combine the IP-address and the mask of the devices in order to get the network-adress, that device is part of.

Combine means bit-by-bit-AND-opperation.

Here are the steps:
1. translate the IP and the mask to binary

IP: `192.168.100.1` in binary: `11000000.10101000.1100100.00000001`

MASK: `255.255.255.0` in binary: `11111111.11111111.11111111.00000000`

2. Combine the two bit by bit


`11000000.10101000.1100100.00000000` in binary or `192.168.100.0` in dot-decimal.

## 1. Special IP-ranges
The following special address-ranges are reserved for Private Networks:

10.0.0.0 – 10.255.255.255

172.16.0.0 – 172.31.255.255

192.168.0.0 – 192.168.255.255


The following address-range is reserved for so called loopback addresses:

127.0.0.0 – 127.255.255.255

## 2. IP addresses

An IP address is a <b>32-bit number</b>. It identifies a host on a TCP/IP network.

IP addresses are normally expressed in dotted-decimal format, with four numbers separated by periods, such as _192.168.123.132_.

An IP address <b>has two parts</b>:

1. The first part is a _network adress_ (192.168.123.0)

2. The second part is a _host address_ (000.000.000.132)

To understand how subnet masks are used, examine an IP address in binary notation.
IP address 192.168.123.132 in binary notation is 11000000.10101000.01111011.10000100.

## 3. Subnet mask

The subnet mask is <b>used to divide IP address</b> into network and host portions. The network portion ensures that data packets reach the right network, while the host portion identifies a specific device on that network.

An example: _255.255.255.0_
