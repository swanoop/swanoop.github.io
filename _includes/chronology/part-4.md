## 2024 — FrostyGoop: heating disrupted through Modbus

**Target:** Municipal district-heating organisation, Lviv, Ukraine  
**Sector:** District heating  
**Type:** Direct OT attack  
**Malware:** FrostyGoop  
**Attribution:** No threat group conclusively identified  
**Known CVE:** No specific CVE publicly established

In January 2024, residents of more than **600 apartment buildings** in Lviv lost heating for almost two days during sub-zero temperatures.

Investigators linked the incident to **FrostyGoop**, malware designed to communicate with industrial systems using Modbus TCP. Attackers sent commands to ENCO controllers used in the heating environment, resulting in incorrect measurements and system malfunction.

### Attack path

```text
Prior compromise of remotely accessible infrastructure
        ↓
Establish access into heating-control environment
        ↓
Reach ENCO industrial controllers
        ↓
Communicate using Modbus TCP
        ↓
Send malicious process commands
        ↓
Controllers/system enter incorrect operating state
        ↓
Heating service disrupted
```

FrostyGoop again illustrates why an OT attack does not require a PLC zero-day. Once an adversary has network access to a controller speaking a protocol without strong authentication or authorization, legitimate protocol functionality can become the attack mechanism.

No public investigation has conclusively assigned the operation to a named Russian APT, despite the Ukrainian target and infrastructure associated with the activity.

---

## 2024–2025 — Pro-Russian hacktivists move from screenshots to physical effects

**Targets:** Water, wastewater, oil and gas and other facilities in the US and allied countries  
**Sector:** Multiple  
**Type:** Opportunistic direct OT access  
**Groups:** CyberArmyofRussia_Reborn, Z-Pentest, Sector16 and related pro-Russian personas  
**Known CVE:** No central CVE; exposed remote-access services and weak credentials were prominent

A series of incidents during 2024 and 2025 demonstrated a lower-cost model of OT attack.

Rather than developing Stuxnet-class malware, pro-Russian groups searched for internet-accessible HMIs, VNC services and other remote interfaces. US and allied agencies warned that these groups were gaining access to operational systems using weak authentication and then manipulating controls directly.

A 2025 joint advisory named **CyberArmyofRussia_Reborn (CARR)**, Z-Pentest and other groups and said compromises had resulted in operational effects and, in some cases, physical damage.

### Typical attack path

```text
Internet reconnaissance
        ↓
Find exposed HMI / VNC / remote-access interface
        ↓
Exploit weak, reused or default credentials
        ↓
Gain operator-level visibility
        ↓
Manipulate available process controls
        ↓
Record activity for propaganda
        ↓
Operational disruption / occasional physical effect
```

The groups' technical sophistication varies. Intelligence agencies also assessed links between some of the ecosystem and Russian state activity, including support associated with GRU Unit 74455, but this does not mean that every operation publicly claimed by a pro-Russian group was directly conducted by the GRU.

The model matters because it reduces the threshold for causing an OT incident. A sophisticated industrial malware framework is unnecessary when an HMI controlling a physical process is already reachable from the public internet.

---

## 2025 — Norwegian dam gate opened remotely

**Target:** Dam in Bremanger, Norway  
**Sector:** Water / hydropower infrastructure  
**Type:** Direct cyber-physical manipulation  
**Attribution:** Russian hackers, according to Norway's security service  
**Known CVE:** None publicly disclosed

On 7 April 2025, attackers gained control of a dam facility in Bremanger and opened a flood gate.

The gate remained open for approximately four hours, releasing around **500 litres of water per second** before control was restored. No injuries were reported.

In August 2025, Norway's counter-intelligence chief publicly blamed Russian hackers for the incident, making it a rare official attribution of a cyber-enabled physical infrastructure event in Norway.

### Attack path

```text
Remote compromise of dam-control environment
        ↓
Access to gate-control capability
        ↓
Issue command opening flood gate
        ↓
Continuous uncontrolled discharge
        ↓
Operators regain control after roughly four hours
```

Public authorities have not disclosed a CVE or detailed forensic route into the facility.

The attack was technically less sophisticated than Stuxnet or Triton. The physical consequence was nevertheless immediate: the adversary obtained a digital path to equipment capable of moving water and used it.

---

## 2025 — Poland: coordinated destructive attacks reach substations and CHP plants

**Targets:** More than 30 wind and solar installations, CHP facilities and a manufacturing company  
**Sector:** Energy and manufacturing  
**Date:** 29 December 2025  
**Type:** Coordinated destructive IT/OT sabotage  
**Attribution:** Strong overlap with Static Tundra/Berserk Bear/Ghost Blizzard/Dragonfly  
**Known CVE:** No single decisive CVE publicly identified

The Polish energy-sector attacks of December 2025 are among the most technically significant additions to the recent OT incident record.

CERT Polska found coordinated destructive activity against more than 30 wind and photovoltaic installations, a manufacturing business and combined heat and power infrastructure.

