### Subnetting

Subnets, like IP Addresses, are just bytes (eight 1s and 0s, or bits).

Bits must be switched on in descending order (from 128 to 0). 

255.255.255.0 is very common, also known as /24

The number of bits "switched off" (0s) is related to the number of hosts available to us. The number of hosts available is 2^n, where n is the number of bits switched to 0.

Table:
Subnet mask groupings
| 1  | 2  | 3  | 4  | 5  | 6  | 7  | 8  |
| 9  | 10 | 11 | 12 | 13 | 14 | 15 | 16 |
| 17 | 18 | 19 | 20 | 21 | 22 | 23 | 24 |
| 25 | 26 | 27 | 28 | 29 | 30 | 31 | 32 |

Hosts
| 128 | 64 | 32 | 16 | 8 | 3 | 2 | 1 |

Subnet
| 128 | 192 | 224 | 240 | 248 | 252 | 254 | 255 |

Examples:
/24		255.255.255.0
/17		255.255.128.0
/6		252.0.0.0
/27		255.255.255.224


The number of hosts doubles for every bit turned off. /20 represents 12 bits at 0, or 2 to the 12. When calculating the number of hosts, we also always subtract 2 from the 2 to the n result.


The larger the company, the lower the /num.

So why?
	How many hosts can we fit, and what is the mask that's behind it?	
	EX: 192.168.1.0/24 tells us there could be up to 254 hosts on that network.
	
	When looking at the subnet mask, any place with a 255 is "locked in place". This means that that place in the IP address is also "locked in place", while anything that isn't a 255 is variable.
	
	
/24 is the most common. /16 is probably the next most common.

Network ID usually first address available to us.
Broadcast IP is usually the last address available to us.
EX:

| IP Address      | Subnet          | Hosts | Network         | Broadcast     |
|-----------------|-----------------|-------|-----------------|---------------|
| 192.168.1.0/24  | 255.255.255.0   | 254   | 192.168.1.0     | 192.168.1.255 |
| 192.168.1.0/28  | 255.255.255.240 | 14    | 192.168.1.0     | 192.168.1.15  |
| 192.168.1.16/28 | 255.255.255.240 | 14    | 192.168.1.16    | 192.168.1.31  |
| 192.168.0.0/23  | 255.255.254.0   | 510   | 192.168.0.0     | 192.168.1.255 |
|                 |                 |       |                 |               |
| 192.168.0.0/22  | 255.255.252.0   | 1022  | 192.168.0.0     | 192.168.3.255 |
| 192.168.1.0/26  | 255.255.255.192 | 62    | 192.168.1.0     | 192.168.1.63  |
| 192.168.1.0/27  | 255.255.255.224 | 30    | 192.168.1.0     | 192.168.1.31  |



It's possible to split a network into subgroups within a network. This is subnetting.
