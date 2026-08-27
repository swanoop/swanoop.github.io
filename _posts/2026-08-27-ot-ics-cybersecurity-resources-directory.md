---
layout: post
title: "OT/ICS Cybersecurity Resources Directory 2026: Standards, Training, Labs, Tools & Books"
description: "A curated OT/ICS cybersecurity directory covering IEC 62443, NIST, training, labs, industrial protocols, tools, threat intelligence, books and UK resources."
date: 2026-08-27
category: "OT / ICS"
tags:
  - OT Cybersecurity
  - ICS Security
  - IEC 62443
  - SCADA Security
  - Industrial Cybersecurity
  - OT Training
read_time: 18
---

Operational Technology and Industrial Control System cybersecurity spans engineering, networking, risk, standards, threat intelligence and the physical process itself. The challenge is rarely finding *a* resource; it is knowing which resources are worth your time and where they fit.

This page is my curated **OT/ICS cybersecurity resources directory** for practitioners, engineers, students and anyone moving into industrial cybersecurity. It brings together the references I find most useful across standards, training, labs, tools, industrial protocols, research, books and the wider OT security community.

**Last reviewed: August 2026.** I will update this page as useful resources appear, links move and the OT security landscape changes.

![OT and ICS cybersecurity resources directory covering standards, training, labs, tools and industrial security research]({{ '/assets/images/ot-ics-resources-directory.svg' | relative_url }})

> **Safety note:** active scanning, exploitation and protocol manipulation can disrupt real industrial systems. Use offensive or active tools only in a lab or on systems where you have explicit authorisation and understand the operational impact.

## If you are new to OT cybersecurity, start here

You do not need to consume everything on this page at once. A strong starting sequence is:

