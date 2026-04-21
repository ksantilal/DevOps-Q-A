Networking
========================================
* Networking is a critical aspect of DevOps, as it enables communication between different components of a system. In this section, we will cover the basics of networking in the context of DevOps.

* Networking Basics
----------------------
* IP Addressing: An IP address is a unique identifier assigned to each device on a network. It allows devices to communicate with each other by providing a way to identify and locate them.

* Subnetting: Subnetting is the process of dividing a larger network into smaller subnetworks. This allows for better organization and management of the network.

* DNS: The Domain Name System (DNS) is a hierarchical system that translates domain names into IP addresses. It allows users to access websites and other resources using easy-to-remember domain names instead of IP addresses.

* Networking in DevOps
----------------------
* Container Networking: In a DevOps environment, containers are often used to deploy applications. Container networking allows containers to communicate with each other and with the outside world.

* Service Discovery: Service discovery is the process of automatically detecting and connecting to services in a network. This is important in a DevOps environment where services may be dynamically created and destroyed.

* Load Balancing: Load balancing is the process of distributing network traffic across multiple servers to ensure that no single server is overwhelmed. This is important in a DevOps environment where applications may experience high traffic.

* Security: Networking security is crucial in a DevOps environment to protect against unauthorized access and data breaches. This includes implementing firewalls, encryption, and other security measures.

### OSI Models
* The OSI (Open Systems Interconnection)
- Application (HTTP,HTTPS)
    - HTTP - Hypertext Transfer Protocol.
    - HTTPS - Hypertext Transfer Protocol Secure.
- Presentation (SSL, TLS)
    - SSL - Secure Sockets Layer  
    - TLS - Transport Layer Security.
- Session (TCP, UDP)
    - TCP - Transmission Control Protocol 
    - UDP - User Datagram Protocol 
- Transport (IP)
- Network (Ethernet)
- Data Link
- Physical

### Usefull Commands:
--------------------------------
* `ip addr` - Display IP addresses and network interfaces.
* `ping <hostname/IP>` - Test connectivity to a host.
* `traceroute <hostname/IP>` - Trace the route packets take to a host.
* `netstat -tuln` - Display active network connections and listening ports.
* `nslookup <hostname>` - Query DNS for the IP address of a hostname.
* `dig <hostname>` - Another tool for querying DNS information.
* `tcpdump` - Capture and analyze network traffic.
* `nmap <hostname/IP>` - Scan for open ports and services on a host.
* `ifconfig` - Display or configure network interfaces (deprecated in favor of `ip addr`).
* `route` - Display or modify the IP routing table.
* `iptables` - Configure firewall rules for network traffic.
* `curl <URL>` - Transfer data from or to a server using various protocols (HTTP, HTTPS, etc.).
* `wget <URL>` - Download files from the web.
* `netcat` - A versatile networking utility for reading from and writing to network connections.
* `ss` - Display socket statistics and information about network connections.
* `ethtool <interface>` - Display or change Ethernet device settings.
* `ip route` - Display or manipulate the IP routing table.
* `ip link` - Display or manage network interfaces.
* `ip neigh` - Display or manipulate the ARP table.
* `iptables -L` - List current firewall rules.
* `iptables -A` - Append a new rule to the firewall.
* `iptables -D` - Delete a rule from the firewall.
* `iptables -F` - Flush all firewall rules.
* `iptables -P` - Set default policy for a chain.
* `tcpdump -i <interface>` - Capture packets on a specific network interface.
* `tcpdump -w <file>` - Write captured packets to a file for later analysis.

----------------------------------------------------------------

* Server
- A server is a computer or system that provides resources, data, services, or programs to other computers, known as clients, over a network. Servers can be physical machines or virtual instances running on cloud platforms.

* Deployment Servers Type
    1. Physical Server
    2. Virtual Server
    3. Cloud Server

