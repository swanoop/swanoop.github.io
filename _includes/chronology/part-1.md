## 2010 — Stuxnet: malware crosses the cyber-physical boundary

**Target:** Natanz uranium enrichment facility, Iran  
**Sector:** Nuclear  
**Type:** Direct OT sabotage  
**Attribution:** Widely attributed to a joint US-Israeli operation known as *Olympic Games*  
**Known CVEs:** CVE-2010-2568, CVE-2010-2729, CVE-2010-2743, CVE-2010-2744 and CVE-2010-2772; Stuxnet also made use of previously patched Windows weaknesses.

Stuxnet remains the reference point for destructive industrial malware because its objective was not to steal information or encrypt computers. It was built to interfere with a specific physical process.

The worm propagated through Windows systems while searching for machines running Siemens STEP7 engineering software. Once it reached the intended industrial environment, it modified code sent to Siemens PLCs while simultaneously interfering with what operators could see from the engineering workstation. The result was a rare combination of process manipulation and deception: equipment could behave abnormally while the supervisory view appeared comparatively normal. The NCSC describes Stuxnet as modifying the program running on specific Siemens PLCs while hiding those changes from the operator.

Microsoft documented several Windows vulnerabilities used by the malware. CVE-2010-2568 allowed exploitation through malicious shortcut files; CVE-2010-2729 affected the Windows Print Spooler; CVE-2010-2743 and CVE-2010-2744 provided privilege-escalation routes. CVE-2010-2772 concerned hard-coded credentials in Siemens WinCC/PCS 7 and was documented by NVD in connection with Stuxnet.

### Attack path

```text
Objective: interfere with uranium enrichment
        ↓
Reach Windows systems associated with the isolated plant
        ↓
Use removable media and multiple Windows vulnerabilities to propagate
        ↓
Locate Siemens STEP7 engineering systems
        ↓
Identify the specific PLC/process configuration
        ↓
Modify PLC control logic
        ↓
Conceal aspects of the manipulation from operators
        ↓
Alter centrifuge behaviour
        ↓
Accelerated equipment degradation and physical damage
```

Reporting based on US officials later described Stuxnet as part of the US-Israeli *Olympic Games* programme and linked the operation to the failure of roughly 1,000 centrifuges. Neither government publicly claimed the operation at the time.

Stuxnet established something that OT security practitioners now take for granted: compromising the process does not necessarily require attacking the physical equipment directly. Compromise the engineering layer that programs the controller and software becomes a route into the physical world.

---

## 2012 — Shamoon: Saudi Aramco loses around 30,000 workstations

**Target:** Saudi Aramco  
**Sector:** Oil and gas  
**Type:** IT-to-operations / destructive enterprise attack  
**Attribution:** Commonly associated with Iran-aligned actors; public attribution has varied  
**Known campaign-specific CVE:** None publicly established

On 15 August 2012, Saudi Aramco suffered one of the largest destructive corporate cyber incidents recorded at the time. Shamoon, also known as Disttrack, propagated through the company's IT environment and destroyed data on approximately 30,000 workstations.

The distinction from Stuxnet is important. Saudi Aramco stated that its primary hydrocarbon exploration and production systems and plant-control systems were unaffected. Isolation between business systems and operational systems prevented the destructive malware from becoming a process-control incident.

### Attack path

```text
Initial compromise of corporate environment
        ↓
Credential acquisition / internal propagation
        ↓
Deployment of Shamoon across Windows systems
        ↓
Destruction of files and disk structures
        ↓
Large-scale loss of corporate computing capability
        ↓
Industrial company forced into major recovery operation
```

The attack demonstrated an enduring OT-security lesson without actually compromising the control system: an industrial organisation can suffer enormous operational and economic consequences even when the malware never reaches a PLC.

Saudi Aramco rebuilt its affected computing estate while oil production continued. The incident also became an early example of destructive wiping being used against an industrial company for geopolitical rather than conventional financial motives.

---

## 2013 — Bowman Avenue Dam: Iranian hackers reach a SCADA system

**Target:** Bowman Avenue Dam, Rye Brook, New York  
**Sector:** Water infrastructure  
**Type:** OT intrusion; physical action prevented  
**Attribution:** Iranian actors linked by US prosecutors to the Islamic Revolutionary Guard Corps  
**Known CVE:** None publicly identified

Between August and September 2013, an Iranian hacker obtained access to the SCADA system controlling the Bowman Avenue Dam.

According to the US Department of Justice, the attacker was able to obtain information including water levels, temperature and the status of the sluice gate. Under normal conditions, the system could also have controlled that gate.

What prevented the incident from becoming a physical attack was not a cybersecurity control. The sluice gate had been manually disconnected for maintenance.

### Attack path

```text
Internet reconnaissance
        ↓
Identification of exposed dam control infrastructure
        ↓
Unauthorised access to SCADA environment
        ↓
Visibility of process information and control status
        ↓
Potential access to sluice-gate control
        ↓
Physical action unavailable because gate was manually disconnected
```

The US later indicted Iranian individuals associated with ITSecTeam and the Mabna/Mersad ecosystem in connection with the intrusion.

Bowman was a comparatively small facility. Its significance lay elsewhere: an internet-reachable control system belonging to physical infrastructure had been accessed remotely by a state-linked adversary, and the difference between observation and physical control was partly accidental.

---

## 2013–2014 — Havex and Dragonfly: industrial espionage through the supply chain

