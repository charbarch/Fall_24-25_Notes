# TCP/IP, Wireshark, and RFC Standards Exam

## Section 1: Concepts of TCP/IP (20 Points)

1. **What is the purpose of encapsulation in the TCP/IP model?**  
   - A. To split data into smaller parts  
   - B. To ensure that data travels securely between applications  
   - C. To add headers for each layer as data moves through the network stack  
   - D. To translate data between different encoding formats

2. **Which protocol in the transport layer provides reliable data transfer with flow control and error checking?**  
   - A. UDP  
   - B. ICMP  
   - C. IP  
   - D. TCP

3. **Which of the following RFCs describe the Internet Protocol (IP)?**  
   - A. RFC 768  
   - B. RFC 791  
   - C. RFC 793  
   - D. RFC 792

4. **Which of the following best describes the OSI model?**  
   - A. A five-layer model for internet communications  
   - B. A model with layers designed to ensure secure data transmission  
   - C. A theoretical model for understanding and designing communication systems  
   - D. A two-layer model that handles application and physical aspects of communication

5. **When analyzing a captured packet, the payload for an HTTP request is located at:**  
   - A. The application layer  
   - B. The network layer  
   - C. The transport layer  
   - D. The data link layer

6. **True or False:**  
   The OSI model has a layer called the 'Internet Layer,' which does not exist in the TCP/IP model.  
   - True  
   - False

7. **True or False:**  
   The transport layer in the TCP/IP model is responsible for defining the best path for data transmission.  
   - True  
   - False

8. **True or False:**  
   Encapsulation occurs in both the OSI and TCP/IP models, and it always starts at the physical layer.  
   - True  
   - False

9. **Explain the process of de-encapsulation and why it is important in network communication. (5 points)**  
   *(Write your answer below)*

10. **Describe the significance of the 'Three-Way Handshake' in TCP communication. What happens if the process is interrupted? (5 points)**  
    *(Write your answer below)*

---

## Section 2: Wireshark and Packet Analysis (25 Points)

11. **What is the primary feature that distinguishes Wireshark from Tcpdump?**  
    - A. Wireshark has a graphical user interface (GUI)  
    - B. Tcpdump can display data at the application layer  
    - C. Tcpdump is more accurate in decoding TCP streams  
    - D. Wireshark cannot handle large packet captures

12. **In Wireshark, what is the most effective method to follow a conversation between two IP addresses?**  
    - A. Using the 'Find Packet' option  
    - B. Reassembling the payloads in the Protocol Hierarchy statistics  
    - C. Using the 'Follow TCP Stream' option  
    - D. Filtering based on MAC addresses

13. **What happens if you filter traffic in Wireshark using the display filter `ip.addr == 192.168.1.1`?**  
    - A. It will display packets with a source address of 192.168.1.1 only  
    - B. It will display packets with a destination address of 192.168.1.1 only  
    - C. It will display packets where 192.168.1.1 is either the source or destination IP  
    - D. It will filter out all packets except those related to ICMP

14. **True or False:**  
    Wireshark can reconstruct entire HTTP conversations, including file downloads, through packet captures.  
    - True  
    - False

15. **True or False:**  
    Wireshark requires a physical interface to be placed into monitor mode to capture traffic on a wireless network.  
    - True  
    - False

16. **Describe how Wireshark categorizes and displays the layers of encapsulation in a captured packet. Include an explanation of how to expand each layer. (5 points)**  
    *(Write your answer below)*

17. **Analyze a scenario in Wireshark where an ICMP packet shows a high round-trip time (RTT). What might this indicate about the network's performance? (5 points)**  
    *(Write your answer below)*

---

## Section 3: RFC Standards and Protocol Behavior (30 Points)

18. **According to RFC 793, which of the following is true about the Transmission Control Protocol (TCP)?**  
    - A. TCP is an unreliable protocol  
    - B. TCP guarantees in-order delivery of packets  
    - C. TCP operates at the network layer of the OSI model  
    - D. TCP does not provide error recovery

19. **RFC 791 specifies which of the following fields in the IPv4 header?**  
    - A. Source and Destination Port  
    - B. Sequence Number  
    - C. Time to Live (TTL)  
    - D. Payload Type

20. **Which of the following protocols described by RFCs is designed to handle error messages for issues in packet delivery?**  
    - A. TCP  
    - B. UDP  
    - C. ICMP  
    - D. IP

21. **True or False:**  
    RFCs (Request for Comments) provide universal implementation guidelines that must be followed by all devices and protocols.  
    - True  
    - False

22. **True or False:**  
    RFC 768 describes a connectionless, unreliable protocol that is used for quick message transmission without error recovery.  
    - True  
    - False

23. **True or False:**  
    According to RFC 793, a SYN packet is the first step in establishing a TCP connection.  
    - True  
    - False

24. **Explain how RFCs contribute to maintaining consistency in network communication. How do vendors implement these standards in their devices and software? (10 points)**  
    *(Write your answer below)*

25. **Discuss the potential consequences of a poorly implemented RFC 791 (IPv4) header field on data transmission between networks. (10 points)**  
    *(Write your answer below)*

---

## Section 4: Advanced Network Calculations (25 Points)

26. **In an IPv4 packet with a header size of 20 bytes and a total datagram size of 1000 bytes, how much data follows the IP header?**  
    - A. 1000 bytes  
    - B. 980 bytes  
    - C. 1020 bytes  
    - D. 960 bytes

27. **Given an IP address of 192.168.10.0/24, what is the maximum number of assignable hosts on the network?**  
    - A. 254  
    - B. 256  
    - C. 512  
    - D. 1024

28. **A TCP segment has a sequence number of 12345 and an acknowledgment number of 54321. What is the next expected acknowledgment number if the segment contains 1500 bytes of data?**  
    - A. 54321  
    - B. 13845  
    - C. 55821  
    - D. 12345

29. **True or False:**  
    A subnet mask of /30 can support 2 usable IP addresses.  
    - True  
    - False

30. **True or False:**  
    The hexadecimal value 0xFF is equivalent to 255 in decimal.  
    - True  
    - False

---

## Final Questions (Extra Credit)

31. **You are given a pcap file containing HTTP and ICMP traffic. Describe a step-by-step process to analyze this traffic in Wireshark, highlighting how you would filter, identify anomalies, and reconstruct sessions. (10 points)**  
    *(Write your answer below)*

32. **Explain how the Time to Live (TTL) field in the IPv4 header can be used for both diagnostic purposes and as a defense against certain network attacks. (10 points)**  
    *(Write your answer below)*