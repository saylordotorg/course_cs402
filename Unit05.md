---
layout: default
title: "CS402: Computer Communications and Networks"
course_description: "A detailed introduction to the basic hardware, software, and architectural components of computer communications in local area networks. Focuses on understanding the basics of computer networks, switching, routing, protocols, and security."
next: ../Unit06
previous: ../Unit04
---
**Unit 5: Network Layer** <span id="5"></span> 
*In this unit, we will learn how* packets *(groupings of data) travel on
a network and how each machine can be addressed uniquely so that data
transport between two nodes is reliable. We will learn that networks can
run out of space, meaning that unique addresses for different machines
are no longer available. In these situations, computer scientists must
manage IP addressing using CIDR and subnetting – techniques we will
learn about in this unit.  
  
 *The network layer is responsible for the delivery of packets from any
source to any destination through intermediate routers. Follow the links
to explore in detail the IPv4, IPv6, RIP, OSPF, and BGP protocols used
in today’s Internet.**

**Unit 5 Time Advisory**  
Completing this unit should take approximately 31 hours.  
  
 ☐    Subunit 5.1: 6.25 hours  
  
 ☐    Subunit 5.2: 5.5 hours  
  
 ☐    Subunit 5.3: 5 hours   
  
 ☐    Subunit 5.4: 2 hours  
  
 ☐    Subunit 5.5: 0.25 hours  
  
 ☐    Subunit 5.6: 12 hours\*  
    
 \*Note that 10 hours are allotted here to experiment with a software
tool.

**Unit5 Learning Outcomes**  
Upon successful completion of this unit, you will be able to:
-   describe and compare network layer protocols;
-   compare and contrast CIDR with subnetting activities within the
    network layer;
-   describe IP addressing and explain its purpose; and
-   define a packet and explain its role in transporting data.

