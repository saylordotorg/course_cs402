---
layout: default
title: "CS402: Computer Communications and Networks"
course_description: "A detailed introduction to the basic hardware, software, and architectural components of computer communications in local area networks. Focuses on understanding the basics of computer networks, switching, routing, protocols, and security."
next: ../Unit04
previous: ../Unit02
---
**Unit 3: The Application Layer** <span id="3"></span> 
*In this unit, we will examine the application layer of the TCP/IP
stack. The application layer is where all network processes and
applications run. We will explore five of this layer’s prominent
applications: the Domain Name System (DNS), e-mail protocols, the World
Wide Web’s Hypertext Transfer Protocol (HTTP), Simple Network Management
Protocol (SNMP), and Secure Shell (SSH). Finally, we will discuss socket
programming and how it can be used to develop network applications.*

**Unit 3 Time Advisory**  
Completing this unit should take approximately 20 hours.  
  
 ☐    Subunit 3.1: 5 hours  
  
 ☐    Subunit 3.2: 6.5 hours  
  
 ☐    Subunit 3.3: 4 hours  
  
 ☐    Subunit 3.4: 0.5 hours  
  
 ☐    Subunit 3.5: 4 hours

**Unit3 Learning Outcomes**  
Upon successful completion of this unit, you will be able to:
-   classify network application layer protocols;
-   describe the DNS application;
-   compare and contrast SMTP with POP3 protocols;
-   compare and contrast the Peer-to-Peer model with the Client-Server
    model;
-   describe the HTTP protocol;
-   describe SNMP protocols;
-   describe SSH based applications; and
-   define socket programming and explain its role in application
    processing.

**3.1 Principles** <span id="3.1"></span> 
*Note: In this subunit we explore the application layer of the TCP/IP
stack. Follow the links provided to expand your understanding of how
emerging applications like social networking and database query are
processed in this layer.*

