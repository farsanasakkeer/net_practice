# net_practice

The following special address-ranges are reserved for Private Networks:
10.0.0.0 – 10.255.255.255 172.16.0.0 – 172.31.255.255 192.168.0.0 – 192.168.255.255 

The following address-range is reserved for so called loopback addresses: 127.0.0.0 – 127.255.255.255

Switches
A switch will enable you to connect more than two devices to the same network.

Routers
As previously mentioned a router is an interface which enables communication between different networks.


Routing Table
The routing table is there to store all the different paths to all the networks, the device is part of.
In Net_Practice the routing table consists of two elements, the destination and the next hop
The destination consists of the network-address that you want to send a package to, combined with the CIDR of that network: 190.3.2.252/30. If you don't want to specify a destination, you can just set it to default or 0.0.0.0/0.
The next hop is the address of the next router that you need to send the packages to in order to reach the destination-network.

CIDR	Dot-decimal	Number of IP-addresses
per subnet	Usable IP-addresses
per subnet	Number of subnets
/32	255.255.255.255	1	0	256
/31	255.255.255.254	2	0	128
/30	255.255.255.252	4	2	64
/29	255.255.255.248	8	6	32
/28	255.255.255.240	16	14	16
/27	255.255.255.224	32	30	8
/26	255.255.255.192	64	62	4
/25	255.255.255.128	128	126	2
/24	255.255.255.0	256	254	1

first address is reserved as the network-address of the subnet and the last address is reserved as a broadcast-adress.
i.e. for mask 255.255.255.252:
network: 190.3.2.252
broadcast: 190.3.2.255
usable IP's: 190.3.2.253, 190.3.2.254

/30
Network Address:	42.42.42.40
Usable Host IP Range:	42.42.42.41 - 42.42.42.42
Broadcast Address:	42.42.42.43
