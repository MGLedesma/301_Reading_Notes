# Port Mirroring - SPAN vs TAP

Resource: [How to capture network traffic ? SPAN vs TAP](https://accedian.com/blog/capture-network-traffic-span-vs-tap/)

## How to Capture Network Traffic?

Port Mirroring aka SPAN, is a method of monitoring network traffic which forwards a copy of each incoming and/or outgoing packet from one/several port/vlan of a switch to another port where the device is connected. 
    - the administrator selects a source port (packets will be copied) and destination port (copies of packets will be sent) and can include all packets or only the transmitted/received parts. 
    - it is most commonly used because its inexpensive, flexible in terms of how much traffic to capture, and can be manage remotely or locally
    - it is the only way to capture intra-switch traffic


Network TAP (Terminal Access Point) is a hardware device which can passively capture traffic on a network commonly used to monitor the traffic between two points in the network. 
    - has at least 3 ports: an A port, a B port, and a monitor port. A TAP is place between port A and B, as all traffic between two network passes the TAP, it copies the traffic to its monitor port to listen for analysis.