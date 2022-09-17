# NAT - Network Address Translation

Resource: (Network Address Translation (NAT))[https://www.geeksforgeeks.org/network-address-translation-nat/]

### NAT - Network Address Translation 

- is a process in which one or more private IP address is translated into one or more public IP address and vice versa in order to provide Internet access to the private hosts.
- it also does translation of port numbers
- it makes a the corresponding entries of IP address and port number in the NAT table.
- it operates on a router or firewall

### Why mask port numbers ?   

NAT masks the source port number and makes an entry in the NAT table to avoid problems when packets arrive at the NAT from multiple sources sending to the same destination. As the NAT will mask the IP address then sends the packets, the destination will send replies of the public IP address to the router, it will be unclear to NAT as to which reply belongs because source port numbers from multiple sender will be the same. 
