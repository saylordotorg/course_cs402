---
layout: default
title: "CS402: Computer Communications and Networks"
course_description: "A detailed introduction to the basic hardware, software, and architectural components of computer communications in local area networks. Focuses on understanding the basics of computer networks, switching, routing, protocols, and security."
next: ../Unit07
previous: ../Unit05
---
**Unit 6: Link Layer** <span id="6"></span> 
*The final layer of the TCP/IP protocol stack that you will learn in
this course is known as the link layer. This unit will explain how you
can address machines on a network from that layer, use IP addresses to
determine physical addresses, and identify the different mechanisms in
the link layer that can correct packet collisions when data is
transferred over the wire.  
    
 *This unit guides you through the principles of the link layer. Then
the textbook will direct your focus to computer networks with a
discussion of how multiple hosts share one transmission medium. The
chapter ends with a detailed discussion of the two types of computer
networks that are important today from a deployment perspective:
Ethernet and WiFi.**

**Unit 6 Time Advisory**  
Completing this unit should take approximately 17.75 hours.  
  
 ☐    Subunit 6.1: 1.5 hours  
  
 ☐    Subunit 6.2: 5.5 hours  
  
 ☐    Subunit 6.3: 6.5 hours   
  
 ☐    Subunit 6.4: 2.25 hours  
  
 ☐    Subunit 6.5: 2 hours

**Unit6 Learning Outcomes**  
Upon successful completion of this unit, you will be able to:
-   demonstrate an understanding of the link layer;
-   compare and contrast IP addresses with physical addressing in the
    link layer;
-   explain packet collisions and how they are corrected in the link
    layer; and
-   define CSMA and describe its use in the link layer.

