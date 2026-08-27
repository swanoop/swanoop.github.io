---
layout: post
title: "OT/ICS Cybersecurity Resources Directory"
description: "A curated OT and ICS cybersecurity resources directory covering IEC 62443, NIST guidance, certifications, training, books, labs, industrial protocols, tools, datasets, threat intelligence and UK critical infrastructure resources."
date: 2026-08-27
category: "OT / ICS"
tags:
  - OT Cybersecurity
  - ICS Security
  - IEC 62443
  - Industrial Cybersecurity
  - Training
  - Resources
read_time: 18
---

A curated directory of useful **Operational Technology (OT)** and **Industrial Control System (ICS) cybersecurity** resources: standards, books, certifications, training, labs, industrial protocols, tools, datasets, threat intelligence, conferences and practitioners worth following.

<span class="directory-updated">Last reviewed: 27 August 2026</span>

This is a reference directory, not a prescribed learning path. Resources are selected for practical value, technical relevance or usefulness as a trusted reference.

<div class="directory-tools">
  <input id="directorySearch" class="directory-search" type="search" placeholder="Search resources — e.g. IEC 62443, Modbus, Wireshark, CISA, GICSP…" aria-label="Search OT cybersecurity resources">
  <span id="directoryCount" class="directory-count"></span>
</div>

## Jump to a section

<div class="directory-toc">
<a href="#standards"><span>01</span> Standards, frameworks & guidance</a>
<a href="#iec62443"><span>02</span> ISA/IEC 62443 reference</a>
<a href="#certifications"><span>03</span> Certifications & professional training</a>
<a href="#free-training"><span>04</span> Free training & education</a>
<a href="#books"><span>05</span> Books</a>
<a href="#labs"><span>06</span> Labs & cyber ranges</a>
<a href="#network-analysis"><span>07</span> Network & protocol analysis</a>
<a href="#protocol-resources"><span>08</span> Industrial protocol resources</a>
<a href="#protocols"><span>09</span> Protocols worth knowing</a>
<a href="#datasets"><span>10</span> PCAPs & datasets</a>
<a href="#tools"><span>11</span> OT security tools</a>
<a href="#platforms"><span>12</span> Commercial OT security platforms</a>
<a href="#advisories"><span>13</span> Vulnerability & security advisories</a>
<a href="#threat-intel"><span>14</span> Threat intelligence & research</a>
<a href="#incidents"><span>15</span> OT malware & incidents to study</a>
<a href="#github"><span>16</span> GitHub collections & projects</a>
<a href="#people"><span>17</span> People to follow</a>
<a href="#conferences"><span>18</span> Conferences & events</a>
<a href="#podcasts"><span>19</span> Podcasts & video</a>
<a href="#reading"><span>20</span> News & regular reading</a>
<a href="#uk"><span>21</span> UK OT & critical infrastructure</a>
<a href="#communities"><span>22</span> Professional organisations & communities</a>
</div>

