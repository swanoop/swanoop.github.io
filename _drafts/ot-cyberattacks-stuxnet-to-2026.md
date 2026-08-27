---
layout: post
title: "From Stuxnet to 2026: A Chronology of Major OT Cyberattacks"
description: "An evidence-based timeline of major OT and ICS cyberattacks from Stuxnet to 2026, including Ukraine, Triton, Industroyer, Colonial Pipeline, FrostyGoop and recent attacks on water and energy infrastructure."
date: 2026-09-01
category: "OT / ICS"
tags:
  - OT Cybersecurity
  - ICS Security
  - Industrial Cybersecurity
  - Stuxnet
  - IEC 62443
  - Critical Infrastructure
  - OT Malware
  - SCADA Security
read_time: 30
image: /assets/images/chronology/ot-attack-surface.svg
---

Cyber incidents involving operational technology are often compressed into the same headline: *hackers attacked critical infrastructure*. That is rarely precise enough.

Stuxnet altered PLC logic and damaged centrifuges. The 2015 Ukraine attack used legitimate control interfaces to open circuit breakers. Triton targeted a safety instrumented system. Colonial Pipeline, by contrast, found no evidence that its OT environment had been directly compromised; a ransomware attack on corporate IT still contributed to the decision to halt pipeline operations.

Those incidents belong in the same history, but they are **not the same kind of attack**.

This chronology separates **direct OT attacks**, **OT-capable intrusions**, and **IT-to-operations incidents**. Attack paths are reconstructed only where public evidence supports them. When initial access, a CVE or attribution remains unknown, it stays unknown.

> **Scope note:** the charts on this page describe the incidents selected for this chronology. They are not intended to represent all OT incidents globally; many industrial compromises are never publicly disclosed.

<div class="chronology-stats">
  <div><strong>24</strong><span>major incidents / campaigns</span></div>
  <div><strong>2010–2026</strong><span>period covered</span></div>
  <div><strong>6</strong><span>sector groupings represented</span></div>
  <div><strong>3</strong><span>cases where a CVE is central to the public attack path</span></div>
</div>

![Major OT cyber incidents included in this chronology by year]({{ '/assets/images/chronology/ot-incidents-by-year.svg' | relative_url }})

## What does the OT attack surface actually look like?

Across sixteen years of incidents, attackers repeatedly arrived through a surprisingly small set of paths: exposed control interfaces, remote-access systems, stolen credentials, enterprise IT, supplier software, communications infrastructure and trusted industrial protocols.

The controller is only one part of the attack surface. The engineering workstation that programs it, the HMI that operates it, the VPN used by a vendor, the Active Directory environment supporting engineers, and the private cellular network connecting a remote site can all become routes to operational consequence.

![OT attack surface showing external access paths, trust boundaries, control-system assets and physical process]({{ '/assets/images/chronology/ot-attack-surface.svg' | relative_url }})

This is also why a vulnerability count alone does not explain OT risk. In this selected chronology, **Stuxnet, NotPetya and the 2023 Denmark campaign** have clearly documented CVEs that form an important part of the public attack path. Many of the other incidents depended instead on legitimate credentials, exposed interfaces, native industrial functionality, compromised suppliers, weak segmentation or operational dependency on IT.

## Sector distribution in this chronology

Energy and water dominate the incidents selected here, which reflects the public record of major, well-documented cyber-physical events. It should **not** be read as a global prevalence chart. Separate industry reporting, particularly for ransomware affecting industrial organisations, consistently shows manufacturing as the largest target category.

![Sector distribution of major incidents included in this chronology]({{ '/assets/images/chronology/ot-sector-distribution.svg' | relative_url }})

## Attack-path matrix

| Route into operations | Representative incidents | What it demonstrates |
|---|---|---|
| **Internet-exposed controls / weak authentication** | Bowman Avenue Dam, CyberAv3ngers, 2026 US water PLC attacks | A sophisticated exploit is unnecessary when an operator or controller interface is already reachable. |
| **Credentials and trusted remote access** | 2015 Ukraine grid attack, Colonial Pipeline, 2024–25 pro-Russian activity | Legitimate access paths can become adversary conduits when identity and privilege controls fail. |
| **Native industrial protocols / legitimate control functions** | Industroyer, Industroyer2, FrostyGoop | Once inside the right network, valid industrial messages can become the attack mechanism. |
| **Supply-chain or supporting infrastructure** | Havex, NotPetya, KA-SAT | OT can be affected through suppliers, update systems, communications and other dependencies outside the plant. |
| **Process-aware malware / logic manipulation** | Stuxnet, Triton, 2025 Poland | The highest-impact attacks combine cyber access with knowledge of the physical process or its protection layers. |

![Attack-path matrix showing recurring routes from cyber access to operational consequence]({{ '/assets/images/chronology/ot-attack-path-matrix.svg' | relative_url }})

## Quick chronology

**2010** Stuxnet · **2012** Shamoon · **2013** Bowman Avenue · **2013–14** Havex · **2014** German steel mill · **2015** Ukraine power grid · **2016** Industroyer · **2017** Triton and NotPetya · **2019** Norsk Hydro · **2020** Israeli water · **2021** Oldsmar and Colonial Pipeline · **2022** KA-SAT, Industroyer2 and Predatory Sparrow · **2023** Denmark and CyberAv3ngers · **2024** FrostyGoop · **2024–25** pro-Russian OT activity · **2025** Norway and Poland · **2026** US water PLCs and UK generation.

---

{% include chronology/part-1.md %}
{% include chronology/part-2.md %}
{% include chronology/part-3.md %}
{% include chronology/part-4.md %}
{% include chronology/part-5.md %}