* There are eight types of server
    1. Web Server
        - Nginx
        - Apache
    2. Application Server
       - Tomcat
       - Apache
    3. Database Server
         - MySQL
         - PostgreSQL
         - MongoDB
    4. File Server
        - Samba
        - NFS
    5. Mail Server
        - Postfix
        - Exim
    6. DNS Server
        - BIND
        - PowerDNS
    7. Proxy Server
        - Squid
        - HAProxy
    8. Monitoring Server
        - Prometheus
        - Grafana
    
* VPC 
- A Virtual Private Cloud (VPC) is a virtual network dedicated to your AWS account. It enables you to launch AWS resources into a virtual network that you've defined. A VPC is logically isolated from other virtual networks in the AWS Cloud.

* Subnet
- A subnet is a range of IP addresses in your VPC. You can launch AWS resources into a specified subnet. Use subnets to group instances based on security and operational needs.

* Internet Gateway
- An Internet Gateway is a horizontally scaled, redundant, and highly available VPC component that allows communication between instances in your VPC and the internet.

* NAT Gateway
- A NAT Gateway enables instances in a private subnet to connect to the internet or other AWS services, but prevents the internet from initiating a connection with those instances.

* Route Table
- A route table contains a set of rules, called routes, that are used to determine where network traffic is directed. Each subnet in your VPC must be associated with a route table.

* Security Group
- A security group acts as a virtual firewall for your instance to control inbound and outbound traffic. You can specify rules that allow or deny traffic to and from your instances.

* Network ACL
- A Network Access Control List (ACL) is an optional layer of security for your VPC that acts as a firewall for controlling traffic in and out of one or more subnets. You can set up network ACLs with rules similar to your security groups to add an additional layer of defense to your VPC.

* Nat Gatway
- A NAT Gateway enables instances in a private subnet to connect to the internet or other AWS services, but prevents the internet from initiating a connection with those instances. It is a managed service that provides better availability and bandwidth compared to a NAT instance.

* LAN
- A Local Area Network (LAN) is a network that connects devices within a limited geographical area, such as a home, office, or campus. LANs are typically used for sharing resources and data among devices in close proximity.

* WAN
- A Wide Area Network (WAN) is a telecommunications network that extends over a large geographical area for the primary purpose of computer networking. WANs are often used to connect multiple smaller networks, such as LANs, together.

* VPN
- A Virtual Private Network (VPN) is a secure connection between two or more devices over the internet. It allows users to send and receive data as if their devices were directly connected to a private network, providing privacy and security.

* DNS
- The Domain Name System (DNS) is a hierarchical system that translates human-readable domain names (like www.example.com) into IP addresses.

* Load Balancing
- Load balancing is the process of distributing network traffic across multiple servers to ensure that no single server becomes overwhelmed. This helps improve the performance and availability of applications.

* Firewall
- A firewall is a network security device that monitors and controls incoming and outgoing network traffic based on predetermined security rules. It acts as a barrier between a trusted internal network and untrusted external networks, such as the internet.
* Firewalls
    - FortyGate
    - Palo Alto
    - CheckPoint
    - Fortinet
    - NextGen Firewall

* Proxy
- A proxy server is an intermediary server that separates end users from the websites they browse. Proxy servers provide varying levels of functionality, security, and privacy depending on your needs, company policies, or privacy concerns.

* Protocol
- A protocol is a set of rules that govern how data is transmitted and received over a network. Common protocols include HTTP, HTTPS, FTP, TCP, and UDP.
* Ports
- A port is a communication endpoint in a network. It is used to identify specific processes or services running on a device. Common ports include 80 for HTTP, 443 for HTTPS, and 22 for SSH.
* VLAN
- A Virtual Local Area Network (VLAN) is a logical partition of a physical network. It allows you to create separate networks within a single physical network, improving security and reducing congestion.
- Default Port No
    - 80 - HTTP
    - 443 - HTTPS
    - 22 - SSH
    - 25 - SMTP
    - 110 - POP3
    - 143 - IMAP
    - 3306 - MySQL
    - 5432 - PostgreSQL
