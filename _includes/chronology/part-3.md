## 2022 — KA-SAT/Viasat: communications attack reaches thousands of wind turbines

**Target:** Viasat KA-SAT satellite network  
**Sector:** Telecommunications with energy-sector consequences  
**Type:** Infrastructure dependency / destructive cyberattack  
**Attribution:** Russian Federation  
**Malware:** AcidRain  
**Known campaign CVE:** No single publicly established CVE defines the attack

Approximately one hour before Russia began its full-scale invasion of Ukraine on 24 February 2022, a cyberattack disrupted Viasat's KA-SAT satellite network.

The European Union formally attributed the operation to Russia. Thousands of satellite modems were rendered inoperable, disrupting communications in Ukraine and elsewhere in Europe.

Among the collateral consequences was loss of remote monitoring connectivity to more than **5,800 wind turbines in Germany**. The turbines themselves had not been taken over; communications to them had been disrupted.

### Attack path

```text
Compromise satellite-network infrastructure
        ↓
Gain management capability affecting customer modems
        ↓
Deploy destructive AcidRain functionality
        ↓
Large number of modems become unusable
        ↓
Satellite communications lost
        ↓
Industrial customers lose remote connectivity/monitoring
```

KA-SAT belongs in an OT chronology because modern industrial systems increasingly depend on communications providers, cloud services, cellular networks and other infrastructure that sits outside the traditional plant boundary.

---

## 2022 — Industroyer2: Sandworm returns to the Ukrainian grid

**Target:** Ukrainian energy provider  
**Sector:** Electricity  
**Type:** Attempted direct OT disruption  
**Attribution:** Sandworm  
**Known CVE:** None required for the central IEC-104 manipulation

In April 2022, Ukrainian defenders and ESET disrupted another attempt to interfere with electricity infrastructure.

The attackers deployed **Industroyer2**, a more targeted descendant of the malware used in the 2016 Kyiv attack. It was configured to communicate with devices using IEC 60870-5-104. Other wipers were prepared to destroy systems in the surrounding Windows, Linux and Solaris environments.

### Attack path

```text
Initial compromise — not publicly established
        ↓
Gain presence inside electricity provider
        ↓
Prepare Industroyer2 for specific substation environment
        ↓
Schedule malicious IEC-104 activity
        ↓
Prepare wipers against supporting systems
        ↓
Attempt coordinated operational disruption
        ↓
Attack detected and interrupted
```

The attempt was stopped before the intended power outage was achieved.

Again, the core OT capability was not a clever memory-corruption exploit. The malware understood the industrial protocol and could issue messages that made sense to the equipment.

---

## 2022 — Predatory Sparrow and the Khouzestan steel mill

**Target:** Khouzestan Steel Company, Iran  
**Sector:** Steel manufacturing  
**Type:** Direct cyber-physical sabotage  
**Attribution:** Predatory Sparrow/Gonjeshke Darande; widely described as Israel-linked, but no formal Israeli acknowledgement  
**Known CVE:** None publicly established

On 27 June 2022, a cyberattack against an Iranian steel facility produced one of the clearest publicly visible examples of digital interference resulting in a dangerous industrial event.

Video subsequently released by the attackers showed molten metal spilling inside the Khouzestan facility and a fire developing. The group calling itself **Predatory Sparrow** claimed responsibility.

### Attack path

```text
Initial compromise — undisclosed
        ↓
Reach industrial production environment
        ↓
Gain sufficient process-control access
        ↓
Interfere with steel-production process
        ↓
Molten material released
        ↓
Fire and plant disruption
```

The precise technical route into the plant has never been publicly reconstructed to the level available for incidents such as Stuxnet or Ukraine.

Predatory Sparrow has also claimed disruptive attacks on Iranian fuel-distribution infrastructure and later financial targets. Reporting has repeatedly described the group as Israel-linked, although the Israeli government has not publicly confirmed control of the group.

---