**5.1 Principles** <span id="5.1"></span> 
-   **Reading: Université Catholique de Louvain: Olivier Bonaventure’s
    Computer Networking: Principles, Protocols, and Practice: “Chapter
    5: Introduction” and “Chapter 5, Section 5.1: Principles”**
    Link: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and
    Practice*: [“Chapter 5:
    Introduction”](http://www.saylor.org/site/wp-content/uploads/2012/02/Computer-Networking-Principles-Bonaventure-1-30-31-OTC1.pdf) **and**
    [“Chapter 5, Section 5.1:
    Principles”](http://www.saylor.org/site/wp-content/uploads/2012/02/Computer-Networking-Principles-Bonaventure-1-30-31-OTC1.pdf) (PDF)  
        
     Instructions: Read the introduction to chapter 5 and the beginning
    of section 5.1, “Principles,” on pages 127–129. Stop at section
    5.1.1, “Organisation of the Network Layer.”  
        
     The network layer includes the datagram and virtual circuit modes,
    the separation between the data plane and the control plane, and the
    algorithms used by routing protocols.  
        
     As you read this section, it is important to understand the purpose
    of the router and the use of the packet in enabling you to send data
    and receive the response. How does the packet interact with the
    router?  
        
     Reading these textbook sections and taking notes should take
    approximately 1 hour.  
        
     Terms of Use: *Computer Networking: Principles, Protocols, and
    Practice* was written by Olivier Bonaventure and relicensed under a
    [Creative Commons Attribution 3.0 Unported
    License](http://creativecommons.org/licenses/by/3.0/) as part of the
    Saylor Foundation’s Open Textbook Challenge.

**5.1.1 Organisation of the Network Layer** <span id="5.1.1"></span> 
-   **Reading: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*: “Chapter
    5, Section 5.1.1: Organisation of the network layer”**
    Link: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*:
    [“Chapter 5, Section 5.1.1: Organisation of the network
    layer”](http://www.saylor.org/site/wp-content/uploads/2012/02/Computer-Networking-Principles-Bonaventure-1-30-31-OTC1.pdf) (PDF)  
        
     Instructions: Read section 5.1.1, “Organisation of the Network
    Layer,” on pages 129–132.  
        
     What are the two internal organizations used in the network layer?
    When are each used? What is a datagram? Explore this section of your
    textbook to see how a datagram is used in the network level. Compare
    and contrast the datagram organization with the virtual circuit
    discussed in this section.  
      
     The concept of hop-by-hop forwarding is this section. What does
    this concept have to do with the routing table? What is the
    difference between the data and control planes?  
        
     Reading this textbook section and taking notes should take
    approximately 2 hours.  
        
     Terms of Use: *Computer Networking: Principles, Protocols, and
    Practice* was written by Olivier Bonaventure and relicensed under
    a [Creative Commons Attribution 3.0 Unported
    License](http://creativecommons.org/licenses/by/3.0/) as part of the
    Saylor Foundation’s Open Te introduced inxtbook Challenge.

-   **Mobile App: Jason Stafford’s *Learning Networking*: “The Network
    Layer”**

    Link: Jason Stafford’s *Learning Networking*: [“The Network
    Layer”](https://itunes.apple.com/us/app/learning-networking/id571370723?mt=8) (iOS
    App)

    Instructions: If you have chosen to download this app, watch the
    video “The Network Layer,” “\#4-ICND1-Video 4, Layer 3-The Network
    Layer-iPad HD.” As you watch the video, pay attention to the
    following techniques in the network layer: logical addressing,
    switching, route discovery and selection, and connection services.
    Note that no quiz or exam questions will be derived from material
    within, but it is still a useful supplementary resource.

    Terms of Use: Please respect the copyright and terms of use
    displayed on the webpage above.

**5.1.2 The Control Plane** <span id="5.1.2"></span> 
-   **Reading: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*: “Chapter
    5, Section 5.1.2: The control plane”**
    Link: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*:
    [“Chapter 5, Section 5.1.2: The control
    plane”](http://www.saylor.org/site/wp-content/uploads/2012/02/Computer-Networking-Principles-Bonaventure-1-30-31-OTC1.pdf) (PDF)  
        
     Instructions: Read the beginning of section 5.1.2, “The control
    plane,” in chapter 5 of your textbook. Stop at “Static routing.”  
        
     In this section, the textbook explains how the control plane
    maintains the routing table. The three techniques to accomplish this
    are static routing, distance vector routing, and link state routing.
    As you explore the next three subunits describing each one in
    detail, note the advantages and disadvantages of each technique. How
    does each method deal with link and router failures?  
        
     Reading this textbook section and taking notes should take
    approximately 15 minutes.  
      
     Terms of Use: *Computer Networking: Principles, Protocols, and
    Practice* was written by Olivier Bonaventure and relicensed under a
    [Creative Commons Attribution 3.0 Unported
    License](http://creativecommons.org/licenses/by/3.0/) as part of the
    Saylor Foundation’s Open Textbook Challenge.

**5.1.2.1 Static Routing** <span id="5.1.2.1"></span> 
-   **Reading: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*: “Chapter
    5, Section 5.1.2: Static routing”**
    Link: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*:
    [“Chapter 5, Section 5.1.2: Static
    Routing”](http://www.saylor.org/site/wp-content/uploads/2012/02/Computer-Networking-Principles-Bonaventure-1-30-31-OTC1.pdf) (PDF)  
        
     Instructions: Read “Static Routing” on pages 132–133. Stop at
    “Distance Vector Routing,” which you will read below. As you read,
    consider the following questions: What is static routing? What are
    its advantages and disadvantages?  
        
     Reading this textbook section and taking notes should take
    approximately 1 hour.  
        
     Terms of Use: *Computer Networking: Principles, Protocols, and
    Practice* was written by Olivier Bonaventure and relicensed under a
    [Creative Commons Attribution 3.0 Unported
    License](http://creativecommons.org/licenses/by/3.0/) as part of the
    Saylor Foundation’s Open Textbook Challenge.

**5.1.2.2 Distance Vendor Routing** <span id="5.1.2.2"></span> 
-   **Reading: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*: “Chapter
    5, Section 5.1.2: Distance vector routing”**
    Link: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*:
    [“Chapter 5, Section 5.1.2: Distance Vector
    Routing”](http://www.saylor.org/site/wp-content/uploads/2012/02/Computer-Networking-Principles-Bonaventure-1-30-31-OTC1.pdf) (PDF)  
      
     Instructions: Read “Distance Vector Routing” on pages 133–137).
    Stop at “Link State Routing,” which you will read below. As you
    read, consider the following questions: What is distance vector
    routing? What are its advantages and disadvantages?  
        
     Reading this textbook section and taking notes should take
    approximately 1 hour.  
        
     Terms of Use: *Computer Networking: Principles, Protocols, and
    Practice* was written by Olivier Bonaventure and relicensed under a
    [Creative Commons Attribution 3.0 Unported
    License](http://creativecommons.org/licenses/by/3.0/) as part of the
    Saylor Foundation’s Open Textbook Challenge.

**5.1.2.3 Link State Routing** <span id="5.1.2.3"></span> 
-   **Reading: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*: “Chapter
    5, Section 5.1.2: Link state routing”**
    Link: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*:
    [“Chapter 5, Section 5.1.2: Link State
    Routing”](http://www.saylor.org/site/wp-content/uploads/2012/02/Computer-Networking-Principles-Bonaventure-1-30-31-OTC1.pdf) (PDF)  
        
     Instructions: Read “Link State Routing” on pages 137–140. Stop at
    section 5.2, “Internet Protocol.” As you read, consider the
    following questions: What is link state routing? What are its
    advantages and disadvantages? How does link state routing handle
    link and routing failures?  
        
     Reading this textbook section and taking notes should take
    approximately 30 minutes.  
        
     Terms of Use: *Computer Networking: Principles, Protocols, and
    Practice* was written by Olivier Bonaventure and relicensed under a
    [Creative Commons Attribution 3.0 Unported
    License](http://creativecommons.org/licenses/by/3.0/) as part of the
    Saylor Foundation’s Open Textbook Challenge.

-   **Reading: Wikipedia: “Bellman–Ford algorithm”**
    Link: Wikipedia: [“Bellman–Ford
    Algorithm”](http://resources.saylor.org.s3.amazonaws.com/CS/CS402/CS402-5.1.2.3-Bellman-Ford-BY-SA_files/CS402-5.1.2.3-Bellman-Ford-BY-SA.html) (HTML)  
      
     Instructions: Read this article for more details about the
    Bellman-Ford routing algorithm. This routing protocol is used in
    RIP, OSPF, and BGP.  
        
     Reading this article and taking notes should take approximately 15
    minutes.  
        
     Terms of Use: Please respect the copyright and terms of use
    displayed on the webpage above.

-   **Reading: Wikipedia: “Dijkstra’s algorithm”**
    Link: Wikipedia: [“Dijkstra’s
    Algorithm”](http://resources.saylor.org.s3.amazonaws.com/CS/CS402/CS402-5.1.2.3-Dijkstra-BY-SA_files/CS402-5.1.2.3-Dijkstra-BY-SA.html) (HTML)  
        
     Instructions: Read this article for more details about the Dijkstra
    routing algorithm. What is the Dijkstra Algorithm? How is the
    Dijkstra Algorithm used in link state routing? Like the Bellman-Ford
    algorithm, this routing protocol is used in RIP, OSPF, and BGP.  
        
     Reading this article and taking notes should take approximately 15
    minutes.  
        
     Terms of Use: Please respect the copyright and terms of use
    displayed on the webpage above.

**5.2 Internet Protocol** <span id="5.2"></span> 
-   **Reading: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*: “Chapter
    5, Section 5.2: Internet Protocol”**
    Link: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*:
    [“Chapter 5, Section 5.2: Internet
    Protocol”](http://www.saylor.org/site/wp-content/uploads/2012/02/Computer-Networking-Principles-Bonaventure-1-30-31-OTC1.pdf) (PDF)  
        
     Instructions: Read the introduction to section 5.2, “Internet
    Protocol.” Stop at section 5.2.1 “IP Version 4,” which you will read
    below.  
        
     In this section we will explore the Internet Protocol (IP) to
    discover how IP enables the applications running above the transport
    layer (UDP/TCP) to utilize any of the different datalink layers
    available.  
        
     Reading this textbook section and taking notes should take
    approximately 15 minutes.  
      
     Terms of Use: *Computer Networking: Principles, Protocols, and
    Practice* was written by Olivier Bonaventure and relicensed under a
    [Creative Commons Attribution 3.0 Unported
    License](http://creativecommons.org/licenses/by/3.0/) as part of the
    Saylor Foundation’s Open Textbook Challenge.

**5.2.1 IP version 4 (IPv4)** <span id="5.2.1"></span> 
-   **Reading: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*: “Chapter
    5, Section 5.2.1: IP version 4”**
    Link: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*:
    [“Chapter 5, Section 5.2.1: IP version
    4”](http://www.saylor.org/site/wp-content/uploads/2012/02/Computer-Networking-Principles-Bonaventure-1-30-31-OTC1.pdf) (PDF)  
      
     Instructions: Read section 5.2.1, “IP version 4,” on pages
    141–150.  
      
     This section starts with a discussion of IP version 4 before
    exploring network addressing in more detail. As you read, consider
    the following questions: What are two of the problems with IP
    version 4 that led to the development of the Classless Interdomain
    Routing (CIDR) architecture? How does CIDR improve the scalability
    of the IP routing system?  
      
     Reading this textbook section and taking notes should take
    approximately 1 hour.  
        
     Terms of Use: *Computer Networking: Principles, Protocols, and
    Practice* was written by Olivier Bonaventure and relicensed under a
    [Creative Commons Attribution 3.0 Unported
    License](http://creativecommons.org/licenses/by/3.0/) as part of the
    Saylor Foundation’s Open Textbook Challenge.

**5.2.2 Internet Control Message Protocol (ICMP) Version 4** <span
id="5.2.2"></span> 
-   **Reading: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*: “Chapter
    5, Section 5.2.2: ICMP version 4”**
    Link: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*:
    [“Chapter 5, Section 5.2.2: ICMP version
    4”](http://www.saylor.org/site/wp-content/uploads/2012/02/Computer-Networking-Principles-Bonaventure-1-30-31-OTC1.pdf) (PDF)  
        
     Instructions: Read section 5.2.2, “ICMP version 4,” on pages
    151–157. Sometimes a router or the destination host has to inform
    the sender of the packet of a problem that occurred while processing
    that packet. In the TCP/IP protocol suite, this reporting is done by
    the Internet Control Message Protocol (ICMP). How are these messages
    generated by the ICMP?  
      
     Reading this textbook section and taking notes should take
    approximately 1 hour.  
      
     Terms of Use: *Computer Networking: Principles, Protocols, and
    Practice* was written by Olivier Bonaventure and relicensed under a
    [Creative Commons Attribution 3.0 Unported
    License](http://creativecommons.org/licenses/by/3.0/) as part of the
    Saylor Foundation’s Open Textbook Challenge.

**5.2.3 IP version 6 (IPv6)** <span id="5.2.3"></span> 
-   **Reading: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*: “Chapter
    5, Section 5.2.3: IP version 6”**
    Link: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*:
    [“Chapter 5, Section 5.2.3: IP version
    6”](http://www.saylor.org/site/wp-content/uploads/2012/02/Computer-Networking-Principles-Bonaventure-1-30-31-OTC1.pdf) (PDF)  
        
     Instructions: Read section 5.2.3, “IP version 6,” on pages 157–164.
    As the popularity of the Internet grew exponentially, it became
    necessary for an expanded addressing architecture, IP version 6
    (IPv6). This section discusses how IPv6 has resolved a number of
    routing issues while becoming the new standard.  
        
     Reading this textbook section and taking notes should take
    approximately 1 hour.  
        
     Terms of Use: *Computer Networking: Principles, Protocols, and
    Practice* was written by Olivier Bonaventure and relicensed under a
    [Creative Commons Attribution 3.0 Unported
    License](http://creativecommons.org/licenses/by/3.0/) as part of the
    Saylor Foundation’s Open Textbook Challenge.

**5.2.4 ICMP Version 6 (ICMPv6)** <span id="5.2.4"></span> 
-   **Reading: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*: “Chapter
    5, Section 5.2.4: ICMP version 6”**
    Link: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*:
    [“Chapter 5, Section 5.2.4: ICMP version
    6”](http://www.saylor.org/site/wp-content/uploads/2012/02/Computer-Networking-Principles-Bonaventure-1-30-31-OTC1.pdf) (PDF)  
        
     Instructions: Read section 5.2.4, “ICMP version 6,” on pages
    164–166. ICMPv6 is the companion protocol for IPv6, just as ICMPv4
    is the companion protocol for IPv4. ICMPv6 is used by routers and
    hosts to report problems when processing IPv6 packets. In addition,
    ICMPv6 is used when auto-configuring addresses. This section
    discusses messaging for IPv6.  
      
     Reading this textbook section and taking notes should take
    approximately 1 hour.  
      
     Terms of Use: *Computer Networking: Principles, Protocols, and
    Practice* was written by Olivier Bonaventure and relicensed under a
    [Creative Commons Attribution 3.0 Unported
    License](http://creativecommons.org/licenses/by/3.0/) as part of the
    Saylor Foundation’s Open Textbook Challenge.

-   **Mobile App: Jason Stafford’s *Learning Networking*: “IP
    Addressing”**

    Link: Jason Stafford’s *Learning Networking*: [“IP
    Addressing”](https://itunes.apple.com/us/app/learning-networking/id571370723?mt=8) (iOS
    App)

    Instructions: If you have chosen to download this app, watch videos
    7 through 9 on IP Addressing. As you watch the videos, try to
    understand how the IP address was converted from one format to
    another and how multicast IP addresses are defined. Note that no
    quiz or exam questions will be derived from material within, but it
    is still a useful supplementary resource.  
      
     Watching these videos should take approximately 1 hour.

    Terms of Use: Please respect the copyright and terms of use
    displayed on the webpage above.

**5.2.5 Middleboxes** <span id="5.2.5"></span> 
-   **Reading: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*: “Chapter
    5, Section 5.2.5: Middleboxes”**
    Link: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*:
    [“Chapter 5, Section 5.2.5:
    Middleboxes”](http://www.saylor.org/site/wp-content/uploads/2012/02/Computer-Networking-Principles-Bonaventure-1-30-31-OTC1.pdf) (PDF)  
        
     Instructions: Read the introduction to section 5.2.5,
    “Middleboxes.” Stop at “Firewalls,” which you will read below. As
    you read, consider the following questions: What is a Middlebox? Why
    do we need them?  
        
     Reading this textbook section and taking notes should take
    approximately 15 minutes.  
        
     Terms of Use: *Computer Networking: Principles, Protocols, and
    Practice* was written by Olivier Bonaventure and relicensed under a
    [Creative Commons Attribution 3.0 Unported
    License](http://creativecommons.org/licenses/by/3.0/) as part of the
    Saylor Foundation’s Open Textbook Challenge.

**5.2.5.1 Firewalls** <span id="5.2.5.1"></span> 
-   **Reading: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*: “Chapter
    5, Section 5.2.5: Firewalls”**
    Link: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*:
    [“Chapter 5, Section 5.2.5:
    Firewalls”](http://www.saylor.org/site/wp-content/uploads/2012/02/Computer-Networking-Principles-Bonaventure-1-30-31-OTC1.pdf) (PDF)  
        
     Instructions: Read “Firewalls” on pages 166–168. Stop at “NAT,”
    which you will read below. As you read, consider the following
    questions: When you first used your computer to access the Internet,
    what was the first security technique you heard about? How does a
    firewall protect your system from the “evil-doers” lurking on the
    Internet?  
        
     Reading this textbook section and taking notes should take
    approximately 30 minutes.  
        
     Terms of Use: *Computer Networking: Principles, Protocols, and
    Practice* was written by Olivier Bonaventure and relicensed under a
    [Creative Commons Attribution 3.0 Unported
    License](http://creativecommons.org/licenses/by/3.0/) as part of the
    Saylor Foundation’s Open Textbook Challenge.

**5.2.5.2 Network Address Translation (NAT)** <span
id="5.2.5.2"></span> 
-   **Reading: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*: “Chapter
    5, Section 5.2.5: NAT”**
    Link: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*:
    [“Chapter 5, Section 5.2.5:
    NAT”](http://www.saylor.org/site/wp-content/uploads/2012/02/Computer-Networking-Principles-Bonaventure-1-30-31-OTC1.pdf) (PDF)  
        
     Instructions: Read “NAT” on pages 168–169. Stop at section 5.3
    “Routing in IP networks.”  
        
     Large corporations and government agencies prefer their networks to
    be private (that is, not seen on the Internet). In this section,
    explore the concept of private networks to learn how their need to
    communicate with the outside world and with specific machines under
    certain conditions has resulted in NAT; the mechanism that allows
    private networks to communicate openly with the outside world. How
    does NAT work?  
        
     Reading this textbook section and taking notes should take
    approximately 30 minutes.  
        
     Terms of Use: *Computer Networking: Principles, Protocols, and
    Practice* was written by Olivier Bonaventure and relicensed under a
    [Creative Commons Attribution 3.0 Unported
    License](http://creativecommons.org/licenses/by/3.0/) as part of the
    Saylor Foundation’s Open Textbook Challenge.  
      

**5.3 Routing in IP Networks** <span id="5.3"></span> 
-   **Reading: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*: “Chapter
    5, Section 5.3: Routing in IP networks”**
    Link: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*:
    [“Chapter 5, Section 5.3: Routing in IP
    Networks”](http://www.saylor.org/site/wp-content/uploads/2012/02/Computer-Networking-Principles-Bonaventure-1-30-31-OTC1.pdf) (PDF)  
        
     Instructions: Read the introduction to section 5.3, “Routing in IP
    Networks,” on page 170. Stop at section 5.3.1, “Intradomain
    Routing,” which you will read below. Routing protocols will be
    discussed in terms of two classifications: intradomain and
    interdomain. What are the differences between these
    classifications?  
      
     Reading this textbook section and taking notes should take
    approximately 30 minutes.  
      
     Terms of Use: *Computer Networking: Principles, Protocols, and
    Practice* was written by Olivier Bonaventure and relicensed under a
    [Creative Commons Attribution 3.0 Unported
    License](http://creativecommons.org/licenses/by/3.0/) as part of the
    Saylor Foundation’s Open Textbook Challenge.

**5.3.1 Intradomain Routing** <span id="5.3.1"></span> 
-   **Reading: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*: “Chapter
    5, Section 5.3.1: Intradomain routing”**
    Link: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*:
    [“Chapter 5, Section 5.3.1: Intradomain
    Routing”](http://www.saylor.org/site/wp-content/uploads/2012/02/Computer-Networking-Principles-Bonaventure-1-30-31-OTC1.pdf) (PDF)  
        
     Instructions: Read the introduction to section 5.3.1, “Intradomain
    Routing,” on page 170. Stop at “RIP,” which you will read below. As
    you read, consider the following question: What are the main
    objectives of intradomain routing protocols?  
        
     Reading this textbook section and taking notes should take
    approximately 30 minutes.  
        
     Terms of Use: *Computer Networking: Principles, Protocols, and
    Practice* was written by Olivier Bonaventure and relicensed under a
    [Creative Commons Attribution 3.0 Unported
    License](http://creativecommons.org/licenses/by/3.0/) as part of the
    Saylor Foundation’s Open Textbook Challenge.

**5.3.1.1 Routing Information Protocol (RIP)** <span
id="5.3.1.1"></span> 
-   **Reading: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*: “Chapter
    5, Section 5.3.1: RIP”**
    Link: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*:
    [“Chapter 5, Section 5.3.1:
    RIP”](http://www.saylor.org/site/wp-content/uploads/2012/02/Computer-Networking-Principles-Bonaventure-1-30-31-OTC1.pdf) (PDF)  
        
     Instructions: Read “RIP” on pages 171–172. Stop at “OSPF,” which
    you will read below. As you read, consider the following questions:
    What is RIP? What are the features of the RIP protocol? How does RIP
    meet the objectives of intradomain routing? What are its
    weaknesses?  
        
     Reading this textbook section and taking notes should take
    approximately 1 hour.  
        
     Terms of Use: *Computer Networking: Principles, Protocols, and
    Practice* was written by Olivier Bonaventure and relicensed under a
    [Creative Commons Attribution 3.0 Unported
    License](http://creativecommons.org/licenses/by/3.0/) as part of the
    Saylor Foundation’s Open Textbook Challenge.

**5.3.1.2 Open Shortest Path First (OSPF)** <span id="5.3.1.2"></span> 
-   **Reading: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*: “Chapter
    5, Section 5.3.1: OSPF”**
    Link: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*:
    [“Chapter 5, Section 5.3.1:
    OSPF”](http://www.saylor.org/site/wp-content/uploads/2012/02/Computer-Networking-Principles-Bonaventure-1-30-31-OTC1.pdf) (PDF)  
        
     Instructions: Read “OSPF” on pages 172–175. Stop at section 5.3.2
    “Interdomain routing,” which you will read below. As you read,
    consider the following questions: What is OSPF? What are the
    features of the OSPF protocol? How does OSPF meet the objectives of
    intradomain routing? What are its weaknesses? How is OSPF different
    from RIP?  
        
     Reading this textbook section and taking notes should take
    approximately 1 hour.  
        
     Terms of Use: *Computer Networking: Principles, Protocols, and
    Practice* was written by Olivier Bonaventure and relicensed under a
    [Creative Commons Attribution 3.0 Unported
    License](http://creativecommons.org/licenses/by/3.0/) as part of the
    Saylor Foundation’s Open Textbook Challenge.

**5.3.2 Interdomain Routing** <span id="5.3.2"></span> 
-   **Reading: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*: “Chapter
    5, Section 5.3.2: Interdomain routing”**
    Link: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*:
    [“Chapter 5, Section 5.3.2: Interdomain
    Routing”](http://www.saylor.org/site/wp-content/uploads/2012/02/Computer-Networking-Principles-Bonaventure-1-30-31-OTC1.pdf) (PDF)  
        
     Instructions: Read section 5.3.2, “Interdomain Routing,” on pages
    175–194. As you read, consider the following questions: What are the
    objectives of interdomain routing? What is the difference between
    transit and stub domains? What are some of the relationships you can
    expect to find in an interdomain routing policy?  
        
     Describe the BGP. How does BGP differ from the intradomain
    protocols RIP and OSPF that you’ve studied? What messages might the
    BGP generate? What is router convergence? Why is router convergence
    necessary? How is router convergence handled by the BGP?  
        
     Reading this textbook section and taking notes should take
    approximately 2 hours.  
      
     Terms of Use: *Computer Networking: Principles, Protocols, and
    Practice* was written by Olivier Bonaventure and relicensed under a
    [Creative Commons Attribution 3.0 Unported
    License](http://creativecommons.org/licenses/by/3.0/) as part of the
    Saylor Foundation’s Open Textbook Challenge.

**5.4 Resource Management** <span id="5.4"></span> 
-   **Reading: Massachussets Institute of Technology OpenCourseWare:
    Prof. Hari Balakrishnan’s *Computer Networks*: “Lecture 8:
    End-to-End Congestion Control”**
    Link: Massachusetts Institute of Technology OpenCourseWare: Prof.
    Hari Balakrishnan’s *Computer Networks*: [“Lecture 8: End-to-End
    Congestion
    Control”](http://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-829-computer-networks-fall-2002/lecture-notes/L8e2ecc.pdf) (PDF)  
        
     Instructions: Read this tutorial to understand congestion
    management at different levels: end-to-end, router assisted, and
    pricing based.  
        
     Reading this tutorial and taking notes should take approximately 2
    hours.  
      
     Terms of Use: Please respect the copyright and terms of use
    displayed on the webpage above.

**5.5 Summary** <span id="5.5"></span> 
-   **Web Media: YouTube: FrippeMax’s “Warriors of the Net”**
    Link: YouTube: FrippeMax’s [“Warriors of the
    Net”](http://www.youtube.com/watch?v=PBWhzz_Gn10) (YouTube)   
        
     Instructions: Watch this video. Note how the concepts from this
    course are animated and the actions they take. Did you see the
    routing protocols (RIP, OSPF, and BGP)?  
        
     Watching the video and taking notes should take approximately 15
    minutes.  
      
     Terms of Use: Please respect the copyright and terms of use
    displayed on the webpage above.

**5.6 Practice Exercises** <span id="5.6"></span> 
-   **Activity: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*: “Chapter
    5, Section 5.5: Exercises”**
    Link: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*:
    [“Chapter 5, Section 5.5:
    Exercises”](http://www.saylor.org/site/wp-content/uploads/2012/02/Computer-Networking-Principles-Bonaventure-1-30-31-OTC1.pdf) (PDF)  
      
     Instructions: Read from section 5.5, “Exercises,” through the end
    of chapter 5, on pages 195–209. These exercises expand the key
    principles in this chapter. If you are a computer professional, you
    will enjoy the challenges and higher-level discussions in this
    section. If you are a novice, explore the presentations and spend
    more time on the topics that are meaningful to you.  
        
     Reading these exercises and taking notes should take approximately
    2 hours.  
        
     Terms of Use: *Computer Networking: Principles, Protocols, and
    Practice* was written by Olivier Bonaventure and relicensed under a
    [Creative Commons Attribution 3.0 Unported
    License](http://creativecommons.org/licenses/by/3.0/) as part of the
    Saylor Foundation’s Open Textbook Challenge.

-   **Activity: “The Network Simulator: ns-2”**
    Link: [“The Network Simulator:
    ns-2”](http://www.isi.edu/nsnam/ns/) (HTML)  
        
     Instructions: This is a software tool that helps you perform
    networking experiments on your computer. Download and try it with a
    few simple examples, such as exercise 5 (page 196) and 6 (page 197)
    in the textbook.  
        
     Reading the instructions, installing ns-2, and practicing two or
    three exercises should take approximately 10 hours.  
        
     Terms of Use: Please respect the copyright and terms of use
    displayed on the webpage above.

-   **Mobile App: Nutec Apps, LLC’s *LAN Scan HD - Network Device
    Scanner***
    Link: Nutec Apps, LLC’s *[LAN Scan HD - Network Device
    Scanner](https://itunes.apple.com/cn/app/lan-scan-hd-network-device/id597952879?mt=8) *(iOS
    App)  
        
     Instructions: This optional app corresponds to the following
    activity. Note that there are costs associated with this app and
    that it is only available to iOS users. No quiz or exam questions
    will be derived from material within, but it is still a useful
    supplementary resource.  
        
     Terms of Use: Please respect the copyright and terms of use
    displayed on the webpage above.  

-   **Activity: The Saylor Foundation’s “Network Device Scanning”**
    Link: The Saylor Foundation’s [“Network Device
    Scanning”](http://www.saylor.org/site/wp-content/uploads/2013/03/CS402-5.6-NetworkDeviceScanning-FINAL.pdf)
    (PDF)  
      
     <span style="font-family: Arial, sans-serif;">Instructions: Follow
    the steps detailed in this document. You will learn how to scan for
    network devices in your local area network using a mobile device, in
    this case, the “LAN Scan HD” app.</span>

**Unit 5 Assessment** <span id="5.7"></span> 
-   **Assessment: The Saylor Foundation’s “Unit 5 Assessment”**
    Link: The Saylor Foundation’s [“Unit 5
    Assessment”](http://school.saylor.org/mod/quiz/view.php?id=1287) (HTML)  
        
     Instructions: Complete this assessment, which will test your
    understanding of the material in this unit. The correct answers will
    be displayed after you click “Submit.”  
      
     *Note: You must be logged into your Saylor Foundation School
    account in order to access this exam. If you do not yet have an
    account, you will be able to create one, free of charge, after
    clicking the link.*


