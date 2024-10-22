# TCP/IP, Wireshark, and RFC Standards Exam (With Answers)

## Section 1: Concepts of TCP/IP (20 Points)

1. **What is the purpose of encapsulation in the TCP/IP model?**  
   **Correct Answer: C**  
   **Explanation:** Encapsulation is the process of adding headers to data as it passes through the layers of the TCP/IP model. Each layer adds its own header, which contains information relevant to that layer.

2. **Which protocol in the transport layer provides reliable data transfer with flow control and error checking?**  
   **Correct Answer: D (TCP)**  
   **Explanation:** TCP (Transmission Control Protocol) is a reliable transport layer protocol that ensures data is delivered in order, with flow control and error checking.

3. **Which of the following RFCs describe the Internet Protocol (IP)?**  
   **Correct Answer: B (RFC 791)**  
   **Explanation:** RFC 791 defines the Internet Protocol (IP), which is a core protocol of the internet layer in the TCP/IP model.

4. **Which of the following best describes the OSI model?**  
   **Correct Answer: C**  
   **Explanation:** The OSI (Open Systems Interconnection) model is a theoretical model used to understand and design communication systems with seven layers.

5. **When analyzing a captured packet, the payload for an HTTP request is located at:**  
   **Correct Answer: A (The application layer)**  
   **Explanation:** HTTP is an application layer protocol, so the payload is found at the application layer in the OSI or TCP/IP model.

6. **True or False:**  
   The OSI model has a layer called the 'Internet Layer,' which does not exist in the TCP/IP model.  
   **Correct Answer: False**  
   **Explanation:** The OSI model does not have an "Internet Layer"; the Internet Layer is part of the TCP/IP model, not the OSI model.

7. **True or False:**  
   The transport layer in the TCP/IP model is responsible for defining the best path for data transmission.  
   **Correct Answer: False**  
   **Explanation:** The transport layer is responsible for reliable data transfer, while path determination is handled by the network layer.

8. **True or False:**  
   Encapsulation occurs in both the OSI and TCP/IP models, and it always starts at the physical layer.  
   **Correct Answer: False**  
   **Explanation:** Encapsulation starts at the application layer in both models and progresses downward to the physical layer.

9. **Explain the process of de-encapsulation and why it is important in network communication. (5 points)**  
   **Correct Answer: (Sample Explanation)**  
   De-encapsulation is the reverse of encapsulation. When data is received, each layer removes its respective header and processes the data. This process is important for ensuring that the data is properly handled by each layer, such as routing by the network layer and delivery to the correct application by the transport layer.

10. **Describe the significance of the 'Three-Way Handshake' in TCP communication. What happens if the process is interrupted? (5 points)**  
    **Correct Answer: (Sample Explanation)**  
    The Three-Way Handshake is used to establish a reliable connection in TCP communication. It involves the exchange of SYN, SYN-ACK, and ACK packets between two hosts. If the process is interrupted, the connection is not established, leading to data transmission failure or retries.

---

## Section 2: Wireshark and Packet Analysis (25 Points)

11. **What is the primary feature that distinguishes Wireshark from Tcpdump?**  
    **Correct Answer: A**  
    **Explanation:** Wireshark provides a graphical user interface (GUI), while Tcpdump is a command-line tool.

12. **In Wireshark, what is the most effective method to follow a conversation between two IP addresses?**  
    **Correct Answer: C (Using the 'Follow TCP Stream' option)**  
    **Explanation:** The 'Follow TCP Stream' option in Wireshark reassembles all packets in a TCP session for easier analysis.

13. **What happens if you filter traffic in Wireshark using the display filter `ip.addr == 192.168.1.1`?**  
    **Correct Answer: C**  
    **Explanation:** This filter will display packets where 192.168.1.1 is either the source or destination IP.

14. **True or False:**  
    Wireshark can reconstruct entire HTTP conversations, including file downloads, through packet captures.  
    **Correct Answer: True**  
    **Explanation:** Wireshark can reconstruct conversations by capturing and reassembling packets at the application layer.

15. **True or False:**  
    Wireshark requires a physical interface to be placed into monitor mode to capture traffic on a wireless network.  
    **Correct Answer: True**  
    **Explanation:** Wireshark requires monitor mode on wireless interfaces to capture all traffic on a wireless network.

16. **Describe how Wireshark categorizes and displays the layers of encapsulation in a captured packet. Include an explanation of how to expand each layer. (5 points)**  
    **Correct Answer: (Sample Explanation)**  
    Wireshark categorizes encapsulated packets by displaying each protocol layer separately. Users can expand each layer, such as Ethernet, IP, and TCP/UDP, to view the corresponding headers and data.

17. **Analyze a scenario in Wireshark where an ICMP packet shows a high round-trip time (RTT). What might this indicate about the network's performance? (5 points)**  
    **Correct Answer: (Sample Explanation)**  
    A high RTT in ICMP packets could indicate network congestion, long propagation delay, or routing issues, affecting the overall network performance.

