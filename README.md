# Cybersecurity Journey

**A documented learning journey from cybersecurity fundamentals to SOC / Blue Team readiness.**

![Focus](https://img.shields.io/badge/Focus-SOC%20%2F%20Blue%20Team-2563eb)
![Status](https://img.shields.io/badge/Status-Actively%20Learning-16a34a)
![Documentation](https://img.shields.io/badge/Documentation-Markdown-475569)
![Version control](https://img.shields.io/badge/Version%20Control-Git-f05032)

This repository is my public learning portfolio as I build a foundation in cybersecurity and work toward becoming a Security Operations Center (SOC) analyst. It documents what I study, how I understand it, where I make mistakes, how I correct them, and eventually how I apply these concepts in hands-on investigations and projects.

The goal is not simply to complete courses. It is to develop practical, explainable skills and maintain an honest record of progress.

[Learning progress](#current-learning-progress) · [Daily notes](#daily-learning-log) · [Roadmap](#learning-roadmap) · [Projects](#planned-portfolio-projects) · [Resources](#learning-resources)

---

## Current learning progress

**Last updated:** 26 November 2026  
**Current phase:** Month 1 — Networking and Linux Foundations  
**Latest completed lesson:** Day 4 — TCP/IP Model  
**Next lesson:** Day 5 — IP Addressing and Subnetting

```text
Week 1  [###########---------]  57.1%  (4 of 7 days)
```

| Metric | Current record |
| --- | --- |
| Week 1 study days completed | 4 / 7 |
| Detailed daily lesson documents | 2 |
| Study videos recorded | 2 |
| Day 3 knowledge test | 7/8 (87.5%) |
| Day 4 active recall | 9/10 (90%) |
| Day 4 first knowledge test | 4.5/8 (56.25%) |
| Day 4 targeted revision | 5/5 (100%) |

Completion indicates the core learning activities were recorded; it is not a certification or a claim of professional mastery. The targeted revision score is kept separate from the original test score to make improvement visible.

The [Networking progress tracker](Networking/README.md) contains the detailed status. This root README is a dated overview and will need updating as new lessons are added.

## Repository structure

```text
Cybersecurity-Journey/
├── README.md
└── Networking/
    ├── README.md
    ├── Day-03-OSI-Model.md
    └── Day-04-TCP-IP-Model.md
```

| Document | Purpose |
| --- | --- |
| [Networking/README.md](Networking/README.md) | Weekly progress, topics and study status |
| [Day 03 — OSI Model](Networking/Day-03-OSI-Model.md) | Seven layers, active recall, assessment, corrections and video resource |
| [Day 04 — TCP/IP Model](Networking/Day-04-TCP-IP-Model.md) | Four layers, model mapping, first assessment, revision and SOC relevance |

Additional subject folders will be added when study begins, rather than listing empty or nonexistent modules as completed.

## Daily learning log

### Week 1 — Environment setup and networking basics

| Day | Topic | Status | Evidence / outcome |
| --- | --- | --- | --- |
| 01 | Learning environment setup | Completed | Learner-reported completion |
| 02 | Linux exploration and networking introduction | Completed | Learner-reported completion |
| 03 | [OSI Model](Networking/Day-03-OSI-Model.md) | Completed | Seven layers recalled; final test 87.5% |
| 04 | [TCP/IP Model](Networking/Day-04-TCP-IP-Model.md) | Completed | Four layers recalled; revision 100% |
| 05 | IP addressing and subnetting | Planned | IPv4, public/private IPs, subnet masks |
| 06 | Ports, protocols and introductory networking labs | Planned | Common ports and authorized practice |
| 07 | Weekly revision and networking labs | Planned | Self-test and concept reinforcement |

### What I have learned so far

- Identify the seven OSI layers and explain their basic functions.
- Identify the four TCP/IP layers and relate them to the OSI reference model.
- Distinguish TCP reliability from UDP's lack of delivery guarantees.
- Associate transport ports, network-layer IP addresses and link-layer MAC addresses.
- Explain encapsulation and decapsulation using protocol headers and applicable trailers.
- Connect suspicious DNS queries, ports and IP addresses with SOC investigations.

**Revision priorities:** strengthen packet-versus-frame explanations, practise complete independent OSI-to-TCP/IP mapping, and apply these concepts to actual packet captures later.

## Learning roadmap

The roadmap prioritizes defensive security and SOC skills. Dates are flexible; advancement depends on understanding and practical evidence rather than course completion alone.

### Month 1 — Networking and Linux foundations

| Week | Focus | Topics |
| --- | --- | --- |
| 1 | Networking fundamentals | OSI, TCP/IP, IPv4, subnetting, common ports and review |
| 2 | Network communication | Deeper IP/subnet practice, DNS, HTTP/HTTPS, TCP/UDP, request flow and browser network tools |
| 3 | Linux command line | Filesystem, file operations, permissions, users/groups and processes |
| 4 | Consolidation | Network troubleshooting, firewall basics, introductory security labs and self-assessment |

Month 1 target: explain how a web request travels from a browser to a server, navigate Linux confidently and demonstrate foundational networking concepts in a controlled lab.

### Subsequent phases (planned)

| Phase | Subject | Intended skills |
| --- | --- | --- |
| 02 | Security fundamentals | CIA triad, threats, vulnerabilities, risk, authentication and access control |
| 03 | Network security and Wireshark | Packet capture, display filters, protocol inspection and authorized network assessment |
| 04 | Windows and Linux security | Event logs, system hardening, permissions, authentication and endpoint telemetry |
| 05 | Python and automation | Log parsing, regular expressions, JSON/CSV processing and security scripting |
| 06 | SIEM and SOC operations | Log ingestion, queries, dashboards, alert triage and investigation workflows |
| 07 | MITRE ATT&CK and threat intelligence | Tactics, techniques, indicators, enrichment and detection context |
| 08 | Incident response and forensics | Triage, evidence handling, timelines, containment and reporting |
| 09 | Threat hunting and detection engineering | Hypothesis-driven hunts, detection rules, validation and false-positive analysis |
| 10 | Portfolio and interview preparation | End-to-end projects, technical write-ups, mock investigations and interview practice |

## Tools and technologies

The following are part of the intended learning toolkit. They are not claims that I have mastered or installed every tool.

| Category | Tools / technologies | Status |
| --- | --- | --- |
| Documentation | Git, GitHub, Markdown | In use |
| Operating systems | Linux, Windows | Linux foundations started |
| Networking | IP, TCP, UDP, DNS, HTTP/S, Ethernet | Studying |
| Traffic analysis | Wireshark, tcpdump | Planned |
| Network assessment | Nmap, ping, traceroute, dig | Planned |
| Programming | Python, Bash, PowerShell | Planned |
| SIEM | Splunk or Microsoft Sentinel | Planned |
| Detection and investigation | Sigma, MITRE ATT&CK, Windows Event Logs, Sysmon | Planned |

## Planned portfolio projects

Projects will be documented with objectives, lab setup, methodology, sanitized evidence, findings, limitations and lessons learned. They will be linked here once actual project files exist.

| Project | Intended outcome | Status |
| --- | --- | --- |
| Wireshark network traffic analysis | Explain DNS, TCP and HTTP/S traffic from a permitted capture | Planned |
| Python authentication log analyzer | Identify and summarize suspicious login patterns in synthetic logs | Planned |
| Linux security hardening lab | Document permissions, services and safe configuration changes | Planned |
| Phishing analysis report | Inspect a safe sample and document indicators and recommended actions | Planned |
| Home SOC lab | Collect endpoint logs and investigate simulated alerts | Planned |
| SIEM detection dashboard | Query events and visualize suspicious behavior | Planned |
| MITRE ATT&CK detection mapping | Map observed lab behaviors to relevant techniques | Planned |
| Incident response case study | Build a timeline and communicate evidence-backed findings | Planned |

## Learning resources

### Videos actually watched

| Day | Topic | Resource |
| --- | --- | --- |
| 03 | OSI Model | [Watch video](https://www.youtube.com/watch?v=AYgXr1dynKU) |
| 04 | TCP/IP Model | [Watch video (original timestamp)](https://www.youtube.com/watch?v=CRdL1PcherM&t=238s) |

### Reference library for future study

- [Professor Messer](https://www.professormesser.com/) — networking and security fundamentals.
- [Cisco Skills for All](https://skillsforall.com/) — networking and cybersecurity learning.
- [Wireshark documentation](https://www.wireshark.org/docs/) — packet analysis reference.
- [MITRE ATT&CK](https://attack.mitre.org/) — adversary behavior knowledge base.
- [Microsoft Learn](https://learn.microsoft.com/) — Windows, security and Sentinel learning.
- [TryHackMe](https://tryhackme.com/) — guided practice when suitable free rooms or access are available.
- [OverTheWire](https://overthewire.org/wargames/) — an alternative for Linux command-line practice.

These reference sites are suggested resources, not completed courses. Availability and access requirements may vary.

## How I document my learning

Each daily note follows a consistent process:

1. Study the topic and record the source.
2. Recall concepts without looking at notes.
3. Explain them in my own words.
4. Complete practice questions and, where appropriate, an authorized lab.
5. Document mistakes, technical corrections and assessment scores.
6. Retest weak areas instead of hiding incorrect first attempts.
7. Commit the updated learning record to GitHub.

### Daily note format

```markdown
# Day XX — Topic

## Learning objectives
## Resources studied
## My explanations and notes
## Active recall / practice exercises
## Practical lab (if performed)
## Assessment and corrections
## Revision and personal takeaways
## Next learning goal
```

## Using this repository locally

Clone the repository and open the Networking folder:

```bash
git clone https://github.com/arun-codex/Cybersecurity-Journey.git
cd Cybersecurity-Journey
ls Networking
```

If a local clone already exists, review local changes and pull the latest commits:

```bash
git status
git pull --ff-only origin main
```

When adding new notes, review the files before committing:

```bash
git status
git diff
git add Networking/Day-XX-Topic.md Networking/README.md README.md
git diff --cached
git commit -m "Document Day XX: Topic and assessment"
git push origin main
```

Replace the example filename and commit message with the actual lesson details.

## Ethical use and documentation standards

This repository is for educational and defensive security purposes. All practical testing should be limited to systems I own, explicitly authorized environments or intentionally vulnerable training labs. I will not publish credentials, tokens, personal information, confidential logs, unauthorized packet captures or private network details.

Notes may contain corrected explanations and conceptual examples. Actual lab evidence will be labeled separately. Planned projects, tools and skills will not be represented as completed until there is supporting work.

## Long-term objective

Develop the skills needed for an entry-level SOC / Blue Team role: understand network and endpoint behavior, analyze security logs and alerts, investigate suspicious activity, communicate findings clearly, and continuously improve through practical learning.

**Maintainer:** [arun-codex](https://github.com/arun-codex)  
**Repository:** [Cybersecurity-Journey](https://github.com/arun-codex/Cybersecurity-Journey)
