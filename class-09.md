# CIDR Block Notation

Resource: [CIDR Block Notation Explained in 2 Minutes](https://medium.com/@ethicalentrepreneur/cidr-block-notation-explained-in-2-minutes-1010ec0dbc15)


## CIDR notation is a way of representing a CIDR block, which is simply a range of IP addresses.
- An IPv4 (version 4 of IP) address is usually represented as four 8-bit decimal numbers or octets separated by dots.
- An 8-bit number when represented in the decimal system as opposed to binary has a range of 0–255.
- So all four octets together add up to 32 bits, for a range of 0.0.0.0–255.255.255.255.
- In CIDR notation, this full range would be represented as 0.0.0.0/0. The final digit after the “/” represents how many bits make up the mask.

---
---

# Network Segmentation

Resource: [What Is Network Segmentation and Why It Matters?](https://www.comptia.org/blog/security-awareness-training-network-segmentation)

## What Is Network Segmentation?
Network segmentation is when different parts of a computer network, or network zones, are separated by devices like bridges, switches and routers. 

## Why Is Network Segmentation Important?
Systems and services need to be isolated from one another to prevent a small breach from becoming a massive incident that leads to a data breach.

Whether you are running a virtual local area network (LAN) in the cloud or running an SDN-powered architecture, network segmentation will protect your assets.

## Types of Network Segmentation

- Users: Users are a network in and of themselves. Make sure you have correct access control on your users in your active directory. Privilege levels should be based on the user’s role in switching administration. Access control lists are typically already a part of your active directory server. 

- Screened Subnet: This includes the subnetworks that expose externally facing systems – where the handshakes take place on your network. You want to separate things that the public can access from your local area network (LAN) and internal data that needs to be protected.

- Guest Network: Guest Wi-Fi should be separate from the corporate Wi-Fi. This may seem like a no brainer, but I find a lot of smaller businesses never bother to set it up. Even residential routers include this feature – you can easily set up a guest Wi-Fi in your home!

- IT Workstations: This is the dev network zone for IT. It’s where IT staff does non-administrative work, and it should be segmented for testing. Giving IT a dedicated internet circuit for testing is a good idea.

- Servers by Department: Do department servers need to talk to one another? Create a public drive and a private drive, and then segment access on the private drives to those within each team or department. This can limit the crawl of malware.

- VoIP/Communications: Placing communications systems on their own network zone boosts performance and enhances quality. But in terms of network security, as communications move toward more APIs unique to your most used software as a service (SaaS) platforms, this network will become a more common attack surface.

- Traditional Physical Security: Cameras, ID card scanners, etc., should be in their own network zone. 

- Industrial Control Systems: HVAC, for example, like the non-segmented network compromised in the Target breach, should have two-factor authentication and be segmented.

- Customer Databases: Due to compliance requirements, customer databases need to be secured more intently than, for instance, print server. PCI-DSS, HIPAA, HiTRUST, FINRA, GDPR and other pieces of data legislation will determine the level of segmentation and cybersecurity that would be best practice in terms of implementation.

Configuring your intrusion detection and intrusion prevention system (IDS/IPS) tools to monitor your internal segmented network zones, just as you would set them to monitor your public-facing networks. Make sure to review your logs or work with an IT partner that will double your vigilance and act as an extra set of eyes.

## Who Needs Network Segmentation?

Each will require a different level of segmentation.

Everyone running internal systems, whether physical or virtualized. The more complicated the architecture, the more important the need for segmentation. 

The only users who won’t need network segmentation are businesses that rely 100% on software as a service (SaaS) solutions or alternatively a business that operates offline/without IT services.

A flat network is an ideal target for a threat actor. 

There is no substitute for network segmentation. Micro-segmentation requires some time to initially set up, but the benefits highly outweigh the upfront time cost.

## Benefits of Network Segmentation

- Damage control and limitation in case of an incident via the smaller attack surface
- Improved access control for external and internal network security
- Reducing the attack plane and scope of compliance requirements related auditing
- Improved performance with less congestion on network traffic
- Better analytics around network monitoring, network access and network devices
- Endpoint device protection, especially important as IoT devices become more commons

