# NMAP

Resource: [What is a Port Scanner and How Does it Work?](https://www.varonis.com/blog/port-scanning-techniques)

## NMAP (Network Mapping) 
is one of the most popular free and open source utility for network discovery and security auditing. Administrators may also find it useful for tasks such as network inventory, managing and monitoring hosts uptime.

What is a port scanner? 
- it's a computer program that checks network ports for open, closed or filtered status.
- it is a valuable tools in diagnosing network and connectivity issues, however could also be a possible access points for infiltration and to identify the devices running on the network. 

Port scanner operates by sending a request to connect to a TCP or UDP port on a computer and records one of the three responses: open = accepted, closed = port is in use, and blocked = silence or no response.

Port Scanning Technique
- Ping Scan = a ping is an ICMP (Internet Control Message Protocol) echo request to different targets to see who responds
- TCP Half Open = the scanner sends an SYN message and just notes SYN-ACK responses, it does not complete the 3-way handshake and leaves the target as an open port, waiting for the final ACK.
- TCP Connect = has an advantage of completing the 3-way handshake connection with just a lower privilege to run the scan. 
- UDP = slower scan than TCP 