1. Read [NIST SP 800-82 Rev. 3](https://csrc.nist.gov/pubs/sp/800/82/r3/final) for the fundamentals of OT security and architecture.
2. Understand the role of [ISA/IEC 62443](https://www.isa.org/standards-and-publications/isa-standards/isa-iec-62443-series-of-standards) across the industrial cybersecurity lifecycle.
3. Use [MITRE ATT&CK for ICS](https://attack.mitre.org/matrices/ics/) to understand adversary behaviour in industrial environments.
4. Learn packet analysis with [Wireshark](https://www.wireshark.org/) and begin recognising industrial protocols.
5. Build a safe lab with [OpenPLC](https://openplcproject.com/), [FUXA](https://github.com/frangoteam/FUXA) or [GRFICS](https://fortiphyd.github.io/grfics/).
6. If you work in the UK, become familiar with the [NCSC Cyber Assessment Framework](https://www.ncsc.gov.uk/collection/cyber-assessment-framework).

## Quick navigation

- [Standards, frameworks and guidance](#standards-frameworks-and-guidance)
- [ISA/IEC 62443 quick reference](#isaiec-62443-quick-reference)
- [Certifications and professional training](#certifications-and-professional-training)
- [Free training and learning](#free-training-and-learning)
- [Books](#books)
- [Labs and cyber ranges](#labs-and-cyber-ranges)
- [Network and protocol analysis](#network-and-protocol-analysis)
- [Industrial protocols worth knowing](#industrial-protocols-worth-knowing)
- [PCAPs and datasets](#pcaps-and-datasets)
- [OT security tools](#ot-security-tools)
- [Commercial OT security platforms](#commercial-ot-security-platforms)
- [Vulnerability and security advisories](#vulnerability-and-security-advisories)
- [Threat intelligence and research](#threat-intelligence-and-research)
- [OT malware and incidents to study](#ot-malware-and-incidents-to-study)
- [GitHub collections and projects](#github-collections-and-projects)
- [People to follow](#people-to-follow)
- [Conferences and events](#conferences-and-events)
- [Podcasts and video](#podcasts-and-video)
- [OT cybersecurity news and regular reading](#ot-cybersecurity-news-and-regular-reading)
- [UK OT and critical-infrastructure resources](#uk-ot-and-critical-infrastructure-resources)
- [Professional organisations and communities](#professional-organisations-and-communities)

## Standards, frameworks and guidance

| Resource | Why it matters |
|---|---|
| [ISA/IEC 62443](https://www.isa.org/standards-and-publications/isa-standards/isa-iec-62443-series-of-standards) | Standards series covering cybersecurity across the lifecycle of industrial automation and control systems. |
| [NIST SP 800-82 Rev. 3](https://csrc.nist.gov/pubs/sp/800/82/r3/final) | NIST's current final guide for securing OT, including ICS, SCADA, DCS and PLC environments. NIST began work toward Rev. 4 in 2026, but Rev. 3 remains the current final publication. |
| [MITRE ATT&CK for ICS](https://attack.mitre.org/matrices/ics/) | Knowledge base of adversary tactics and techniques relevant to industrial control systems. |
| [NCSC Cyber Assessment Framework](https://www.ncsc.gov.uk/collection/cyber-assessment-framework) | UK outcome-focused framework for assessing cyber security and resilience of organisations providing essential functions. |
| [CISA Industrial Control Systems](https://www.cisa.gov/topics/industrial-control-systems) | US government guidance, advisories, tools and training for ICS and critical infrastructure. |
| [CISA Cybersecurity Performance Goals](https://www.cisa.gov/cybersecurity-performance-goals) | Prioritised practices intended to reduce risk across critical infrastructure, including OT. |
| [CIS Controls v8.1 ICS Guide](https://www.cisecurity.org/insights/white-papers/cis-critical-security-controls-v8-1-industrial-control-systems-ics-guide) | Guidance for adapting the CIS Critical Security Controls to industrial environments. |
| [ISO/IEC 27001](https://www.iso.org/isoiec-27001-information-security.html) | International standard for information security management systems and organisational security governance. |
| [NIS2 Directive](https://digital-strategy.ec.europa.eu/en/policies/nis2-directive) | EU cybersecurity framework covering essential and important entities across 18 critical sectors. |
| [EU Cyber Resilience Act](https://digital-strategy.ec.europa.eu/en/policies/cyber-resilience-act) | EU requirements for cybersecurity of hardware and software products with digital elements across their lifecycle. |
| [IEC 61850](https://iec61850.dvl.iec.ch/) | Standards and communication architecture used extensively in electrical substation automation and protection. |

## ISA/IEC 62443 quick reference

You do not need every part of IEC 62443 for every role. These are the parts I most often see referenced in OT cybersecurity programmes and projects.

| Standard | Focus |
|---|---|
| **IEC 62443-2-1** | Security programme requirements for IACS asset owners. |
| **IEC 62443-2-4** | Security programme requirements for IACS service providers. |
| **IEC 62443-3-2** | Security risk assessment, System Under Consideration, zones and conduits, and target security levels. |
| **IEC 62443-3-3** | System security requirements and security levels. |
| **IEC 62443-4-1** | Secure product development lifecycle requirements. |
| **IEC 62443-4-2** | Technical security requirements for IACS components. |
| [ISA99 Committee](https://www.isa.org/standards-and-publications/isa-standards/isa-standards-committees/isa99) | ISA committee responsible for developing and maintaining the ISA/IEC 62443 series. |
| [ISASecure](https://isasecure.org/) | Certification and assurance schemes based on ISA/IEC 62443. |

## Certifications and professional training

These are established options, not a ranking or a recommendation that everyone needs them.

| Resource | Focus |
|---|---|
| [ISA/IEC 62443 IC32](https://www.isa.org/training/course-description/ic32) | Cybersecurity Fundamentals Specialist covering core industrial cybersecurity concepts. |
| [ISA/IEC 62443 IC33](https://www.isa.org/training/course-description/ic33) | Cybersecurity Risk Assessment Specialist focused on IEC 62443-3-2. |
| [ISA/IEC 62443 IC34](https://www.isa.org/training/course-description/ic34) | Cybersecurity Design Specialist covering industrial security architecture and countermeasure design. |
| [ISA/IEC 62443 IC37](https://www.isa.org/training/course-description/ic37) | Cybersecurity Maintenance Specialist focused on operating and maintaining secure IACS environments. |
| [ISA/IEC 62443 Cybersecurity Expert](https://www.isa.org/certification/certificate-programs/isa-iec-62443-cybersecurity-certificate-program) | ISA designation awarded after completing all four specialist certificates. |
| [ISASecure ACSSA for Evaluators](https://isasecure.org/acssa-consultants) | Specialist training for evaluating operating automation and control systems through the ACSSA scheme. |
| [GIAC GICSP](https://www.giac.org/certifications/global-industrial-cyber-security-professional-gicsp/) | Broad industrial cybersecurity certification combining cybersecurity and engineering concepts. |
| [SANS ICS410](https://www.sans.org/cyber-security-courses/ics-scada-cyber-security-essentials/) | ICS/SCADA security fundamentals and preparation for GICSP. |
| [SANS ICS515](https://www.sans.org/cyber-security-courses/ics-visibility-detection-response/) | Industrial visibility, detection, threat hunting and incident response; aligned with GRID. |
| [GIAC GRID](https://www.giac.org/certifications/response-industrial-defense-grid/) | Industrial detection, defence and incident-response certification. |
| [GIAC GCIP](https://www.giac.org/certifications/critical-infrastructure-protection-gcip/) | Critical-infrastructure protection with particular relevance to electricity and NERC CIP. |

## Free training and learning

| Resource | What you get |
|---|---|
| [CISA ICS Training](https://www.cisa.gov/ics-training-calendar) | Free ICS cybersecurity training, including virtual and hands-on options. |
| [Mike Holcomb / UtilSec](https://www.youtube.com/@utilsec) | Extensive practical OT/ICS cybersecurity tutorials, courses and lab walkthroughs. |
| [TryHackMe](https://tryhackme.com/) | Interactive rooms covering introductory ICS/OT concepts and wider networking/security fundamentals. |
| [SANS ICS Resources](https://www.sans.org/industrial-control-systems-security/) | Free posters, papers, webinars and presentations alongside paid training. |
| [S4 Events](https://s4xevents.com/) | Technical industrial-security presentations and conference material. |
| [ICS Village](https://www.icsvillage.com/) | Hands-on educational resources and demonstrations around industrial control-system security. |

## Books

A mixture of engineering, security, incident history and practical implementation.

| Title | Why read it |
|---|---|
| **Industrial Network Security** — Eric D. Knapp & Joel Thomas Langill | Industrial networks, architectures, protocols and ICS security fundamentals. |
| **Industrial Cybersecurity** — Pascal Ackerman | Practical introduction to securing industrial control systems and networks. |
| **Practical Industrial Cybersecurity** — Charles J. Brooks & Philip A. Craig Jr. | Broad coverage of ICS architecture, secure design, governance and industrial security practice. |
| **Engineering-Grade OT Security** — Andrew Ginter | Consequence-driven OT security from an engineering and operational-risk perspective. |
| **Implementing IEC 62443: A Pragmatic Approach to Cybersecurity** — Medoff & O'Brien | Practical guidance for organisations implementing IEC 62443. |
| **Industrial Cybersecurity: Case Studies and Best Practices** — Steve Mustard | Governance, design and operational security through practical examples. |
| **Countering Cyber Sabotage** — Andrew Bochman & Sarah Freeman | Introduces Consequence-Driven, Cyber-Informed Engineering for critical infrastructure. |
| **Pentesting Industrial Control Systems** — Paul Smith | Hands-on security testing of industrial environments and protocols. |
| **Hacking Exposed: Industrial Control Systems** | Technical coverage of ICS attack surfaces, vulnerabilities and security testing. |
| **Applied Cyber Security and the Smart Grid** — Eric D. Knapp & Raj Samani | Cybersecurity applied to power systems and smart-grid infrastructure. |
| **Countdown to Zero Day** — Kim Zetter | Investigation of Stuxnet and the compromise of Iran's nuclear enrichment programme. |
| **Sandworm** — Andy Greenberg | Investigation of disruptive cyber operations against critical infrastructure, including Ukraine's electricity network. |

## Labs and cyber ranges

| Resource | Use case |
|---|---|
| [OpenPLC](https://openplcproject.com/) | Open-source PLC runtime and programming environment for automation and cybersecurity labs. |
| [GRFICS](https://fortiphyd.github.io/grfics/) | Containerised OT/ICS cyber range with PLCs, HMIs, engineering components and attack/defence scenarios. |
| [GasPot HMI Lab](https://github.com/cutaway-security/gaspot-hmi-lab) | Experimental vulnerable HMI/industrial simulator based on the GasPot concept. |
| [Conpot](https://github.com/mushorg/conpot) | Open-source ICS/SCADA honeypot supporting several industrial protocols. |
| [MiniCPS](https://github.com/scy-phy/minicps) | Framework for modelling and experimenting with cyber-physical systems using network emulation. |
| [FUXA](https://github.com/frangoteam/FUXA) | Open-source web-based SCADA/HMI/dashboard platform supporting Modbus, S7, OPC UA, BACnet, MQTT and EtherNet/IP. |
| [Factory I/O](https://factoryio.com/) | Commercial 3D industrial process simulator that can communicate with real or simulated PLCs. |

## Network and protocol analysis

| Resource | Use case |
|---|---|
| [Wireshark](https://www.wireshark.org/) | Packet capture and protocol analysis with support for many industrial protocols. |
| [Zeek](https://zeek.org/) | Network security monitoring and rich traffic metadata. |
| [Suricata](https://suricata.io/) | Open-source IDS/IPS and network security monitoring. |
| [Snort](https://www.snort.org/) | Network intrusion detection and prevention. |
| [tcpdump](https://www.tcpdump.org/) | Command-line packet capture and troubleshooting. |
| [NetworkMiner](https://www.netresec.com/?page=NetworkMiner) | Network forensic analysis of PCAPs, hosts, sessions and transferred files. |

## Industrial protocols worth knowing

| Protocol | Common use | Reference |
|---|---|---|
| **Modbus TCP / RTU** | PLC, SCADA and field-device communication | [Modbus Organisation](https://www.modbus.org/) |
| **OPC UA** | Industrial data exchange and interoperability | [OPC Foundation](https://opcfoundation.org/) |
| **DNP3** | Electric utilities and SCADA | [DNP Users Group](https://www.dnp.org/) |
| **IEC 60870-5-104** | Power-system telecontrol | [IEC](https://www.iec.ch/) |
| **IEC 61850** | Electrical substation automation and protection | [IEC 61850 resource](https://iec61850.dvl.iec.ch/) |
| **PROFINET** | Industrial automation and manufacturing | [PROFIBUS & PROFINET International](https://www.profibus.com/) |
| **PROFIBUS** | Industrial fieldbus communication | [PROFIBUS & PROFINET International](https://www.profibus.com/) |
| **EtherNet/IP** | Industrial Ethernet, especially Rockwell ecosystems | [ODVA](https://www.odva.org/) |
| **CIP** | Industrial device communication and control | [ODVA](https://www.odva.org/) |
| **S7comm** | Siemens PLC communications | [Siemens](https://www.siemens.com/) |
| **BACnet** | Building management and building automation | [BACnet International](https://bacnetinternational.org/) |
| **HART** | Process instrumentation and field devices | [FieldComm Group](https://www.fieldcommgroup.org/) |
| **MQTT** | IoT, IIoT and industrial telemetry | [MQTT](https://mqtt.org/) |

## PCAPs and datasets

| Resource | Use case |
|---|---|
| [Wireshark Sample Captures](https://wiki.wireshark.org/SampleCaptures) | Public packet captures for learning protocol analysis. |
| [Netresec PCAP Files](https://www.netresec.com/?page=PcapFiles) | Public packet captures and network-forensic datasets. |
| [SWaT Dataset](https://itrust.sutd.edu.sg/itrust-labs_datasets/dataset_info/) | Data from the Secure Water Treatment cyber-physical testbed. |
| [WADI Dataset](https://itrust.sutd.edu.sg/itrust-labs_datasets/dataset_info/) | Water Distribution testbed data used in ICS anomaly-detection research. |
| [HAI Dataset](https://github.com/icsdataset/hai) | Industrial control-system dataset for anomaly-detection and security research. |

## OT security tools

These tools can be useful, but several are **active**. Do not point them at production OT simply because they work well on IT networks.

| Resource | Use case |
|---|---|
| [Nmap](https://nmap.org/) | Network discovery and service identification. Active scanning should be carefully controlled in OT. |
| [Scapy](https://scapy.net/) | Python packet manipulation for controlled protocol analysis and research. |
| [pymodbus](https://github.com/pymodbus-dev/pymodbus) | Python implementation of Modbus for clients, servers and test environments. |
| [Snap7](https://snap7.sourceforge.net/) | Communication library for interacting with Siemens S7 systems in authorised environments. |
| [CISA CSET](https://www.cisa.gov/downloading-and-installing-cset) | Cyber Security Evaluation Tool for structured cybersecurity assessment. |

## Commercial OT security platforms

These are examples of widely encountered platforms, **not product endorsements**.

| Platform | Typical capability area |
|---|---|
| [Dragos Platform](https://www.dragos.com/platform/) | OT asset visibility, threat detection, vulnerability management and industrial threat intelligence. |
| [Claroty](https://claroty.com/) | Cyber-physical asset visibility, exposure management and threat detection. |
| [Nozomi Networks](https://www.nozominetworks.com/) | OT/IoT visibility, monitoring and threat detection. |
| [Microsoft Defender for IoT](https://learn.microsoft.com/azure/defender-for-iot/) | OT/IoT discovery and monitoring integrated with the Microsoft security ecosystem. |
| [Tenable OT Security](https://www.tenable.com/products/ot-security) | OT asset visibility, vulnerability and exposure management. |
| [TXOne Networks](https://www.txone.com/) | Security technologies designed for industrial endpoints and OT networks. |
| [Forescout](https://www.forescout.com/) | Device visibility and security across IT, IoT and OT environments. |

## Vulnerability and security advisories

| Resource | What to monitor |
|---|---|
| [CISA ICS Advisories](https://www.cisa.gov/news-events/ics-advisories) | Vulnerabilities affecting industrial automation and control products. |
| [National Vulnerability Database](https://nvd.nist.gov/) | CVE enrichment and CVSS information. |
| [CVE](https://www.cve.org/) | Global catalogue of publicly disclosed vulnerabilities. |
| [Siemens ProductCERT](https://www.siemens.com/cert) | Siemens product security advisories. |
| [Schneider Electric Security Notifications](https://www.se.com/ww/en/work/support/cybersecurity/security-notifications.jsp) | Schneider Electric product vulnerabilities and notifications. |
| [Rockwell Automation Security Advisories](https://www.rockwellautomation.com/en-us/trust-center/security-advisories.html) | Rockwell Automation security advisories. |
| [ABB Cybersecurity](https://global.abb/group/en/technology/cyber-security/alerts-and-notifications) | ABB product cybersecurity advisories and notifications. |

## Threat intelligence and research

| Resource | Focus |
|---|---|
| [Dragos](https://www.dragos.com/resources/) | Industrial threat intelligence, malware analysis, incident research and annual OT reports. |
| [Claroty Team82](https://claroty.com/team82) | Vulnerability research across OT, IoT, medical and cyber-physical systems. |
| [Nozomi Networks Labs](https://www.nozominetworks.com/labs) | OT malware, vulnerability and threat research. |
| [Forescout Vedere Labs](https://www.forescout.com/research-labs/) | Vulnerability research across connected, IoT and OT devices. |
| [Google Threat Intelligence / Mandiant](https://cloud.google.com/security/resources) | Threat intelligence and incident-response research, including critical infrastructure activity. |
| [Unit 42](https://unit42.paloaltonetworks.com/) | Threat actor, malware and vulnerability research. |
| [Microsoft Security Blog](https://www.microsoft.com/en-us/security/blog/) | Nation-state, malware and critical-infrastructure threat intelligence. |
| [RITICS](https://www.ritics.org/) | UK research focused on trustworthy and resilient cyber-physical systems. |

## OT malware and incidents to study

Understanding historical incidents is one of the fastest ways to understand why OT security controls exist.

| Incident / malware | Why it matters |
|---|---|
| **Stuxnet** | Malware designed to manipulate Siemens control systems while concealing physical process changes. |
| **Havex** | Cyber-espionage campaign targeting organisations operating industrial control systems. |
| **BlackEnergy** | Malware associated with attacks against Ukrainian electricity infrastructure. |
| **Industroyer / CrashOverride** | Malware framework designed to interact with electricity-grid protocols. |
| **Industroyer2** | Later industrial malware used against Ukrainian electricity infrastructure. |
| **TRITON / TRISIS** | Malware targeting Schneider Electric Triconex Safety Instrumented Systems. |
| **PIPEDREAM / INCONTROLLER** | Industrial attack framework able to interact with multiple OT technologies. |
| **FrostyGoop** | Malware associated with disruptive use of Modbus communications. |
| **Oldsmar water-treatment intrusion** | Useful case study in remote access and operator visibility. |
| **Colonial Pipeline** | Demonstrates how compromise of enterprise IT can create major operational consequences. |
| **Norsk Hydro** | Large-scale ransomware incident affecting global industrial operations. |

## GitHub collections and projects

| Resource | Description |
|---|---|
| [Awesome Industrial Control System Security](https://github.com/hslatman/awesome-industrial-control-system-security) | Long-running community-curated list of ICS security tools, data, literature and training. |
| [ICS Security Tools](https://github.com/ITI/ICS-Security-Tools) | Tools, protocol references, PCAPs and resources for ICS security research. |
| [OpenPLC](https://github.com/thiagoralves/OpenPLC_v3) | Open-source PLC environment useful for labs and automation experiments. |
| [GRFICSv3](https://github.com/Fortiphyd/GRFICSv3) | Containerised industrial cybersecurity simulation environment. |
| [Conpot](https://github.com/mushorg/conpot) | Open-source ICS honeypot. |
| [MiniCPS](https://github.com/scy-phy/minicps) | Cyber-physical system simulation framework. |

## People to follow

This is not exhaustive; it is a starting list of practitioners, researchers and educators whose work regularly contributes to OT/ICS cybersecurity discussions.

| Person | Focus |
|---|---|
| **Robert M. Lee** | ICS threat intelligence, incident response, adversary activity and industrial defence. |
| **Dale Peterson** | ICS security research, S4 and industrial cybersecurity industry analysis. |
| **Sarah Fluchs** | IEC 62443, OT security engineering, risk and European cyber regulation. |
| **Lesley Carhart** | Industrial incident response, digital forensics and threat hunting. |
| **Mike Holcomb** | OT/ICS cybersecurity education, labs and practical training. |
| **Joel Langill** | Industrial control engineering and cybersecurity. |
| **Ralph Langner** | Industrial cybersecurity and Stuxnet research. |
| **Marina Krotofil** | Industrial security research and cyber-physical attack techniques. |
| **Chris Sistrunk** | ICS cybersecurity, network defence and incident response. |
| **Andrew Ginter** | Engineering-focused OT security and industrial network architecture. |

## Conferences and events

| Event | Focus |
|---|---|
| [S4](https://s4xevents.com/) | One of the best-known technical conferences dedicated to ICS and OT cybersecurity. |
| [SANS ICS Security Summit](https://www.sans.org/cyber-security-training-events/ics-security-summit/) | Practitioner-focused industrial defence, incident response and detection. |
| [BSidesICS/OT](https://www.bsidesics.org/) | Community-driven conference focused specifically on ICS and OT. |
| [ICS Cybersecurity Conference](https://www.icscybersecurityconference.com/) | Long-running industrial cybersecurity and critical-infrastructure event. |
| [ICS Village](https://www.icsvillage.com/) | Hands-on demonstrations, training and community events. |
| [CS3STHLM](https://cs3sthlm.se/) | Industrial-control-system and critical-infrastructure security conference. |
| [Black Hat](https://www.blackhat.com/) | Frequently includes ICS, embedded, hardware and critical-infrastructure research. |
| [DEF CON](https://defcon.org/) | Includes ICS, hardware, embedded and cyber-physical security communities. |

## Podcasts and video

| Resource | Focus |
|---|---|
| [Unsolicited Response](https://dale-peterson.com/podcast/) | Dale Peterson's interviews and discussions across the OT security community. |
| [The Industrial Security Podcast](https://waterfall-security.com/ot-insights-center/industrial-security-podcast/) | Industrial cybersecurity, engineering and critical-infrastructure conversations. |
| [PrOTect IT All](https://protectitall.co/) | OT cybersecurity, IT/OT convergence and practitioner discussions. |
| [Nexus: A Claroty Podcast](https://claroty.com/resources/podcasts) | Cyber-physical security and OT/IoT research discussions. |
| [Bites & Bytes](https://www.bitesandbytespodcast.com/) | Cybersecurity across food, agriculture and increasingly automated critical systems. |
| [Mike Holcomb / UtilSec](https://www.youtube.com/@utilsec) | Practical OT security tutorials and lab walkthroughs. |
| [SANS ICS](https://www.youtube.com/@SANSICS) | Industrial cybersecurity presentations and education. |
| [S4 Events](https://www.youtube.com/@S4Events) | Conference presentations from industrial security practitioners and researchers. |

## OT cybersecurity news and regular reading

| Resource | Why follow it |
|---|---|
| [CISA ICS Advisories](https://www.cisa.gov/news-events/ics-advisories) | Regular industrial-product vulnerability advisories. |
| [SecurityWeek ICS/OT](https://www.securityweek.com/category/ics-ot/) | Dedicated reporting on ICS vulnerabilities, incidents and industrial security. |
| [The Record](https://therecord.media/) | Cybersecurity reporting with strong ransomware and critical-infrastructure coverage. |
| [Dragos Blog](https://www.dragos.com/blog/) | Industrial threat intelligence and defensive analysis. |
| [Claroty Team82](https://claroty.com/team82) | Technical vulnerability research. |
| [Nozomi Networks Labs](https://www.nozominetworks.com/labs) | OT threat and vulnerability research. |
| [NCSC](https://www.ncsc.gov.uk/) | UK cybersecurity advisories, guidance and threat information. |

## UK OT and critical-infrastructure resources

| Resource | Relevance |
|---|---|
| [National Cyber Security Centre](https://www.ncsc.gov.uk/) | UK national technical authority for cybersecurity guidance and threat information. |
| [NCSC Cyber Assessment Framework](https://www.ncsc.gov.uk/collection/cyber-assessment-framework) | Outcome-based framework widely used around UK essential services and CNI. |
| [RITICS](https://www.ritics.org/) | UK research community focused on trustworthy and resilient cyber-physical systems. |
| [UK Cyber Security Council](https://www.ukcybersecuritycouncil.org.uk/) | Professional standards, career pathways and chartered recognition. |
| [Institution of Engineering and Technology](https://www.theiet.org/) | Engineering professional body spanning cybersecurity, control systems, transport, energy and infrastructure. |

## Professional organisations and communities

| Resource | Focus |
|---|---|
| [International Society of Automation](https://www.isa.org/) | Automation, control-system engineering and industrial cybersecurity. |
| [ISA99](https://www.isa.org/standards-and-publications/isa-standards/isa-standards-committees/isa99) | Standards committee behind the ISA/IEC 62443 series. |
| [ISASecure](https://isasecure.org/) | Industrial cybersecurity certification and assurance schemes. |
| [ICS Village](https://www.icsvillage.com/) | Practical ICS security education and community activity. |
| [IET](https://www.theiet.org/) | Professional engineering institution covering cybersecurity and industrial systems. |
| [UK Cyber Security Council](https://www.ukcybersecuritycouncil.org.uk/) | UK cybersecurity professionalisation and career development. |

## Keeping this directory updated

OT/ICS cybersecurity changes continuously. Standards evolve, vendors release advisories, new labs appear, projects become unmaintained and threat research changes what practitioners need to understand.

I will periodically review this directory to add useful resources, replace dead links and remove material that is no longer relevant or maintained.

If you know of an OT/ICS cybersecurity resource that genuinely deserves to be here, feel free to [connect with me on LinkedIn](https://www.linkedin.com/in/swanoop-r/) and suggest it.

---

*This directory is curated for learning and reference. Inclusion does not imply endorsement of a commercial product, course, certification or individual.*
