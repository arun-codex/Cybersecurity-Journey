# Day 03 — OSI Model

**Date:** 25 November 2026  
**Status:** Completed — core assessment (7/8)  
**Track:** SOC / Blue Team  
**Study window:** 11:00 PM–1:00 AM IST (ends 26 November)

## Learning objectives

- Understand the purpose of the OSI reference model.
- Name all seven layers in both directions.
- Explain each layer with one real-world example in my own words.

## Study plan

| Time (IST) | Activity |
| --- | --- |
| 11:00–11:30 PM | Watch the OSI model study video (see learning resource below) |
| 11:30–11:40 PM | Break |
| 11:40 PM–12:10 AM | Active recall: write the seven layers and one example each without notes |
| 12:10–12:30 AM | Check answers against the lesson and correct mistakes |
| 12:30–1:00 AM | Recite the layers from top to bottom and bottom to top |

## Learning resource — video watched

- [OSI model — Day 3 study video](https://www.youtube.com/watch?v=AYgXr1dynKU)
- Status: Watched (learner confirmed).

## Reference table for review

Use this after the active recall exercise, not before it.

| Layer | Name | Example |
| --- | --- | --- |
| 7 | Application | Browser requesting a webpage |
| 6 | Presentation | Data encoding or formatting |
| 5 | Session | Managing a communication session |
| 4 | Transport | TCP segmentation |
| 3 | Network | Routing IP packets |
| 2 | Data Link | Ethernet switching using MAC addresses |
| 1 | Physical | Electrical, optical or radio signals |

## My notes — reviewed with technical corrections

| Layer | Explanation | Example |
| --- | --- | --- |
| 1. Physical | Transmits raw bits as electrical, optical or radio signals. | Copper cable, fiber, Wi-Fi radio |
| 2. Data Link | Transfers frames across a local link using link-layer addresses such as Ethernet MAC addresses. | Ethernet switch |
| 3. Network | Uses logical addresses and routing to deliver packets across networks. | IP, router |
| 4. Transport | Provides communication between application endpoints using ports; TCP provides reliable ordered delivery, UDP sends datagrams without that guarantee. | TCP, UDP |
| 5. Session | Establishes, manages and terminates communication sessions in the OSI reference model. | RPC session |
| 6. Presentation | Handles representation, encoding, compression and encryption functions. | UTF-8, JPEG |
| 7. Application | Provides network services to applications. | HTTP, DNS |

TLS performs security functions often associated with the upper OSI layers; its handshake is not exclusively a Session-layer protocol. Real TCP/IP implementations do not always map exactly to the OSI model.

## Active recall exercise

Learner recalled all seven layers in the correct bottom-to-top order (7/7; corrected spelling of Data Link).

Original explanations (lightly edited for readability; these are the learner's answers before corrections):

1. Physical: Data converts to electrical signals; fiber, cables, etc.
2. Data Link: Communication with another computer or network using MAC addresses.
3. Network: Routers and IP; communication with other devices using IP.
4. Transport: Transport data between computers using TCP or UDP.
5. Session: Establish, start, stop or break sessions to share data, e.g. TLS handshake.
6. Presentation: Encrypt or decrypt data using SSL/TLS.
7. Application: Send or read data using DNS, HTTP, etc.

Review: MAC-based frame delivery is link-local, whereas IP can operate both within and across networks. TLS does not belong exclusively to a single OSI layer.

## Final knowledge test

| Question | Learner answer (lightly edited) | Marks |
| --- | --- | --- |
| Which layer uses MAC addresses? | Data Link | 1/1 |
| Which layer uses IP addresses? | Network | 1/1 |
| Which layer uses TCP and UDP? | Transport | 1/1 |
| Which layer does a traditional router operate at? | Network | 1/1 |
| Which layer does a traditional Ethernet switch operate at? | Data Link | 1/1 |
| Difference between a packet and a frame? | Frame travels inside a local network using MAC; packet travels outside using IP/router. | 0.5/1 |
| Which layer do HTTP and DNS operate at? | Application | 1/1 |
| What is encapsulation? | Application > Presentation > Session > Transport > Network > Data Link > Physical. | 0.5/1 |

**Final score: 7/8 (87.5%).** Six correct and two partially correct; half credit for each partial answer.

### Corrections to revise

- A packet is a network-layer PDU containing IP addressing information; packets also travel within local networks. An Ethernet frame is a data-link PDU carrying a packet over a local link, with MAC addressing and an FCS trailer. Routers typically remove the incoming link-layer frame and build a new one for the outgoing link.
- Encapsulation is not simply the order of layers: it is the process of wrapping data in protocol information, such as a TCP header, IP header, and Ethernet header/trailer, for transmission. Decapsulation is the reverse process.

```text
Application data
  -> TCP segment (or UDP datagram)
  -> IP packet
  -> Ethernet frame
  -> bits carried as signals
```

## SOC relevance

When analyzing traffic in Wireshark, distinguish Ethernet MAC addresses, IP addresses, TCP/UDP ports and application protocols. Use these layers to narrow down connectivity and security issues. This is a conceptual example; no packet capture or lab was performed or verified here.

## Completion checklist

- [x] Watch the lesson (learner confirmed).
- [x] Recall all seven layers and provide explanations.
- [x] Review and correct answers.
- [ ] Practise reciting the layers aloud in both directions (not confirmed).
- [x] Complete the final knowledge test.
- [x] Document reviewed learning notes.
- [ ] Revisit packet vs. frame and encapsulation.

**Learning status:** Core Day 3 assessment completed. Oral practice remains unconfirmed; packet/frame and encapsulation revision is recommended.

## Next topic

Day 04 — TCP/IP model and its mapping to OSI.
