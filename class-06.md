# Wireshark and Layers 2 and 3 of OSI Model

Resources:

- [What Is Wireshark and How Is It Used?](https://www.comptia.org/content/articles/what-is-wireshark-and-how-to-use-it)
- [Understanding Network Data Delivery: Layers 2 and 3 of the OSI Model](https://www.comptia.org/blog/layers-2-and-3-osi-model)

## Wireshark

- Wireshark is a network protocol analyzer, or an application that captures discrete unit of data from a network connection.
- Does three things: Packet capture, Filtering, and Visualization
- Uses: troubleshoot networks, trace connections, view contents of suspect transactions and identify burst of network traffic.
- When to use: can be used as a learning tools, and  understand network traffic analysis
- Limitation: can only grab traffic on modern networks that use switches, can only sniff traffic between local computer and the remote system it is talking to, can show malformed packets, can't help with decryption, and wireshark can't tell if IP address it finds is real or not.
- Colors: 
    - Black - packets with error
    - Light Purple - TCP
    - Light Blue - UDP
    - Light Green - HTTP traffic
    - Light Yellow - Windows-specific traffic, SMB and NetBIOS
    - Dark Yellow - Routing
    - Dark Gray - TCP, SYN, FIN and ACK traffic