**Targets:** Energy and industrial organisations across several countries  
**Sector:** Energy, manufacturing and other ICS environments  
**Type:** OT reconnaissance campaign  
**Attribution:** Russian FSB-linked activity commonly tracked as Dragonfly, Energetic Bear, Berserk Bear and related names  
**Known campaign-specific CVE:** No single CVE defined the campaign

Havex represented a different phase of industrial intrusion. Instead of immediately manipulating a plant, the attackers concentrated on understanding one.

CISA says the campaign used spearphishing, compromised websites and malicious versions of legitimate software distributed from ICS vendor websites. Once installed, the Havex remote-access trojan could enumerate network resources and query OPC infrastructure to collect details about industrial systems.

### Attack path

```text
Compromise supplier website / phishing target
        ↓
Trojanise legitimate industrial software or installer
        ↓
Asset owner installs apparently legitimate software
        ↓
Havex establishes remote access
        ↓
Enumerate network and OPC servers
        ↓
Collect controller, tag and industrial configuration information
        ↓
Exfiltrate intelligence useful for future operations
```

CISA subsequently associated the broader campaign with Russia's FSB and documented energy-sector targeting extending from 2011 to 2018.

There is no confirmed Havex event comparable with the physical destruction caused by Stuxnet. Its importance comes from the reconnaissance model. An attacker preparing to interfere with an industrial process first needs to understand what equipment exists, how it communicates and what it controls. Havex automated part of that preparation.

---

## 2014 — German steel mill: cyber intrusion ends in physical damage

**Target:** Unnamed steel mill, Germany  
**Sector:** Manufacturing  
**Type:** Direct operational disruption  
**Attribution:** Unknown  
**Known CVE:** None publicly disclosed

Germany's Federal Office for Information Security, BSI, disclosed a cyber incident involving a German steel facility in its 2014 reporting.

The intrusion reportedly began with spearphishing against the corporate network. Attackers subsequently moved into production-related systems and disrupted control components. Operators were unable to shut down a blast furnace in the normal controlled manner, resulting in what BSI described as massive physical damage.

### Attack path

```text
Spearphishing
        ↓
Corporate network compromise
        ↓
Lateral movement toward production systems
        ↓
Compromise/disruption of industrial control components
        ↓
Loss of normal process-control capability
        ↓
Blast furnace cannot be shut down correctly
        ↓
Physical plant damage
```

Public technical information remains limited. The victim was not named, no specific controller vulnerability was published and no threat group was conclusively attributed.

That lack of detail is itself important when building a historical record. OT incidents are frequently discussed publicly with only a fraction of the forensic information available to investigators.

---

## 2015 — Ukraine: the first widely recognised cyberattack to cause an electricity outage

**Targets:** Three Ukrainian electricity distribution companies  
**Sector:** Electric power  
**Type:** Direct OT attack  
**Attribution:** Sandworm; Russian GRU  
**Known CVE:** No single CVE formed the decisive OT attack path

On 23 December 2015, attackers remotely operated Ukrainian electricity-distribution systems and opened circuit breakers, cutting electricity to approximately 225,000 customers.

The intrusion had begun months earlier. BlackEnergy malware and credential theft gave the adversary a foothold from which it could study the environment and eventually reach systems used for grid operations. During the attack, operators watched cursors move across their screens while remote sessions were used to issue legitimate control commands.

The attackers also interfered with supporting systems and deployed KillDisk on machines in the environment. CISA documented outages lasting between one and six hours.

### Attack path

```text
Spearphishing / BlackEnergy foothold
        ↓
Credential theft
        ↓
Extended reconnaissance and lateral movement
        ↓
Access to systems used for distribution operations
        ↓
Hijack operator/HMI sessions
        ↓
Issue legitimate commands to open breakers
        ↓
Disrupt supporting systems and recovery
        ↓
Electricity outage
```

The technical point is easily missed: this was not primarily an exploit against the circuit breakers themselves. Once the attackers reached the control environment with sufficient privileges, they could use the same interfaces that legitimate operators used.

The US Department of Justice later charged members of Russia's GRU in connection with destructive campaigns including the Ukrainian power attacks, associating the activity with Sandworm.

---

## 2016 — Industroyer/CrashOverride: malware learns the language of the power grid

**Target:** Ukrainian electricity infrastructure, including Kyiv  
**Sector:** Electric power  
**Type:** Direct OT attack  
**Attribution:** Sandworm / GRU-linked activity  
**Known CVE:** No critical CVE was required for the core process manipulation

A second major Ukrainian electricity incident arrived in December 2016, but the technical approach had changed.

The malware later named **Industroyer** or **CrashOverride** contained components capable of communicating using protocols employed in electricity transmission and distribution, including IEC 60870-5-101, IEC 60870-5-104, IEC 61850 and OPC DA.

Instead of relying entirely on remote operation of an HMI, the malware could interact with grid equipment using the protocols that the industrial environment expected.

### Attack path

```text
Compromise utility environment
        ↓
Reach control-system network
        ↓
Map relevant substation/control equipment
        ↓
Deploy Industroyer modules
        ↓
Communicate using native electricity-control protocols
        ↓
Issue malicious switching/control instructions
        ↓
Power disruption
```

This matters when considering CVEs. Industrial attacks do not necessarily need a software vulnerability once the adversary has reached the right network. A protocol designed on the assumption that anyone able to communicate with the equipment is trusted can itself provide the attacker with the necessary control surface.

---