-   **Reading: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*: “Chapter
    3, Section 3.1 Introduction: Principles”**
    Link: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*:
    [“Chapter 3, Section 3.1 Introduction:
    Principles”](http://www.saylor.org/site/wp-content/uploads/2012/02/Computer-Networking-Principles-Bonaventure-1-30-31-OTC1.pdf) (PDF)  
        
     Instructions: Read the introduction to Section 3.1, “Principles,”
    on pages 27–30. Stop at Section 3.1.1.  
        
     As you read, consider these questions: What is the client-server
    model? What is the function of the client? Where does the server
    reside?  
        
     *Note: On page 28, the textbook lists the binary code of A as “A :
    1000011b.” This is incorrect. The binary code for A should be: “A :
    1000001b.”*  
        
     Reading this article and taking notes should take approximately 30
    minutes.  
        
     Terms of Use: *Computer Networking: Principles, Protocols, and
    Practice* was written by Olivier Bonaventure and relicensed under a
    Creative Commons Attribution 3.0 License as part of the Saylor
    Foundation’s Open Textbook Challenge.

-   **Reading: Wikipedia: “Endianness”**
    Link: Wikipedia:
    [“Endianness”](http://resources.saylor.org.s3.amazonaws.com/CS/CS402/CS402-3.1-Endianess-BY-SA_files/CS402-3.1-Endianess-BY-SA.html) (HTML)  
        
     Instructions: Read this article. As you read, note that most
    languages/platforms provide libraries that convert from network
    order to host order in the event that the host does not agree.  
        
     Reading this article and taking notes should take approximately 30
    minutes.  
        
     Terms of Use: Please respect the copyright and terms of use
    displayed on the webpage above.

**3.1.1 Peer-to-Peer Model** <span id="3.1.1"></span> 
-   **Reading: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*: “Chapter
    3, Section 3.1.1: Peer-to-Peer Model”**
    Link: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*:
    [“Chapter 3, Section 3.1.1: Peer-to Peer
    Model”](http://www.saylor.org/site/wp-content/uploads/2012/02/Computer-Networking-Principles-Bonaventure-1-30-31-OTC1.pdf) (PDF)  
        
     Instructions: Read Section 3.1.1, “The Peer-to-Peer Model,” on page
    30. This section introduces the peer-to-peer model, which will be
    discussed further.  
        
     Reading this article and taking notes should take approximately 30
    minutes.  

     

    Terms of Use: Please respect the copyright and terms of use
    displayed on the webpages above. *Computer Networking: Principles,
    Protocols, and Practice *was written by Olivier Bonaventure and
    relicensed under a Creative Commons Attribution 3.0 License as part
    of the Saylor Foundation’s Open Textbook Challenge.

-   **Reading: Massachussets Institute of Technology OpenCourseWare:
    Prof. Hari Balakrishnan’s *Computer Networks*: “Overlay Routing in
    the Internet”**
    Link: Massachussets Institute of Technology OpenCourseWare: Prof.
    Hari Balakrishnan’s *Computer Networks*: [“Lecture 17: Overlay
    Routing in the
    Internet”](http://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-829-computer-networks-fall-2002/lecture-notes/L17overlay.pdf) (PDF)  
      
     Instructions: As you read, try to answer the following question:
    how does the peer-to-peer model change or improve the client-server
    model discussed in the previous section?  
      
     Reading this article and taking notes should take approximately 2
    hours and 30 minutes.  
      
     Terms of Use: Please respect the copyright and terms of use
    displayed on the webpage above.

**3.1.2 Transport Services** <span id="3.1.2"></span> 
-   **Reading: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*: “Chapter
    3, Section 3.1.2: The transport services”**
    Link: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*:
    [“Chapter 3, Section 3.1.2: The transport
    services”](http://www.saylor.org/site/wp-content/uploads/2012/02/Computer-Networking-Principles-Bonaventure-1-30-31-OTC1.pdf) (PDF)  
        
     Instructions: Read Section 3.1.2, “The Transport Services,” on
    pages 30-31.  
        
     This section discusses how networked applications are built on top
    of the transport service. There are two main types of transport
    services: connectionless and connection-oriented. What are the
    similarities and differences between the two types of services?  
        
     Reading this article and taking notes should take approximately 1
    hour.  
        
     Terms of Use: *Computer Networking: Principles, Protocols, and
    Practice* was written by Olivier Bonaventure and relicensed under a
    Creative Commons Attribution 3.0 License as part of the Saylor
    Foundation’s Open Textbook Challenge.

**3.2 Application-Level Protocols** <span id="3.2"></span> 
*Note: There are a number of application protocols available, but only
three have been included in your textbook: Domain Name System (DNS),
Electronic Mail (SMTP and POP3), and HyperText Transfer Protocol (HTTP).
The DNS protocol allows you to easily reference resources outside of
your network. E-mail protocols allow you to reach out and communicate
with friends and family, and HTTP is the popular protocol for accessing
webpages on other systems.*  
    
 *In addition to the three application protocols covered in your
textbook you will also take a look at the SNMP and SSH protocols. These
two protocols are being used more and more in Internet applications. In
particular, the SNMP protocol allows the administrators to manage a
large network in a more efficient way, and the SSH protocol allows us to
design virtual private networks over public networks.  
    
 As you read through these subunits, think about your own social
networking activities. How does each of these protocols allow you to
communicate using a variety of media, equipment, and file
types/software?*

-   **Mobile App: WAGmob’s *Learn Computer Science, MIS & Networking* or
    WAGmob’s *Networking 101***

    Link: WAGmob’s *[Learn Computer Science, MIS &
    Networking](https://itunes.apple.com/us/app/computer-science-mis-in-app/id403644734?mt=8)* (iOS
    App) or WAGmob’s *[Networking
    101](https://play.google.com/store/apps/details?id=com.quizmine.androidnetworking&hl=en)*
    (Android App)

    Instructions: If you have chosen to download this app, read the
    “Communication Protocols” tutorial. Once you have a firm grasp of
    the material, quiz yourself with the “Communication Protocols”
    flashcards, and take the “Communication Protocols” quiz. Retake the
    quiz as needed until you fully understand all of the concepts. Note
    that no quiz or exam questions will be derived from material within,
    but they are still useful supplementary resources.

    Terms of Use: Please respect the copyright and terms of use
    displayed on the webpage above.

**3.2.1 Domain Name System (DNS)** <span id="3.2.1"></span> 
-   **Reading: University of Washington: “CSE 341: Grammars, Language
    Specification, and Interpreters”**
    Link: University of Washington: Keunwoo Lee’s [“CSE 341: Grammars,
    Language Specification, and
    Interpreters”](http://www.cs.washington.edu/education/courses/cse341/04wi/lectures/11-interpreters.html) (HTML)  
        
     Instructions: In order to understand the materials in Chapter 3 of
    the textbook, you need to learn BNF notation. Read this webpage to
    learn BNF notation.  
      
     Reading this article and taking notes should take approximately 1
    hour.  
      
     Terms of Use: Please respect the copyright and terms of use
    displayed on the webpage above.

-   **Reading: Université Catholique de Louvain: Olivier Bonaventure’s
    Computer Networking: Principles, Protocols, and Practice: “Chapter
    3, Section 3.2.1: The Domain Name System”**
    Link: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*:
    [“Chapter 3, Section 3.2.1:The Domain Name
    System”](http://www.saylor.org/site/wp-content/uploads/2012/02/Computer-Networking-Principles-Bonaventure-1-30-31-OTC1.pdf) (PDF)  
      
     Instructions: Read section 3.2.1, “The Domain Name System,” on
    pages 32–37.  
        
     In order to access a website, you need to know the website’s IP
    address. IP addresses can be somewhat cumbersome and difficult to
    remember, since they are simply four numbers separated by periods
    (e.g., 120.755.3.9). The Domain Name System (DNS) is the application
    that has solved this problem by allowing us to use “human readable”
    names for websites. What is the domain name for your home page on
    your work, school, or home LAN? What is the IP address for each one?
    Which would you rather use – the IP address or the domain name?  
        
     Reading this textbook section and taking notes should take
    approximately 1 hour.  
        
     Terms of Use: *Computer Networking: Principles, Protocols, and
    Practice* was written by Olivier Bonaventure and relicensed under a
    [Creative Commons Attribution 3.0 Unported
    License](http://creativecommons.org/licenses/by/3.0/)as part of the
    Saylor Foundation’s Open Textbook Challenge.

-   **Reading: Zytrax.com’s “DNS Concepts”**
    Link: Zytrax.com’s [“DNS
    Concepts”](http://www.zytrax.com/books/dns/ch2/) (HTML)  
      
     Instructions: Read this article. As you read, pay special attention
    to the DNS recursive and iterative query concepts.  
      
     Reading this article and taking notes should take approximately 1
    hour.  
      
     Terms of Use: Please respect the copyright and terms of use
    displayed on the webpage above.

-   **Mobile App: WAGmob’s *Learn Computer Science, MIS & Networking* or
    WAGmob’s *Networking 101***

    Link: WAGmob’s *[Learn Computer Science, MIS &
    Networking](https://itunes.apple.com/us/app/computer-science-mis-in-app/id403644734?mt=8)* (iOS
    App) or WAGmob’s *[Networking
    101](https://play.google.com/store/apps/details?id=com.quizmine.androidnetworking&hl=en)*
    (Android App)

    Instructions: If you have chosen to download this app, read the
    “Internet Basics” tutorial.

    Terms of Use: Please respect the copyright and terms of use
    displayed on the webpage above.

**3.2.2 Electronic Mail (SMTP and POP3)** <span id="3.2.2"></span> 
-   **Reading: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*: “Chapter
    3, Section 3.2.2: Electronic mail”**
    Link: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*:
    [“Chapter 3, Section 3.2.2: Electronic
    mail”](http://www.saylor.org/site/wp-content/uploads/2012/02/Computer-Networking-Principles-Bonaventure-1-30-31-OTC1.pdf) (PDF)  
      
     Instructions: Read Section 3.2.2, “Electronic mail,” on pages
    37-46. In this section you will look at the e-mail application and
    explore two of the more popular protocols: SMTP and POP3. How does
    e-mail work? How long does it take for a message to reach its
    destination? Then what happens?  

     

    Reading this textbook section and taking notes should take
    approximately 1 hour.  
        
     Terms of Use: *Computer Networking: Principles, Protocols, and
    Practice* was written by Olivier Bonaventure and relicensed under a
    Creative Commons Attribution 3.0 License as part of the Saylor
    Foundation’s Open Textbook Challenge.

**3.2.3 HyperText Transfer Protocol (HTTP)** <span id="3.2.3"></span> 
-   **Reading: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*: “Chapter
    3, Section 3.2.3: HyperText Transfer Protocol”**
    Link: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*:
    [“Chapter 3, Section 3.2.3: HyperText Transfer
    Protocol”](http://www.saylor.org/site/wp-content/uploads/2012/02/Computer-Networking-Principles-Bonaventure-1-30-31-OTC1.pdf) (PDF)  
        
     Instructions: Read Section 3.2.3, “HyperText Transfer Protocol,” on
    pages 46-55. HTTP is a text-based protocol, in which the client
    sends a request and the server returns a response. In this section
    link across the World Wide Web via your textbook to see how this is
    accomplished.  
        
     As you read, consider the following questions: How did the telnet
    and FTP protocols lead to HTTP? What is HTML?  
      
     Reading this textbook section and taking notes should take
    approximately 1 hour.  
      
     Terms of Use: *Computer Networking: Principles, Protocols, and
    Practice* was written by Olivier Bonaventure and relicensed under a
    Creative Commons Attribution 3.0 License as part of the Saylor
    Foundation’s Open Textbook Challenge.

**3.2.4 Simple Network Management Protocol (SNMP)** <span
id="3.2.4"></span> 
-   **Reading: Wikipedia: “Simple Network Management Protocol”**
    Link: Wikipedia: [“Simple Network Management
    Protocol”](http://resources.saylor.org.s3.amazonaws.com/CS/CS402/CS402-3.2.4-SimpleNetworkingTool-BY-SA_files/CS402-3.2.4-SimpleNetworkingTool-BY-SA.html) (HTML)  
      
     Instructions: Read this article. As you read, pay special attention
    to the definitions of *managed devices*, *agent*, and *network
    management system* *(NMS)*. At the same time, try to explain what
    kind of message flows are defined in NMS.  
        
     Reading this article and taking notes should take approximately 30
    minutes.  
        
     Terms of Use: Please respect the copyright and terms of use
    displayed on the webpage above.

-   **Mobile App: WAGmob’s *Learn Computer Science, MIS & Networking* or
    WAGmob’s *Networking 101***

    Link: WAGmob’s *[Learn Computer Science, MIS &
    Networking](https://itunes.apple.com/us/app/computer-science-mis-in-app/id403644734?mt=8)* (iOS
    App) or WAGmob’s *[Networking
    101](https://play.google.com/store/apps/details?id=com.quizmine.androidnetworking&hl=en)*
    (Android App)

    Instructions: If you have chosen to download this app, read the
    “Network Management” tutorial. Once you have a firm grasp of the
    material, quiz yourself with the “Network Management” flashcards.
    Note that no quiz or exam questions will be derived from material
    within, but they are still useful supplementary resources.

    Terms of Use: Please respect the copyright and terms of use
    displayed on the webpage above.

**3.2.5 The Secure Shell (SSH) Protocol Architecture** <span
id="3.2.5"></span> 
-   **Reading: Wikibooks.com: “OpenSSH/SSH Protocols”**
    Link: Wikibooks.com: [“OpenSSH/SSH
    Protocols”](http://resources.saylor.org.s3.amazonaws.com/CS/CS402/CS402-3.2.5-OpenSSH-BY-SA_files/CS402-3.2.5-OpenSSH-BY-SA.html) (HTML)  
      
     Instructions: Read this article. As you read, pay attention to how
    SSH protocol is defined and the difference between FTP and SSH-based
    Secure FTP.  
        
     Reading this article and taking notes should take approximately 1
    hour.  
        
     Terms of Use: Please respect the copyright and terms of use
    displayed on the webpage above.

**3.3 Writing Simple Networked Applications** <span id="3.3"></span> 
-   **Reading: Doug Hellmann: “SocketServer – Creating network
    servers”**
    Link: Doug Hellmann: [“SocketServer – Creating Network
    Servers”](http://www.doughellmann.com/PyMOTW/SocketServer/) (HTML)  
        
     Instructions: Read this tutorial on how to make a simple network
    application program with Python socket. It is recommended that you
    download and install Python from the Python official website
    (<http://www.python.org/>) and run the sample program.  
        
     Reading this article and taking notes should take approximately 4
    hours.  
        
     Terms of Use: Please respect the copyright and terms of use
    displayed on the webpage above.

**3.4 Summary** <span id="3.4"></span> 
-   **Reading: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*: “Chapter
    3, Section 3.4: Summary”**
    Link: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*:
    [“Chapter 3, Section 3.4:
    Summary”](http://www.saylor.org/site/wp-content/uploads/2012/02/Computer-Networking-Principles-Bonaventure-1-30-31-OTC1.pdf) (PDF)  
      
     Instructions: Read Section 3.4, “Summary,” on page 61.  
      
     This unit discusses the evolution of the Internet from IPv4 to IPv6
    in application processing. Why was the change from 32-bit IPv4
    to128-bit IPv6 critical for the application layer?  
      
     Reading this article and taking notes should take approximately 30
    minutes.  
      
     Terms of Use: *Computer Networking: Principles, Protocols, and
    Practice* was written by Olivier Bonaventure and relicensed under a
    Creative Commons Attribution 3.0 License as part of the Saylor
    Foundation’s Open Textbook Challenge.

-   **Mobile App: Jason Stafford’s *Learning Networking*: “The Upper
    Layers”**
    Link: Jason Stafford’s *Learning Networking*: [“The Upper
    Layers”](https://itunes.apple.com/us/app/learning-networking/id571370723?mt=8) (iOS
    App)  
        
     Instructions: If you have an iOS device and have chosen to download
    this app, watch “The Upper Layers” video, “\#6-ICND1-Video 6-Layers
    5-7-The Upper Layers-iPad HD.” As you watch the video, try to
    understand how each layer of the OSI model is related to the
    immediate neighbor layer. For example, how the NETBIOS messages are
    assembled in the other layers. Note that no quiz or exam questions
    will be derived from material within, but it is still a useful
    supplementary resource.  
      
     Watching this video should take approximately 15 minutes.  
        
     Terms of Use: Please respect the copyright and terms of use
    displayed on the webpage above.

**3.5 Practice Exercises** <span id="3.5"></span> 
-   **Activity: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*: “Chapter
    3, Section 3.5: Exercises”**
    Link: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*:
    [“Chapter 3, Section 3.5:
    Exercises”](http://www.saylor.org/site/wp-content/uploads/2012/02/Computer-Networking-Principles-Bonaventure-1-30-31-OTC1.pdf) (PDF)  
        
     Instructions: Read from Section 3.5, “Exercises,” to the end of
    Chapter 3, on pages 61-65. These exercises further expand the key
    principles in this chapter. If you are a computer professional, you
    will enjoy the challenges and higher-level discussions in this
    section. For the novice, just wander through the presentations and
    spend more time on the topics that are meaningful to you.  
        
     It will take a significant amount of time for you to finish these
    exercises. We recommend that you schedule 4 hours and attempt a few
    challenging exercises.  
        
     Terms of Use: *Computer Networking: Principles, Protocols, and
    Practice* was written by Olivier Bonaventure and relicensed under a
    Creative Commons Attribution 3.0 License as part of the Saylor
    Foundation’s Open Textbook Challenge.

-   **Mobile App: Remote Desktop Apps**
    Links:  
      
     - Phase Five Systems’s *[Jump Desktop (Remote Desktop) - RDP /
    VNC](https://itunes.apple.com/us/app/jump-desktop-remote-desktop/id364876095?mt=8) *(iOS
    App)  
     - Software Ltd’s *[2X Client RDP/Remote
    Desktop](https://play.google.com/store/apps/details?id=com.tux.client&feature=search_result#?t=W251bGwsMSwxLDEsImNvbS50dXguY2xpZW50Il0.) *(Android
    App)  
     - Kołakowski Damian’s *[Remote
    Desktop](https://play.google.com/store/apps/details?id=pl.androiddev.mobiletab&feature=search_result#?t=W251bGwsMSwyLDEsInBsLmFuZHJvaWRkZXYubW9iaWxldGFiIl0.) *(Android
    App)  
     - Xtralogic Inc.’s *[Remote Desktop
    Client](https://play.google.com/store/apps/details?id=com.xtralogic.android.rdpclient&hl=en) *(Android
    App)  
     <span id="cke_bm_534E" style="display: none;"> </span><span
    id="cke_bm_533E" style="display: none;"> </span>  
     Instructions: These optional apps correspond to the following
    activity. There are costs associated with two of these apps while
    the “2X Client RDP/Remote Desktop” app and the “Remote Desktop”app
    are free. Spend some time reviewing each of these apps, but any of
    them will work for this activity. Note that no quiz or exam
    questions will be derived from material within, but they are still
    useful supplementary resources.  
        
     Terms of Use: Please respect the copyright and terms of use
    displayed on the webpages above.

-   **Activity: The Saylor Foundation’s “Enabling Remote Desktops”**
    Link: The Saylor Foundation’s [“Enabling Remote
    Desktops”](http://www.saylor.org/site/wp-content/uploads/2013/03/CS402-3.5-EnablingRemoteDesktops-FINAL.pdf)
    (PDF)  
        
     Instructions: Click on the link above and follow the steps detailed
    in order to control your computer from a mobile device.

-   **Mobile App: Phase Five Systems’s *Jump Desktop (Remote Desktop)* -
    RDP / VNC or androidVNC team + antlersoft’s *android-vnc-viewer***
    Link: Phase Five Systems’s *[Jump Desktop (Remote Desktop) - RDP /
    VNC](https://itunes.apple.com/us/app/jump-desktop-remote-desktop/id364876095?mt=8) *(iOS
    App) or androidVNC team + antlersoft’s
    *[android-vnc-viewer](https://play.google.com/store/apps/details?id=android.androidVNC&feature=search_result#?t=W251bGwsMSwxLDEsImFuZHJvaWQuYW5kcm9pZFZOQyJd) *(Android
    App)  
      
     Instructions: These optional apps correspond to the following
    activity. If you chose to download the iOS app in the previous
    activity, you can use that same app here, or you can download the
    free Android app.  
      
     Terms of Use: Please respect the copyright and terms of use
    displayed on the webpage above.

-   **Activity: The Saylor Foundation’s “Virtual Network Computing
    (VNC)”**
    Link: The Saylor Foundation’s [“Virtual Network Computing
    (VNC)”](http://www.saylor.org/site/wp-content/uploads/2013/03/CS402-3.5-VirtualNetworkComputing-FINAL.pdf)
    (PDF)  
      
     Instructions: Follow the steps detailed in this document in order
    to control your computer from a mobile device via Virtual Network
    Computing. Even if you choose not to download the above apps,
    reading this PDF is still valuable as it provides an explanation of
    the difference between RDP and VNC.

**Unit 3 Assessment** <span id="3.6"></span> 
-   **Assessment: The Saylor Foundation’s “Unit 3 Assessment”**
    Link: The Saylor Foundation’s [“Unit 3
    Assessment”](http://school.saylor.org/mod/quiz/view.php?id=1285) (HTML)  
        
     Instructions: Complete this assessment, which will test your
    understanding of the material in this unit. The correct answers will
    be displayed after you click “Submit.”  
      
     *Note: You must be logged into your Saylor Foundation School
    account in order to access this exam. If you do not yet have an
    account, you will be able to create one, free of charge, after
    clicking the link.*


