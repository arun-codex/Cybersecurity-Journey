# Day 04 — TCP/IP Model

**Date:** 26 November 2026  
**Status:** In progress — video watched and active recall reviewed (9/10)  
**Track:** SOC / Blue Team

## Learning resource

- [TCP/IP model — Day 4 study video](https://www.youtube.com/watch?v=CRdL1PcherM&t=238s)
- Status: Watched (learner confirmed).
- The original timestamp supplied by the learner is preserved.

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

Final knowledge test and personal takeaways are pending.

## Completion checklist

- [x] Watch the TCP/IP study video (learner confirmed).
- [x] Recall and explain the four layers (9/10).
- [ ] Independently map all TCP/IP layers to OSI layers (application mapping demonstrated; remaining mappings reviewed).
- [ ] Complete the self-assessment and review corrections.
- [ ] Document personal takeaways.

## Next topic

Day 05 — IP addressing and subnetting basics.
