## 2017 — Triton/TRISIS: the safety system becomes the target

**Target:** Petrochemical facility in the Middle East  
**Sector:** Oil, gas and petrochemical  
**Type:** Direct attack against a Safety Instrumented System  
**Attribution:** Russian-linked TsNIIKhM; activity tracked as TEMP.Veles/XENOTIME  
**Known CVE:** No campaign-defining public CVE; investigators found exploitation of previously unknown Triconex firmware behaviour

Triton changed the stakes again.

Industrial safety systems exist partly to prevent a dangerous process from becoming catastrophic when normal process control fails. The attackers behind Triton did not merely target production. They reached Schneider Electric Triconex safety controllers.

The malware attempted to modify the safety system's behaviour. Programming errors in the attackers' activity instead triggered safety shutdowns, bringing the operation to a halt and exposing the intrusion.

### Attack path

```text
Compromise plant environment
        ↓
Move into OT network
        ↓
Reach engineering workstation associated with Triconex SIS
        ↓
Interact with safety controllers
        ↓
Attempt to modify SIS logic / behaviour
        ↓
Malware error triggers controller fault
        ↓
Safety system trips the process
        ↓
Facility shutdown exposes the intrusion
```

The US Department of Justice later charged a Russian national working with Russia's Central Scientific Research Institute of Chemistry and Mechanics, TsNIIKhM, over the campaign. Prosecutors said the malware was intended to prevent the safety system from operating correctly and that the attackers later conducted reconnaissance against US critical infrastructure.

Triton is one of the most serious incidents in the OT record because compromising process control can stop production, but compromising the protection intended to make failures safe can create the conditions for injury, environmental damage or loss of life.

---

## 2017 — NotPetya: an enterprise wiper creates industrial disruption worldwide

**Initial target:** Ukraine, with global spillover  
**Sector:** Multiple, including shipping, manufacturing and pharmaceuticals  
**Type:** IT-to-operations destructive attack  
**Attribution:** Sandworm / Russian GRU  
**Known CVEs:** CVE-2017-0144 and CVE-2017-0145

NotPetya was not purpose-built OT malware. It nevertheless belongs in any serious industrial incident history because it demonstrated how quickly destructive enterprise malware could stop physical businesses.

Microsoft found that the malware was initially distributed through the compromised update infrastructure of Ukrainian accounting software M.E.Doc. Once inside organisations, it used several mechanisms to move laterally, including SMB vulnerabilities addressed by MS17-010. Microsoft specifically identified CVE-2017-0144 and CVE-2017-0145.

### Attack path

```text
Compromise M.E.Doc software-update mechanism
        ↓
Deliver destructive malware to customers
        ↓
Credential harvesting and SMB-based propagation
        ↓
CVE-2017-0144 / CVE-2017-0145 used against unpatched systems
        ↓
Rapid spread through enterprise networks
        ↓
Destruction of Windows systems
        ↓
Business and industrial operations lose supporting IT
        ↓
Global operational disruption
```

Shipping terminals, logistics operations, pharmaceutical businesses and manufacturers were among those affected. The US later attributed NotPetya to GRU officers associated with Sandworm.

NotPetya reinforced a point that remains relevant today: OT segmentation does not eliminate operational dependency on identity services, logistics systems, scheduling, engineering repositories and other IT infrastructure.

---

## 2019 — Norsk Hydro: ransomware forces a global manufacturer back to manual operations

**Target:** Norsk Hydro  
**Sector:** Aluminium and manufacturing  
**Type:** IT-to-operations ransomware  
**Malware:** LockerGoga  
**Attribution:** Criminal actors; no state APT publicly established  
**Known CVE:** No defining campaign CVE publicly identified

On 19 March 2019, Norwegian aluminium producer Norsk Hydro disclosed a cyberattack affecting its global organisation.

LockerGoga ransomware disrupted Windows-based infrastructure across the company. Some production facilities were temporarily stopped; elsewhere, employees reverted to manual procedures to keep operations running. Hydro deliberately chose a transparent recovery strategy, providing regular public updates rather than quietly negotiating with the attackers.

### Attack path