## A 2022 event that did **not** become an attack: PIPEDREAM/INCONTROLLER

One development deserves inclusion precisely because defenders encountered it before a destructive incident occurred.

In 2022, researchers disclosed **PIPEDREAM**, also called INCONTROLLER, developed by the threat group Dragos tracks as CHERNOVITE. It contained capabilities for interacting with Schneider Electric and Omron controllers as well as CODESYS, Modbus and OPC UA environments.

Dragos assessed with high confidence that PIPEDREAM had **not yet been used to produce destructive effects in the wild** when it was discovered.

Later laboratory analysis showed part of the toolkit could leverage **CVE-2022-34151**, a hard-coded credential issue affecting certain Omron controllers. Other functionality relied simply on native industrial features rather than software vulnerabilities.

It therefore belongs in the history of OT threats, but not in a list of successful attacks.

---

## 2023 — Denmark: coordinated attacks compromise energy-sector infrastructure

**Targets:** Danish energy organisations  
**Sector:** Energy  
**Type:** Critical-infrastructure intrusion  
**Attribution:** Possible state involvement; Sandworm links discussed but not conclusively established  
**Known CVEs:** CVE-2023-28771; possible use of CVE-2023-33009/CVE-2023-33010 in later activity

In May 2023, Denmark's SektorCERT responded to what it described as the largest attack against Danish critical infrastructure at that time.

Twenty-two energy organisations were targeted. In the first wave, vulnerable Zyxel firewall appliances were attacked using **CVE-2023-28771**, an unauthenticated command-injection vulnerability. Eleven organisations were compromised during that phase.

A second wave followed. SektorCERT investigated indications that vulnerabilities which had not yet been publicly disclosed, later associated with **CVE-2023-33009 and CVE-2023-33010**, may have been involved, but the evidence did not permit a definitive conclusion.

### Attack path

```text
Internet-facing Zyxel firewalls
        ↓
Exploit CVE-2023-28771
        ↓
Compromise perimeter devices
        ↓
Collect configuration and credentials
        ↓
Establish access into energy organisations
        ↓
Further exploitation / attempted expansion
        ↓
Defenders isolate affected sites
```

Some organisations temporarily entered islanded operating modes, but Denmark avoided a major public power disruption.

Infrastructure used during part of the campaign had previously been associated with Sandworm activity. SektorCERT did not consider the evidence sufficient for definitive attribution, a distinction that should be retained when the incident is cited.

---

## 2023 — CyberAv3ngers attacks internet-facing Unitronics PLCs

**Targets:** Water and other infrastructure in the US and abroad  
**Sector:** Primarily water and wastewater  
**Type:** Direct PLC compromise  
**Attribution:** IRGC-affiliated CyberAv3ngers  
**Known CVE:** None required; exposed devices and weak/default authentication were central

In November 2023, operators began discovering messages on Unitronics Vision PLC/HMI devices stating that they had been hacked.

US agencies attributed the activity to **CyberAv3ngers**, an Iranian Islamic Revolutionary Guard Corps-affiliated persona. The targets included water utilities and other facilities using Israeli-made Unitronics equipment.

The joint government advisory found that attackers were exploiting devices exposed directly to the internet and, in many cases, protected by default or absent passwords. They could access the PLC/HMI, alter configurations, erase existing ladder logic and replace it with their own configuration.

### Attack path

```text
Internet scan for exposed Unitronics PLC/HMI
        ↓
Identify devices using weak/default authentication
        ↓
Log in remotely
        ↓
Change device configuration
        ↓
Remove or replace PLC logic / alter HMI
        ↓
Loss of legitimate control until recovery
```

The campaign is useful precisely because there was no sophisticated CVE chain. Basic exposure of industrial controllers to the internet gave a state-linked actor a route directly into control equipment.

The US Treasury subsequently sanctioned six officials associated with the IRGC Cyber-Electronic Command over cyber operations including PLC attacks.

---