**6.1 Principles** <span id="6.1"></span> 
-   **Reading: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*: “Chapter
    6: Introduction” and “Chapter 6, Section 6.1: Principles”**
    Link: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*:
    [“Chapter 6:
    Introduction”](http://www.saylor.org/site/wp-content/uploads/2012/02/Computer-Networking-Principles-Bonaventure-1-30-31-OTC1.pdf) (PDF)
    and** **[“Chapter 6, Section 6.1:
    Principles”](http://www.saylor.org/site/wp-content/uploads/2012/02/Computer-Networking-Principles-Bonaventure-1-30-31-OTC1.pdf) (PDF)  
        
     Instructions: Read the introduction to chapter 6 and the beginning
    of section 6.1, “Principles,” on pages 211–212. Stop at section
    6.1.1 “Framing,” which you will read below.  
      
     The datalink layer uses the service provided by each of the
    different technologies found in the physical layer to send and
    receive bits between directly connected devices. The datalink layer
    receives packets from the network layer. What are the two main
    services provided by the datalink layer? Why are these services
    necessary?  
        
     Reading these textbook sections and taking notes should take
    approximately 30 minutes.  
      
     Terms of Use: *Computer Networking: Principles, Protocols, and
    Practice* was written by Olivier Bonaventure and relicensed under a
    [Creative Commons Attribution 3.0 Unported
    License](http://creativecommons.org/licenses/by/3.0/) as part of the
    Saylor Foundation’s Open Textbook Challenge.

**6.1.1 Framing** <span id="6.1.1"></span> 
-   **Reading: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*: “Chapter
    6, Section 6.1.1: Framing”**
    Link: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*:
    [“Chapter 6, Section 6.1.1:
    Framing”](http://www.saylor.org/site/wp-content/uploads/2012/02/Computer-Networking-Principles-Bonaventure-1-30-31-OTC1.pdf) (PDF)  
        
     Instructions: Read section 6.1.1, “Framing,” on pages 212–213. As
    you read, consider the following questions: What is the framing
    problem? What service does the datalink layer provide to resolve
    this problem?  
        
     Reading this textbook section and taking notes should take
    approximately 30 minutes.  
      
     Terms of Use: *Computer Networking: Principles, Protocols, and
    Practice* was written by Olivier Bonaventure and relicensed under a
    [Creative Commons Attribution 3.0 Unported
    License](http://creativecommons.org/licenses/by/3.0/) as part of the
    Saylor Foundation’s Open Textbook Challenge.

**6.1.2 Error Detection** <span id="6.1.2"></span> 
-   **Reading: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*: “Chapter
    6, Section 6.1.2: Error Detection”**
    Link: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*:
    [“Chapter 6, Section 6.1.2: Error
    Detection”](http://www.saylor.org/site/wp-content/uploads/2012/02/Computer-Networking-Principles-Bonaventure-1-30-31-OTC1.pdf) (PDF)  
        
     Instructions: Read section 6.1.2, “Error Detection,” on pages
    213–214. Datalink mechanisms also help solve problems related to
    detecting transmission error.  
        
     Reading this textbook section and taking notes should take
    approximately 30 minutes.  
        
     Terms of Use: *Computer Networking: Principles, Protocols, and
    Practice* was written by Olivier Bonaventure and relicensed under a
    [Creative Commons Attribution 3.0 Unported
    License](http://creativecommons.org/licenses/by/3.0/) as part of the
    Saylor Foundation’s Open Textbook Challenge.

**6.2 Medium Access Control** <span id="6.2"></span> 
-   **Reading: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*: “Chapter
    6, Section 6.2: Medium Access Control”**
    Link: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*:
    [“Chapter 6, Section 6.2: Medium Access
    Control”](http://www.saylor.org/site/wp-content/uploads/2012/02/Computer-Networking-Principles-Bonaventure-1-30-31-OTC1.pdf) (PDF)  
        
     Instructions: Read the beginning of section 6.2, “Medium Access
    Control,” on pages 214–215. Stop at section 6.2.1 “Static Allocation
    Methods,” which you will read below.  
        
     A *computer network* environment faces additional problems beyond
    the framing and error detection issues that are resolved in the
    datalink layer. What are these problems? How does the Medium Access
    Control algorithm(s) function in any of the *computer network*
    topologies?  
        
     Reading this textbook article and taking notes should take
    approximately 30 minutes.  
        
     Terms of Use: *Computer Networking: Principles, Protocols, and
    Practice* was written by Olivier Bonaventure and relicensed under a
    [Creative Commons Attribution 3.0 Unported
    License](http://creativecommons.org/licenses/by/3.0/) as part of the
    Saylor Foundation’s Open Textbook Challenge.

**6.2.1 Static Allocation Methods** <span id="6.2.1"></span> 
-   **Reading: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*: “Chapter
    6, Section 6.2.1: Static allocation methods”**
    Link: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*:
    [“Chapter 6, Section 6.2.1: Static allocation
    methods”](http://www.saylor.org/site/wp-content/uploads/2012/02/Computer-Networking-Principles-Bonaventure-1-30-31-OTC1.pdf) (PDF)  
        
     Instructions: Read section 6.2.1, “Static Allocation Methods,” on
    pages 215–216. As you read, consider the following questions: What
    is static allocation? What are some of the static allocation methods
    utilized in the datalink layer to share resources in a *computer
    network*? Describe each method and how each handles the available
    resources.  
        
     Reading this textbook section and taking notes should take
    approximately 30 minutes.  
        
     Terms of Use: *Computer Networking: Principles, Protocols, and
    Practice* was written by Olivier Bonaventure and relicensed under a
    [Creative Commons Attribution 3.0 Unported
    License](http://creativecommons.org/licenses/by/3.0/) as part of the
    Saylor Foundation’s Open Textbook Challenge.

**6.2.2 ALOHA** <span id="6.2.2"></span> 
-   **Reading: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*: “Chapter
    6, Section 6.2.2: ALOHA”**
    Link: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*:
    [“Chapter 6, Section 6.2.2:
    ALOHA”](http://www.saylor.org/site/wp-content/uploads/2012/02/Computer-Networking-Principles-Bonaventure-1-30-31-OTC1.pdf) (PDF)  
        
     Instructions: Read section 6.2.2, “ALOHA,” on pages 216–217. The
    University of Hawaii addressed the problem of sharing resources with
    its network of remote island campuses in a unique way. This
    description of the ALOHAnet explores their solution.  
      
     Reading this textbook section and taking notes should take
    approximately 15 minutes.  
      
     Terms of Use: *Computer Networking: Principles, Protocols, and
    Practice* was written by Olivier Bonaventure and relicensed under a
    [Creative Commons Attribution 3.0 Unported
    License](http://creativecommons.org/licenses/by/3.0/) as part of the
    Saylor Foundation’s Open Textbook Challenge.

-   **Reading: Wikipedia: “ALOHAnet”**
    Link: Wikipedia:
    [“ALOHAnet”](http://en.wikipedia.org/wiki/ALOHAnet) (HTML)  
        
     Instructions: Read this article, which provides a more detailed
    examination of the ALOHAnet structure.  
        
     Reading this article and taking notes should take approximately 15
    minutes.  
        
     Terms of Use: Please respect the copyright and terms of use
    displayed on the webpage above.

**6.2.3 Carrier Sense Multiple Access (CSMA)** <span id="6.2.3"></span> 
-   **Reading: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*: “Chapter
    6, Section 6.2.3: Carrier Sense Multiple Access”**
    Link: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*:
    [“Chapter 6, Section 6.2.3: Carrier Sense Multiple
    Access”](http://www.saylor.org/site/wp-content/uploads/2012/02/Computer-Networking-Principles-Bonaventure-1-30-31-OTC1.pdf) (PDF)  
        
     Instructions: Read section 6.2.3, “Carrier Sense Multiple Access,”
    on pages 217–218. The ALOHA solution has been enhanced by CSMA. As
    you read, be able to describe CSMA and how it works to share
    *computer network* resources.  
        
     Reading this textbook section and taking notes should take
    approximately 30 minutes.  
        
     Terms of Use: *Computer Networking: Principles, Protocols, and
    Practice* was written by Olivier Bonaventure and relicensed under a
    [Creative Commons Attribution 3.0 Unported
    License](http://creativecommons.org/licenses/by/3.0/) as part of the
    Saylor Foundation’s Open Textbook Challenge.

**6.2.4 CSMA With Collision Detection** <span id="6.2.4"></span> 
-   **Reading: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*: “Chapter
    6, Section 6.2.4: Carrier Sense Multiple Access with Collision
    Detection”**
    Link: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*:
    [“Chapter 6, Section 6.2.4: Carrier Sense Multiple Access with
    Collision
    Detection”](http://www.saylor.org/site/wp-content/uploads/2012/02/Computer-Networking-Principles-Bonaventure-1-30-31-OTC1.pdf) (PDF)  
        
     Instructions: Read section 6.2.4, “Carrier Sense Multiple Access
    with Collision Detection,” on pages 218–222. In a wired environment,
    both ALOHA and CSMA performance are better able to detect collision.
    Can you explain why that is?  
     Reading this textbook section and taking notes should take
    approximately 1.5 hours.  
        
     Terms of Use: *Computer Networking: Principles, Protocols, and
    Practice* was written by Olivier Bonaventure and relicensed under a
    [Creative Commons Attribution 3.0 Unported
    License](http://creativecommons.org/licenses/by/3.0/) as part of the
    Saylor Foundation’s Open Textbook Challenge.

**6.2.5 CSMA with Collision Avoidance (CSMA/CA)** <span
id="6.2.5"></span> 
-   **Reading: Université Catholique de Louvain: Olivier Bonaventure’s
    Computer Networking: Principles, Protocols, and Practice: “Chapter
    6, Section 6.2.5: Carrier Sense Multiple Access with Collision
    Avoidance”**
    Link: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*:
    [“Chapter 6, Section 6.2.5: Carrier Sense Multiple Access with
    Collision
    Avoidance”](http://www.saylor.org/site/wp-content/uploads/2012/02/Computer-Networking-Principles-Bonaventure-1-30-31-OTC1.pdf) (PDF)  
        
     Instructions: Read section 6.2.5, “Carrier Sense Multiple Access
    with Collision Avoidance,” on pages 222–225. CSMA/CA is found in the
    Wi-Fi environment. How are collisions avoided?  
        
     Reading this textbook section and taking notes should take
    approximately 1 hour.  
        
     Terms of Use: *Computer Networking: Principles, Protocols, and
    Practice* was written by Olivier Bonaventure and relicensed under a
    [Creative Commons Attribution 3.0 Unported
    License](http://creativecommons.org/licenses/by/3.0/) as part of the
    Saylor Foundation’s Open Textbook Challenge.

**6.2.6 Deterministic Medium Access Control Algorithms** <span
id="6.2.6"></span> 
-   **Reading: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*: “Chapter
    6, Section 6.2.6: Deterministic Medium Access Control algorithms”**
    Link: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*:
    [“Chapter 6, Section 6.2.6: Deterministic Medium Access Control
    algorithms”](http://www.saylor.org/site/wp-content/uploads/2012/02/Computer-Networking-Principles-Bonaventure-1-30-31-OTC1.pdf) (PDF)  
        
     Instructions: Read section 6.2.6, “Deterministic Medium Access
    Control algorithms,” on pages 226–228. Some applications are
    sensitive to the time delay of transmissions. Deterministic Medium
    Access Control algorithms have been used to resolve this problem.
    Explore this section to see some of the deterministic algorithms.  
     Reading this textbook section and taking notes should take
    approximately 1 hour.  
        
     Terms of Use: *Computer Networking: Principles, Protocols, and
    Practice* was written by Olivier Bonaventure and relicensed under a
    [Creative Commons Attribution 3.0 Unported
    License](http://creativecommons.org/licenses/by/3.0/) as part of the
    Saylor Foundation’s Open Textbook Challenge.

-   **Mobile App: Jason Stafford’s *Learning Networking*: “The Physical”
    and “The Data Link Layer”**

    Link: Jason Stafford’s *Learning Networking*: [“The Physical
    Layer”](https://itunes.apple.com/us/app/learning-networking/id571370723?mt=8)
    and [“The Data Link
    Layer”](https://itunes.apple.com/us/app/learning-networking/id571370723?mt=8)
    (iOS App)

    Instructions: If you have chosen to download this app, watch videos
    2 and 3, “The Physical Layer” and “The Data Link Layer.” Note that
    no quiz or exam questions will be derived from material within, but
    it is still a useful supplementary resource.

    Terms of Use: Please respect the copyright and terms of use
    displayed on the webpage above.

**6.3 Technologies** <span id="6.3"></span> 
-   **Reading: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*: “Chapter
    6, Section 6.3: Datalink layer technologies”**
    Link: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*:
    [“Chapter 6, Section 6.3: Datalink Layer
    Technologies”](http://www.saylor.org/site/wp-content/uploads/2012/02/Computer-Networking-Principles-Bonaventure-1-30-31-OTC1.pdf) (PDF)  
        
     Instructions: Read the beginning of section 6.3, “Datalink Layer
    Technologies,” on page 229. Stop at section 6.3.1 “The
    Point-to-Point Protocol,” which you will read below.  
        
     It would take a library full of volumes to discuss all of the
    technologies used on the Internet. Your textbook has condensed this
    information into a discussion of six major categories. The following
    subunits address the datalink services of these technologies.  
        
     Reading this textbook section and taking notes should take
    approximately 30 minutes.  
      
     Terms of Use: *Computer Networking: Principles, Protocols, and
    Practice* was written by Olivier Bonaventure and relicensed under a
    [Creative Commons Attribution 3.0 Unported
    License](http://creativecommons.org/licenses/by/3.0/) as part of the
    Saylor Foundation’s Open Textbook Challenge.

**6.3.1 Point-to-Point Protocol** <span id="6.3.1"></span> 
-   **Reading: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*: “Chapter
    6, Section 6.3.1: The Point-to-Point Protocol”**
    Link: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and
    Practice*: [“Chapter 6, Section 6.3.1: The Point-to-Point
    Protocol”](http://www.saylor.org/site/wp-content/uploads/2012/02/Computer-Networking-Principles-Bonaventure-1-30-31-OTC1.pdf) (PDF)  
      
     Instructions: Read section 6.3.1, “The Point-to-Point Protocol,” on
    pages 228–230.  
        
     This section explores how the point-to-point protocols are handled
    in the datalink layer. What are the three members combined in the
    point-to-point protocol?  
        
     Reading this textbook section and taking notes should take
    approximately 1 hour.  
        
     Terms of Use: *Computer Networking: Principles, Protocols, and
    Practice* was written by Olivier Bonaventure and relicensed under a
    [Creative Commons Attribution 3.0 Unported
    License](http://creativecommons.org/licenses/by/3.0/) as part of the
    Saylor Foundation’s Open Textbook Challenge.

**6.3.2 Ethernet** <span id="6.3.2"></span> 
-   **Reading: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*: “Chapter
    6, Section 6.3.2: Ethernet”**
    Link: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*:
    [“Chapter 6, Section 6.3.2:
    Ethernet”](http://www.saylor.org/site/wp-content/uploads/2012/02/Computer-Networking-Principles-Bonaventure-1-30-31-OTC1.pdf) (PDF)  
        
     Instructions: Read the beginning of section 6.3.2, “Ethernet,” on
    pages 230–234. Stop at “Ethernet switches,” which you will read
    below. MAC addresses are the datalink services found in an Ethernet
    environment.  
        
     Reading this textbook section and taking notes should take
    approximately 1 hour.  
        
     Terms of Use: *Computer Networking: Principles, Protocols, and
    Practice* was written by Olivier Bonaventure and relicensed under a
    [Creative Commons Attribution 3.0 Unported
    License](http://creativecommons.org/licenses/by/3.0/) as part of the
    Saylor Foundation’s Open Textbook Challenge.

**6.3.2.1 Ethernet Switches** <span id="6.3.2.1"></span> 
-   **Reading: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*: “Chapter
    6, Section 6.3.2: Ethernet Switches”**
    Link: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*:
    [“Chapter 6, Section 6.3.2: Ethernet
    Switches”](file:///C:/Users/Holly/Documents/Saylor/CS402/v) (PDF)  
        
     Instructions: Read “Ethernet Switches” on pages 234–237. Stop at
    “The Spanning Tree Protocol (802.1d),” which you will read below. As
    you read, consider the following questions: What is an Ethernet
    switch? How does it function in the datalink layer? How does it
    utilize Medium Access Control mechanisms?  
        
     Reading this textbook section and taking notes should take
    approximately 1 hour.  
        
     Terms of Use: *Computer Networking: Principles, Protocols, and
    Practice* was written by Olivier Bonaventure and relicensed under a
    [Creative Commons Attribution 3.0 Unported
    License](http://creativecommons.org/licenses/by/3.0/) as part of the
    Saylor Foundation’s Open Textbook Challenge.  
      

**6.3.2.2 The Spanning Tree Protocol (802.1d)** <span
id="6.3.2.2"></span> 
-   **Reading: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*: “Chapter
    6, Section 6.3.2: The Spanning Tree Protocol (802.1d)”**
    Link: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*:
    [“Chapter 6, Section 6.3.2: The Spanning Tree Protocol
    (802.1d)”](http://www.saylor.org/site/wp-content/uploads/2012/02/Computer-Networking-Principles-Bonaventure-1-30-31-OTC1.pdf) (PDF)  
        
     Instructions: Read “The Spanning Tree Protocol (802.1d)” on pages
    237–240. Stop at the “Virtual LANs” section, which you will read
    below. The spanning tree protocol is a distributed standard that is
    used by switches to reduce the network topology to a spanning tree
    by eliminating all cycles. Explore the examples in your textbook to
    see how this technology processes frames in the datalink layer.  
        
     Reading this textbook section and taking notes should take
    approximately 1 hour.  
      
     Terms of Use: *Computer Networking: Principles, Protocols, and
    Practice* was written by Olivier Bonaventure and relicensed under a
    [Creative Commons Attribution 3.0 Unported
    License](http://creativecommons.org/licenses/by/3.0/) as part of the
    Saylor Foundation’s Open Textbook Challenge

**6.3.2.3 Virtual LANs** <span id="6.3.2.3"></span> 
-   **Reading: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*: “Chapter
    6, Section 6.3.2: Virtual LANs”**
    Link: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*:
    [“Chapter 6, Section 6.3.2: Virtual
    LANs”](http://www.saylor.org/site/wp-content/uploads/2012/02/Computer-Networking-Principles-Bonaventure-1-30-31-OTC1.pdf) (PDF)  
        
     Instructions: Read “Virtual LANs” on pages 2401–241. Stop at
    section 6.3.3 “802.11 wireless networks,” which you will read below.
    As you read, consider the following question: How do Ethernet
    switches create virtual LANs?   
        
     Reading this textbook section and taking notes should take
    approximately 1 hour.  
        
     Terms of Use: *Computer Networking: Principles, Protocols, and
    Practice* was written by Olivier Bonaventure and relicensed under a
    [Creative Commons Attribution 3.0 Unported
    License](http://creativecommons.org/licenses/by/3.0/) as part of the
    Saylor Foundation’s Open Textbook

**6.3.3 802.11 Wireless Networks** <span id="6.3.3"></span> 
-   **Reading: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*: “Chapter
    6, Section 6.3.3: 802.11 Wireless Networks”**
    Link: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*:
    [“Chapter 6, Section 6.3.3: 802.11 Wireless
    Networks”](http://www.saylor.org/site/wp-content/uploads/2012/02/Computer-Networking-Principles-Bonaventure-1-30-31-OTC1.pdf) (PDF)  
        
     Instructions: Read section 6.3.3, “802.11 Wireless Networks,” on
    pages 241–246. Wi-Fi is a very popular wireless networking
    technology. There are hundreds of millions of Wi-Fi devices,
    resulting in multiple wireless networking standards that use
    different frequency ranges and different physical layers. Explore
    the wireless revolution into the datalink layer in this section.  
        
     Reading this textbook section and taking notes should take
    approximately 1 hour.  
      
     Terms of Use: *Computer Networking: Principles, Protocols, and
    Practice* was written by Olivier Bonaventure and relicensed under a
    [Creative Commons Attribution 3.0 Unported
    License](http://creativecommons.org/licenses/by/3.0/) as part of the
    Saylor Foundation’s Open Textbook Challenge.

-   **Mobile App: WAGmob’s *Learn Computer Science, MIS & Networking*:
    “Network Technology” and “Wireless Networking”**
    Link: WAGmob’s [*Learn Computer Science, MIS &
    Networking*](https://itunes.apple.com/us/app/computer-science-mis-in-app/id403644734?mt=8) (iOS
    App) or WAGmob’s *[Networking
    101](https://play.google.com/store/apps/details?id=com.quizmine.androidnetworking&hl=en) *(Android
    App)  
        
     Instructions: If you have chosen to download this app, read the
    “Network Technology” and “Wireless Networking” tutorials. Once you
    have a firm grasp of the material, quiz yourself with the “Wireless
    Networking” flashcards, and take the “Network Technology” quiz.
    Retake the quiz as needed until you fully understand all of the
    concepts. Note that no quiz or exam questions will be derived from
    material within, but they are still useful supplementary
    resources.  
        
     Terms of Use: Please respect the copyright and terms of use
    displayed on the webpage above.

**6.4 Summary and a Review of Hub, Switch, and Network Router** <span
id="6.4"></span> 
-   **Reading: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*: “Chapter
    6, Section 6.4: Summary”**
    Link: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*:
    [“Chapter 6, Section 6.4:
    Summary”](http://www.saylor.org/site/wp-content/uploads/2012/02/Computer-Networking-Principles-Bonaventure-1-30-31-OTC1.pdf) (PDF)  
      
     Instructions: Read section 6.4, “Summary,” on page 246. In chapter
    6, you explored how Local Area Networks pose a problem for
    transporting frames since several devices share the same
    transmission channel. A variety of Medium Access Control algorithms
    have been necessary to regulate the access to the transmission
    channel by reducing collisions: ALOHA, CSMA, CSMA/CD, and CSMA/CA.
    Review the key technologies discussed in this section.  
      
     Reading this textbook section and taking notes should take
    approximately 2 hours.  
        
     Terms of Use: *Computer Networking: Principles, Protocols, and
    Practice* was written by Olivier Bonaventure and relicensed under a
    [Creative Commons Attribution 3.0 Unported
    License](http://creativecommons.org/licenses/by/3.0/) as part of the
    Saylor Foundation’s Open Textbook Challenge.

-   **Web Media: YouTube: Keith Barker’s “Switches, and Routers, and
    Hubs!”**
    Link: YouTube: Keith Barker’s [“Switches, and Routers, and
    Hubs!”](http://www.youtube.com/watch?v=reXS_e3fTAk) (YouTube)  
        
     Instructions: Watch this video to understand the functions of hub,
    switch, and network routers.  
        
     Watching this video and pausing to take notes should take less than
    15 minutes.  
        
     Terms of Use: Please respect the copyright and terms of use
    displayed on the webpage above.

-   **Mobile App: WAGmob’s *Learn Computer Science, MIS & Networking*:
    “Network Hardware” and “Switching Techniques”**
    Link: WAGmob’s [*Learn Computer Science, MIS &
    Networking*](https://itunes.apple.com/us/app/computer-science-mis-in-app/id403644734?mt=8) (iOS
    App) or WAGmob’s *[Networking
    101](https://play.google.com/store/apps/details?id=com.quizmine.androidnetworking&hl=en) *(Android
    App)  
        

    Instructions: If you have chosen to download this app, read the
    “Network Hardware” and “Switching Techniques” tutorials. Once you
    have a firm grasp of the material, quiz yourself with the “Network
    Hardware” flashcards, and take the “Network Hardware” quiz. Retake
    the quiz as needed until you fully understand all of the concepts.
    Note that no quiz or exam questions will be derived from material
    within, but they are still useful supplementary resources.  
        
     Terms of Use: Please respect the copyright and terms of use
    displayed on the webpage above.

-   **Mobile App: Jason Stafford’s *Learning Networking*: “Ethernet
    Switch Configuration”**

    Link: Jason Stafford’s *Learning Networking*: [“Ethernet Switch
    Configuration”](https://itunes.apple.com/us/app/learning-networking/id571370723?mt=8) (iOS
    App)

    Instructions: If you have chosen to download this app, watch videos
    10 and 12 on Ethernet Switch Configuration. As you watch the videos,
    try to learn the techniques to configure the speed, duplex, and MDIX
    for switch administration, and to learn the techniques for creating
    a virtual LAN (VLAN) via switch administration. Note that no quiz or
    exam questions will be derived from material within, but it is still
    a useful supplementary resource.

    Terms of Use: Please respect the copyright and terms of use
    displayed on the webpage above.

**6.5 Practice Exercises** <span id="6.5"></span> 
-   **Activity: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*: “Chapter
    6, Section 6.5: Exercises”**
    Link: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*:
    [“Chapter 6, Section 6.5:
    Exercises”](http://www.saylor.org/site/wp-content/uploads/2012/02/Computer-Networking-Principles-Bonaventure-1-30-31-OTC1.pdf) (PDF)  
        
     Instructions: Read section 6.5, “Exercises,” through the end of
    chapter 6, on pages 246–247. These exercises expand the key
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

-   **Mobile App: Jason Stafford’s *Learning Networking*: “Exams”**
    Link: Jason Stafford’s *Learning Networking*:
    [“Exams”](https://itunes.apple.com/us/app/learning-networking/id571370723?mt=8) (iOS
    App)  
        
     Instructions: If you have chosen to download this app, work through
    the “Practice Exam” questions at your own pace. Once you have a firm
    grasp of the material, take the “Virtual Exam.” Retake the exam as
    needed until you fully understand all of the concepts. Note that no
    quiz or exam questions will be derived from material within, but it
    is still a useful supplementary resource.  
      
     Terms of Use: Please respect the copyright and terms of use
    displayed on the webpage above.

-   **Mobile App: *Network Scanner Apps***
    Links:   
     - 10base-t Interactive’s *[IP Network Scanner
    Lite](https://itunes.apple.com/us/app/ip-network-scanner-lite/id335517828?l=es&mt=8) *(iOS
    App);  
     - Overlook’s *[Fing - Network
    Scanner](https://itunes.apple.com/us/app/fing-network-scanner/id430921107?mt=8) *(iOS
    App); or  
     - Overlook’s *[Fing - Network
    Tools](https://play.google.com/store/apps/details?id=com.overlook.android.fing&feature=search_result#?t=W251bGwsMSwxLDEsImNvbS5vdmVybG9vay5hbmRyb2lkLmZpbmciXQ..) *(Android
    App)  
        
     Instructions: These apps correspond to the following activity.Spend
    some time reviewing each of these apps, but any of them will work
    for this activity. Note that no quiz or exam questions will be
    derived from material within, but they are still useful
    supplementary resources.  
        
     Terms of Use: Please respect the copyright and terms of use
    displayed on the webpage above.

-   **Activity: The Saylor Foundation’s “Local Area Network Service Scan
    and Wake on LAN”**
    Link: The Saylor Foundation’s [“Local Area Network Service Scan and
    Wake on
    LAN”](http://www.saylor.org/site/wp-content/uploads/2013/03/CS402-6.5-LocalAreaNetworkServiceScanandWakeonLAN-FINAL.pdf)
    (PDF)  
      
     Instructions: Follow the steps detailed in this document in order
    to control your computer from a mobile device

**Unit 6 Assessment** <span id="6.6"></span> 
-   **Assessment: The Saylor Foundation’s “Unit 6 Assessment”**
    Link: The Saylor Foundation’s [“Unit 6
    Assessment”](http://school.saylor.org/mod/quiz/view.php?id=1288) (HTML)  
        
     Instructions: Complete this assessment, which will test your
    understanding of the material in this unit. The correct answers will
    be displayed after you click “Submit.”  
      
     *Note: You must be logged into your Saylor Foundation School
    account in order to access this exam. If you do not yet have an
    account, you will be able to create one, free of charge, after
    clicking the link.*


