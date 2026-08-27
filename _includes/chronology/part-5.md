## The pattern across sixteen years of OT attacks

Looking chronologically at these incidents produces a different picture from looking only at industrial malware families.

Stuxnet demonstrated that a highly resourced adversary could understand an industrial process, compromise its engineering environment, change PLC logic and deliberately damage equipment. Ukraine demonstrated that attackers did not necessarily need to develop that level of bespoke malware: once inside an operational network, stolen credentials and legitimate operator interfaces could be enough to switch electricity off.

Industroyer took another route and spoke the protocols used by the grid. Triton moved from production control to the safety layer. Havex showed the value of silently collecting the engineering information required to prepare future attacks.

Then the threat broadened.

NotPetya, Norsk Hydro and Colonial Pipeline showed that attackers can stop industrial operations without touching a PLC. CyberAv3ngers and the later pro-Russian campaigns demonstrated almost the opposite extreme: attackers may not need sophisticated malware at all when controllers, HMIs and remote-access interfaces are exposed with weak authentication.

FrostyGoop returned attention to native industrial protocols. The 2025 Polish campaign showed coordinated destructive activity simultaneously targeting traditional IT systems and physical industrial equipment. The 2026 US water campaign has again shown that basic internet exposure of field controllers can translate directly into loss of process visibility, water pressure and physical flooding.

The historical record therefore does not support the idea that OT defence is primarily a race to patch CVEs.

Some attacks certainly depended on vulnerabilities. Stuxnet used several. NotPetya weaponised already patched SMB flaws. The Danish energy campaign exploited CVE-2023-28771 at scale.

But other incidents succeeded because an attacker obtained legitimate credentials, reached an HMI, found a controller exposed to the internet, abused an industrial protocol, compromised a trusted supplier, crossed an inadequately controlled IT/OT boundary or discovered that a supposedly private communications network was not actually isolated.

The more useful attack tree for the history of OT security is therefore broader:

```text
                         PHYSICAL OR OPERATIONAL EFFECT
                                     │
                 ┌───────────────────┼───────────────────┐
                 │                   │                   │
          Direct OT access      IT dependency       OT malware
                 │                   │                   │
          HMI / PLC / EWS       Identity / ERP      Process-aware
                 │              / communications       capability
                 │                   │                   │
        ┌────────┼────────┐          │          ┌────────┼────────┐
        │        │        │          │          │        │        │
      Weak    Exposed   Stolen    IT outage   Native    CVE     Logic
      auth    service    creds    stops ops   protocol  exploit  change
        │        │        │          │          │        │        │
        └────────┴────────┴──────────┴──────────┴────────┴────────┘
                                     │
                             INDUSTRIAL CONSEQUENCE
```

That is the central lesson running from Natanz in 2010 to water utilities in 2026: **the attacker does not necessarily need to break the industrial process. The attacker needs a trusted path to something that can control it.**

---

## Where the record stands in August 2026

The chronology is still moving.

Industrial threat-intelligence teams reported further maturation during 2025. Dragos documented adversaries conducting deeper reconnaissance of control loops and continuing to develop capabilities intended to reach the second stage of the ICS Cyber Kill Chain, where knowledge of a specific industrial process is converted into an operational effect.

On 19 August 2026, the US National Security Agency also warned that cyber actors were conducting targeted reconnaissance and capability development against Siemens PLC environments used across critical manufacturing, energy, water, chemical and food sectors. That activity should currently be treated as an **active threat campaign**, not added to the list above as a successful physical attack.

That distinction matters. A professional incident history should separate what attackers *could* do, what they *attempted* to do and what forensic evidence shows they *actually did*.

The same standard should apply to attribution. “Russia-linked”, “Iran-linked” or “suspected Sandworm” are not interchangeable with an official government attribution. Likewise, the existence of a vulnerable product in an affected environment does not prove that a particular CVE was exploited.

This chronology will therefore need revision as investigations are completed, governments declassify evidence, researchers publish forensic findings and newly disclosed incidents become part of the public record.

## Selected primary and authoritative references

This chronology draws on government incident reporting, victim disclosures and technical research. Key sources include:

- [CISA — Primary Stuxnet Advisory](https://www.cisa.gov/uscert/ics/advisories/ICSA-10-272-01)
- [US Department of Justice — Bowman Avenue Dam intrusion](https://www.justice.gov/archives/opa/pr/seven-iranians-working-islamic-revolutionary-guard-corps-affiliated-entities-charged)
- [US Department of Justice — GRU charges covering the Ukraine power attacks and NotPetya](https://www.justice.gov/d9/press-releases/attachments/2020/10/19/2020_10_19_unsealed_indictment_0.pdf)
- [US Department of Justice — Triton/TRISIS critical-infrastructure campaign](https://www.justice.gov/usao-dc/pr/four-russian-government-employees-charged-two-historical-hacking-campaigns-targeting)
- [Norsk Hydro — 2019 cyberattack](https://www.hydro.com/en/global/media/on-the-agenda/cyber-attack/)
- [CISA/FBI — DarkSide ransomware and Colonial Pipeline](https://www.cisa.gov/sites/default/files/publications/AA21-131A_Darkside_Ransomware.pdf)
- [ESET — Industroyer2 research](https://www.eset.com/uk/research/)
- [CISA — CyberAv3ngers and Unitronics PLC compromises](https://www.cisa.gov/news-events/cybersecurity-advisories/aa23-335a)
- [CERT Polska — December 2025 energy-sector incident](https://cert.pl/en/posts/2026/01/incident-report-energy-sector-2025/)
- [CERT Polska — follow-up report and private-APN attack path](https://cert.pl/en/posts/2026/08/incident-follow-up-report-energy-sector-2025/)
- [FBI/EPA — 2026 attacks on internet-facing water-sector PLCs](https://www.fbi.gov/investigate/cyber/alerts/2026/malicious-cyber-actors-targeting-water-and-wastewater-sector-internet--facing-programmable-logic-controllers-causing-operational-disruptions)

For broader industry context, Dragos reported **1,693 ransomware attacks against industrial organisations in 2024**, an 87% year-on-year increase, with manufacturing remaining the hardest-hit sector. That dataset measures industrial ransomware activity and is different from the curated cyber-physical chronology above.

*Last updated: 1 September 2026. This article is intended as a living chronology of major publicly documented OT/ICS cyber incidents. It does not claim that every OT compromise is represented: many incidents are never disclosed publicly, and others are reported without sufficient technical evidence to reconstruct an attack path reliably.*