## Standards, Frameworks & Guidance
{: #standards}

| Resource | Description |
| --- | --- |
| [ISA/IEC 62443](https://www.isa.org/standards-and-publications/isa-standards/isa-iec-62443-series-of-standards) | International standards series covering cybersecurity across the lifecycle of industrial automation and control systems (IACS). |
| [NIST SP 800-82 Rev. 3](https://csrc.nist.gov/pubs/sp/800/82/r3/final) | NIST guidance for securing operational technology, including ICS, SCADA, DCS and PLC environments. |
| [MITRE ATT&CK for ICS](https://attack.mitre.org/matrices/ics/) | Knowledge base of adversary tactics and techniques observed against industrial control systems. |
| [NCSC Cyber Assessment Framework](https://www.ncsc.gov.uk/collection/cyber-assessment-framework) | UK framework for assessing cybersecurity and resilience of organisations providing essential functions. |
| [CISA Industrial Control Systems](https://www.cisa.gov/topics/industrial-control-systems) | US government guidance, advisories, tools and resources for ICS and critical infrastructure security. |
| [CISA Cybersecurity Performance Goals](https://www.cisa.gov/cybersecurity-performance-goals) | Prioritised baseline practices intended to reduce risk across critical infrastructure, including OT. |
| [CIS Critical Security Controls](https://www.cisecurity.org/controls) | Prioritised safeguards that can support broader IT and OT cybersecurity programmes when appropriately adapted. |
| [ISO/IEC 27001](https://www.iso.org/isoiec-27001-information-security.html) | International standard for information security management systems and organisational security governance. |
| [IEC 61850](https://webstore.iec.ch/en/publication/6028) | Standards series for communication networks and systems used extensively in power utility automation. |
{: .resource-table}

## ISA/IEC 62443 Reference
{: #iec62443}

| Standard / Resource | What it covers |
| --- | --- |
| [IEC 62443-2-1](https://www.isa.org/standards-and-publications/isa-standards/isa-iec-62443-series-of-standards) | Security programme requirements for IACS asset owners. |
| [IEC 62443-2-4](https://www.isa.org/standards-and-publications/isa-standards/isa-iec-62443-series-of-standards) | Security programme requirements for IACS service providers. |
| [IEC 62443-3-2](https://www.isa.org/standards-and-publications/isa-standards/isa-iec-62443-series-of-standards) | Security risk assessment, System Under Consideration, zones and conduits, and target security levels. |
| [IEC 62443-3-3](https://www.isa.org/standards-and-publications/isa-standards/isa-iec-62443-series-of-standards) | System security requirements and security levels. |
| [IEC 62443-4-1](https://www.isa.org/standards-and-publications/isa-standards/isa-iec-62443-series-of-standards) | Secure product development lifecycle requirements. |
| [IEC 62443-4-2](https://www.isa.org/standards-and-publications/isa-standards/isa-iec-62443-series-of-standards) | Technical security requirements for IACS components. |
| [ISA99 Committee](https://www.isa.org/standards-and-publications/isa-standards/isa-standards-committees/isa99) | ISA committee responsible for developing and maintaining the ISA/IEC 62443 series. |
| [ISASecure](https://isasecure.org/) | Industrial cybersecurity certification and assurance schemes based on ISA/IEC 62443. |
{: .resource-table}

## Certifications & Professional Training
{: #certifications}

| Resource | Description |
| --- | --- |
| [ISA/IEC 62443 IC32](https://www.isa.org/training/course-description/ic32) | Cybersecurity Fundamentals Specialist covering core industrial cybersecurity concepts and the 62443 series. |
| [ISA/IEC 62443 IC33](https://www.isa.org/training/course-description/ic33) | Cybersecurity Risk Assessment Specialist focused on assessment of new or existing IACS. |
| [ISA/IEC 62443 IC34](https://www.isa.org/training/course-description/ic34) | Cybersecurity Design Specialist covering secure industrial system design and implementation. |
| [ISA/IEC 62443 IC37](https://www.isa.org/training/course-description/ic37) | Cybersecurity Maintenance Specialist focused on secure IACS operations and maintenance. |
| [ISA/IEC 62443 Cybersecurity Expert](https://www.isa.org/certification/certificate-programs/isa-iec-62443-cybersecurity-certificate-program) | ISA designation awarded after completing all four specialist certificates. |
| [ISASecure ACSSA for Evaluators](https://www.isa.org/certification/certificate-programs) | Specialist programme for assessing operating automation and control systems against applicable IEC 62443 requirements. |
| [GIAC GICSP](https://www.giac.org/certifications/global-industrial-cyber-security-professional-gicsp) | Broad industrial cybersecurity certification combining cybersecurity, engineering and operational concepts. |
| [SANS ICS410](https://www.sans.org/cyber-security-courses/ics-scada-cyber-security-essentials/) | ICS/SCADA security fundamentals and preparation for GICSP. |
| [SANS ICS515](https://www.sans.org/cyber-security-courses/ics-visibility-detection-response/) | Industrial network visibility, threat detection, threat hunting and incident response. |
| [GIAC GRID](https://www.giac.org/certifications/response-industrial-defense-grid/) | Certification focused on industrial detection, defence and incident response. |
| [GIAC GCIP](https://www.giac.org/certifications/critical-infrastructure-protection-gcip) | Critical infrastructure protection certification with strong relevance to electric-sector NERC CIP environments. |
{: .resource-table}

## Free Training & Education
{: #free-training}

| Resource | Description |
| --- | --- |
| [CISA ICS Training](https://www.cisa.gov/resources-tools/programs/ics-training-available-through-cisa) | Free ICS cybersecurity training covering industrial systems, defence, assessment and hands-on exercises. |
| [CISA ICS Training Calendar](https://www.cisa.gov/ics-training-calendar) | Current schedule for CISA ICS virtual and instructor-led courses. |
| [Mike Holcomb / UtilSec](https://www.utilsec.com/) | Extensive free OT/ICS cybersecurity tutorials, courses and practical learning material. |
| [TryHackMe — Introduction to the World of OT/ICS](https://tryhackme.com/room/introductiontotheworldofotics) | Interactive introduction to PLCs, HMIs, industrial architectures and OT security. |
| [SANS ICS Library](https://www.sans.org/blog/industrial-control-systems-library) | Free ICS/OT posters, whitepapers, defence use cases and reference material. |
| [SANS ICS/OT Resources](https://www.sans.org/cybersecurity-focus-areas/industrial-control-systems-security) | Webcasts, papers, posters, videos and other industrial cybersecurity material. |
| [S4 Events](https://s4xevents.com/) | Technical ICS/OT cybersecurity conference presentations and research. |
| [ICS Village](https://www.icsvillage.com/) | Hands-on educational resources and demonstrations focused on industrial control system security. |
{: .resource-table}

## Books
{: #books}

| Title | Why it is useful |
| --- | --- |
| [Industrial Network Security — Eric D. Knapp](https://shop.elsevier.com/books/industrial-network-security/knapp/978-0-443-13737-2) | Industrial networks, protocols, architectures and ICS security fundamentals. The third edition is the current edition. |
| [Industrial Cybersecurity — Pascal Ackerman](https://www.packtpub.com/en-gb/product/industrial-cybersecurity-9781800202092) | Practical coverage of industrial architecture, monitoring, assessment, threat hunting and incident response. |
| **Hacking Exposed: Industrial Control Systems** | Technical coverage of ICS attack surfaces, protocols, vulnerabilities and security testing. |
| **Practical Industrial Cybersecurity — Charles J. Brooks & Philip A. Craig Jr.** | Accessible treatment of industrial cybersecurity, risk management and secure architecture. |
| [Engineering-Grade OT Security — Andrew Ginter](https://books.google.com/books/about/Engineering_Grade_OT_Security_A_manager.html?id=yLrrEAAAQBAJ) | Engineering and consequence-driven perspective on OT cyber risk and protection. |
| **Implementing IEC 62443: A Pragmatic Approach to Cybersecurity — Medoff & O'Brien** | Practical guidance for organisations applying IEC 62443. |
| [Industrial Cybersecurity: Case Studies and Best Practices — Steve Mustard](https://www.wiley-vch.de/en/areas-interest/engineering/industrial-cybersecurity-978-1-64331-154-8) | Governance, design, implementation and operational security through industrial case studies. |
| [Countering Cyber Sabotage — Andrew Bochman & Sarah Freeman](https://www.oreilly.com/library/view/countering-cyber-sabotage/9781000292978/) | Introduces Consequence-Driven, Cyber-Informed Engineering for critical infrastructure. |
| **Pentesting Industrial Control Systems — Paul Smith** | Practical security testing of ICS environments and industrial protocols. |
| **Applied Cyber Security and the Smart Grid — Eric D. Knapp & Raj Samani** | Cybersecurity applied to power systems and smart-grid infrastructure. |
| [Countdown to Zero Day — Kim Zetter](https://www.penguinrandomhouse.com/books/316238/countdown-to-zero-day-by-kim-zetter/) | Investigation of Stuxnet and the compromise of Iran's nuclear enrichment programme. |
| [Sandworm — Andy Greenberg](https://www.penguinrandomhouse.com/books/597684/sandworm-by-andy-greenberg/) | Investigation of destructive cyber operations against critical infrastructure, including Ukraine's electricity network. |
{: .resource-table}

## Labs & Cyber Ranges
{: #labs}

<div class="directory-note"><strong>Safety:</strong> keep offensive testing, active scanning and protocol manipulation inside isolated labs or environments where you have explicit authorisation. Production OT can be fragile, safety-critical and intolerant of conventional IT security testing.</div>

| Resource | Description |
| --- | --- |
| [OpenPLC](https://github.com/thiagoralves/OpenPLC_v3) | Open-source PLC runtime and programming environment useful for automation and cybersecurity labs. |
| [Labshock](https://github.com/zakharb/labshock) | Container-based OT security lab with PLC, SCADA, EWS, DMZ, telemetry and security components. |
| [GRFICSv3](https://github.com/Fortiphyd/GRFICSv3) | Free OT cyber range combining realistic networking with a 3D industrial process simulation. |
| [Conpot](https://github.com/mushorg/conpot) | Open-source ICS/SCADA honeypot supporting industrial protocols and attacker-behaviour research. |
| [MiniCPS](https://github.com/scy-phy/minicps) | Framework for cyber-physical system simulation combining process, control-device and network emulation. |
| [FUXA](https://github.com/frangoteam/fuxa) | Open-source web-based SCADA/HMI platform supporting Modbus, OPC UA, S7, BACnet, MQTT and EtherNet/IP. |
| [Factory I/O](https://factoryio.com/) | 3D industrial process simulator capable of communicating with physical and simulated PLCs. |
{: .resource-table}

## Network & Protocol Analysis
{: #network-analysis}

| Resource | Description |
| --- | --- |
| [Wireshark](https://www.wireshark.org/) | Packet capture and analysis with dissectors for many industrial protocols. |
| [Zeek](https://zeek.org/) | Network security monitoring and rich traffic-analysis framework. |
| [Suricata](https://suricata.io/) | Open-source IDS/IPS and network security monitoring engine. |
| [Snort](https://www.snort.org/) | Network intrusion detection and prevention platform. |
| [tcpdump](https://www.tcpdump.org/) | Command-line packet capture and network troubleshooting utility. |
| [NetworkMiner](https://www.netresec.com/?page=NetworkMiner) | Network forensic analysis tool for PCAPs, hosts, sessions and extracted artefacts. |
{: .resource-table}

## Industrial Protocol Resources
{: #protocol-resources}

| Resource | Description |
| --- | --- |
| [Modbus Organization](https://www.modbus.org/specifications) | Official Modbus specifications and implementation guides. |
| [OPC Foundation](https://opcfoundation.org/) | Specifications and resources for OPC Classic and OPC UA. |
| [ODVA](https://www.odva.org/) | Specifications and technical resources for CIP, EtherNet/IP and related technologies. |
| [DNP Users Group](https://www.dnp.org/) | Technical resources relating to DNP3. |
| [IEC 61850](https://webstore.iec.ch/en/publication/6028) | Communication standards for power utility and electrical substation automation. |
| [PROFIBUS & PROFINET International](https://www.profibus.com/) | Technical resources for PROFINET, PROFIBUS and related industrial networking technologies. |
| [BACnet International](https://bacnetinternational.org/) | Resources for BACnet and building automation communications. |
| [MQTT 5.0 — OASIS](https://www.oasis-open.org/standard/mqtt-v5-0-os/) | Official MQTT standard used widely in IoT, IIoT and telemetry systems. |
| [Awesome Industrial Protocols](https://github.com/Orange-Cyberdefense/awesome-industrial-protocols) | Security-oriented collection covering dozens of industrial network protocols. |
{: .resource-table}

## Industrial Protocols Worth Knowing
{: #protocols}

| Protocol | Common use |
| --- | --- |
| Modbus TCP / RTU | PLC, SCADA and field-device communications. |
| OPC UA | Industrial data exchange and interoperability. |
| DNP3 | Electric utilities and SCADA systems. |
| IEC 60870-5-104 | Power-system telecontrol and utility communications. |
| IEC 61850 | Electrical substation automation and protection. |
| PROFINET | Industrial automation and manufacturing. |
| PROFIBUS | Industrial fieldbus communication. |
| EtherNet/IP | Industrial Ethernet, particularly within Rockwell environments. |
| CIP | Industrial device communication and control. |
| S7comm | Siemens PLC communications. |
| BACnet | Building management systems and building automation. |
| HART | Process instrumentation and field-device communications. |
| MQTT | IoT, IIoT and industrial telemetry. |
{: .resource-table}

## PCAPs & Datasets
{: #datasets}

| Resource | Description |
| --- | --- |
| [Wireshark Sample Captures](https://www.wireshark.org/resources) | Public packet captures for learning protocol analysis. |
| [Netresec PCAP Files](https://www.netresec.com/?page=PcapFiles) | Public network forensic datasets and packet captures. |
| [SWaT Dataset](https://itrust.sutd.edu.sg/itrust-labs_datasets/) | Dataset generated from the Secure Water Treatment cyber-physical testbed. |
| [WADI Dataset](https://itrust.sutd.edu.sg/itrust-labs_datasets/) | Water Distribution testbed dataset used in ICS anomaly-detection research. |
| [HAI Dataset](https://github.com/icsdataset/hai) | Industrial control system dataset designed for anomaly-detection and security research. |
{: .resource-table}

## OT Security Tools
{: #tools}

| Resource | Description |
| --- | --- |
| [Nmap](https://nmap.org/) | Network discovery and service identification. Use active scanning cautiously and only with approval in operational OT. |
| [Scapy](https://scapy.net/) | Python packet-manipulation framework useful for protocol analysis and controlled security research. |
| [pymodbus](https://github.com/pymodbus-dev/pymodbus) | Python Modbus implementation useful for clients, servers and lab environments. |
| [Snap7](https://snap7.sourceforge.net/) | Communication library for interacting with Siemens S7 systems in controlled environments. |
| [CISA CSET](https://github.com/cisagov/cset) | Cyber Security Evaluation Tool for assessing cybersecurity practices and architectures. |
{: .resource-table}

## Commercial OT Security Platforms
{: #platforms}

Examples below are included as market references, **not endorsements**.

| Resource | Focus |
| --- | --- |
| [Dragos Platform](https://www.dragos.com/platform/) | OT asset visibility, threat detection, vulnerability management and industrial threat intelligence. |
| [Claroty](https://claroty.com/) | Cyber-physical asset visibility, exposure management and threat detection. |
| [Nozomi Networks](https://www.nozominetworks.com/) | OT/IoT visibility, monitoring and threat detection. |
| [Microsoft Defender for IoT](https://www.microsoft.com/en-us/security/business/endpoint-security/microsoft-defender-iot) | OT and IoT asset discovery, monitoring and integration with Microsoft's security ecosystem. |
| [Tenable OT Security](https://www.tenable.com/products/ot-security) | OT asset visibility, vulnerability management and exposure assessment. |
| [TXOne Networks](https://www.txone.com/) | Security technologies designed specifically for industrial endpoints and OT networks. |
| [Forescout](https://www.forescout.com/) | Device visibility and control across IT, IoT and OT environments. |
{: .resource-table}

## Vulnerability & Security Advisories
{: #advisories}

| Resource | Description |
| --- | --- |
| [CISA ICS Advisories](https://www.cisa.gov/news-events/ics-advisories) | Vulnerability advisories affecting industrial automation and control-system products. |
| [National Vulnerability Database](https://nvd.nist.gov/) | NIST vulnerability database containing CVE and CVSS information. |
| [CVE](https://www.cve.org/) | Global catalogue of publicly disclosed cybersecurity vulnerabilities. |
| [Siemens ProductCERT](https://www.siemens.com/global/en/products/services/cert.html) | Product security advisories for Siemens technologies. |
| [Schneider Electric Security Notifications](https://www.se.com/ww/en/work/support/cybersecurity/security-notifications.jsp) | Vulnerability and cybersecurity notifications for Schneider Electric products. |
| [Rockwell Automation Security Advisories](https://www.rockwellautomation.com/en-us/trust-center/security-advisories.html) | Product security advisories for Rockwell Automation technologies. |
| [ABB Cybersecurity Alerts & Notifications](https://global.abb/group/en/technology/cyber-security/alerts-and-notifications) | ABB product cybersecurity advisories and security information. |
{: .resource-table}

## Threat Intelligence & Research
{: #threat-intel}

| Resource | Description |
| --- | --- |
| [Dragos](https://www.dragos.com/resources/) | Industrial threat intelligence, malware analysis, incident research and annual OT security reports. |
| [Claroty Team82](https://claroty.com/team82) | Vulnerability research covering OT, IoT, medical devices and other cyber-physical systems. |
| [Nozomi Networks Labs](https://www.nozominetworks.com/labs) | Research covering OT malware, vulnerabilities and industrial threat activity. |
| [Forescout Research — Vedere Labs](https://www.forescout.com/research-labs/) | Research into vulnerabilities affecting connected, IoT and OT devices. |
| [Google Threat Intelligence / Mandiant](https://cloud.google.com/blog/topics/threat-intelligence) | Threat intelligence and incident-response research, including critical infrastructure campaigns. |
| [Unit 42](https://unit42.paloaltonetworks.com/) | Threat-actor, malware and vulnerability research. |
| [Microsoft Security Blog](https://www.microsoft.com/en-us/security/blog/) | Threat intelligence covering nation-state activity and attacks against critical infrastructure. |
| [RITICS](https://ritics.org/) | UK research focused on trustworthy and resilient cyber-physical critical systems. |
{: .resource-table}

## OT Malware & Incidents to Study
{: #incidents}

| Incident / Malware | Why it matters |
| --- | --- |
| Stuxnet | Purpose-built malware manipulating Siemens industrial control systems while concealing process changes. |
| Havex | Cyberespionage campaign targeting organisations operating industrial control systems. |
| BlackEnergy | Malware associated with attacks against Ukrainian electricity infrastructure. |
| Industroyer / CrashOverride | Malware framework designed to interact directly with electric-grid protocols. |
| Industroyer2 | Later industrial malware used against Ukrainian electricity infrastructure. |
| TRITON / TRISIS | Malware targeting Schneider Electric Triconex Safety Instrumented Systems. |
| PIPEDREAM / INCONTROLLER | Industrial attack framework capable of interacting with multiple OT technologies. |
| FrostyGoop | Industrial malware associated with disruption involving Modbus communications. |
| Oldsmar Water Treatment | Intrusion involving unauthorised remote interaction with a water-treatment control environment. |
| Colonial Pipeline | Ransomware incident demonstrating how enterprise IT compromise can cause major operational consequences. |
| Norsk Hydro | Large-scale ransomware incident affecting global industrial operations. |
{: .resource-table}

## GitHub Collections & Projects
{: #github}

| Resource | Description |
| --- | --- |
| [Cybersecurity-OT](https://github.com/paulveillard/cybersecurity-OT) | Community-curated collection of OT/ICS tools, research, datasets, labs and learning resources. |
| [Awesome Industrial Control System Security](https://github.com/hslatman/awesome-industrial-control-system-security) | Established curated collection of ICS security tools, papers, books and projects. |
| [Awesome Industrial Protocols](https://github.com/Orange-Cyberdefense/awesome-industrial-protocols) | Security-oriented collection of industrial protocol specifications, tools, PCAPs and research. |
| [OpenPLC](https://github.com/thiagoralves/OpenPLC_v3) | Open-source PLC environment suitable for industrial cybersecurity labs. |
| [GRFICSv3](https://github.com/Fortiphyd/GRFICSv3) | Open-source industrial cybersecurity simulation environment. |
| [Conpot](https://github.com/mushorg/conpot) | Open-source ICS honeypot. |
| [MiniCPS](https://github.com/scy-phy/minicps) | Cyber-physical system simulation framework. |
| [MITRE ATT&CK](https://github.com/mitre-attack) | Open ATT&CK datasets and supporting projects. |
{: .resource-table}

## People to Follow
{: #people}

| Person | Focus |
| --- | --- |
| Robert M. Lee | ICS threat intelligence, incident response, adversary activity and industrial defence. |
| Dale Peterson | ICS security research, S4 and industrial cybersecurity industry analysis. |
| Sarah Fluchs | IEC 62443, OT security engineering, risk and European cyber regulation. |
| Lesley Carhart | Industrial incident response, digital forensics and threat hunting. |
| Mike Holcomb | OT/ICS cybersecurity education, labs and practical training. |
| Joel Langill | Industrial control engineering and cybersecurity. |
| Ralph Langner | Industrial cybersecurity and Stuxnet research. |
| Marina Krotofil | Industrial security research and cyber-physical attack techniques. |
| Chris Sistrunk | ICS cybersecurity, industrial network defence and incident response. |
| Andrew Ginter | Engineering-focused OT security and industrial network architecture. |
{: .resource-table}

## Conferences & Events
{: #conferences}

| Resource | Description |
| --- | --- |
| [S4](https://s4xevents.com/) | One of the leading technical conferences dedicated to ICS and OT cybersecurity. |
| [SANS ICS Security Summit](https://www.sans.org/cyber-security-training-events/ics-security-summit/) | Practitioner-focused event covering industrial defence, incident response and threat detection. |
| [BSidesICS/OT](https://bsidesics.org/) | Community-driven security event focused specifically on ICS and OT. |
| [ICS Cybersecurity Conference](https://www.icscybersecurityconference.com/) | Long-running conference dedicated to industrial cybersecurity and critical infrastructure. |
| [ICS Village](https://www.icsvillage.com/) | Hands-on industrial security demonstrations, training and community events. |
| [CS3STHLM](https://www.cs3sthlm.se/) | Conference focused on cybersecurity of industrial control systems and critical infrastructure. |
| [Black Hat](https://www.blackhat.com/) | Security conference regularly featuring ICS, embedded and critical-infrastructure research. |
| [DEF CON](https://defcon.org/) | Security conference featuring ICS, hardware, embedded and cyber-physical security research. |
{: .resource-table}

## Podcasts & Video
{: #podcasts}

| Resource | Description |
| --- | --- |
| [Unsolicited Response](https://dale-peterson.com/) | Dale Peterson's interviews and discussions with researchers and practitioners across the OT security community. |
| [The Industrial Security Podcast](https://waterfall-security.com/industrial-security-podcast/) | Conversations covering industrial cybersecurity, engineering and critical infrastructure. |
| [Nexus: A Claroty Podcast](https://claroty.com/nexus) | Interviews covering OT, IoT, cyber-physical security and industrial research. |
| [Mike Holcomb / UtilSec](https://www.youtube.com/@UtilSec) | Free OT cybersecurity tutorials, courses and lab walkthroughs. |
| [SANS ICS](https://www.youtube.com/@SANSInstitute) | Industrial cybersecurity presentations, webinars and technical education. |
| [S4 Events](https://www.youtube.com/@S4Events) | Conference presentations from industrial cybersecurity researchers and practitioners. |
{: .resource-table}

## OT Cybersecurity News & Regular Reading
{: #reading}

| Resource | Description |
| --- | --- |
| [CISA ICS Advisories](https://www.cisa.gov/news-events/ics-advisories) | Regular vulnerability advisories affecting industrial systems and products. |
| [SecurityWeek ICS/OT](https://www.securityweek.com/category/ics-ot/) | Reporting dedicated to ICS vulnerabilities, incidents and industrial security. |
| [The Record](https://therecord.media/) | Cybersecurity reporting with strong coverage of ransomware and critical infrastructure. |
| [Dragos Blog & Resources](https://www.dragos.com/resources/) | Industrial threat intelligence and defensive analysis. |
| [Claroty Team82](https://claroty.com/team82) | Vulnerability research and technical analysis of cyber-physical systems. |
| [Nozomi Networks Labs](https://www.nozominetworks.com/labs) | OT threat research, vulnerabilities and malware analysis. |
| [NCSC](https://www.ncsc.gov.uk/) | UK cybersecurity advisories, guidance and threat information. |
{: .resource-table}

## UK OT & Critical Infrastructure Resources
{: #uk}

| Resource | Description |
| --- | --- |
| [National Cyber Security Centre](https://www.ncsc.gov.uk/) | UK government's national technical authority for cybersecurity guidance and threat information. |
| [NCSC Cyber Assessment Framework](https://www.ncsc.gov.uk/collection/cyber-assessment-framework) | Framework used to assess cybersecurity and resilience of UK essential functions and CNI-related sectors. |
| [RITICS](https://ritics.org/) | UK research community focused on trustworthy and resilient cyber-physical critical systems. |
| [UK Cyber Security Council](https://www.ukcybersecuritycouncil.org.uk/) | Professional standards, career pathways and chartered recognition for UK cybersecurity practitioners. |
| [Institution of Engineering and Technology](https://www.theiet.org/) | Engineering professional body spanning cybersecurity, control systems, transport, energy and critical infrastructure. |
{: .resource-table}

## Professional Organisations & Communities
{: #communities}

| Resource | Description |
| --- | --- |
| [International Society of Automation](https://www.isa.org/) | Professional organisation focused on automation, control-system engineering and industrial cybersecurity. |
| [ISA99](https://www.isa.org/standards-and-publications/isa-standards/isa-standards-committees/isa99) | Standards committee responsible for the ISA/IEC 62443 cybersecurity series. |
| [ISASecure](https://isasecure.org/) | Industrial cybersecurity certification and assurance programme. |
| [ICS Village](https://www.icsvillage.com/) | Community promoting practical ICS cybersecurity education and hands-on learning. |
| [IET](https://www.theiet.org/) | Professional engineering institution covering cybersecurity and industrial systems. |
| [UK Cyber Security Council](https://www.ukcybersecuritycouncil.org.uk/) | UK professional body supporting cybersecurity professionalisation and career development. |
{: .resource-table}

## Keeping This Directory Updated

OT/ICS cybersecurity changes continuously. New vulnerabilities, standards, research, tools, laboratories, courses and community resources appear regularly, while older material can become outdated or unmaintained.

This directory will be reviewed periodically to add useful resources, replace broken or outdated links, and remove material that is no longer relevant.

If you know of a strong OT/ICS cybersecurity resource that belongs here, feel free to suggest it.

*Structure inspired in part by the community-curated [Cybersecurity-OT](https://github.com/paulveillard/cybersecurity-OT) and [Awesome Industrial Control System Security](https://github.com/hslatman/awesome-industrial-control-system-security) collections.*

<script>
(function(){
  const input=document.getElementById('directorySearch');
  const count=document.getElementById('directoryCount');
  if(!input||!count)return;
  const rows=[...document.querySelectorAll('table.resource-table tbody tr')];
  function update(){
    const q=input.value.trim().toLowerCase();
    let visible=0;
    rows.forEach(row=>{
      const match=!q||row.textContent.toLowerCase().includes(q);
      row.style.display=match?'':'none';
      if(match)visible++;
    });
    count.textContent=q?`${visible} matches`:`${rows.length} resources`;
  }
  input.addEventListener('input',update);
  update();
})();
</script>
