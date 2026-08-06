# Computer Networks Interview Questions & Answers — Complete Revision Guide

A complete, structured collection of Computer Networks interview questions — from core networking fundamentals and the OSI/TCP-IP models to routing, the transport and application layers, DNS, security, and troubleshooting — with clear, exam- and interview-ready answers. Built to be your one-stop revision resource for CS fundamentals interviews or exams.

## 📚 Table of Contents

- [🔥 Most Asked / Tricky Questions](#-most-asked--tricky-questions)
  - [What is the difference between TCP and UDP?](#what-is-the-difference-between-tcp-and-udp)
  - [What happens when you type a URL into a browser and press Enter?](#what-happens-when-you-type-a-url-into-a-browser-and-press-enter)
  - [What is the difference between the OSI model and the TCP/IP model?](#what-is-the-difference-between-the-osi-model-and-the-tcpip-model)
  - [What is the three-way handshake in TCP, and why is it needed?](#what-is-the-three-way-handshake-in-tcp-and-why-is-it-needed)
  - [What is the difference between a router and a switch?](#what-is-the-difference-between-a-router-and-a-switch)
  - [What is NAT (Network Address Translation), and why is it used?](#what-is-nat-network-address-translation-and-why-is-it-used)
  - [What is the difference between a public IP and a private IP address?](#what-is-the-difference-between-a-public-ip-and-a-private-ip-address)
  - [What is the difference between HTTP and HTTPS?](#what-is-the-difference-between-http-and-https)
  - [What is DNS, and why is it needed?](#what-is-dns-and-why-is-it-needed)
  - [What is the difference between a MAC address and an IP address?](#what-is-the-difference-between-a-mac-address-and-an-ip-address)
  - [What is a subnet mask, and what is it used for?](#what-is-a-subnet-mask-and-what-is-it-used-for)
  - [What is the difference between symmetric and asymmetric encryption, and how are both typically used together in TLS?](#what-is-the-difference-between-symmetric-and-asymmetric-encryption-and-how-are-both-typically-used-together-in-tls)
  - [What is the difference between a firewall and a proxy server?](#what-is-the-difference-between-a-firewall-and-a-proxy-server)
  - [What is a socket, and what identifies one uniquely?](#what-is-a-socket-and-what-identifies-one-uniquely)
  - [What is the difference between congestion control and flow control in TCP?](#what-is-the-difference-between-congestion-control-and-flow-control-in-tcp)
- [Networking Basics & Fundamentals](#networking-basics--fundamentals)
  - [What is a computer network, and what are its main goals?](#what-is-a-computer-network-and-what-are-its-main-goals)
  - [What is the difference between LAN, MAN, and WAN?](#what-is-the-difference-between-lan-man-and-wan)
  - [What is the difference between a client-server architecture and a peer-to-peer (P2P) architecture?](#what-is-the-difference-between-a-client-server-architecture-and-a-peer-to-peer-p2p-architecture)
  - [What is bandwidth, and how does it differ from latency?](#what-is-bandwidth-and-how-does-it-differ-from-latency)
  - [What is the difference between unicast, broadcast, and multicast communication?](#what-is-the-difference-between-unicast-broadcast-and-multicast-communication)
  - [What is a protocol, in networking terms?](#what-is-a-protocol-in-networking-terms)
  - [What is encapsulation in the context of networking, and how does it relate to the layered network models?](#what-is-encapsulation-in-the-context-of-networking-and-how-does-it-relate-to-the-layered-network-models)
  - [What is the difference between circuit switching and packet switching?](#what-is-the-difference-between-circuit-switching-and-packet-switching)
  - [What is the difference between half-duplex and full-duplex communication?](#what-is-the-difference-between-half-duplex-and-full-duplex-communication)
  - [What is a MAC address, and what is its typical structure?](#what-is-a-mac-address-and-what-is-its-typical-structure)
- [OSI Model & TCP/IP Model](#osi-model--tcpip-model)
  - [What are the seven layers of the OSI model, from bottom to top?](#what-are-the-seven-layers-of-the-osi-model-from-bottom-to-top)
  - [What is the role of the Physical layer?](#what-is-the-role-of-the-physical-layer)
  - [What is the role of the Data Link layer, and what are its two sublayers?](#what-is-the-role-of-the-data-link-layer-and-what-are-its-two-sublayers)
  - [What is the role of the Network layer, and what is its primary addressing scheme?](#what-is-the-role-of-the-network-layer-and-what-is-its-primary-addressing-scheme)
  - [What is the role of the Transport layer?](#what-is-the-role-of-the-transport-layer)
  - [What is the role of the Session, Presentation, and Application layers, and why are they often merged into a single "Application layer" in the TCP/IP model?](#what-is-the-role-of-the-session-presentation-and-application-layers-and-why-are-they-often-merged-into-a-single-application-layer-in-the-tcpip-model)
  - [What are the four layers of the TCP/IP model, and how do they map roughly to the OSI model?](#what-are-the-four-layers-of-the-tcpip-model-and-how-do-they-map-roughly-to-the-osi-model)
  - [At which OSI layer does a switch typically operate, and at which layer does a router operate?](#at-which-osi-layer-does-a-switch-typically-operate-and-at-which-layer-does-a-router-operate)
- [Physical & Data Link Layer](#physical--data-link-layer)
  - [What is the difference between a hub, a switch, and a bridge?](#what-is-the-difference-between-a-hub-a-switch-and-a-bridge)
  - [What is CSMA/CD, and where was it historically used?](#what-is-csmacd-and-where-was-it-historically-used)
  - [What is CSMA/CA, and how does it differ from CSMA/CD?](#what-is-csmaca-and-how-does-it-differ-from-csmacd)
  - [What is a VLAN (Virtual LAN), and why is it used?](#what-is-a-vlan-virtual-lan-and-why-is-it-used)
  - [What is the difference between error detection and error correction at the Data Link layer?](#what-is-the-difference-between-error-detection-and-error-correction-at-the-data-link-layer)
  - [What is a CRC (Cyclic Redundancy Check), and what is it used for?](#what-is-a-crc-cyclic-redundancy-check-and-what-is-it-used-for)
  - [What is the difference between a MAC address and a port number in terms of what they identify?](#what-is-the-difference-between-a-mac-address-and-a-port-number-in-terms-of-what-they-identify)
  - [What is ARP (Address Resolution Protocol), and what problem does it solve?](#what-is-arp-address-resolution-protocol-and-what-problem-does-it-solve)
  - [What is Ethernet, and what is a typical Ethernet frame's structure at a high level?](#what-is-ethernet-and-what-is-a-typical-ethernet-frames-structure-at-a-high-level)
  - [What is the difference between store-and-forward switching and cut-through switching?](#what-is-the-difference-between-store-and-forward-switching-and-cut-through-switching)
- [Network Layer & IP Addressing](#network-layer--ip-addressing)
  - [What is an IP address, and what is the difference between IPv4 and IPv6?](#what-is-an-ip-address-and-what-is-the-difference-between-ipv4-and-ipv6)
  - [What is CIDR (Classless Inter-Domain Routing) notation, and what does the number after the slash mean?](#what-is-cidr-classless-inter-domain-routing-notation-and-what-does-the-number-after-the-slash-mean)
  - [What is subnetting, and why is it used?](#what-is-subnetting-and-why-is-it-used)
  - [What is the difference between a network address, a broadcast address, and a host address within a subnet?](#what-is-the-difference-between-a-network-address-a-broadcast-address-and-a-host-address-within-a-subnet)
  - [What are the private IP address ranges defined by RFC 1918?](#what-are-the-private-ip-address-ranges-defined-by-rfc-1918)
  - [What is the difference between a static IP address and a dynamic IP address, and what protocol typically assigns dynamic addresses?](#what-is-the-difference-between-a-static-ip-address-and-a-dynamic-ip-address-and-what-protocol-typically-assigns-dynamic-addresses)
  - [What is DHCP, and what is the typical DORA process it uses to assign an address?](#what-is-dhcp-and-what-is-the-typical-dora-process-it-uses-to-assign-an-address)
  - [What is the default gateway, and what role does it play?](#what-is-the-default-gateway-and-what-role-does-it-play)
  - [What is IP fragmentation, and why does it happen?](#what-is-ip-fragmentation-and-why-does-it-happen)
  - [What is the difference between IPv4's use of ARP and IPv6's use of NDP (Neighbor Discovery Protocol)?](#what-is-the-difference-between-ipv4s-use-of-arp-and-ipv6s-use-of-ndp-neighbor-discovery-protocol)
  - [What is TTL (Time To Live) in an IP packet, and what is it used for?](#what-is-ttl-time-to-live-in-an-ip-packet-and-what-is-it-used-for)
  - [What is anycast addressing, and where is it commonly used?](#what-is-anycast-addressing-and-where-is-it-commonly-used)
- [Routing](#routing)
  - [What is routing, and what is a routing table?](#what-is-routing-and-what-is-a-routing-table)
  - [What is the difference between static routing and dynamic routing?](#what-is-the-difference-between-static-routing-and-dynamic-routing)
  - [What is the difference between distance-vector and link-state routing protocols?](#what-is-the-difference-between-distance-vector-and-link-state-routing-protocols)
  - [What is the difference between an interior gateway protocol (IGP) and an exterior gateway protocol (EGP)?](#what-is-the-difference-between-an-interior-gateway-protocol-igp-and-an-exterior-gateway-protocol-egp)
  - [What is BGP (Border Gateway Protocol), and why is it described as the routing protocol of the internet?](#what-is-bgp-border-gateway-protocol-and-why-is-it-described-as-the-routing-protocol-of-the-internet)
  - [What is the difference between a routing loop and how protocols like RIP try to prevent one?](#what-is-the-difference-between-a-routing-loop-and-how-protocols-like-rip-try-to-prevent-one)
  - [What is the difference between routing and forwarding?](#what-is-the-difference-between-routing-and-forwarding)
  - [What is administrative distance, and why does it matter when a router learns the same destination from multiple sources?](#what-is-administrative-distance-and-why-does-it-matter-when-a-router-learns-the-same-destination-from-multiple-sources)
- [Transport Layer (TCP & UDP)](#transport-layer-tcp--udp)
  - [What is a port number, and what is the difference between well-known, registered, and dynamic/private ports?](#what-is-a-port-number-and-what-is-the-difference-between-well-known-registered-and-dynamicprivate-ports)
  - [How does TCP achieve reliable delivery?](#how-does-tcp-achieve-reliable-delivery)
  - [What is the TCP sliding window, and what is it used for?](#what-is-the-tcp-sliding-window-and-what-is-it-used-for)
  - [What is the difference between TCP's flow control and congestion control mechanisms?](#what-is-the-difference-between-tcps-flow-control-and-congestion-control-mechanisms)
  - [What is TCP's "slow start" mechanism?](#what-is-tcps-slow-start-mechanism)
  - [What is the four-way (or sometimes described as three-way) handshake used to close a TCP connection?](#what-is-the-four-way-or-sometimes-described-as-three-way-handshake-used-to-close-a-tcp-connection)
  - [What is the TIME_WAIT state in TCP, and why does it exist?](#what-is-the-time_wait-state-in-tcp-and-why-does-it-exist)
  - [What are the main differences in the UDP header compared to the TCP header?](#what-are-the-main-differences-in-the-udp-header-compared-to-the-tcp-header)
  - [What is head-of-line blocking, and how does it relate to TCP?](#what-is-head-of-line-blocking-and-how-does-it-relate-to-tcp)
  - [What is Nagle's algorithm, and what problem does it address?](#what-is-nagles-algorithm-and-what-problem-does-it-address)
  - [What is the difference between a TCP segment, an IP packet, and an Ethernet frame?](#what-is-the-difference-between-a-tcp-segment-an-ip-packet-and-an-ethernet-frame)
  - [Why might an application choose UDP over TCP despite UDP's lack of reliability?](#why-might-an-application-choose-udp-over-tcp-despite-udps-lack-of-reliability)
- [Application Layer & Protocols](#application-layer--protocols)
  - [What is the difference between HTTP/1.1, HTTP/2, and HTTP/3?](#what-is-the-difference-between-http11-http2-and-http3)
  - [What is the difference between an HTTP GET request and a POST request?](#what-is-the-difference-between-an-http-get-request-and-a-post-request)
  - [What is the difference between HTTP status code categories (1xx, 2xx, 3xx, 4xx, 5xx)?](#what-is-the-difference-between-http-status-code-categories-1xx-2xx-3xx-4xx-5xx)
  - [What is the difference between FTP and SFTP?](#what-is-the-difference-between-ftp-and-sftp)
  - [What is SMTP, and what role does it play in sending email?](#what-is-smtp-and-what-role-does-it-play-in-sending-email)
  - [What is the difference between IMAP and POP3 for retrieving email?](#what-is-the-difference-between-imap-and-pop3-for-retrieving-email)
  - [What is a cookie, and what is it typically used for in HTTP?](#what-is-a-cookie-and-what-is-it-typically-used-for-in-http)
  - [What is the difference between HTTP being "stateless" and how web applications maintain sessions across multiple requests?](#what-is-the-difference-between-http-being-stateless-and-how-web-applications-maintain-sessions-across-multiple-requests)
  - [What is WebSocket, and how does it differ from traditional HTTP request/response communication?](#what-is-websocket-and-how-does-it-differ-from-traditional-http-requestresponse-communication)
  - [What is a REST API, and what are some key architectural principles it follows?](#what-is-a-rest-api-and-what-are-some-key-architectural-principles-it-follows)
- [DNS](#dns)
  - [What is the hierarchical structure of the DNS system, from top to bottom?](#what-is-the-hierarchical-structure-of-the-dns-system-from-top-to-bottom)
  - [What is the difference between a recursive DNS resolver and an authoritative DNS server?](#what-is-the-difference-between-a-recursive-dns-resolver-and-an-authoritative-dns-server)
  - [What is the difference between an A record, an AAAA record, a CNAME record, and an MX record?](#what-is-the-difference-between-an-a-record-an-aaaa-record-a-cname-record-and-an-mx-record)
  - [What is DNS caching, and why does TTL matter for it?](#what-is-dns-caching-and-why-does-ttl-matter-for-it)
  - [What is a DNS zone, and what is zone transfer?](#what-is-a-dns-zone-and-what-is-zone-transfer)
  - [What is DNS spoofing/cache poisoning, and what does it exploit?](#what-is-dns-spoofingcache-poisoning-and-what-does-it-exploit)
- [Network Security](#network-security)
  - [What is a firewall, and what is the difference between a stateless and a stateful firewall?](#what-is-a-firewall-and-what-is-the-difference-between-a-stateless-and-a-stateful-firewall)
  - [What is the difference between a VPN and a proxy, from a security perspective?](#what-is-the-difference-between-a-vpn-and-a-proxy-from-a-security-perspective)
  - [What is a man-in-the-middle (MITM) attack, and how does HTTPS/TLS help prevent one?](#what-is-a-man-in-the-middle-mitm-attack-and-how-does-httpstls-help-prevent-one)
  - [What is a DDoS attack, and what is the difference between it and a regular DoS attack?](#what-is-a-ddos-attack-and-what-is-the-difference-between-it-and-a-regular-dos-attack)
  - [What is port scanning, and why is it relevant to network security?](#what-is-port-scanning-and-why-is-it-relevant-to-network-security)
  - [What is the purpose of a Certificate Authority (CA) in the context of TLS/SSL certificates?](#what-is-the-purpose-of-a-certificate-authority-ca-in-the-context-of-tlsssl-certificates)
  - [What is the difference between IDS and IPS?](#what-is-the-difference-between-ids-and-ips)
  - [What is ARP spoofing, and what can an attacker achieve with it?](#what-is-arp-spoofing-and-what-can-an-attacker-achieve-with-it)
  - [What is the principle of "defense in depth" in network security?](#what-is-the-principle-of-defense-in-depth-in-network-security)
  - [What is a VPN tunnel, and what does "tunneling" mean in this context?](#what-is-a-vpn-tunnel-and-what-does-tunneling-mean-in-this-context)
- [Wireless & Modern Networking](#wireless--modern-networking)
  - [What is the difference between 802.11 Wi-Fi standards (like 802.11n, ac, ax)?](#what-is-the-difference-between-80211-wi-fi-standards-like-80211n-ac-ax)
  - [What is the difference between the 2.4GHz and 5GHz Wi-Fi bands?](#what-is-the-difference-between-the-24ghz-and-5ghz-wi-fi-bands)
  - [What is a Content Delivery Network (CDN), and what problem does it solve?](#what-is-a-content-delivery-network-cdn-and-what-problem-does-it-solve)
  - [What is a load balancer, and what is the difference between Layer 4 and Layer 7 load balancing?](#what-is-a-load-balancer-and-what-is-the-difference-between-layer-4-and-layer-7-load-balancing)
  - [What is QUIC, and what advantage does it offer over traditional TCP for web traffic?](#what-is-quic-and-what-advantage-does-it-offer-over-traditional-tcp-for-web-traffic)
  - [What is the basic idea behind Software-Defined Networking (SDN)?](#what-is-the-basic-idea-behind-software-defined-networking-sdn)
- [Network Performance & Troubleshooting](#network-performance--troubleshooting)
  - [What is the `ping` command used for, and what does it actually measure?](#what-is-the-ping-command-used-for-and-what-does-it-actually-measure)
  - [What is the `traceroute` (or `tracert`) command used for, and how does it work?](#what-is-the-traceroute-or-tracert-command-used-for-and-how-does-it-work)
  - [What is jitter, in the context of network performance, and why does it matter for real-time applications?](#what-is-jitter-in-the-context-of-network-performance-and-why-does-it-matter-for-real-time-applications)
  - [What is packet loss, and what are some common causes?](#what-is-packet-loss-and-what-are-some-common-causes)
  - [What is the difference between throughput and goodput?](#what-is-the-difference-between-throughput-and-goodput)
  - [What tools or approaches would you use to diagnose a "the network feels slow" complaint?](#what-tools-or-approaches-would-you-use-to-diagnose-a-the-network-feels-slow-complaint)
- [Behavioral / Scenario-Based Questions](#behavioral--scenario-based-questions)
  - [A user reports they can't access a specific website, but other websites work fine — how would you troubleshoot it?](#a-user-reports-they-cant-access-a-specific-website-but-other-websites-work-fine--how-would-you-troubleshoot-it)
  - [Users on your network report intermittent slow performance during peak hours — how would you investigate whether it's bandwidth-related?](#users-on-your-network-report-intermittent-slow-performance-during-peak-hours--how-would-you-investigate-whether-its-bandwidth-related)
  - [You're designing a real-time video conferencing application — would you choose TCP or UDP for the media stream, and why?](#youre-designing-a-real-time-video-conferencing-application--would-you-choose-tcp-or-udp-for-the-media-stream-and-why)
  - [A web application is experiencing a spike in traffic and starting to slow down — how would networking concepts like load balancing and CDNs help address this?](#a-web-application-is-experiencing-a-spike-in-traffic-and-starting-to-slow-down--how-would-networking-concepts-like-load-balancing-and-cdns-help-address-this)
  - [How would you explain to a non-technical stakeholder why a website might load slowly for users in a different country, even though it works fine for you locally?](#how-would-you-explain-to-a-non-technical-stakeholder-why-a-website-might-load-slowly-for-users-in-a-different-country-even-though-it-works-fine-for-you-locally)
  - [You suspect a security breach might involve compromised credentials sent in plain text — what would you check, and how would you confirm your suspicion?](#you-suspect-a-security-breach-might-involve-compromised-credentials-sent-in-plain-text--what-would-you-check-and-how-would-you-confirm-your-suspicion)
  - [How would you decide the right subnet size when designing a new office network for around 50 devices, with room to grow?](#how-would-you-decide-the-right-subnet-size-when-designing-a-new-office-network-for-around-50-devices-with-room-to-grow)
  - [A colleague asks why their local development server, running on `localhost`, still uses TCP/IP concepts like ports at all — how would you explain it?](#a-colleague-asks-why-their-local-development-server-running-on-localhost-still-uses-tcpip-concepts-like-ports-at-all--how-would-you-explain-it)
- [How to Use This Guide](#how-to-use-this-guide)

---

<a id="-most-asked--tricky-questions"></a>
## 🔥 Most Asked / Tricky Questions

These come up in almost every Computer Networks interview. If you're short on time, start here.

<a id="what-is-the-difference-between-tcp-and-udp"></a>
### Q: What is the difference between TCP and UDP?
**Answer:** TCP (Transmission Control Protocol) is connection-oriented, establishing a session before data transfer, and guarantees reliable, in-order delivery through acknowledgments, retransmission, and flow/congestion control — at the cost of more overhead and latency. UDP (User Datagram Protocol) is connectionless, sending packets ("datagrams") without any delivery guarantee, ordering, or built-in error recovery, making it faster and lower-overhead, suited to latency-sensitive applications like video streaming or gaming where occasional loss is more acceptable than delay.

<a id="what-happens-when-you-type-a-url-into-a-browser-and-press-enter"></a>
### Q: What happens when you type a URL into a browser and press Enter?
**Answer:** The browser first checks its cache, then resolves the domain name to an IP address via DNS (checking local resolver caches before querying DNS servers). It establishes a TCP connection to that IP (typically on port 443 for HTTPS), performs a TLS handshake to encrypt the connection, sends an HTTP request, and the server processes it and returns an HTTP response, which the browser then parses and renders — fetching any additional resources (CSS, JS, images) referenced along the way through the same process.

<a id="what-is-the-difference-between-the-osi-model-and-the-tcpip-model"></a>
### Q: What is the difference between the OSI model and the TCP/IP model?
**Answer:** The OSI model is a theoretical, seven-layer reference model (Physical, Data Link, Network, Transport, Session, Presentation, Application) used mainly for teaching and conceptual understanding. The TCP/IP model is the practical, four-layer model (Network Interface, Internet, Transport, Application) that the actual Internet is built on, combining some of OSI's separate layers (like Session, Presentation, and Application into one Application layer).

<a id="what-is-the-three-way-handshake-in-tcp-and-why-is-it-needed"></a>
### Q: What is the three-way handshake in TCP, and why is it needed?
**Answer:** The process TCP uses to establish a connection: the client sends a SYN packet, the server responds with a SYN-ACK, and the client replies with an ACK. It's needed to synchronize both sides' initial sequence numbers and confirm that both sides are ready and able to send and receive data before any actual application data is exchanged.

<a id="what-is-the-difference-between-a-router-and-a-switch"></a>
### Q: What is the difference between a router and a switch?
**Answer:** A switch operates primarily at the Data Link layer (Layer 2), forwarding frames within a single local network based on MAC addresses. A router operates at the Network layer (Layer 3), forwarding packets between different networks based on IP addresses, and is what connects a local network to other networks, including the internet.

<a id="what-is-nat-network-address-translation-and-why-is-it-used"></a>
### Q: What is NAT (Network Address Translation), and why is it used?
**Answer:** NAT translates private, internal IP addresses to a single (or small pool of) public IP address(es) as traffic leaves a local network, and translates responses back to the correct internal address on the way in. It's used because the pool of available public IPv4 addresses is limited, letting many devices on a private network share one public IP, while also adding a layer of obscurity/protection for internal addressing.

<a id="what-is-the-difference-between-a-public-ip-and-a-private-ip-address"></a>
### Q: What is the difference between a public IP and a private IP address?
**Answer:** A public IP address is globally unique and routable directly over the internet. A private IP address (from reserved ranges like 10.0.0.0/8 or 192.168.0.0/16) is only valid within a local network and isn't routable on the public internet — devices using private IPs typically need NAT to communicate externally.

<a id="what-is-the-difference-between-http-and-https"></a>
### Q: What is the difference between HTTP and HTTPS?
**Answer:** HTTP transmits data in plain text, with no encryption, leaving it vulnerable to eavesdropping or tampering in transit. HTTPS is HTTP layered on top of TLS/SSL, encrypting the connection between client and server, and also authenticating the server's identity via its certificate, protecting both confidentiality and integrity of the exchanged data.

<a id="what-is-dns-and-why-is-it-needed"></a>
### Q: What is DNS, and why is it needed?
**Answer:** DNS (Domain Name System) translates human-readable domain names (like `example.com`) into the numeric IP addresses computers actually use to route traffic. It's needed because IP addresses are hard for people to remember and can change over time, while a domain name gives a stable, memorable identifier that DNS can map to the current correct address.

<a id="what-is-the-difference-between-a-mac-address-and-an-ip-address"></a>
### Q: What is the difference between a MAC address and an IP address?
**Answer:** A MAC address is a hardware-assigned identifier burned into a network interface card, unique at the Data Link layer, and used for communication within a local network segment. An IP address is a logical, software-assignable address at the Network layer, used to route traffic between different networks, and can change depending on which network a device connects to.

<a id="what-is-a-subnet-mask-and-what-is-it-used-for"></a>
### Q: What is a subnet mask, and what is it used for?
**Answer:** A subnet mask defines which portion of an IP address represents the network and which represents the specific host within that network, letting devices determine whether another IP address is on the same local network or needs to be reached through a router.

<a id="what-is-the-difference-between-symmetric-and-asymmetric-encryption-and-how-are-both-typically-used-together-in-tls"></a>
### Q: What is the difference between symmetric and asymmetric encryption, and how are both typically used together in TLS?
**Answer:** Symmetric encryption uses the same single key for both encryption and decryption — fast, but the key must somehow be securely shared between both parties first. Asymmetric encryption uses a public/private key pair, where anything encrypted with the public key can only be decrypted with the corresponding private key — slower, but solves the key-distribution problem. TLS typically uses asymmetric encryption during the initial handshake to securely exchange a symmetric session key, then switches to fast symmetric encryption for the actual bulk data transfer.

<a id="what-is-the-difference-between-a-firewall-and-a-proxy-server"></a>
### Q: What is the difference between a firewall and a proxy server?
**Answer:** A firewall monitors and filters network traffic based on defined rules (like IP addresses, ports, or protocols), primarily to block unauthorized or malicious traffic. A proxy server acts as an intermediary that forwards requests on behalf of a client (or server), which can be used for caching, anonymity, load balancing, or content filtering — the two serve different primary purposes, though they're sometimes combined in practice.

<a id="what-is-a-socket-and-what-identifies-one-uniquely"></a>
### Q: What is a socket, and what identifies one uniquely?
**Answer:** A socket is an endpoint for network communication, representing one side of a connection between two machines. A socket is uniquely identified by the combination of an IP address, a port number, and (for TCP) the protocol — this combination lets a single machine handle many simultaneous distinct connections.

<a id="what-is-the-difference-between-congestion-control-and-flow-control-in-tcp"></a>
### Q: What is the difference between congestion control and flow control in TCP?
**Answer:** Flow control prevents a fast sender from overwhelming a slow receiver, managed via the receiver's advertised window size, which reflects how much buffer space the receiver currently has available. Congestion control prevents the sender from overwhelming the network itself (routers/links between sender and receiver), managed via the sender dynamically adjusting how much data it sends based on detected network congestion (like packet loss or delay).

---

<a id="networking-basics--fundamentals"></a>
## Networking Basics & Fundamentals

<a id="what-is-a-computer-network-and-what-are-its-main-goals"></a>
### Q: What is a computer network, and what are its main goals?
**Answer:** A computer network is a collection of interconnected devices that can communicate and share resources with each other. Main goals include resource sharing (files, printers, internet access), communication between users/systems, reliability through redundancy, and scalability to support growing numbers of devices and traffic.

<a id="what-is-the-difference-between-lan-man-and-wan"></a>
### Q: What is the difference between LAN, MAN, and WAN?
**Answer:** A LAN (Local Area Network) covers a small geographic area, like a single building or campus. A MAN (Metropolitan Area Network) spans a larger area, like a city. A WAN (Wide Area Network) spans a very large geographic area, potentially across countries or continents — the internet itself is the largest WAN.

<a id="what-is-the-difference-between-a-client-server-architecture-and-a-peer-to-peer-p2p-architecture"></a>
### Q: What is the difference between a client-server architecture and a peer-to-peer (P2P) architecture?
**Answer:** In client-server architecture, dedicated server machines provide services/resources, and client machines request and consume them — a clear division of roles. In peer-to-peer architecture, every participating machine can act as both a client and a server simultaneously, sharing resources directly with other peers without a centralized server.

<a id="what-is-bandwidth-and-how-does-it-differ-from-latency"></a>
### Q: What is bandwidth, and how does it differ from latency?
**Answer:** Bandwidth is the maximum rate of data that can be transmitted over a network connection in a given time (throughput capacity, e.g. measured in Mbps). Latency is the time it takes for a single piece of data to travel from source to destination (delay) — a connection can have high bandwidth but still have high latency, and the two affect perceived performance differently depending on the workload.

<a id="what-is-the-difference-between-unicast-broadcast-and-multicast-communication"></a>
### Q: What is the difference between unicast, broadcast, and multicast communication?
**Answer:** Unicast sends data from one sender to exactly one specific receiver. Broadcast sends data from one sender to every device on the network segment. Multicast sends data from one sender to a specific group of interested receivers, without needing to send to every device on the network.

<a id="what-is-a-protocol-in-networking-terms"></a>
### Q: What is a protocol, in networking terms?
**Answer:** A protocol is a formally defined set of rules and conventions that govern how devices communicate — specifying the format of messages, the order of exchanges, and how errors are handled — ensuring that different devices and implementations can interoperate correctly.

<a id="what-is-encapsulation-in-the-context-of-networking-and-how-does-it-relate-to-the-layered-network-models"></a>
### Q: What is encapsulation in the context of networking, and how does it relate to the layered network models?
**Answer:** Encapsulation is the process of wrapping data with additional protocol-specific header (and sometimes trailer) information as it passes down through each layer of the network stack — e.g., application data gets a TCP header, then an IP header, then a frame header — with each layer's receiving counterpart on the other end stripping off its corresponding header (decapsulation) as the data moves back up the stack.

<a id="what-is-the-difference-between-circuit-switching-and-packet-switching"></a>
### Q: What is the difference between circuit switching and packet switching?
**Answer:** Circuit switching establishes a dedicated, fixed communication path between two endpoints for the entire duration of a session (like a traditional telephone call), reserving that capacity even during silence. Packet switching breaks data into independent packets that are routed individually and can take different paths, sharing network capacity dynamically and efficiently among many simultaneous communications — the approach the modern internet is built on.

<a id="what-is-the-difference-between-half-duplex-and-full-duplex-communication"></a>
### Q: What is the difference between half-duplex and full-duplex communication?
**Answer:** Half-duplex allows communication in both directions, but only one direction at a time (like a walkie-talkie). Full-duplex allows simultaneous communication in both directions at the same time (like a telephone call).

<a id="what-is-a-mac-address-and-what-is-its-typical-structure"></a>
### Q: What is a MAC address, and what is its typical structure?
**Answer:** A Media Access Control address is a unique 48-bit hardware identifier assigned to a network interface, typically written as six pairs of hexadecimal digits (e.g. `00:1A:2B:3C:4D:5E`). The first half generally identifies the manufacturer (the Organizationally Unique Identifier), and the second half is a unique identifier assigned by that manufacturer.

---

<a id="osi-model--tcpip-model"></a>
## OSI Model & TCP/IP Model

<a id="what-are-the-seven-layers-of-the-osi-model-from-bottom-to-top"></a>
### Q: What are the seven layers of the OSI model, from bottom to top?
**Answer:** Physical, Data Link, Network, Transport, Session, Presentation, and Application — often remembered with a mnemonic like "Please Do Not Throw Sausage Pizza Away."

<a id="what-is-the-role-of-the-physical-layer"></a>
### Q: What is the role of the Physical layer?
**Answer:** It's responsible for the actual transmission of raw, unstructured bits over a physical medium (like cables, radio waves, or fiber optics), dealing with concerns like voltage levels, cable types, connectors, and bit synchronization/timing.

<a id="what-is-the-role-of-the-data-link-layer-and-what-are-its-two-sublayers"></a>
### Q: What is the role of the Data Link layer, and what are its two sublayers?
**Answer:** It handles node-to-node data transfer within the same local network, framing raw bits into structured frames, performing error detection, and controlling access to the shared physical medium. Its two sublayers are LLC (Logical Link Control, handling flow control and error checking) and MAC (Media Access Control, handling addressing and medium access).

<a id="what-is-the-role-of-the-network-layer-and-what-is-its-primary-addressing-scheme"></a>
### Q: What is the role of the Network layer, and what is its primary addressing scheme?
**Answer:** It's responsible for routing packets between different networks, determining the best path from source to destination across potentially many intermediate networks. Its primary addressing scheme is the IP (Internet Protocol) address.

<a id="what-is-the-role-of-the-transport-layer"></a>
### Q: What is the role of the Transport layer?
**Answer:** It provides end-to-end communication services for applications, including segmentation of data, reliability (in the case of TCP), flow control, and multiplexing multiple application connections over the network using port numbers.

<a id="what-is-the-role-of-the-session-presentation-and-application-layers-and-why-are-they-often-merged-into-a-single-application-layer-in-the-tcpip-model"></a>
### Q: What is the role of the Session, Presentation, and Application layers, and why are they often merged into a single "Application layer" in the TCP/IP model?
**Answer:** The Session layer manages and maintains connections/sessions between applications. The Presentation layer handles data formatting, translation, encryption, and compression, ensuring data is presented in a usable format. The Application layer provides the actual interface applications use to access network services. They're merged in the TCP/IP model because, in practice, most real-world protocols and applications handle these concerns together rather than as strictly separate layers.

<a id="what-are-the-four-layers-of-the-tcpip-model-and-how-do-they-map-roughly-to-the-osi-model"></a>
### Q: What are the four layers of the TCP/IP model, and how do they map roughly to the OSI model?
**Answer:** Network Interface (Link) layer (maps to OSI's Physical + Data Link), Internet layer (maps to OSI's Network layer), Transport layer (maps to OSI's Transport layer), and Application layer (maps to OSI's Session + Presentation + Application layers combined).

<a id="at-which-osi-layer-does-a-switch-typically-operate-and-at-which-layer-does-a-router-operate"></a>
### Q: At which OSI layer does a switch typically operate, and at which layer does a router operate?
**Answer:** A traditional switch operates at Layer 2 (Data Link), forwarding based on MAC addresses. A router operates at Layer 3 (Network), forwarding based on IP addresses — though "Layer 3 switches" also exist, blending switching speed with routing capability.

---

<a id="physical--data-link-layer"></a>
## Physical & Data Link Layer

<a id="what-is-the-difference-between-a-hub-a-switch-and-a-bridge"></a>
### Q: What is the difference between a hub, a switch, and a bridge?
**Answer:** A hub is a simple, "dumb" physical-layer device that broadcasts every incoming signal to all connected ports, with no awareness of addressing at all. A bridge operates at the Data Link layer, connecting two network segments and forwarding frames selectively based on MAC addresses, reducing unnecessary traffic. A switch is essentially a multi-port bridge, providing the same MAC-address-based selective forwarding but for many more ports.

<a id="what-is-csmacd-and-where-was-it-historically-used"></a>
### Q: What is CSMA/CD, and where was it historically used?
**Answer:** Carrier Sense Multiple Access with Collision Detection — a media access control method where a device listens to the shared medium before transmitting (carrier sense), and if a collision is detected during transmission, both devices stop, wait a random backoff time, and retry. It was historically used in traditional shared-medium Ethernet (using hubs); modern switched Ethernet largely avoids collisions entirely via full-duplex, dedicated links.

<a id="what-is-csmaca-and-how-does-it-differ-from-csmacd"></a>
### Q: What is CSMA/CA, and how does it differ from CSMA/CD?
**Answer:** Carrier Sense Multiple Access with Collision Avoidance — instead of detecting collisions after they happen, it tries to avoid them proactively, e.g. by having a device wait a random time before transmitting even after sensing the medium is clear. It's used in Wi-Fi (802.11) networks, where detecting collisions directly (as CSMA/CD does) isn't practical because a transmitting radio can't simultaneously listen for a collision on the same frequency.

<a id="what-is-a-vlan-virtual-lan-and-why-is-it-used"></a>
### Q: What is a VLAN (Virtual LAN), and why is it used?
**Answer:** A VLAN logically segments a single physical switched network into multiple separate, isolated broadcast domains, as if they were on entirely separate physical switches, without needing separate physical hardware for each. It's used to improve security (isolating sensitive traffic), reduce broadcast traffic, and organize a network logically (e.g. by department) independent of physical device location.

<a id="what-is-the-difference-between-error-detection-and-error-correction-at-the-data-link-layer"></a>
### Q: What is the difference between error detection and error correction at the Data Link layer?
**Answer:** Error detection identifies that a transmission error occurred (e.g. via a checksum or CRC), but doesn't fix it — typically the receiver just requests retransmission. Error correction (like using Hamming codes) can actually identify and fix certain errors without needing retransmission, at the cost of extra redundant bits sent with every frame.

<a id="what-is-a-crc-cyclic-redundancy-check-and-what-is-it-used-for"></a>
### Q: What is a CRC (Cyclic Redundancy Check), and what is it used for?
**Answer:** A CRC is an error-detection technique that computes a short, fixed-size checksum value from a block of data using polynomial division, appended to the transmitted frame. The receiver recomputes the CRC on the received data and compares it to the transmitted value — a mismatch indicates the data was corrupted in transit.

<a id="what-is-the-difference-between-a-mac-address-and-a-port-number-in-terms-of-what-they-identify"></a>
### Q: What is the difference between a MAC address and a port number in terms of what they identify?
**Answer:** A MAC address identifies a specific physical network interface/device at the Data Link layer. A port number identifies a specific application or service running on a device at the Transport layer — the two operate at completely different layers and serve different addressing purposes.

<a id="what-is-arp-address-resolution-protocol-and-what-problem-does-it-solve"></a>
### Q: What is ARP (Address Resolution Protocol), and what problem does it solve?
**Answer:** ARP resolves a known IP address to the corresponding MAC address on a local network segment, by broadcasting a request ("who has this IP?") and having the owning device respond with its MAC address. It's needed because Data Link layer frames require a destination MAC address, but applications and higher layers only know the destination's IP address.

<a id="what-is-ethernet-and-what-is-a-typical-ethernet-frames-structure-at-a-high-level"></a>
### Q: What is Ethernet, and what is a typical Ethernet frame's structure at a high level?
**Answer:** Ethernet is the dominant Data Link layer technology for wired LANs, defining how devices format and transmit frames over a shared or switched medium. A typical Ethernet frame includes a preamble (for synchronization), destination and source MAC addresses, a type/length field, the actual payload data, and a trailing CRC checksum for error detection.

<a id="what-is-the-difference-between-store-and-forward-switching-and-cut-through-switching"></a>
### Q: What is the difference between store-and-forward switching and cut-through switching?
**Answer:** Store-and-forward switching receives an entire frame into a buffer, checks it for errors (via CRC), and only then forwards it — more reliable but adds latency. Cut-through switching starts forwarding a frame as soon as it reads the destination address, without waiting for the whole frame or checking for errors — lower latency, but can propagate corrupted frames.

---

<a id="network-layer--ip-addressing"></a>
## Network Layer & IP Addressing

<a id="what-is-an-ip-address-and-what-is-the-difference-between-ipv4-and-ipv6"></a>
### Q: What is an IP address, and what is the difference between IPv4 and IPv6?
**Answer:** An IP address is a numeric label assigned to a device to identify it on a network and enable routing. IPv4 addresses are 32 bits, written as four decimal octets (e.g. `192.168.1.1`), providing about 4.3 billion unique addresses — a supply that has effectively run out given today's number of connected devices. IPv6 addresses are 128 bits, written as eight groups of hexadecimal digits, providing a vastly larger address space designed to accommodate the internet's continued growth.

<a id="what-is-cidr-classless-inter-domain-routing-notation-and-what-does-the-number-after-the-slash-mean"></a>
### Q: What is CIDR (Classless Inter-Domain Routing) notation, and what does the number after the slash mean?
**Answer:** CIDR notation (e.g. `192.168.1.0/24`) specifies an IP address range along with a prefix length indicating how many leading bits represent the fixed network portion — the remaining bits are available for host addresses within that network. A `/24` means the first 24 bits are the network portion, leaving 8 bits (256 addresses) for hosts.

<a id="what-is-subnetting-and-why-is-it-used"></a>
### Q: What is subnetting, and why is it used?
**Answer:** Subnetting divides a larger network into smaller, logically separate sub-networks (subnets), each with its own address range. It's used to improve network organization and management, reduce broadcast traffic within each smaller subnet, and allocate address space more efficiently based on actual need rather than in large, wasteful blocks.

<a id="what-is-the-difference-between-a-network-address-a-broadcast-address-and-a-host-address-within-a-subnet"></a>
### Q: What is the difference between a network address, a broadcast address, and a host address within a subnet?
**Answer:** The network address (all host bits set to 0) identifies the subnet itself, and isn't assignable to any individual device. The broadcast address (all host bits set to 1) is used to send a message to every device on that subnet simultaneously. Host addresses are all the addresses in between, individually assignable to specific devices.

<a id="what-are-the-private-ip-address-ranges-defined-by-rfc-1918"></a>
### Q: What are the private IP address ranges defined by RFC 1918?
**Answer:** `10.0.0.0/8`, `172.16.0.0/12`, and `192.168.0.0/16` — these ranges are reserved for use within private networks and are never routed on the public internet.

<a id="what-is-the-difference-between-a-static-ip-address-and-a-dynamic-ip-address-and-what-protocol-typically-assigns-dynamic-addresses"></a>
### Q: What is the difference between a static IP address and a dynamic IP address, and what protocol typically assigns dynamic addresses?
**Answer:** A static IP address is manually configured and doesn't change over time. A dynamic IP address is automatically assigned, often temporarily, and can change — typically assigned via DHCP (Dynamic Host Configuration Protocol).

<a id="what-is-dhcp-and-what-is-the-typical-dora-process-it-uses-to-assign-an-address"></a>
### Q: What is DHCP, and what is the typical DORA process it uses to assign an address?
**Answer:** DHCP automatically assigns IP addresses (and other network configuration, like the default gateway and DNS servers) to devices joining a network. The DORA process: the client broadcasts a Discover message, a DHCP server responds with an Offer, the client sends a Request confirming it wants that offer, and the server sends an Acknowledgment finalizing the assignment.

<a id="what-is-the-default-gateway-and-what-role-does-it-play"></a>
### Q: What is the default gateway, and what role does it play?
**Answer:** The default gateway is the router a device sends traffic to when the destination address is on a different network than its own — it acts as the local "exit point" from a device's own subnet toward the rest of the network/internet.

<a id="what-is-ip-fragmentation-and-why-does-it-happen"></a>
### Q: What is IP fragmentation, and why does it happen?
**Answer:** IP fragmentation splits a single IP packet into multiple smaller packets when it's larger than the Maximum Transmission Unit (MTU) of a network link it needs to cross, since that link can't carry a packet that large in one piece — the fragments are reassembled by the receiving host once all pieces arrive.

<a id="what-is-the-difference-between-ipv4s-use-of-arp-and-ipv6s-use-of-ndp-neighbor-discovery-protocol"></a>
### Q: What is the difference between IPv4's use of ARP and IPv6's use of NDP (Neighbor Discovery Protocol)?
**Answer:** Both resolve a Layer 3 address to a Layer 2 MAC address on a local network, but IPv6's NDP is a more integrated, modern replacement built directly into ICMPv6, additionally handling tasks like router discovery, address autoconfiguration, and duplicate address detection — functions IPv4 needed several separate protocols (ARP, ICMP Router Discovery, etc.) to cover.

<a id="what-is-ttl-time-to-live-in-an-ip-packet-and-what-is-it-used-for"></a>
### Q: What is TTL (Time To Live) in an IP packet, and what is it used for?
**Answer:** A field that starts at some value and is decremented by 1 at each router (hop) the packet passes through; if it reaches 0, the packet is discarded and an error is sent back to the sender. It's used to prevent packets from looping indefinitely due to routing errors, and is also the mechanism the `traceroute` tool exploits to map a packet's path.

<a id="what-is-anycast-addressing-and-where-is-it-commonly-used"></a>
### Q: What is anycast addressing, and where is it commonly used?
**Answer:** Anycast assigns the same IP address to multiple physically distributed servers, and routing automatically directs a client's request to whichever instance is topologically "nearest" (by routing metrics) at that moment. It's commonly used for services needing both redundancy and low latency, like DNS root servers and CDNs.

---

<a id="routing"></a>
## Routing

<a id="what-is-routing-and-what-is-a-routing-table"></a>
### Q: What is routing, and what is a routing table?
**Answer:** Routing is the process of determining the path data should take across a network (or interconnected networks) to reach its destination. A routing table is a data structure maintained by a router listing known destination networks and the corresponding "next hop" to forward traffic toward each one.

<a id="what-is-the-difference-between-static-routing-and-dynamic-routing"></a>
### Q: What is the difference between static routing and dynamic routing?
**Answer:** Static routing uses manually configured, fixed routes that don't change unless an administrator updates them — simple and predictable, but doesn't adapt to network changes or failures automatically. Dynamic routing uses routing protocols that automatically discover and adapt routes based on the current state of the network, adjusting to failures or changes without manual intervention.

<a id="what-is-the-difference-between-distance-vector-and-link-state-routing-protocols"></a>
### Q: What is the difference between distance-vector and link-state routing protocols?
**Answer:** Distance-vector protocols (like RIP) have each router share its own routing table (distances to known destinations) with its immediate neighbors, gradually building up network-wide knowledge indirectly — simple, but slower to converge and prone to routing loops. Link-state protocols (like OSPF) have each router build and share a complete map of the network's topology with all other routers, then independently compute the best paths — more complex, but converges faster and avoids many of distance-vector's loop issues.

<a id="what-is-the-difference-between-an-interior-gateway-protocol-igp-and-an-exterior-gateway-protocol-egp"></a>
### Q: What is the difference between an interior gateway protocol (IGP) and an exterior gateway protocol (EGP)?
**Answer:** An IGP (like OSPF or RIP) routes traffic within a single autonomous system (a network under one administrative control, like a single organization). An EGP (most notably BGP) routes traffic between different autonomous systems, which is how the global internet's various independently-operated networks interconnect.

<a id="what-is-bgp-border-gateway-protocol-and-why-is-it-described-as-the-routing-protocol-of-the-internet"></a>
### Q: What is BGP (Border Gateway Protocol), and why is it described as the routing protocol of the internet?
**Answer:** BGP is the protocol autonomous systems use to exchange routing information with each other, making decisions based on configurable policies (not just shortest path) like business relationships and traffic preferences. It's described this way because it's the protocol that actually determines how traffic flows between the thousands of independently operated networks that together make up the global internet.

<a id="what-is-the-difference-between-a-routing-loop-and-how-protocols-like-rip-try-to-prevent-one"></a>
### Q: What is the difference between a routing loop and how protocols like RIP try to prevent one?
**Answer:** A routing loop occurs when packets get forwarded in a circular path between routers, never actually reaching their destination, often due to inconsistent/outdated routing information. RIP mitigates this with techniques like split horizon (not advertising a route back to the neighbor it was learned from) and setting a maximum hop count (16 is considered "infinity"/unreachable) to bound how long a loop can persist.

<a id="what-is-the-difference-between-routing-and-forwarding"></a>
### Q: What is the difference between routing and forwarding?
**Answer:** Routing is the control-plane process of building and maintaining the routing table — figuring out the best paths through the network. Forwarding is the data-plane process of actually moving an individual packet from an incoming interface to the correct outgoing interface, based on a lookup in that already-built routing table.

<a id="what-is-administrative-distance-and-why-does-it-matter-when-a-router-learns-the-same-destination-from-multiple-sources"></a>
### Q: What is administrative distance, and why does it matter when a router learns the same destination from multiple sources?
**Answer:** Administrative distance is a trust ranking a router assigns to different sources of routing information (e.g., a directly connected route, a static route, or a route learned via a specific dynamic protocol) — when a router learns about the same destination network from multiple different sources, it prefers the route with the lowest administrative distance.

---

<a id="transport-layer-tcp--udp"></a>
## Transport Layer (TCP & UDP)

<a id="what-is-a-port-number-and-what-is-the-difference-between-well-known-registered-and-dynamicprivate-ports"></a>
### Q: What is a port number, and what is the difference between well-known, registered, and dynamic/private ports?
**Answer:** A port number identifies a specific application or service on a device, letting a single IP address handle many simultaneous distinct connections. Well-known ports (0–1023) are reserved for standard, common services (like port 80 for HTTP). Registered ports (1024–49151) can be registered for specific applications by organizations. Dynamic/private ports (49152–65535) are used for temporary, ephemeral connections, like a client's outgoing connection port.

<a id="how-does-tcp-achieve-reliable-delivery"></a>
### Q: How does TCP achieve reliable delivery?
**Answer:** Through sequence numbers (so the receiver can detect missing or out-of-order data), acknowledgments (confirming received data), retransmission (resending data if an acknowledgment isn't received within a timeout), and checksums (detecting corrupted data).

<a id="what-is-the-tcp-sliding-window-and-what-is-it-used-for"></a>
### Q: What is the TCP sliding window, and what is it used for?
**Answer:** A mechanism that lets a sender transmit multiple segments before waiting for an acknowledgment, up to a window size the receiver has advertised based on its available buffer space, improving throughput compared to waiting for each individual segment's acknowledgment before sending the next.

<a id="what-is-the-difference-between-tcps-flow-control-and-congestion-control-mechanisms"></a>
### Q: What is the difference between TCP's flow control and congestion control mechanisms?
**Answer:** Flow control (managed via the receiver's advertised window) prevents the sender from overwhelming the specific receiver's ability to process incoming data. Congestion control (managed via mechanisms like slow start and congestion avoidance) prevents the sender from overwhelming the shared network path itself, adjusting the sending rate based on inferred network congestion.

<a id="what-is-tcps-slow-start-mechanism"></a>
### Q: What is TCP's "slow start" mechanism?
**Answer:** At the beginning of a connection (or after detecting congestion), TCP starts sending data conservatively with a small congestion window, then roughly doubles that window with each successful round trip until it either reaches a threshold or detects congestion (like packet loss) — gradually probing for the available network capacity rather than starting at full speed.

<a id="what-is-the-four-way-or-sometimes-described-as-three-way-handshake-used-to-close-a-tcp-connection"></a>
### Q: What is the four-way (or sometimes described as three-way) handshake used to close a TCP connection?
**Answer:** Either side can initiate closing: it sends a FIN, the other side acknowledges it with an ACK, then that other side sends its own FIN when it's also ready to close, and the original side acknowledges that with a final ACK — since data can still flow in one direction after the other side has finished sending, this is typically a four-step exchange (though the middle ACK and FIN can sometimes be combined).

<a id="what-is-the-time_wait-state-in-tcp-and-why-does-it-exist"></a>
### Q: What is the TIME_WAIT state in TCP, and why does it exist?
**Answer:** After actively closing a connection, the side that sent the final ACK enters TIME_WAIT for a period (typically related to twice the maximum expected packet lifetime) before fully releasing the connection's resources. It exists to ensure any delayed/duplicate packets from the old connection are properly discarded, and to make sure the final ACK actually got through (allowing retransmission if the other side didn't receive it).

<a id="what-are-the-main-differences-in-the-udp-header-compared-to-the-tcp-header"></a>
### Q: What are the main differences in the UDP header compared to the TCP header?
**Answer:** UDP's header is much simpler and smaller — just source port, destination port, length, and checksum — with no sequence numbers, acknowledgment numbers, window size, or connection-state flags, reflecting its lack of built-in reliability, ordering, or flow/congestion control.

<a id="what-is-head-of-line-blocking-and-how-does-it-relate-to-tcp"></a>
### Q: What is head-of-line blocking, and how does it relate to TCP?
**Answer:** Head-of-line blocking occurs when a single lost or delayed packet forces all subsequently received data to wait, even if that later data has already fully arrived, because TCP guarantees strictly in-order delivery to the application — one missing segment blocks everything behind it in the stream until it's retransmitted and received.

<a id="what-is-nagles-algorithm-and-what-problem-does-it-address"></a>
### Q: What is Nagle's algorithm, and what problem does it address?
**Answer:** Nagle's algorithm delays sending small TCP segments briefly, buffering and combining them into fewer, larger segments when possible, to avoid the network being flooded with many tiny, inefficient packets (each carrying significant relative overhead) — commonly disabled (via `TCP_NODELAY`) for latency-sensitive applications where that small buffering delay is undesirable.

<a id="what-is-the-difference-between-a-tcp-segment-an-ip-packet-and-an-ethernet-frame"></a>
### Q: What is the difference between a TCP segment, an IP packet, and an Ethernet frame?
**Answer:** A TCP segment is the unit of data at the Transport layer, containing the TCP header and application data. An IP packet wraps that TCP segment with an IP header, adding source/destination IP addressing for routing at the Network layer. An Ethernet frame wraps that IP packet with a frame header/trailer, adding MAC addressing for local delivery at the Data Link layer — each is the same underlying data with progressively more headers added at each layer down the stack.

<a id="why-might-an-application-choose-udp-over-tcp-despite-udps-lack-of-reliability"></a>
### Q: Why might an application choose UDP over TCP despite UDP's lack of reliability?
**Answer:** For latency-sensitive, real-time applications (like video calls, live streaming, or online gaming) where a lost or late packet is better simply dropped and skipped over rather than waited on and retransmitted, since by the time a retransmission arrived it would likely already be too outdated to be useful — trading guaranteed delivery for lower, more consistent latency.

---

<a id="application-layer--protocols"></a>
## Application Layer & Protocols

<a id="what-is-the-difference-between-http11-http2-and-http3"></a>
### Q: What is the difference between HTTP/1.1, HTTP/2, and HTTP/3?
**Answer:** HTTP/1.1 processes requests over a connection largely sequentially (with limited pipelining issues), often requiring multiple parallel TCP connections for performance. HTTP/2 introduces multiplexing multiple requests/responses over a single TCP connection concurrently, along with header compression, significantly reducing overhead. HTTP/3 replaces TCP with QUIC (built on UDP) as its transport, avoiding TCP's head-of-line blocking at the transport level and improving connection setup speed.

<a id="what-is-the-difference-between-an-http-get-request-and-a-post-request"></a>
### Q: What is the difference between an HTTP GET request and a POST request?
**Answer:** GET requests are meant to retrieve data without side effects, are idempotent (repeating the same request has the same effect as doing it once), and typically pass parameters in the URL, which can be cached and bookmarked. POST requests are meant to submit data that changes server state, aren't guaranteed idempotent, and pass data in the request body rather than the URL.

<a id="what-is-the-difference-between-http-status-code-categories-1xx-2xx-3xx-4xx-5xx"></a>
### Q: What is the difference between HTTP status code categories (1xx, 2xx, 3xx, 4xx, 5xx)?
**Answer:** 1xx are informational responses (rare, mid-request). 2xx indicate success (like 200 OK). 3xx indicate redirection (the client needs to take further action, like following a new URL). 4xx indicate a client error (the request itself was invalid, like 404 Not Found). 5xx indicate a server error (the request was valid, but the server failed to fulfill it, like 500 Internal Server Error).

<a id="what-is-the-difference-between-ftp-and-sftp"></a>
### Q: What is the difference between FTP and SFTP?
**Answer:** FTP (File Transfer Protocol) transmits data, including credentials, in plain text with no encryption, making it insecure over untrusted networks. SFTP (SSH File Transfer Protocol) runs file transfers over an encrypted SSH connection, protecting both credentials and data in transit.

<a id="what-is-smtp-and-what-role-does-it-play-in-sending-email"></a>
### Q: What is SMTP, and what role does it play in sending email?
**Answer:** SMTP (Simple Mail Transfer Protocol) is the protocol used to send email from a client to a mail server, and between mail servers, to route a message toward its destination — it's not used for retrieving/reading email, which is instead handled by protocols like IMAP or POP3.

<a id="what-is-the-difference-between-imap-and-pop3-for-retrieving-email"></a>
### Q: What is the difference between IMAP and POP3 for retrieving email?
**Answer:** POP3 typically downloads email messages to the client and removes them from the server (though "leave a copy" configurations exist), designed around a single-device, offline-access model. IMAP keeps messages synchronized on the server, allowing multiple devices to access and stay in sync with the same mailbox simultaneously, better suited to today's multi-device usage.

<a id="what-is-a-cookie-and-what-is-it-typically-used-for-in-http"></a>
### Q: What is a cookie, and what is it typically used for in HTTP?
**Answer:** A small piece of data a server asks the client's browser to store and automatically send back with future requests to that same domain, since HTTP itself is stateless. Cookies are commonly used for session management (keeping a user logged in), tracking, and personalization.

<a id="what-is-the-difference-between-http-being-stateless-and-how-web-applications-maintain-sessions-across-multiple-requests"></a>
### Q: What is the difference between HTTP being "stateless" and how web applications maintain sessions across multiple requests?
**Answer:** HTTP itself treats every request as independent, with no built-in memory of previous requests from the same client. Applications work around this by using mechanisms like cookies (storing a session identifier client-side) or tokens, which are sent with each subsequent request and let the server associate that request with previously stored session state.

<a id="what-is-websocket-and-how-does-it-differ-from-traditional-http-requestresponse-communication"></a>
### Q: What is WebSocket, and how does it differ from traditional HTTP request/response communication?
**Answer:** WebSocket establishes a single, persistent, full-duplex connection between client and server (after an initial HTTP-based handshake/upgrade), allowing either side to send messages to the other at any time without the overhead of repeated HTTP requests — well suited to real-time applications like chat or live updates, unlike traditional HTTP's request-then-response-then-close pattern.

<a id="what-is-a-rest-api-and-what-are-some-key-architectural-principles-it-follows"></a>
### Q: What is a REST API, and what are some key architectural principles it follows?
**Answer:** A REST (Representational State Transfer) API is a style of designing networked applications around standard HTTP methods and stateless request/response interactions with resources identified by URLs. Key principles include statelessness (each request contains all information needed to process it), a uniform interface (consistent use of HTTP methods and resource-based URLs), and typically representing resources in a standard format like JSON.

---

<a id="dns"></a>
## DNS

<a id="what-is-the-hierarchical-structure-of-the-dns-system-from-top-to-bottom"></a>
### Q: What is the hierarchical structure of the DNS system, from top to bottom?
**Answer:** The root domain (represented by a trailing dot), then top-level domains (TLDs) like `.com` or `.org`, then second-level domains (like `example` in `example.com`), and then any further subdomains (like `www` or `mail`) — each level is managed by different, delegated authorities.

<a id="what-is-the-difference-between-a-recursive-dns-resolver-and-an-authoritative-dns-server"></a>
### Q: What is the difference between a recursive DNS resolver and an authoritative DNS server?
**Answer:** A recursive resolver (often run by your ISP or a public service like Google's 8.8.8.8) takes a client's query and does the work of tracking down the answer by querying other DNS servers on the client's behalf, caching the result along the way. An authoritative DNS server is the definitive source of truth for a specific domain's actual records, directly answering queries about that domain.

<a id="what-is-the-difference-between-an-a-record-an-aaaa-record-a-cname-record-and-an-mx-record"></a>
### Q: What is the difference between an A record, an AAAA record, a CNAME record, and an MX record?
**Answer:** An A record maps a domain name to an IPv4 address. An AAAA record maps a domain name to an IPv6 address. A CNAME record maps a domain name as an alias pointing to another domain name (which is then further resolved). An MX record specifies which mail server(s) should receive email for a domain, along with a priority.

<a id="what-is-dns-caching-and-why-does-ttl-matter-for-it"></a>
### Q: What is DNS caching, and why does TTL matter for it?
**Answer:** DNS caching stores previously resolved domain-to-IP mappings temporarily (at various points: the OS, the browser, the resolver) to avoid repeating the full resolution process for every single request. The TTL (Time To Live) value on a DNS record specifies how long that cached result should be considered valid before it must be re-queried, balancing performance (longer TTL, fewer lookups) against how quickly changes to the record propagate (shorter TTL, faster updates).

<a id="what-is-a-dns-zone-and-what-is-zone-transfer"></a>
### Q: What is a DNS zone, and what is zone transfer?
**Answer:** A DNS zone is a distinct, administratively separate portion of the DNS namespace (like a specific domain and its subdomains) managed by a particular authority. Zone transfer is the process of replicating a zone's DNS records from a primary (master) DNS server to secondary (slave) servers, so multiple servers can authoritatively answer queries for that zone redundantly.

<a id="what-is-dns-spoofingcache-poisoning-and-what-does-it-exploit"></a>
### Q: What is DNS spoofing/cache poisoning, and what does it exploit?
**Answer:** An attack where false DNS response data is injected into a resolver's cache, causing it to return an incorrect (attacker-controlled) IP address for a domain, potentially redirecting users to a malicious site. It exploits the fact that traditional DNS responses aren't cryptographically authenticated, so a resolver has limited ability to verify a response actually came from the legitimate authoritative server — a problem that DNSSEC (DNS Security Extensions) was designed to address through cryptographic signing of records.

---

<a id="network-security"></a>
## Network Security

<a id="what-is-a-firewall-and-what-is-the-difference-between-a-stateless-and-a-stateful-firewall"></a>
### Q: What is a firewall, and what is the difference between a stateless and a stateful firewall?
**Answer:** A firewall filters network traffic based on defined security rules. A stateless firewall evaluates each packet independently against its rules, with no memory of previous packets/connections. A stateful firewall tracks the state of active connections, and can make smarter decisions based on that context — e.g., automatically allowing return traffic for a connection that was legitimately initiated from inside the network.

<a id="what-is-the-difference-between-a-vpn-and-a-proxy-from-a-security-perspective"></a>
### Q: What is the difference between a VPN and a proxy, from a security perspective?
**Answer:** A proxy forwards specific application-level traffic (like web requests) on a client's behalf, and typically doesn't encrypt traffic between the client and the proxy itself unless additional encryption is layered on top. A VPN encrypts and tunnels essentially all of a device's network traffic through a secure connection to the VPN server, providing broader, more consistent protection and often better privacy/security guarantees.

<a id="what-is-a-man-in-the-middle-mitm-attack-and-how-does-httpstls-help-prevent-one"></a>
### Q: What is a man-in-the-middle (MITM) attack, and how does HTTPS/TLS help prevent one?
**Answer:** A MITM attack occurs when an attacker secretly intercepts and potentially alters communication between two parties who believe they're communicating directly with each other. HTTPS/TLS helps prevent this by encrypting the traffic (so an intercepted message can't be read) and authenticating the server's identity via a certificate signed by a trusted certificate authority (so a client can detect if it's actually talking to an impostor).

<a id="what-is-a-ddos-attack-and-what-is-the-difference-between-it-and-a-regular-dos-attack"></a>
### Q: What is a DDoS attack, and what is the difference between it and a regular DoS attack?
**Answer:** A Denial of Service (DoS) attack attempts to make a service unavailable, typically by overwhelming it with traffic or exploiting a resource-exhaustion vulnerability, originating from a single source. A Distributed Denial of Service (DDoS) attack does the same thing but from many distributed sources simultaneously (often a botnet of compromised devices), making it much harder to block by simply filtering a single source, and generating far greater total traffic volume.

<a id="what-is-port-scanning-and-why-is-it-relevant-to-network-security"></a>
### Q: What is port scanning, and why is it relevant to network security?
**Answer:** Port scanning systematically probes a range of ports on a target machine to determine which ones are open and what services are listening on them. It's relevant because it's a common reconnaissance technique attackers use to identify potential entry points/vulnerabilities before attempting an actual attack, which is also why organizations monitor for and often restrict unsolicited port-scanning activity.

<a id="what-is-the-purpose-of-a-certificate-authority-ca-in-the-context-of-tlsssl-certificates"></a>
### Q: What is the purpose of a Certificate Authority (CA) in the context of TLS/SSL certificates?
**Answer:** A CA is a trusted third-party organization that verifies the identity of an entity (like a website owner) and issues a digitally signed certificate vouching for that identity. Browsers and operating systems maintain a list of trusted CAs, and trust any certificate signed by one of them, forming the basis of trust for HTTPS connections across the web.

<a id="what-is-the-difference-between-ids-and-ips"></a>
### Q: What is the difference between IDS and IPS?
**Answer:** An IDS (Intrusion Detection System) monitors network traffic for suspicious activity and alerts administrators, but doesn't take direct action to block it. An IPS (Intrusion Prevention System) also monitors for suspicious activity, but can actively intervene and block or drop malicious traffic in real time.

<a id="what-is-arp-spoofing-and-what-can-an-attacker-achieve-with-it"></a>
### Q: What is ARP spoofing, and what can an attacker achieve with it?
**Answer:** ARP spoofing sends falsified ARP responses onto a local network, associating an attacker's own MAC address with another device's (often the default gateway's) IP address. This can let an attacker intercept, modify, or redirect traffic intended for that device, forming the basis of local-network man-in-the-middle attacks.

<a id="what-is-the-principle-of-defense-in-depth-in-network-security"></a>
### Q: What is the principle of "defense in depth" in network security?
**Answer:** A strategy of layering multiple, independent security controls (firewalls, encryption, access controls, monitoring, intrusion detection) throughout a system, rather than relying on any single defense — so that if one layer is bypassed or fails, other layers still provide protection.

<a id="what-is-a-vpn-tunnel-and-what-does-tunneling-mean-in-this-context"></a>
### Q: What is a VPN tunnel, and what does "tunneling" mean in this context?
**Answer:** Tunneling means encapsulating one network protocol's traffic inside another, effectively creating a private, often encrypted logical path across a public/untrusted network (like the internet). A VPN tunnel wraps a device's actual network traffic inside an encrypted outer protocol, so intermediate network devices only see the encrypted outer packets, not the original traffic's content or, depending on configuration, even its true destination.

---

<a id="wireless--modern-networking"></a>
## Wireless & Modern Networking

<a id="what-is-the-difference-between-80211-wi-fi-standards-like-80211n-ac-ax"></a>
### Q: What is the difference between 802.11 Wi-Fi standards (like 802.11n, ac, ax)?
**Answer:** Each successive standard generally increases maximum theoretical throughput, improves spectral efficiency, and adds features like better handling of multiple simultaneous devices — e.g., 802.11ac introduced wider channels and multi-user MIMO, and 802.11ax (Wi-Fi 6) added further efficiency improvements particularly beneficial in dense, many-device environments.

<a id="what-is-the-difference-between-the-24ghz-and-5ghz-wi-fi-bands"></a>
### Q: What is the difference between the 2.4GHz and 5GHz Wi-Fi bands?
**Answer:** The 2.4GHz band has a longer range and better penetration through walls/obstacles, but lower maximum throughput and more interference (since more devices, including non-Wi-Fi ones like microwaves, use this crowded band). The 5GHz band offers higher throughput and less interference, but a shorter range and weaker penetration through obstacles.

<a id="what-is-a-content-delivery-network-cdn-and-what-problem-does-it-solve"></a>
### Q: What is a Content Delivery Network (CDN), and what problem does it solve?
**Answer:** A CDN is a geographically distributed network of servers that cache and serve content from a location physically closer to the requesting user. It solves the problem of latency and load for serving content globally, since fetching data from a nearby CDN edge server is faster than always fetching it from a single, potentially distant origin server, while also reducing load on that origin server.

<a id="what-is-a-load-balancer-and-what-is-the-difference-between-layer-4-and-layer-7-load-balancing"></a>
### Q: What is a load balancer, and what is the difference between Layer 4 and Layer 7 load balancing?
**Answer:** A load balancer distributes incoming network traffic across multiple backend servers to improve reliability and handle higher traffic volumes. Layer 4 load balancing makes routing decisions based on lower-level information like IP address and port, without inspecting the actual application content. Layer 7 load balancing operates at the application layer, and can make smarter routing decisions based on the actual content of the request, like the URL path or HTTP headers.

<a id="what-is-quic-and-what-advantage-does-it-offer-over-traditional-tcp-for-web-traffic"></a>
### Q: What is QUIC, and what advantage does it offer over traditional TCP for web traffic?
**Answer:** QUIC is a transport protocol built on top of UDP (rather than TCP) that provides reliability and congestion control itself, while also integrating encryption by default and supporting multiplexed streams without TCP's head-of-line blocking problem — it's the transport protocol underlying HTTP/3, offering faster connection establishment and better performance especially on lossy or high-latency networks.

<a id="what-is-the-basic-idea-behind-software-defined-networking-sdn"></a>
### Q: What is the basic idea behind Software-Defined Networking (SDN)?
**Answer:** SDN separates a network's control plane (the logic deciding how traffic should be routed) from its data plane (the actual hardware forwarding traffic), centralizing the control logic in software rather than distributing it across each individual physical device's own configuration — allowing more flexible, programmatic, and centrally managed network behavior.

---

<a id="network-performance--troubleshooting"></a>
## Network Performance & Troubleshooting

<a id="what-is-the-ping-command-used-for-and-what-does-it-actually-measure"></a>
### Q: What is the `ping` command used for, and what does it actually measure?
**Answer:** `ping` sends ICMP Echo Request packets to a target host and measures the round-trip time until an Echo Reply is received, used to check basic reachability and measure latency to a given destination.

<a id="what-is-the-traceroute-or-tracert-command-used-for-and-how-does-it-work"></a>
### Q: What is the `traceroute` (or `tracert`) command used for, and how does it work?
**Answer:** It maps the path (sequence of routers/hops) packets take to reach a destination, by sending packets with progressively increasing TTL values — each router along the path that discards a packet due to TTL expiration sends back an error message revealing its own address, letting the tool reconstruct the full path one hop at a time.

<a id="what-is-jitter-in-the-context-of-network-performance-and-why-does-it-matter-for-real-time-applications"></a>
### Q: What is jitter, in the context of network performance, and why does it matter for real-time applications?
**Answer:** Jitter is the variation in latency/delay between successive packets, rather than the absolute delay itself. It matters significantly for real-time applications like video calls or VoIP, where inconsistent arrival timing (even with acceptable average latency) can cause noticeable audio/video stuttering or require larger buffers to smooth out.

<a id="what-is-packet-loss-and-what-are-some-common-causes"></a>
### Q: What is packet loss, and what are some common causes?
**Answer:** Packet loss is when data packets fail to reach their destination at all. Common causes include network congestion (routers dropping packets when overwhelmed), hardware failures, wireless interference/signal issues, and misconfigured network devices.

<a id="what-is-the-difference-between-throughput-and-goodput"></a>
### Q: What is the difference between throughput and goodput?
**Answer:** Throughput is the total raw rate of data successfully transmitted over a network connection, including protocol overhead (headers, retransmissions). Goodput is the rate of only the actual useful application-level data delivered, excluding that overhead — goodput is always less than or equal to throughput.

<a id="what-tools-or-approaches-would-you-use-to-diagnose-a-the-network-feels-slow-complaint"></a>
### Q: What tools or approaches would you use to diagnose a "the network feels slow" complaint?
**Answer:** Start with `ping` to check basic reachability and latency, `traceroute` to identify where along the path delay is being introduced, checking for packet loss, and comparing performance across different destinations/times to isolate whether the issue is local (device/local network), ISP-related, or specific to a particular remote service.

---

<a id="behavioral--scenario-based-questions"></a>
## Behavioral / Scenario-Based Questions

<a id="a-user-reports-they-cant-access-a-specific-website-but-other-websites-work-fine--how-would-you-troubleshoot-it"></a>
### Q: A user reports they can't access a specific website, but other websites work fine — how would you troubleshoot it?
**Answer:** Check whether it's a DNS issue (try accessing the site by its IP address directly, or query DNS manually) versus a connectivity/routing issue (try `ping`/`traceroute` to that specific server) versus an application-level issue (check if the site itself is down for everyone via a third-party status checker), narrowing down which layer the problem is actually occurring at.

<a id="users-on-your-network-report-intermittent-slow-performance-during-peak-hours--how-would-you-investigate-whether-its-bandwidth-related"></a>
### Q: Users on your network report intermittent slow performance during peak hours — how would you investigate whether it's bandwidth-related?
**Answer:** Monitor network utilization/bandwidth usage during those peak periods to see if it's approaching the link's capacity, check for packet loss or increased latency correlating with the slow periods (suggesting congestion), and consider whether specific high-bandwidth applications or a growing number of connected devices are consuming disproportionate capacity during those windows.

<a id="youre-designing-a-real-time-video-conferencing-application--would-you-choose-tcp-or-udp-for-the-media-stream-and-why"></a>
### Q: You're designing a real-time video conferencing application — would you choose TCP or UDP for the media stream, and why?
**Answer:** UDP, generally — for real-time audio/video, a late-arriving retransmitted packet (which TCP would insist on) is often already useless by the time it arrives, since the moment it represents has passed; it's usually better to simply drop a lost packet and continue with fresher data, accepting brief, minor quality degradation over TCP's added latency from retransmission and strict in-order delivery.

<a id="a-web-application-is-experiencing-a-spike-in-traffic-and-starting-to-slow-down--how-would-networking-concepts-like-load-balancing-and-cdns-help-address-this"></a>
### Q: A web application is experiencing a spike in traffic and starting to slow down — how would networking concepts like load balancing and CDNs help address this?
**Answer:** A load balancer can distribute incoming requests across multiple backend server instances rather than overwhelming a single server, allowing horizontal scaling. A CDN can offload static content (images, CSS, JS) to geographically distributed edge servers, reducing both the load on the origin server and the latency experienced by users, letting the origin server focus its capacity on dynamic, non-cacheable requests.

<a id="how-would-you-explain-to-a-non-technical-stakeholder-why-a-website-might-load-slowly-for-users-in-a-different-country-even-though-it-works-fine-for-you-locally"></a>
### Q: How would you explain to a non-technical stakeholder why a website might load slowly for users in a different country, even though it works fine for you locally?
**Answer:** Explain that data has to physically travel over long distances to reach a distant server, and physical distance introduces real, unavoidable latency (the speed of light in fiber, plus each intermediate router's own processing delay) — describe how using a CDN or a server located closer to those users can significantly reduce that geographic latency.

<a id="you-suspect-a-security-breach-might-involve-compromised-credentials-sent-in-plain-text--what-would-you-check-and-how-would-you-confirm-your-suspicion"></a>
### Q: You suspect a security breach might involve compromised credentials sent in plain text — what would you check, and how would you confirm your suspicion?
**Answer:** Check whether the affected service/protocol was using an unencrypted connection (like plain HTTP or FTP rather than HTTPS or SFTP), potentially by capturing and inspecting network traffic (with proper authorization) to confirm credentials were visible in plain text, and recommend migrating that traffic to an encrypted equivalent protocol going forward.

<a id="how-would-you-decide-the-right-subnet-size-when-designing-a-new-office-network-for-around-50-devices-with-room-to-grow"></a>
### Q: How would you decide the right subnet size when designing a new office network for around 50 devices, with room to grow?
**Answer:** Calculate the minimum host bits needed to comfortably cover 50 devices plus reasonable future growth (a /26 subnet provides 62 usable host addresses, for example), while balancing against not allocating an excessively large subnet that wastes address space and increases the broadcast domain size unnecessarily — planning slightly ahead for growth rather than sizing the subnet exactly to today's count.

<a id="a-colleague-asks-why-their-local-development-server-running-on-localhost-still-uses-tcpip-concepts-like-ports-at-all--how-would-you-explain-it"></a>
### Q: A colleague asks why their local development server, running on `localhost`, still uses TCP/IP concepts like ports at all — how would you explain it?
**Answer:** Explain that `localhost` (127.0.0.1) still goes through the same core networking stack conceptually — the OS still needs a port number to know which specific listening application should receive an incoming connection, even though the "network" traffic never actually leaves the machine — the loopback interface just means the physical/data-link layers are essentially skipped, not that the transport-layer concepts like ports stop applying.

---

<a id="how-to-use-this-guide"></a>
## How to Use This Guide

- **A few days before an interview or exam?** Go section by section, top to bottom — each one builds on the last, from basics to routing, transport, and security.
- **Revising the night before?** Jump straight to 🔥 Most Asked / Tricky Questions, then skim section headers for anything you're unsure about.
- **During quick revision:** Use `Ctrl+F` (or `Cmd+F`) to jump straight to a keyword or topic instead of scrolling.
- **After every interview:** Come back and add any question you got asked that isn't already here — this file is meant to grow with you.

Good luck — you've got this. 🚀
