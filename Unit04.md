**Unit 4: The Transport Layer (TCP/UDP)** <span id="4"></span> 
*When we talk about networks, we are talking about data transport. The
TCP/IP stack provides a TCP/UDP layer that handles the data transport
between machines across networks. In this unit, you will learn the TCP
and UDP protocols by examining the structure of TCP and UDP segments and
identifying how this layer serves as the application layer in the TCP/IP
stack.  
     
 *Each application relies on the transport layer that is described in
this unit. It is a key layer in today’s networks as it contains all the
mechanisms necessary to provide a reliable delivery of data over any
unreliable network. First, we will develop a simple reliable transport
layer protocol. Then, your textbook links you through the details of the
TCP and UDP protocols used in TCP/IP networks. We will also study Stream
Control Transmission Protocol (SCTP) and Real Time Transport Protocol
(RTP), which are not covered by the textbook. These protocols are the
fundamental protocols for modern multimedia applications over the
Internet.**

**Unit 4 Time Advisory**  
Completing this unit should take approximately 18 hours.  
  
 ☐    Subunit 4.1: 4 hours  
  
 ☐    Subunit 4.2: 1 hours  
  
 ☐    Subunit 4.3: 8.5 hours  
  
 ☐    Subunit 4.4: 1 hour        
  
 ☐    Subunit 4.5: 1 hour   
  
 ☐    Subunit 4.6: 0.5 hours   
  
 ☐    Subunit 4.7: 2 hours

**Unit4 Learning Outcomes**  
Upon successful completion of this unit, you will be able to:
-   describe and compare the transport protocols TCP and UDP;
-   describe the SCTP and RTP protocols and the applications based on
    these protocols; and
-   compare and contrast TCP activities at the transport layer.

