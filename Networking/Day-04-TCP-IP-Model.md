# Day 04 — TCP/IP Model

**Date:** 26 November 2026  
**Status:** Completed — core assessment and targeted revision (5/5)  
**Track:** SOC / Blue Team

## Learning resource

- [TCP/IP model — Day 4 study video](https://www.youtube.com/watch?v=CRdL1PcherM)
- Status: Watched (learner confirmed).

## Learning objectives

- Recall the four layers of the TCP/IP model.
- Map the TCP/IP layers to the seven OSI layers.
- Explain why both models are useful.
- Review encapsulation and the difference between a frame and a packet.

## Active recall — my answers

| Layer (bottom to top) | TCP/IP layer | Function and example | Corresponding OSI layers |
| --- | --- | --- | --- |
| 1 | Network Access | Converts frames into electrical signals and manages local data transmission; hubs, switches, Ethernet, optical fiber. | Physical and Data Link (reviewed mapping) |
| 2 | Internet | Logical IPv4/IPv6 addressing and routing packets between interconnected networks. | Network (reviewed mapping) |
| 3 | Transport | Transports data from one side to another. | Transport (reviewed mapping) |
| 4 | Application | Application, Presentation and Session functions; TLS handshake, session management, HTTP, DNS, encryption and decryption. | Application, Presentation, Session (learner identified) |

Learner answers are lightly edited for spelling and readability. OSI mappings not explicitly given by the learner are supplied as review notes.

### Active recall assessment

| Layer | Marks | Feedback |
| --- | --- | --- |
| Application | 2.5/2.5 | Correct in the four-layer model. |
| Transport | 2/2.5 | Add TCP, UDP and ports; use the term Transport. |
| Internet | 2.5/2.5 | Correct addressing and routing explanation. |
| Network Access | 2/2.5 | Include MAC addressing, optical and radio signals as well as electrical signals. |

**Score: 9/10 (90%).** All four layers recalled in correct order. This is the active recall score, not the final assessment.

## Self-assessment questions

1. What are the four layers of the TCP/IP model in order?
2. Which OSI layers correspond to the TCP/IP Application layer?
3. Which TCP/IP layer handles IP addressing and routing?
4. Which TCP/IP layer uses TCP and UDP?
5. Why do we learn both the OSI and TCP/IP models?
6. Explain encapsulation in your own words.

## My notes

### Reviewed technical notes

- **Application:** Network services, application protocols and upper-layer data representation/session/security functions; examples HTTP, DNS, SMTP and TLS. Mapping to OSI layers 5–7 is approximate, not a strict protocol assignment.
- **Transport:** End-to-end communication between application endpoints, using TCP or UDP and ports. TCP provides reliable ordered delivery; UDP provides datagrams without those guarantees.
- **Internet:** Logical IPv4/IPv6 addressing and routing of IP packets across networks; ICMP is another Internet-layer protocol.
- **Network Access:** Link-local frame delivery (e.g. Ethernet MAC addresses) and transmission as electrical, optical or radio signals. Maps approximately to OSI layers 1–2.

OSI is a conceptual seven-layer reference model; TCP/IP is the architecture of the protocol suite used by the Internet. Both help describe network communication and troubleshoot it.

Personal takeaways are recorded in the revision assessment below.

## Final knowledge test — first attempt

| Question | Learner answer (lightly edited for readability) | Score |
| --- | --- | --- |
| Main difference between OSI and TCP/IP? | OSI has seven layers; TCP/IP has four. | 0.5/1 |
| Which OSI layers combine into Network Access? | Physical and Data Link. | 1/1 |
| Difference between TCP and UDP? | TCP is reliable and ensures data reaches the receiver, unlike UDP. | 1/1 |
| Which layer uses port numbers? | Application. | 0/1 |
| Which layer uses MAC addresses? | Network layer. | 0.5/1 |
| Which layer handles ICMP? | Internet layer. | 1/1 |
| What are encapsulation and decapsulation? | Application > Transport > Internet > Network Access; reverse for decapsulation. | 0.5/1 |
| Why are networking models important for SOC analysts? | I don't know. | 0/1 |

**Final test, first attempt: 4.5/8 (56.25%).** Three correct, three partial, one incorrect and one unanswered. Half credit on the MAC question reflects the possibility that the learner meant Network Access, not the OSI Network layer.

### Corrections and revision

- OSI is a seven-layer conceptual reference model; TCP/IP is the four-layer Internet protocol architecture.
- TCP uses sequencing, acknowledgements and retransmissions to provide reliable ordered delivery when a connection succeeds. It cannot guarantee that a failed connection delivers all data. UDP does not guarantee delivery or ordering.
- Transport: TCP/UDP port numbers. Internet: IP addresses and ICMP. Network Access: MAC addresses and local frames.
- Encapsulation adds protocol headers and applicable trailers to data. Decapsulation processes and removes them in reverse. Example: data -> TCP segment -> IP packet -> Ethernet frame -> bits/signals.
- SOC analysts use these layers to interpret packet captures, firewall logs and SIEM alerts, and distinguish application activity, transport ports, network IPs and link-local MAC addresses. Example: a connection to TCP port 443 identifies a transport endpoint, but the port alone does not prove HTTPS or malicious activity.

### Revision assessment — completed

| Question | Learner answer (lightly edited for readability) | Marks |
| --- | --- | --- |
| Which layer uses port numbers? | Transport. | 1/1 |
| Which layer uses MAC addresses? | Network Access. | 1/1 |
| Which layer handles IP addresses and ICMP? | Internet. | 1/1 |
| What happens during encapsulation and decapsulation? | During encapsulation, protocol information is added when applicable; during decapsulation, it is removed when receiving data. | 1/1 |
| How does a SOC analyst use networking models? | Application: suspicious DNS queries; Transport: which ports are being used; Internet: suspicious IP addresses. | 1/1 |

**Revision test: 5/5 (100%).** This is a targeted retest of the concepts missed in the first assessment, not a replacement for the original score.

Technical clarification: encapsulation adds headers and applicable trailers; decapsulation processes and removes them at the receiver.

Learner's demonstrated takeaways: distinguish transport ports, link-local MAC addresses and IP addresses; explain encapsulation and decapsulation; relate DNS queries, ports and IP addresses to SOC investigations.

**Learning status:** Day 4 core assessment and targeted revision completed. Full independent OSI mapping has not been separately tested. No practical lab is claimed.

## Completion checklist

- [x] Watch the TCP/IP study video (learner confirmed).
- [x] Recall and explain the four layers (9/10).
- [ ] Independently map all TCP/IP layers to OSI layers (application and Network Access mappings demonstrated; full independent mapping not separately tested).
- [x] Attempt final knowledge test (4.5/8).
- [x] Demonstrate understanding of corrections in revision test (5/5).
- [x] Document demonstrated personal takeaways.

## Next topic

Day 05 — IP addressing and subnetting basics.
