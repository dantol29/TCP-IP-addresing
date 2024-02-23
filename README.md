# TCP/IP addresing

## 1. IP addresses

An IP address is a <b>32-bit number</b>. It identifies a host on a TCP/IP network.

IP addresses are normally expressed in dotted-decimal format, with four numbers separated by periods, such as _192.168.123.132_.

An IP address <b>has two parts</b>:

1. The first part is a _network adress_ (192.168.123.0)

2. The second part is a _host address_ (000.000.000.132)

To understand how subnet masks are used, examine an IP address in binary notation.
IP address 192.168.123.132 in binary notation is 11000000.10101000.01111011.10000100.

## 2. Subnet mask

The subnet mask is <b>used to divide IP address</b> into network and host portions. The network portion ensures that data packets reach the right network, while the host portion identifies a specific device on that network.

An example: _255.255.255.0_