**4.1 The Transport Layer** <span id="4.1"></span> 
-   **Reading: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*: “Chapter
    4: Introduction” and “Chapter 4, Section 4.1: Principles of a
    reliable transport protocol”**
    Link: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*:
    [“Chapter 4:
    Introduction”](http://www.saylor.org/site/wp-content/uploads/2012/02/Computer-Networking-Principles-Bonaventure-1-30-31-OTC1.pdf) (PDF)
    and [“Chapter 4, Section 4.1: Principles of a reliable transport
    protocol”](http://www.saylor.org/site/wp-content/uploads/2012/02/Computer-Networking-Principles-Bonaventure-1-30-31-OTC1.pdf) (PDF)  
        
     Instructions: Read the introduction to Chapter 4 and Section 4.1,
    “Principles of a Reliable Transport Protocol,” on pages 67–87.  
      
     This section discusses the transport protocol in perfect and
    imperfect network service environments in terms of interactions with
    the Service Data Unit (SDU) at various stages of the transmission
    between sending and receiving nodes. What happens to your
    transmission when the environment is perfect? If your data gets
    corrupted by transmission errors, lost, reordered, or duplicated,
    then what happens? Explore the links in your textbook for a better
    understanding of what goes wrong in cyberspace and the mechanisms
    used to repair impacted activity.  
      
     Reading this section and taking notes should take approximately 4
    hours.  
      
     Terms of Use: *Computer Networking: Principles, Protocols, and
    Practice* was written by Olivier Bonaventure and relicensed under a
    Creative Commons Attribution 3.0 License as part of the Saylor
    Foundation’s Open Textbook Challenge.

**4.2 User Datagram Protocol (UDP)** <span id="4.2"></span> 
-   **Reading: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*: “Chapter
    4, Section 4.2: The User Datagram Protocol”**
    Link: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*:
    [“Chapter 4, Section 4.2: The User Datagram
    Protocol”](http://www.saylor.org/site/wp-content/uploads/2012/02/Computer-Networking-Principles-Bonaventure-1-30-31-OTC1.pdf) (PDF)  
      
     Instructions: Read section 4.2, “The User Datagram Protocol,” on
    pages 87–89.  
        
     The UDP allows several applications running on a host to exchange
    SDUs with several other applications running on remote hosts. This
    section explores the checksum process and how the UDP accomplishes
    this multiprocessing.  
      
     Reading this textbook section and taking notes should take
    approximately 1 hour.  
      
     Terms of Use: *Computer Networking: Principles, Protocols, and
    Practice* was written by Olivier Bonaventure and relicensed under a
    [Creative Commons Attribution 3.0 Unported
    License](http://creativecommons.org/licenses/by/3.0/) as part of the
    Saylor Foundation’s Open Textbook Challenge.

**4.3 Transmission Control Protocol (TCP)** <span id="4.3"></span> 
-   **Reading: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*: “Chapter
    4, Section 4.3: The Transmission Control Protocol”**
    Link: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*:
    [“Chapter 4, Section 4.3: The Transmission Control
    Protocol”](http://www.saylor.org/site/wp-content/uploads/2012/02/Computer-Networking-Principles-Bonaventure-1-30-31-OTC1.pdf) (PDF)  
        
     Instructions: Read the introduction to Section 4.3, “The
    Transmission Control Protocol,” on pages 89–90. Stop at Section
    4.3.1.  
        
     Almost every Internet application relies on the TCP in the
    transport layer. In this section you will discover how your favorite
    Internet activity exchanges data around the world. Then in the
    following subunits, you can travel with your data as it streams to
    its destination and back.  
        
     Reading this article and taking notes should take approximately 30
    minutes.  
        
     Terms of Use: *Computer Networking: Principles, Protocols, and
    Practice* was written by Olivier Bonaventure and relicensed under a
    Creative Commons Attribution 3.0 License as part of the Saylor
    Foundation’s Open Textbook Challenge.

**4.3.1 TCP Connection Establishment** <span id="4.3.1"></span> 
-   **Reading: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*: “Chapter
    4, Section 4.3.1: TCP connection establishment”**
    Link: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*:
    [“Chapter 4, Section 4.3.1: TCP connection
    establishment”](http://www.saylor.org/site/wp-content/uploads/2012/02/Computer-Networking-Principles-Bonaventure-1-30-31-OTC1.pdf) (PDF)  
      
     Instructions: Read section 4.3.1, “TCP Connection Establishment,”
    on pages 90–95. As you read, be able to describe the three-way
    handshake used by TCP to establish a connection.  
        
     Reading this textbook section and taking notes should take
    approximately 2 hours.  
      
     Terms of Use: *Computer Networking: Principles, Protocols, and
    Practice* was written by Olivier Bonaventure and relicensed under a
    [Creative Commons Attribution 3.0 Unported
    License](http://creativecommons.org/licenses/by/3.0/) as part of the
    Saylor Foundation’s Open Textbook Challenge.

**4.3.2 TCP Connection Release** <span id="4.3.2"></span> 
-   **Reading: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*: “Chapter
    4, Section 4.3.2: TCP connection release”**
    Link: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*:
    [“Chapter 4, Section 4.3.2: TCP connection
    release”](http://www.saylor.org/site/wp-content/uploads/2012/02/Computer-Networking-Principles-Bonaventure-1-30-31-OTC1.pdf)(PDF)  
        
     Instructions: Read section 4.3.2, “TCP Connection Release,” on
    pages 95–97. As you read, make sure you are able to identify and
    explain the two types of connection release.  
        
     Reading this textbook section and taking notes should take
    approximately 1 hour.  
        
     Terms of Use: *Computer Networking: Principles, Protocols, and
    Practice* was written by Olivier Bonaventure and relicensed under a
    [Creative Commons Attribution 3.0 Unported
    License](http://creativecommons.org/licenses/by/3.0/) as part of the
    Saylor Foundation’s Open Textbook Challenge.

**4.3.3 TCP: A Reliable Data Transport Mechanism** <span
id="4.3.3"></span> 
-   **Reading: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*: “Chapter
    4, Section 4.3.3: TCP reliable data transfer”**
    Link: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*:
    [“Chapter 4, Section 4.3.3: TCP Reliable Data
    Transfer”](http://www.saylor.org/site/wp-content/uploads/2012/02/Computer-Networking-Principles-Bonaventure-1-30-31-OTC1.pdf) (PDF)  
      
     Instructions: Read the beginning of section 4.3.3, “TCP Reliable
    Data Transfer,” on pages 97–98. Stop when you get to “Segment
    Transmission Strategies.”  
        
     This section reviews the three data transfer mechanisms used by
    TCP. What are they, and what is the purpose of each one?  
      
     Reading this textbook section and taking notes should take
    approximately 30 minutes.  
      
     Terms of Use: *Computer Networking: Principles, Protocols, and
    Practice* was written by Olivier Bonaventure and relicensed under a
    [Creative Commons Attribution 3.0 Unported
    License](http://creativecommons.org/licenses/by/3.0/) as part of the
    Saylor Foundation’s Open Textbook Challenge.

**4.3.3.1 TCP Segment Transmission Strategies** <span
id="4.3.3.1"></span> 
-   **Reading: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*: “Chapter
    4, Section 4.3.3: Segment transmission strategies”**
    Link: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*:
    [“Chapter 4, Section 4.3.3: Segment transmission
    strategies”](http://www.saylor.org/site/wp-content/uploads/2012/02/Computer-Networking-Principles-Bonaventure-1-30-31-OTC1.pdf) (PDF)  
        
     Instructions: Read “Segment Transmission Strategies” on pages
    98–99. Stop at the “TCP Windows” section.  
        
     This section of your textbook presents the Nagle Algorithm. What is
    it, and what two strategies does it provide for data transmission?  
        
     Reading this article and taking notes should take approximately 30
    minutes.  
      
     Terms of Use: *Computer Networking: Principles, Protocols, and
    Practice* was written by Olivier Bonaventure and relicensed under a
    Creative Commons Attribution 3.0 License as part of the Saylor
    Foundation’s Open Textbook Challenge.

**4.3.3.2 TCP Windows** <span id="4.3.3.2"></span> 
-   **Reading: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*: “Chapter
    4, Section 4.3.3: TCP Windows”**
    Link: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*:
    [“Chapter 4, Section 4.3.3: TCP
    Windows”](http://www.saylor.org/site/wp-content/uploads/2012/02/Computer-Networking-Principles-Bonaventure-1-30-31-OTC1.pdf) (PDF)  
        
     Instructions: Read “TCP Windows” on pages 99–100. Stop at “TCP’s
    Retransmission Timeout.” As you read, consider the following
    questions: What is a TCP window according to the information
    provided in this section of your textbook? How does a TCP window
    improve processing in the transport layer?  
        
     Reading this textbook section and taking notes should take
    approximately 30 minutes.  
      
     Terms of Use: *Computer Networking: Principles, Protocols, and
    Practice* was written by Olivier Bonaventure and relicensed under a
    [Creative Commons Attribution 3.0 Unported
    License](http://creativecommons.org/licenses/by/3.0/) as part of the
    Saylor Foundation’s Open Textbook Challenge.

**4.3.3.3 TCP Retransmission Timeout** <span id="4.3.3.3"></span> 
-   **Reading: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*: “Chapter
    4, Section 4.3.3: TCP’s retransmission timeout”**
    Link: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*:
    [“Chapter 4, Section 4.3.3: TCP’s Retransmission
    Timeout”](http://www.saylor.org/site/wp-content/uploads/2012/02/Computer-Networking-Principles-Bonaventure-1-30-31-OTC1.pdf) (PDF)  
        
     Instructions: Read section 4.3.3, “TCP’s Retransmission Timeout,”
    on pages 100–102. Stop at “Advanced Retransmission Strategies.”  
        
     Follow the path in this section of your textbook to see how the TCP
    retransmission timeout improves transport performance.  
        
     Reading this textbook section and taking notes should take
    approximately 30 minutes.  
        
     Terms of Use: *Computer Networking: Principles, Protocols, and
    Practice* was written by Olivier Bonaventure and relicensed under a
    [Creative Commons Attribution 3.0 Unported
    License](http://creativecommons.org/licenses/by/3.0/) as part of the
    Saylor Foundation’s Open Textbook Challenge.

**4.3.3.4 Advanced Retransmission Strategies** <span
id="4.3.3.4"></span> 
-   **Reading: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*: “Chapter
    4, Section 4.3.3: Advanced retransmission strategies”**
    Link: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*:
    [“Chapter 4, Section 4.3.3: Advanced retransmission
    strategies”](http://www.saylor.org/site/wp-content/uploads/2012/02/Computer-Networking-Principles-Bonaventure-1-30-31-OTC1.pdf) (PDF)  
        
     Instructions: Read “Advanced Retransmission Strategies” on pages
    102–105. Stop at “TCP Congestion Control.”  
        
     As you read, consider the following questions: What is the
    exponential back off and how does TCP use it? What is the delayed
    acknowledgement strategy in TCP? What is the fast retransmit
    heuristic as utilized by TCP? What is the SACK option?  
        
     Reading this textbook section and taking notes should take
    approximately 1 hour.  
      
     Terms of Use: *Computer Networking: Principles, Protocols, and
    Practice* was written by Olivier Bonaventure and relicensed under a
    [Creative Commons Attribution 3.0 Unported
    License](http://creativecommons.org/licenses/by/3.0/) as part of the
    Saylor Foundation’s Open Textbook Challenge.

**4.3.3.5 TCP Congestion Control** <span id="4.3.3.5"></span> 
-   **Reading: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*: “Chapter
    4, Section 4.3.3: TCP congestion control”**
    Link: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*:
    [“Chapter 4, Section 4.3.3: TCP Congestion
    Control”](http://www.saylor.org/site/wp-content/uploads/2012/02/Computer-Networking-Principles-Bonaventure-1-30-31-OTC1.pdf) (PDF)  
        
     Instructions: Read “TCP Congestion Control” on pages 105–113. Stop
    at the summary.  
        
     TCP’s congestion control is one of its best performance control
    features. This section explains this feature and how it improves
    performance in the transport layer.  
        
     Reading this textbook article and taking notes should take
    approximately 2 hours.  
        
     Terms of Use: *Computer Networking: Principles, Protocols, and
    Practice* was written by Olivier Bonaventure and relicensed under a
    [Creative Commons Attribution 3.0 Unported
    License](http://creativecommons.org/licenses/by/3.0/) as part of the
    Saylor Foundation’s Open Textbook Challenge.

**4.4 Stream Control Transmission Protocol (SCTP)** <span
id="4.4"></span> 
-   **Reading: Wikipedia: “Stream Control Transmission Protocol”**
    Link: Wikipedia: [“Stream Control Transmission
    Protocol”](http://resources.saylor.org.s3.amazonaws.com/CS/CS402/CS402-4.4-StreamControl-BY-SA_files/CS402-4.4-StreamControl-BY-SA.html) (HTML)  
        
     Instructions: Read this article, which explains why we need the new
    SCTP protocol and how it works.  
        
     Reading this article and taking notes should take approximately 1
    hour.  
      
     Terms of Use: Please respect the copyright and terms of use
    displayed on the webpage above.

**4.5 Real Time Transport Protocol (RTP)** <span id="4.5"></span> 
-   **Reading: Isnare.com: “Real-time Transport Protocol”**
    Link: Isnare.com: [“Real-Time Transport
    Protocol”](http://www.isnare.com/wp/Real-time_Transport_Protocol) (HTML)  
        
     Instructions: Read this webpage to understand how RTP is used for
    streaming multimedia data. As you read, pay special attention to how
    RTP protocol is different from TCP protocols and how it is used for
    multimedia data transport.  
        
     Reading this article and taking notes should take approximately 1
    hour.  
      
     Terms of Use: Please respect the copyright and terms of use
    displayed on the webpage above.

**4.6 Summary** <span id="4.6"></span> 
-   **Reading: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*: “Chapter
    4, Section 4.4: Summary”**
    Link: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*:
    [“Chapter 4, Section 4.4:
    Summary”](http://www.saylor.org/site/wp-content/uploads/2012/02/Computer-Networking-Principles-Bonaventure-1-30-31-OTC1.pdf) (PDF)  
        
     Instructions: Read the “Summary” section of chapter 4 on pages
    113–114.  
        
     The transport layer relies on TCP mechanisms to recover from the
    errors of the network layer. The chapter 4 summary reviews the
    strategies at each stage of the transmission.  
        
     Reading this chapter summary and taking notes should take
    approximately 30 minutes.  
        
     Terms of Use: *Computer Networking: Principles, Protocols, and
    Practice* was written by Olivier Bonaventure and relicensed under a
    [Creative Commons Attribution 3.0 Unported
    License](http://creativecommons.org/licenses/by/3.0/) as part of the
    Saylor Foundation’s Open Textbook Challenge.

-   **Mobile App: Jason Stafford’s *Learning Networking*: “The Transport
    Layer”**

    Link: Jason Stafford’s *Learning Networking*: [“The Transport
    Layer”](https://itunes.apple.com/us/app/learning-networking/id571370723?mt=8) (iOS
    App)  
        
     Instructions: If you have chosen to download this app, watch the
    video “The Transport Layer,” “\#5-ICBD1-Video 5-Layer 4-The
    Transport Layer-iPad HD.” As you watch the video, pay attention to
    these three topics: TCP/UDP, Windowing concepts in transport layer,
    and buffering techniques in the transport layer. Note that no quiz
    or exam questions will be derived from material within, but they are
    still useful supplementary resources.  
      

    Terms of Use: Please respect the copyright and terms of use
    displayed on the webpage above.

**4.7 Practice Exercises** <span id="4.7"></span> 
-   **Activity: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*: “Chapter
    4, Section 4.5: Exercises”**
    Link: Université Catholique de Louvain: Olivier Bonaventure’s
    *Computer Networking: Principles, Protocols, and Practice*:
    [“Chapter 4, Section 4.5:
    Exercises”](http://www.saylor.org/site/wp-content/uploads/2012/02/Computer-Networking-Principles-Bonaventure-1-30-31-OTC1.pdf) (PDF)  
        
     Instructions: Read through the practice exercises on pages 113–126.
    These exercises further expand the key principles in this chapter.
    If you are a computer professional, you will enjoy the challenges
    and higher-level discussions in this section. If you are a novice,
    explore the presentations and spend more time on the topics that are
    meaningful to you.  
        
     Reading these exercises and taking notes should take approximately
    2 hours.  
      
     Terms of Use: *Computer Networking: Principles, Protocols, and
    Practice* was written by Olivier Bonaventure and relicensed under a
    [Creative Commons Attribution 3.0 Unported
    License](http://creativecommons.org/licenses/by/3.0/) as part of the
    Saylor Foundation’s Open Textbook Challenge.

-   **Mobile App: m.r.androids’ *Computer Networking***
    Link: m.r.androids’ [*Computer
    Networking*](https://play.google.com/store/apps/details?id=com.mrdroids.networking.quiz&feature=search_result#?t=W251bGwsMSwxLDEsImNvbS5tcmRyb2lkcy5uZXR3b3JraW5nLnF1aXoiXQ..) (Android
    App)  
      
     Instructions: If you choose to use this app, you will first need to
    download it to your Android device. Note that the app is optional as
    it is not available on the iOS platform. No quiz or exam questions
    will be derived from material within, but it is still a useful
    supplementary resource. Once you have downloaded the app, open it
    and select “New Game.” There are five quizzes within – take all of
    them until you understand all the concepts completely.  
      
     Terms of Use: Please respect the copyright and terms of use
    displayed on the webpage above.

**Unit 4 Assessment** <span id="4.8"></span> 
-   **Assessment: The Saylor Foundation’s “Unit 4 Assessment”**
    Link: The Saylor Foundation’s [“Unit 4
    Assessment”](http://school.saylor.org/mod/quiz/view.php?id=1286) (HTML)  
        
     Instructions: Complete this assessment, which will test your
    understanding of the material in this unit. The correct answers will
    be displayed after you click “Submit.”  
      
     *Note: You must be logged into your Saylor Foundation School
    account in order to access this exam. If you do not yet have an
    account, you will be able to create one, free of charge, after
    clicking the link.*