---

## Section 3: RFC Standards and Protocol Behavior (30 Points)

18. **According to RFC 793, which of the following is true about the Transmission Control Protocol (TCP)?**  
    **Correct Answer: B (TCP guarantees in-order delivery of packets)**  
    **Explanation:** TCP ensures that data is delivered in the correct order through sequence numbers and acknowledgments.

19. **RFC 791 specifies which of the following fields in the IPv4 header?**  
    **Correct Answer: C (Time to Live - TTL)**  
    **Explanation:** The TTL field is used to limit the lifespan of a packet to prevent it from circulating endlessly.

20. **Which of the following protocols described by RFCs is designed to handle error messages for issues in packet delivery?**  
    **Correct Answer: C (ICMP)**  
    **Explanation:** ICMP (Internet Control Message Protocol) handles error and diagnostic messages related to packet delivery.

21. **True or False:**  
    RFCs (Request for Comments) provide universal implementation guidelines that must be followed by all devices and protocols.  
    **Correct Answer: False**  
    **Explanation:** RFCs are not always mandatory; they are often guidelines or recommendations. Some may be adopted as standards.

22. **True or False:**  
    RFC 768 describes a connectionless, unreliable protocol that is used for quick message transmission without error recovery.  
    **Correct Answer: True**  
    **Explanation:** RFC 768 describes UDP (User Datagram Protocol), which is a connectionless and unreliable protocol.

23. **True or False:**  
    According to RFC 793, a SYN packet is the first step in establishing a TCP connection.  
    **Correct Answer: True**  
    **Explanation:** The SYN packet initiates the TCP Three-Way Handshake to establish a connection.

24. **Explain how RFCs contribute to maintaining consistency in network communication. How do vendors implement these standards in their devices and software? (10 points)**  
    **Correct Answer: (Sample Explanation)**  
    RFCs provide a structured way to define how protocols and systems should behave, ensuring interoperability between different vendors. Vendors implement these standards to ensure their devices can communicate with others following the same guidelines.

25. **Discuss the potential consequences of a poorly implemented RFC 791 (IPv4) header field on data transmission between networks. (10 points)**  
    **Correct Answer: (Sample Explanation)**  
    Poor implementation of the IPv4 header (RFC 791) can lead to issues such as incorrect packet routing, improper handling of TTL, or security vulnerabilities, which could disrupt communication between networks.

---

## Section 4: Advanced Network Calculations (25 Points)

26. **In an IPv4 packet with a header size of 20 bytes and a total datagram size of 1000 bytes, how much data follows the IP header?**  
    **Correct Answer: B (980 bytes)**  
    **Explanation:** The IP header is 20 bytes, so the remaining 980 bytes are the payload following the header.

27. **Given an IP address of 192.168.10.0/24, what is the maximum number of assignable hosts on the network?**  
    **Correct Answer: A (254)**  
    **Explanation:** A /24 subnet allows for 256 IP addresses, but two are reserved (network and broadcast addresses), leaving 254 assignable hosts.

28. **A TCP segment has a sequence number of 12345 and an acknowledgment number of 54321. What is the next expected acknowledgment number if the segment contains 1500 bytes of data?**  
    **Correct Answer: C (55821)**  
    **Explanation:** The next acknowledgment number would be the previous acknowledgment number (54321) plus the 1500 bytes of data, which equals 55821.

29. **True or False:**  
    A subnet mask of /30 can support 2 usable IP addresses.  
    **Correct Answer: True**  
    **Explanation:** A /30 subnet provides 4 IP addresses, but 2 are reserved for network and broadcast addresses, leaving 2 usable IPs.

30. **True or False:**  
    The hexadecimal value 0xFF is equivalent to 255 in decimal.  
    **Correct Answer: True**  
    **Explanation:** 0xFF in hexadecimal is 255 in decimal (F = 15 in hexadecimal, so FF = 15*16 + 15 = 255).

---

## Final Questions (Extra Credit)

31. **You are given a pcap file containing HTTP and ICMP traffic. Describe a step-by-step process to analyze this traffic in Wireshark, highlighting how you would filter, identify anomalies, and reconstruct sessions. (10 points)**  
    **Correct Answer: (Sample Explanation)**  
    First, open the pcap file in Wireshark. Use the display filter `http` to filter HTTP traffic, and `icmp` for ICMP traffic. Follow TCP streams for HTTP sessions and analyze the payload. Identify anomalies such as unusual request sizes, missing packets, or delays. For ICMP, examine round-trip times to check for potential network issues.

32. **Explain how the Time to Live (TTL) field in the IPv4 header can be used for both diagnostic purposes and as a defense against certain network attacks. (10 points)**  
    **Correct Answer: (Sample Explanation)**  
    The TTL field prevents packets from circulating indefinitely by reducing the TTL value at each hop. It is used in traceroute to diagnose network paths. It also protects against certain attacks, like packet loops or amplification attacks, by limiting the packet's lifespan.