At renewable facilities, attackers reached grid-connection substations containing RTUs, HMIs, protection relays, routers, switches and other automation equipment. They conducted reconnaissance and then launched destructive actions including controller-firmware damage, deletion of files and wiper malware. Damage to RTUs removed communication and remote-control capability between sites and the distribution-system operator, although electricity production continued.

### Attack path

```text
Long-term infrastructure compromise
        ↓
Internal reconnaissance and credential acquisition
        ↓
Reach energy / substation environments
        ↓
Identify RTUs, HMIs and communications equipment
        ↓
Prepare coordinated destructive actions
        ↓
Damage firmware / delete files / deploy wipers
        ↓
Loss of remote visibility and control
```

The attack on a large CHP plant had been preceded by long-term infiltration and theft of operational information. The attacker obtained privileged accounts, but endpoint protection blocked the attempted wiper before the intended interruption of heat supply was achieved.

The story developed further in August 2026. CERT Polska disclosed that a **second CHP plant**, supplying heat to approximately 50,000 residents, had also been attacked. A steam turbine and process-water treatment system were shut down, briefly interrupting cogeneration. Operators prevented loss of heat to consumers.

Investigators reconstructed an unusual route into that OT environment: a **misconfigured private cellular APN** allowed devices inside the supposedly private network to communicate in ways that should not have been possible. CERT Polska described it as the first known observation of this particular private-APN attack vector in a real cyber incident.

### Second CHP attack path

```text
Access to device connected through private APN
        ↓
APN misconfiguration allows unintended device-to-device communication
        ↓
Reach OT network
        ↓
Access plant systems
        ↓
Interfere with turbine and process-water treatment
        ↓
Cogeneration interrupted
        ↓
Operators restore operation before customer heat supply is lost
```

CERT Polska found substantial infrastructure overlap with the actor tracked under names including **Static Tundra, Berserk Bear, Ghost Blizzard and Dragonfly**, an activity cluster historically linked with Russian state operations.

---

## 2026 — Internet-facing PLC attacks disrupt US water utilities

**Targets:** Water and wastewater utilities across multiple US states  
**Sector:** Water and wastewater  
**Type:** Direct PLC compromise  
**Devices publicly identified:** Rockwell Automation / Allen-Bradley MicroLogix 1100 and 1400  
**Attribution:** Publicly unresolved in the initial federal advisory  
**Known CVE:** None identified as the principal attack method

This is the newest large-scale OT campaign in the public record at the time of writing.

On 30 July 2026, the FBI and US Environmental Protection Agency warned that malicious actors were actively attacking internet-facing PLCs at water and wastewater utilities.

The agencies said incidents had been reported in at least seven states since 27 July and that some had degraded water operations. Attackers remotely accessed exposed MicroLogix PLCs, changed IP addresses and passwords and caused facilities to lose monitoring or control. At least one victim found modified PLC project files and discrepancies in ladder logic.

Reported operational effects included **loss of water pressure and flooding**.

### Attack path

```text
Internet reconnaissance
        ↓
Identify directly exposed PLC
        ↓
Remote unauthorised access
        ↓
Change PLC network configuration/passwords
        ↓
In some cases modify PLC project/logic
        ↓
Operator loses visibility or control
        ↓
Pressure loss, flooding and manual-operation requirements
```

The striking element is what the federal advisory did **not** describe: there was no headline zero-day.

The defensive recommendations instead focused on removing PLCs from direct internet exposure, securing cellular modems, enforcing strong authentication and access controls, locking controllers into appropriate operating modes and maintaining tested manual operating capability.

The investigation and attribution remain active. Later reporting has examined possible links with Iran-aligned activity, but a public federal attribution should not be inferred until the investigating agencies make one.

---

## 2026 — Cyberattack shuts a small UK power generator for four days

**Target:** Unnamed small-scale UK power generator  
**Sector:** Electricity generation  
**Incident:** July 2026; publicly disclosed in August  
**Type:** Operational disruption  
**Attribution:** Reported as Iran-linked; not publicly confirmed in detail by the UK government  
**Known CVE:** None publicly disclosed

In August 2026, British media reported that a cyberattack the previous month had taken a small power generator offline for **four days**.

The Department for Energy Security and Net Zero confirmed that an incident had affected a small-scale generator and stressed that there had been no threat to the wider electricity grid and no loss of power to consumers. The identity and location of the facility have not been released for security reasons.

### What can currently be said about the attack path

```text
Initial access — not publicly disclosed
        ↓
Compromise affecting a small power-generation facility
        ↓
Operational capability disrupted
        ↓
Generator taken offline
        ↓
Four-day outage at the facility
        ↓
No wider grid interruption
```

Media reporting has attributed the incident to Iran-linked hackers. That attribution should presently be described as **reported rather than formally established through a detailed public NCSC incident report**. Technical claims about the initial access vector, affected PLC model or specific commands should likewise be avoided unless the UK authorities subsequently disclose them.

The incident is particularly relevant because small generators may fall outside some of the security structures applied to major national power stations while still forming part of an increasingly distributed electricity system.

---