```text
Initial enterprise compromise
        ↓
Obtain privileged access and spread through Windows estate
        ↓
Deploy LockerGoga ransomware
        ↓
Corporate and production-support systems become unavailable
        ↓
Sites isolate systems
        ↓
Some production stops; other facilities revert to manual operation
```

Hydro later estimated the financial impact at roughly **NOK 800 million**.

No evidence showed LockerGoga rewriting PLC logic. The event instead showed why manual operating procedures and the ability to separate plant operation from compromised business infrastructure are practical cyber-resilience controls rather than paperwork exercises.

---

## 2020 — Reported attacks on Israeli water infrastructure

**Target:** Israeli water and wastewater facilities  
**Sector:** Water  
**Type:** Attempted OT manipulation  
**Attribution:** Iranian actors were publicly suspected  
**Known CVE:** None publicly established

In April 2020, Israel reported cyber activity against water infrastructure. Public reporting suggested attackers attempted to manipulate control systems associated with pumping and treatment, including efforts that could have affected chemical levels.

The attempt did not result in publicly confirmed contamination or significant harm. Israel subsequently hardened water-sector systems, while the episode became part of a broader series of reported cyber exchanges between Iran and Israel.

### Publicly reconstructed attack path

```text
Remote access to water-sector control infrastructure
        ↓
Attempt to reach operational controls
        ↓
Attempted changes affecting treatment/pumping
        ↓
Operators / defensive systems intervene
        ↓
No confirmed harmful process outcome
```

Much of the forensic record remains classified or was reported through government and media sources rather than a detailed public incident report. Claims about the precise access mechanism should therefore be treated cautiously.

---

## 2021 — Oldsmar water treatment incident: an important case, but a contested one

**Target:** Oldsmar water treatment facility, Florida  
**Sector:** Water  
**Type:** Initially reported as attempted OT manipulation; later evidence disputed external compromise  
**Attribution:** None  
**Known CVE:** None

On 5 February 2021, officials in Oldsmar, Florida, reported that an unknown person had remotely accessed a workstation at a water treatment facility and increased the configured amount of sodium hydroxide.

An operator observed the activity and immediately restored the setting. Local authorities said the water never became dangerous. CISA and other agencies subsequently warned water utilities about remote-access security, shared credentials and outdated operating systems.

The story later became more complicated.

In 2023, reporting based on an FBI investigation and comments from former Oldsmar officials indicated investigators had found no evidence confirming an external intrusion and considered the possibility that the change resulted from user error or another non-malicious cause.

### Initially reported attack path

```text
Remote-access session observed
        ↓
Water-treatment workstation accessed
        ↓
Chemical-treatment setting changed
        ↓
Operator notices abnormal change
        ↓
Setting immediately restored
        ↓
No effect on drinking water
```

Oldsmar should therefore not be presented as a conclusively proven cyberattack. It remains useful historically because the initial disclosure exposed genuine weaknesses common to small water utilities, but the evidence no longer supports treating the originally reported narrative as settled fact.

---

## 2021 — Colonial Pipeline: ransomware reaches IT, operations stop anyway

**Target:** Colonial Pipeline  
**Sector:** Oil and gas / pipeline  
**Type:** IT-to-operations ransomware  
**Attribution:** DarkSide ransomware group  
**Known CVE:** No central exploited CVE publicly identified

Colonial Pipeline illustrates one of the most frequently misunderstood distinctions in OT incident reporting.

The attackers compromised a VPN account associated with Colonial's corporate environment. DarkSide ransomware affected IT systems. The FBI later said it found no indication that the attackers directly accessed operational technology.

Colonial nevertheless shut pipeline operations while the company assessed the compromise and its ability to safely conduct business. The shutdown lasted five days and produced fuel-supply disruption across parts of the US East Coast.

### Attack path

```text
Compromised VPN account
        ↓
Access to corporate IT
        ↓
DarkSide ransomware deployment
        ↓
Business systems become unavailable / integrity uncertain
        ↓
Company isolates environment and halts pipeline operations
        ↓
Regional fuel-supply disruption
```

Colonial paid approximately $4.4 million in ransom; US authorities later recovered a significant portion of the cryptocurrency payment.

The event was not evidence that DarkSide had developed specialist pipeline malware. It demonstrated something more mundane and arguably more widely applicable: business and OT environments may be technically segmented while operations remain organisationally dependent on IT.

---
