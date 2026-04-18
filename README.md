# 🎯 MASTER CYBERSECURITY STUDY GUIDE
## **THE ULTIMATE CENTUM (100/100) PREPARATION MATERIAL**

**Course Code:** 23CYC01  
**Course Title:** Cyber Security Essentials  
**Target:** Complete Mastery - 100/100 Marks  
**Edition:** Comprehensive Exam Preparation Guide

---

## 📋 TABLE OF CONTENTS

### **UNIT 1: INTRODUCTION TO SECURITY** (Pages 1-25)
1.1 Computer Security Concepts  
1.2 Cybersecurity Threats, Vulnerabilities and Attacks  
1.3 The OSI Security Architecture  
1.4 Security Attacks (Passive & Active)  
1.5 Security Services and Mechanisms  
1.6 A Model for Network Security  
1.7 Classical Encryption Techniques  
1.8 Modern Cryptography Foundations  
1.9 Zero Trust Security  

### **UNIT 2: SECURITY IN OPERATING SYSTEMS AND DEFENCES** (Pages 26-50)
2.1 Security in Operating System Design  
2.2 Rootkits  
2.3 Network Security Attacks  
2.4 Wireless Network Security  
2.5 Denial of Service (DoS)  
2.6 Distributed Denial of Service (DDoS)  
2.7 Cryptography in Network Security  
2.8 Firewalls  
2.9 Intrusion Detection and Prevention Systems  
2.10 Network Management and SNMP Security  
2.11 Database Security Requirements  
2.12 Database Reliability and Integrity  
2.13 Database Disclosure  

### **UNIT 3: CYBER SECURITY MANAGEMENT** (Pages 51-75)
3.1 Security Planning  
3.2 Business Continuity Planning  
3.3 Handling Incidents  
3.4 Risk Analysis  
3.5 Dealing with Disaster  
3.6 Incident Response and Management  
3.7 Information Governance in Industry  
3.8 Securing Industrial Internet of Things (IIoT)  
3.9 Intrusion Detection in OT  
3.10 Compliance Standards  
3.11 Computer Ethics  

---

# 🔐 UNIT 1: INTRODUCTION TO SECURITY

## 1.1 COMPUTER SECURITY CONCEPTS

### **Definition of Computer Security (NIST)**

**Computer Security** is the protection afforded to an automated information system in order to attain the applicable objectives of preserving the **Integrity, Availability, and Confidentiality** of information system resources (includes hardware, software, firmware, information/data, and telecommunications).

### **The Triple Role of Technology in Cybersecurity**

Technology acts in three distinct ways:

```
┌─────────────────────────────────────────────────────────┐
│                    TECHNOLOGY ROLES                      │
├─────────────────────────────────────────────────────────┤
│  1. SOURCE OF THREAT (The Weapon)                       │
│     • Malware, Exploit Scripts, Attack Tools            │
│     • Example: Ransomware, SQL Injection Scripts        │
├─────────────────────────────────────────────────────────┤
│  2. ASSET TO PROTECT (The Victim)                       │
│     • Databases, Servers, Proprietary Data              │
│     • Example: Customer Records, Financial Data         │
├─────────────────────────────────────────────────────────┤
│  3. DEFENSE WEAPON (The Shield)                         │
│     • Firewalls, Encryption, IDS/IPS                    │
│     • Example: AES Encryption, Next-Gen Firewalls       │
└─────────────────────────────────────────────────────────┘
```

---

## 1.2 THE CIA TRIAD vs DAD TRIAD

### **The Security Triad (CIA) - Goals**

```
                    ┌─────────────┐
                    │CONFIDENTIALITY│
                    │  (Privacy)   │
                    └──────┬──────┘
                           │
                          ╱ ╲
                         ╱   ╲
                             ╲
                       ╱       ╲
                      ╱         ╲
                     ╱           ╲
                    ╱             ╲
┌─────────────┐    ╱               ╲    ┌─────────────┐
│  INTEGRITY  │═══╱                 ╲═══│ AVAILABILITY│
│ (Accuracy)  │   ╲   CIA TRIAD    ╱   │  (Uptime)   │
└─────────────┘    ╲               ╱    └─────────────┘
                    ╲             ╱
                     ╲           ╱
                      ╲         ╱
                       ╲       ╱
                        ╲     ╱
                         ╲   ╱
                          ╲ ╱
```

**Detailed Explanation:**

| **Principle** | **Definition** | **Real-World Example** | **Violation Consequence** |
|---------------|----------------|------------------------|---------------------------|
| **Confidentiality** | Ensuring information is not disclosed to unauthorized individuals | Encrypting patient medical records | Data breach exposing sensitive information |
| **Integrity** | Ensuring data is not altered or modified illegally | Using checksums to verify file integrity | Tampered financial transaction amounts |
| **Availability** | Ensuring authorized users can access systems when needed | Redundant servers for 99.99% uptime | DoS attack taking down e-commerce site |

### **The Failure Triad (DAD) - Attacks**

```
                    ┌─────────────┐
                    │ DISCLOSURE  │
                    │(Data Leaks) │
                    └──────┬──────
                           │
                          ╱ ╲
                         ╱   ╲
                        ╱     ╲
                       ╱       ╲
                      ╱         ╲
                     ╱           ╲
                    ╱             ╲
┌─────────────┐    ╱               ╲    ┌─────────────┐
│ ALTERATION  │═══╱                 ╲═══│   DENIAL    │
│ (Tampering) │   ╲   DAD TRIAD    ╱   │ (Downtime)  │
└─────────────┘    ╲               ╱    └─────────────┘
                    ╲             ╱
                     ╲           ╱
                      ╲         ╱
                       ╲       ╱
                        ╲     ╱
                         ╲   ╱
                          ╲ ╱
```

**Mapping CIA to DAD:**
- **Confidentiality ←→ Disclosure** (Breach of privacy)
- **Integrity ←→ Alteration** (Unauthorized modification)
- **Availability ←→ Denial** (Service disruption)

---

## 1.3 ADDITIONAL SECURITY CONCEPTS

### **Authenticity**
The property of being genuine and able to be verified and trusted; confidence in the validity of a transmission, message, or message origin.

**Example:** Digital certificates verify that a website is genuinely owned by the claimed organization.

### **Accountability (Non-Repudiation)**
The security goal that generates the requirement for actions of an entity to be traced uniquely to that entity. Prevents denial of an action.

**Example:** Digital signatures on legal documents prevent the signer from denying they signed it.

---

## 1.4 FIPS 199 IMPACT LEVELS

When security is breached, the impact is categorized into three levels:

```
┌──────────────────────────────────────────────────────────────────┐
│                     FIPS 199 IMPACT LEVELS                       │
├────────────┬──────────────────┬──────────────────────────────────┤
│   LEVEL    │   ADVERSE EFFECT │           EXAMPLES               │
├──────────────────────────────┼──────────────────────────────────┤
│ LOW        │ Limited adverse  │ • University public website      │
│            │ effect           │   defacement                     │
│            │ • Minor financial│ • Non-sensitive public info leak │
│            │   loss           │                                  │
│            │ • Minor harm     │                                  │
├────────────┼──────────────────┼──────────────────────────────────┤
│ MODERATE   │ Serious adverse  │ • Student enrollment data leaked │
│            │ effect           │ • Employee personal info breach  │
│            │ • Significant    │ • $10K-$100K financial loss      │
│            │   financial loss │ • Non-life-threatening harm      │
├────────────┼──────────────────┼──────────────────────────────────┤
│ HIGH       │ Severe or        │ • Patient allergy info altered   │
│            │ catastrophic     │ • SCADA power grid hacked        │
│            │ effect           │ • Loss of life/serious injury    │
│            │ • Major financial│ • National security compromise   │
│            │   loss           │                                  │
│            │ • Loss of mission│                                  │
│            │ • Loss of life   │                                  │
└────────────┴──────────────────┴──────────────────────────────────┘
```

---

## 1.5 CYBERSECURITY THREATS CLASSIFICATION

Threats are classified based on resources, organization, and funding:

### **1. Unstructured Threats**
```
┌─────────────────────────────────────────┐
│        UNSTRUCTURED THREATS             │
├─────────────────────────────────────────┤
│ • Individuals/small groups              │
│ • Low skill level                       │
│ • Use known exploits                    │
│ • Limited resources                     │
│                                         │
│ EXAMPLE: Script kiddies using LOIC      │
│          (Low Orbit Ion Cannon)         │
└─────────────────────────────────────────┘
```

### **2. Structured Threats**
```
┌─────────────────────────────────────────┐
│         STRUCTURED THREATS              │
├─────────────────────────────────────────┤
│ • Organized cybercriminals              │
│ • Well-funded                           │
│ • Targeted attacks                      │
│ • Trained personnel                     │
│ • Moderate to high skill                │
│                                         │
│ EXAMPLE: Using Nmap for reconnaissance  │
│          Shodan for IoT device hunting  │
└─────────────────────────────────────────┘
```

### **3. Highly Structured Threats**
```
┌─────────────────────────────────────────┐
│      HIGHLY STRUCTURED THREATS          │
├─────────────────────────────────────────┤
│ • State-sponsored/Nation-states         │
│ • Long-term planning (months/years)     │
│ • Multi-vector attacks                  │
│ • Advanced Persistent Threats (APTs)    │
│ • Zero-day exploits                     │
│ • Massive resources                     │
│                                         │
│ EXAMPLE: Stuxnet destroying Iranian     │
│          nuclear centrifuges            │
└─────────────────────────────────────────┘
```

---

## 1.6 TYPES OF MALICIOUS CODE

### **Comprehensive Malware Classification**

```
┌─────────────────────────────────────────────────────────────────┐
│                      MALWARE TAXONOMY                            │
├──────────────┬──────────────────────────────────────────────────┤
│   MALWARE    │                   DESCRIPTION                    │
│     TYPE     │                                                  │
├──────────────┼──────────────────────────────────────────────────┤
│ VIRUS        │ • Injects into legitimate programs               │
│              │ • Requires user action to execute                │
│              │ • Attaches to .exe, .doc files                   │
│              │ • Example: Melissa Virus, ILOVEYOU               │
├──────────────┼──────────────────────────────────────────────────┤
│ WORM         │ • Self-replicating malware                       │
│              │ • Spreads independently across networks          │
│              │ • No user action required                        │
│              │ • Example: Code Red, SQL Slammer                 │
├──────────────┼──────────────────────────────────────────────────┤
│ TROJAN       │ • Disguised as legitimate software               │
│              │ • Contains hidden malicious functionality        │
│              │ • Creates backdoors                              │
│              │ • Example: Zeus Trojan, Back Orifice             │
├──────────────┼──────────────────────────────────────────────────┤
│ BOTNET       │ • Network of remote-controlled infected machines │
│              │ • Infected machines called "Zombies"             │
│              │ • Used for DDoS, spam, credential theft          │
│              │ • Example: Mirai Botnet (600K IoT devices)       │
├──────────────┼──────────────────────────────────────────────────┤
│ KEYLOGGER    │ • Captures keystrokes                            │
│              │ • Steals passwords, credit cards                 │
│              │ • Hardware or software based                     │
│              │ • Example: Spyrix, Refog                         │
├──────────────┼──────────────────────────────────────────────────┤
│ SPYWARE      │ • Covertly collects information                  │
│              │ • Monitors browsing habits                       │
│              │ • Tracks user behavior                           │
│              │ • Example: CoolWebSearch, Gator                  │
├──────────────┼──────────────────────────────────────────────────┤
│ ZERO-DAY     │ • Exploits unknown vulnerability                 │
│              │ • No patch exists                                │
│              │ • Developers unaware of flaw                     │
│              │ • Highly valuable on black market                │
└──────────────┴──────────────────────────────────────────────────┘
```

---

## 1.7 SECURITY ATTACKS - X.800 & RFC 2828

### **Classification of Security Attacks**

According to **RFC 2828** and **X.800**, security attacks are classified into two broad categories:

```
                    ┌────────────────────┐
                    │  SECURITY ATTACKS  │
                    └──────────┬─────────┘
                               │
                    ┌──────────┴──────────┐
                   ╱                       ╲
                  ╱                         ╲
                 ╱                           ╲
                ╱                             ╲
               ╱                               ╲
              ╱                                 ╲
             ╱                                   ╲
            ╱                                     ╲
           ╱                                       ╲
┌──────────────────┐                       ┌──────────────────┐
│  PASSIVE ATTACKS │                       │  ACTIVE ATTACKS  │
└────────┬─────────┘                       └────────┬─────────┘
         │                                          │
  ┌────────────┐                            ┌──────┴──────┐
 │               │                           │               │
Release of    Traffic                    Masquerade    Denial of
  Message      Analysis                     Replay      Service
 Contents     (Pattern                    Modification  (DoS)
(Eavesdrop)    Analysis)
```

### **PASSIVE ATTACKS**

**Definition:** Attempt to learn or make use of information from the system without affecting system resources.

**Characteristics:**
- ✓ Attacker only **observes** and **listens**
- ✓ **No modification** of data
- ✓ **Very difficult to detect** (no changes made)
- ✓ Breaks **Confidentiality**
- ✓ Prevention is better than detection

#### **Types of Passive Attacks:**

**1. Release of Message Contents (Eavesdropping)**
```
┌─────────────────────────────────────────────────────────┐
│            EAVESDROPPING ATTACK                         │
├─────────────────────────────────────────────────────────┤
│                                                         │
│   ALICE                    BOB                          │
│   (Sender)                (Receiver)                    │
│     │                        │                          │
│     │═══ "Hello Bob" ════════▶│                          │
│     │    (Unencrypted)      │                          │
│     │                        │                          │
│          ╲              ╱                               │
│           ╲            ╱                                │
│            ╲          ╱                                 │
│             ▼        ▼                                  │
│          ┌──────────────┐                              │
│          │   ATTACKER   │                              │
│          │  (Eavesdrop) │                              │
│          │  Reads:      │                              │
│          │  "Hello Bob" │                              │
│          └──────────────┘                              │
│                                                         │
│ IMPACT: Confidentiality Broken                         │
│ PREVENTION: Encryption (TLS, SSH, HTTPS)               │
└─────────────────────────────────────────────────────────┘
```

**2. Traffic Analysis**
```
┌─────────────────────────────────────────────────────────┐
│            TRAFFIC ANALYSIS ATTACK                      │
├─────────────────────────────────────────────────────────┤
│                                                         │
│ Even when data is ENCRYPTED, attacker can analyze:     │
│                                                         │
│ • Frequency of messages                                │
│ • Length of messages                                   │
│ • Timing patterns                                      │
│ • Source and destination                               │
│                                                         │
│ Example:                                                 │
│ ─────────                                               │
│ Company A sends 500 encrypted emails to Company B      │
│ every Monday at 9 AM.                                  │
│                                                         │
│ Inference: Companies are negotiating a deal!           │
│ (Even though content is encrypted)                     │
│                                                         │
│ PREVENTION: Traffic Padding (dummy data insertion)     │
└─────────────────────────────────────────────────────────┘
```

### **ACTIVE ATTACKS**

**Definition:** Attempt to alter system resources or affect their operation.

**Characteristics:**
- ✓ Attacker **modifies, creates, or blocks** data
- ✓ **Causes real damage** to system
- ✓ **Easier to detect** (changes are made)
- ✓ Breaks **Integrity, Availability, Authentication**
- ✓ Requires both prevention and detection

#### **Types of Active Attacks:**

**1. Masquerade**
```
┌─────────────────────────────────────────────────────────┐
│              MASQUERADE ATTACK                          │
├─────────────────────────────────────────────────────────┤
│                                                         │
│   LEGITIMATE USER          SERVER                      │
│   "john@company.com"      (Banking System)             │
│         │                      │                        │
│         │                      │                        │
│         ╲                    ╱                         │
│          ╲                  ╱                          │
│           ▼                ▼                           │
│        ┌──────────────────────┐                       │
│        │     ATTACKER         │                       │
│        │ Spoofs: john@company │                       │
│        │ Steals session token │                       │
│        │ Gains unauthorized   │                       │
│        │ access               │                       │
│        └──────────────────────┘                       │
│                                                         │
│ IMPACT: Authentication Broken                          │
│ EXAMPLE: Phishing, Session Hijacking                   │
│ PREVENTION: Strong Authentication, MFA                 │
└─────────────────────────────────────────────────────────┘
```

**2. Replay Attack**
```
┌─────────────────────────────────────────────────────────┐
│              REPLAY ATTACK                              │
├─────────────────────────────────────────────────────────┤
│                                                         │
│ PHASE 1 - CAPTURE (Legitimate Transaction):            │
│ ─────────────────────────────────                        │
│   ALICE                    BOB                          │
│     │                        │                          │
│     │══ "Transfer $100" ════▶│                          │
│     │   [Timestamp: 10:00] │                          │
│     │   [Seq Number: 4521] │                          │
│     │                        │                          │
│          ╲              ╱                               │
│           ╲  ATTACKER   ╱                               │
│            ╲  CAPTURES ╱                                │
│             ▼          ▼                                │
│        ┌──────────────────┐                            │
│        │ Stores packet    │                            │
│        └──────────────────┘                            │
│                                                         │
│ PHASE 2 - REPLAY (Fraudulent):                         │
│ ──────────────────────────────                          │
│   ATTACKER                 BOB                          │
│     │                        │                          │
│     │══ "Transfer $100" ════▶│                          │
│     │   [Timestamp: 10:00] │                          │
│     │   [Seq Number: 4521] │ (Same packet!)           │
│     │                        │                          │
│                          RESULT:                       │
│                  $100 transferred TWICE!               │
│                                                         │
│ IMPACT: Integrity Broken                               │
│ PREVENTION: Timestamps, Sequence Numbers, Nonces       │
└─────────────────────────────────────────────────────────┘
```

**3. Modification of Messages**
```
┌─────────────────────────────────────────────────────────┐
│           MESSAGE MODIFICATION ATTACK                   │
├─────────────────────────────────────────────────────────┤
│                                                         │
│   ALICE                    BOB                          │
│   (Customer)              (Bank)                        │
│     │                        │                          │
│     │══ "Transfer $100 to Account 123" ═════▶│          │
│     │                        │                          │
│          ╲              ╱                               │
│           ╲            ╱                                │
│            ▼          ▼                                 │
│        ┌──────────────────┐                            │
│        │   MAN-IN-THE     │                            │
│        │   MIDDLE (MITM)  │                            │
│        │                  │                            │
│        │ MODIFIES TO:     │                            │
│        │ "Transfer $10,000│                            │
│        │  to Account 999" │                            │
│        └──────────────────┘                            │
│                    │                                    │
│                    ▼                                    │
│     ══════════════════════════▶                         │
│                                                         │
│ IMPACT: Integrity Broken                               │
│ PREVENTION: Message Authentication Codes (MAC),        │
│             Digital Signatures, Hashing                │
└─────────────────────────────────────────────────────────┘
```

**4. Denial of Service (DoS)**
```
┌─────────────────────────────────────────────────────────┐
│            DENIAL OF SERVICE ATTACK                     │
├─────────────────────────────────────────────────────────┤
│                                                         │
│                    ┌─────────┐                          │
│                    │ ATTACKER│                          │
│                    └────┬────┘                          │
│                         │                               │
│         ════════════════╪════════════════               │
│                    Massive Traffic                      │
│                    (SYN Flood,                          │
│                     Ping of Death)                      │
│                         │                               │
│                         ▼                               │
│                    ┌─────────┐                          │
│                    │  SERVER │                          │
│                    │Resources│                          │
│                    │ EXHAUSTED│                         │
│                    │ CPU: 100%│                         │
│                    │ RAM: 100%│                         │
│                    │Bandwidth│                          │
│                    │  SATURATED│                        │
│                    └────┬────┘                          │
│                         │                               │
│              ═══════════╪══════════                     │
│                         │                               │
│                    ┌────┴────┐                          │
│                    ▼         ▼                          │
│              ┌─────────┐ ┌─────────                   │
│              │ LEGITIMATE│ │ LEGITIMATE│                │
│              │  USER 1  │ │  USER 2  │                  │
│              └─────────┘ └─────────                   │
│                              ❌                        │
│            Connection Failed  Timeout                   │
│                                                         │
│ IMPACT: Availability Broken                            │
│ PREVENTION: Rate Limiting, Firewalls, Load Balancing   │
└─────────────────────────────────────────────────────────┘
```

---

## 1.8 SECURITY SERVICES (X.800)

### **Five Main Security Services**

```
┌─────────────────────────────────────────────────────────────────┐
│                    X.800 SECURITY SERVICES                      │
├──────────────┬──────────────────────────────────────────────────┤
│   SERVICE    │                   DESCRIPTION                    │
├──────────────┼──────────────────────────────────────────────────┤
│              │                                                  │
│ 1. AUTHENTI- │ Confirms the identity of communicating entities │
│ CATION       │                                                  │
│              │ Types:                                           │
│              │ • Peer Entity Authentication                     │
│              │   (Verifies identity at connection start)        │
│              │ • Data Origin Authentication                     │
│              │   (Verifies source of data)                      │
│              │                                                  │
│              │ Technologies: Passwords, Digital Certificates,  │
│              │             Kerberos, Biometrics                 │
├──────────────┼──────────────────────────────────────────────────┤
│              │                                                  │
│ 2. ACCESS    │ Prevention of unauthorized use of resources     │
│ CONTROL      │                                                  │
│              │ Implements:                                      │
│              │ • Who can access what                            │
│              │ • Under what conditions                          │
│              │                                                  │
│              │ Tools: Access Control Lists (ACLs),             │
│              │        Role-Based Access Control (RBAC),         │
│              │        Firewalls, Permissions                    │
├──────────────┼──────────────────────────────────────────────────┤
│              │                                                  │
│ 3. DATA      │ Ensures information is not disclosed to         │
│ CONFIDENTIAL-│ unauthorized persons                            │
│ ITY          │                                                  │
│              │ Types:                                           │
│              │ • Connection Confidentiality                     │
│              │   (All data on connection encrypted)             │
│              │ • Selective Field Confidentiality                │
│              │   (Only specific fields encrypted)               │
│              │ • Traffic Flow Confidentiality                   │
│              │   (Hides communication patterns)                 │
│              │                                                  │
│              │ Technologies: AES, TLS, PGP, VPN                │
├──────────────┼──────────────────────────────────────────────────┤
│              │                                                  │
│ 4. DATA      │ Ensures data is not altered or modified         │
│ INTEGRITY    │ illegally during transmission                   │
│              │                                                  │
│              │ Types:                                           │
│              │ • Connection Integrity                           │
│              │ • Connectionless Integrity                       │
│              │ • Selective Field Integrity                      │
│              │                                                  │
│              │ Technologies: Hash Functions (SHA-256),         │
│              │             Message Authentication Codes (MAC),  │
│              │             Digital Signatures                   │
├──────────────┼──────────────────────────────────────────────────┤
│              │                                                  │
│ 5. NON-      │ Protects against denial by one of the entities  │
│ REPUDIATION  │ involved in communication                       │
│              │                                                  │
│              │ Types:                                           │
│              │ • Non-Repudiation of Origin                      │
│              │   (Sender cannot deny sending)                   │
│              │ • Non-Repudiation of Delivery                    │
│              │   (Receiver cannot deny receiving)               │
│              │                                                  │
│              │ Technologies: Digital Signatures,               │
│              │             PKI, Audit Trails                    │
└──────────────┴──────────────────────────────────────────────────┘
```

---

## 1.9 SECURITY MECHANISMS

Security mechanisms are the tools used to implement security services. They are classified into:

### **A. Specific Security Mechanisms (Layer-Specific)**

```
┌─────────────────────────────────────────────────────────────────┐
│              SPECIFIC SECURITY MECHANISMS                       │
├──────────────┬──────────────────────────────────────────────────┤
│   MECHANISM  │                   FUNCTION                       │
├──────────────┼──────────────────────────────────────────────────┤
│              │                                                  │
│ 1. ENCIPHER- │ Transforms plaintext into ciphertext to protect │
│ MENT         │ confidentiality                                 │
│              │                                                  │
│              │ Algorithms: AES, DES, RSA, Blowfish             │
│              │                                                  │
│              │ Example:                                         │
│              │ Plaintext: "HELLO"                              │
│              │ Key: "SECRET123"                                │
│              │ Ciphertext: "X7#mK9" (unreadable)              │
├──────────────┼──────────────────────────────────────────────────┤
│              │                                                  │
│ 2. DIGITAL   │ Data appended to a message that allows receiver │
│ SIGNATURE    │ to prove source and integrity                   │
│              │                                                  │
│              │ Provides:                                        │
│              │ • Authentication (Who sent it)                   │
│              │ • Integrity (Not modified)                       │
│              │ • Non-Repudiation (Cannot deny)                  │
│              │                                                  │
│              │ Algorithm: RSA, DSA, ECDSA                      │
├──────────────┼──────────────────────────────────────────────────┤
│              │                                                  │
│ 3. ACCESS    │ Mechanisms that enforce rules dictating who can │
│ CONTROL      │ access a resource                               │
│              │                                                  │
│              │ Methods:                                         │
│              │ • Access Control Lists (ACLs)                    │
│              │ • Role-Based Access Control (RBAC)               │
│              │ • Mandatory Access Control (MAC)                 │
│              │ • Discretionary Access Control (DAC)             │
├──────────────┼──────────────────────────────────────────────────┤
│              │                                                  │
│ 4. DATA      │ Mechanisms used to assure data has not been     │
│ INTEGRITY    │ modified in transit                             │
│              │                                                  │
│              │ Techniques:                                      │
│              │ • Checksums                                      │
│              │ • Cryptographic Hash Functions (SHA-256)         │
│              │ • Message Authentication Codes (HMAC)            │
│              │ • Cyclic Redundancy Check (CRC)                  │
├──────────────┼──────────────────────────────────────────────────┤
│              │                                                  │
│ 5. AUTHENTI- │ Process of verifying identity via information   │
│ CATION       │ exchange                                        │
│ EXCHANGE     │                                                  │
│              │ Methods:                                         │
│              │ • Passwords                                      │
│              │ • Challenge-Response protocols                   │
│              │ • Kerberos authentication                        │
│              │ • Biometric verification                         │
│              │ • Multi-Factor Authentication (MFA)              │
├──────────────┼──────────────────────────────────────────────────┤
│              │                                                  │
│ 6. TRAFFIC   │ Inserting dummy data bits into gaps in data     │
│ PADDING      │ stream to frustrate traffic analysis            │
│              │                                                  │
│              │ Purpose:                                         │
│              │ • Hides actual traffic patterns                  │
│              │ • Prevents analysis of message frequency         │
│              │ • Masks real communication volume                │
│              │                                                  │
│              │ Example: Sending random encrypted data during    │
│              │          idle periods to maintain constant flow  │
├──────────────┼──────────────────────────────────────────────────┤
│              │                                                  │
│ 7. ROUTING   │ Enables selection of specific, physically       │
│ CONTROL      │ secure network routes for sensitive data        │
│              │                                                  │
│              │ Features:                                        │
│              │ • Avoids compromised nodes                       │
│              │ • Uses trusted paths                             │
│              │ • Dynamic route selection based on security      │
│              │                                                  │
│              │ Example: Financial data routed through           │
│              │          dedicated secure lines                  │
└──────────────┴──────────────────────────────────────────────────┘
```

### **B. Pervasive Security Mechanisms (System-Wide)**

```
┌─────────────────────────────────────────────────────────────────┐
│             PERVASIVE SECURITY MECHANISMS                       │
├──────────────┬──────────────────────────────────────────────────┤
│   MECHANISM  │                   FUNCTION                       │
├──────────────┼──────────────────────────────────────────────────┤
│              │                                                  │
│ 1. TRUSTED   │ Code/Hardware perceived to be perfectly correct │
│ FUNCTIONALITY│ with respect to security policy                 │
│              │                                                  │
│              │ Ensures system components operate as expected    │
│              │ without failure or backdoors                     │
│              │                                                  │
│              │ Example: Trusted Platform Module (TPM)          │
│              │          Secure Boot processes                   │
├──────────────┼──────────────────────────────────────────────────┤
│              │                                                  │
│ 2. SECURITY  │ Tags bound to a resource that name its security │
│ LABELS       │ attributes/clearance level                      │
│              │                                                  │
│              │ Classification Levels:                           │
│              │ • Unclassified                                   │
│              │ • Confidential                                   │
│              │ • Secret                                         │
│              │ • Top Secret                                     │
│              │                                                  │
│              │ Example: Document marked "CONFIDENTIAL" can     │
│              │          only be accessed by cleared personnel   │
├──────────────┼──────────────────────────────────────────────────┤
│              │                                                  │
│ 3. EVENT     │ System-wide monitoring for security-relevant    │
│ DETECTION    │ breaches                                        │
│              │                                                  │
│              │ Monitors:                                        │
│              │ • Failed login attempts                          │
│              │ • Unauthorized access attempts                   │
│              │ • Unusual network traffic                        │
│              │ • File integrity violations                      │
│              │                                                  │
│              │ Tools: Intrusion Detection Systems (IDS),       │
│              │        Security Information and Event            │
│              │        Management (SIEM)                         │
├──────────────┼──────────────────────────────────────────────────┤
│              │                                                  │
│ 4. SECURITY  │ Secure log of who accessed what, when, and how  │
│ AUDIT TRAIL  │ for independent review                          │
│              │                                                  │
│              │ Records:                                         │
│              │ • User login/logout times                        │
│              │ • Files accessed/modified                        │
│              │ • Commands executed                              │
│              │ • Privilege changes                              │
│              │ • Security violations                            │
│              │                                                  │
│              │ Purpose: Forensic analysis, Compliance,         │
│              │          Non-repudiation                         │
├──────────────┼──────────────────────────────────────────────────┤
│              │                                                  │
│ 5. SECURITY  │ Mechanisms to restore system operations after   │
│ RECOVERY     │ security failure                                │
│              │                                                  │
│              │ Includes:                                        │
│              │ • System backups                                 │
│              │ • Disaster recovery procedures                   │
│              │ • Failover systems                               │
│              │ • Data restoration processes                     │
│              │                                                  │
│              │ Example: After ransomware attack, restore       │
│              │          systems from clean backups              │
└──────────────┴──────────────────────────────────────────────────┘
```

---

## 1.10 MODEL FOR NETWORK SECURITY

### **Basic Network Security Model**

```
                    ┌─────────────────────┐
                    │ TRUSTED THIRD PARTY │
                    │  (Key Distribution  │
                    │   Center/Certificate│
                    │    Authority)       │
                    └──────────┬──────────┘
                               │
                    ┌──────────┴──────────┐
                   ╱                       ╲
                  ╱                         ╲
         Secret Key                         Secret Key
        (Secure Channel)                   (Secure Channel)
                ╲                             ╱
                 ╲                           ╱
                  ╲                         ╱
                   ╲                       ╱
┌──────────┐       ╲                     ╱        ┌──────────┐
│  SENDER  │        ╲                   ╱         │ RECEIVER │
│  (Alice) │         ╲                 ╱          │  (Bob)   │
└────┬─────┘          ╲               ╱           └────┬─────┘
     │                ╲               ╱                     │
     │                 ╲             ╱                      │
     │                  ╲           ╱                       │
     │                   ▼         ▼                        │
     │              ┌─────────────────┐                     │
     │              │   ENCRYPTION    │                     │
     │              │   ALGORITHM     │                     │
     │              │                 │                     │
     │              │  Plaintext +    │                     │
     │              │  Secret Key     │                     │
     │              │       =         │                     │
     │              │  Ciphertext     │                     │
     │              └────────┬────────┘                     │
     │                       │                               │
     │                       │ CIPHERTEXT                    │
     │                       │ (Encrypted)                   │
     │                       │                               │
     │                       ▼                               │
     │              ┌─────────────────┐                     │
     │              │  INSECURE       │                     │
     │              │  NETWORK        │                     │
     │              │  (Internet)     │                     │
     │              │                 │                     │
     │              │  ⚠️ OPPONENT    │                     │
     │              │  (Eavesdropper) │                     │
     │              │  Can see but    │                     │
     │              │  cannot read    │                     │
     │              └────────────────┘                     │
     │                       │                               │
     │                       │                               │
     │                       ▼                               │
     │              ┌─────────────────┐                     │
     │              │   DECRYPTION    │                     │
     │              │   ALGORITHM     │                     │
     │              │                 │                     │
     │              │  Ciphertext +   │                     │
     │              │  Secret Key     │                     │
     │              │       =         │                     │
     │              │  Plaintext      │                     │
     │              └────────┬────────┘                     │
     │                       │                               │
     │                       │                               │
     ▼                       ▼                               ▼
┌──────────         ┌─────────────┐               ┌──────────┐
│Original  │         │  Ciphertext │               │Original  │
│Message   │────────▶│  (Secure)   │──────────────▶│Message   │
│"HELLO"   │         │  "X7#mK9"   │               │"HELLO"   │
└──────────┘         └─────────────┘               └──────────┘
```

### **Four Basic Tasks in Network Security Model**

```
┌─────────────────────────────────────────────────────────────────┐
│              FOUR BASIC TASKS IN NETWORK SECURITY               │
├──────────┬──────────────────────────────────────────────────────┤
│   TASK   │                     DESCRIPTION                      │
├────────────────────────────────────────────────────────────────┤
│          │                                                      │
│    1     │ DESIGN THE ALGORITHM                               │
│          │ ────────────────────                                │
│          │ Create a secure encryption/decryption algorithm     │
│          │ that is computationally infeasible to break         │
│          │                                                      │
│          │ Requirements:                                        │
│          │ • Strong mathematical foundation                     │
│          │ • Resistant to cryptanalysis                         │
│          │ • Efficient implementation                           │
│          │                                                      │
│          │ Example: AES (Advanced Encryption Standard)         │
├──────────┼──────────────────────────────────────────────────────┤
│          │                                                      │
│    2     │ GENERATE THE SECRET KEY                            │
│          │ ─────────────────────                               │
│          │ Produce cryptographically strong random keys used   │
│          │ for security transformation                         │
│          │                                                      │
│          │ Requirements:                                        │
│          │ • True randomness (not pseudo-random)                │
│          │ • Sufficient key length                              │
│          │ • Secure key generation process                      │
│          │                                                      │
│          │ Example: Using hardware random number generator     │
│          │          to create 256-bit AES key                  │
├──────────┼──────────────────────────────────────────────────────┤
│          │                                                      │
│    3     │ DISTRIBUTE THE TRUST                               │
│          │ ─────────────────────                               │
│          │ Securely share keys between communicating parties   │
│          │ using a trusted third party                         │
│          │                                                      │
│          │ Methods:                                             │
│          │ • Key Distribution Center (KDC)                      │
│          │ • Public Key Infrastructure (PKI)                    │
│          │ • Diffie-Hellman Key Exchange                        │
│          │                                                      │
│          │ Challenge: Key distribution problem                  │
│          │ Solution: Asymmetric cryptography or trusted KDC    │
├──────────┼──────────────────────────────────────────────────────┤
│          │                                                      │
│    4     │ SPECIFY THE PROTOCOL                               │
│          │ ────────────────────                                │
│          │ Define rules and procedures for secure              │
│          │ communication between parties                       │
│          │                                                      │
│          │ Includes:                                            │
│          │ • Message format                                     │
│          │ • Sequence of operations                             │
│          │ • Error handling                                     │
│          │ • Authentication steps                               │
│          │                                                      │
│          │ Example: TLS/SSL protocol for HTTPS                 │
│          │          SSH protocol for remote access             │
└──────────┴──────────────────────────────────────────────────────┘
```

---

## 1.11 CLASSICAL ENCRYPTION TECHNIQUES

### **A. SUBSTITUTION TECHNIQUES**

In substitution techniques, letters of plaintext are replaced by other letters, numbers, or symbols.

#### **1. Caesar Cipher**

**Definition:** A monoalphabetic cipher where each letter is shifted by a fixed number of positions in the alphabet.

**Formula:**
- **Encryption:** C = (P + k) mod 26
- **Decryption:** P = (C - k) mod 26

Where:
- P = Position of plaintext letter (A=0, B=1, ..., Z=25)
- C = Position of ciphertext letter
- k = Key (shift value)

**Example Problem:** Encrypt "HELLO" with key k=3

**Step-by-Step Solution:**

```
┌─────────────────────────────────────────────────────────────────┐
│              CAESAR CIPHER ENCRYPTION                           │
│              Plaintext: HELLO, Key: k=3                         │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│ STEP 1: Convert letters to numbers (A=0, B=1, ..., Z=25)       │
│ ──────────────────────────────────────────────────────────     │
│                                                                 │
│   H    E    L    L    O                                        │
│   ↓    ↓    ↓    ↓    ↓                                        │
│   7    4   11   11   14                                        │
│                                                                 │
│ STEP 2: Apply encryption formula C = (P + k) mod 26           │
│ ──────────────────────────────────────────────────────────     │
│                                                                 │
│   For H (P=7):   C = (7 + 3) mod 26 = 10 mod 26 = 10  → K     │
│   For E (P=4):   C = (4 + 3) mod 26 = 7 mod 26 = 7   → H     │
│   For L (P=11):  C = (11 + 3) mod 26 = 14 mod 26 = 14 → O     │
│   For L (P=11):  C = (11 + 3) mod 26 = 14 mod 26 = 14 → O     │
│   For O (P=14):  C = (14 + 3) mod 26 = 17 mod 26 = 17 → R     │
│                                                                 │
│ STEP 3: Convert numbers back to letters                        │
│ ──────────────────────────────────────────────────────────     │
│                                                                 │
│   10   7   14   14   17                                        │
│   ↓    ↓    ↓    ↓    ↓                                        │
│   K    H    O    O    R                                        │
│                                                                 │
│ ═══════════════════════════════════════════════════════════   │
│                    FINAL RESULT                                 │
│              Plaintext:  HELLO                                 │
│              Ciphertext: KHOOR                                 │
│ ═══════════════════════════════════════════════════════════   │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

**Example Problem:** Decrypt "PHHW" with key k=3

**Step-by-Step Solution:**

```
┌─────────────────────────────────────────────────────────────────┐
│              CAESAR CIPHER DECRYPTION                           │
│              Ciphertext: PHHW, Key: k=3                         │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│ STEP 1: Convert letters to numbers                              │
│ ──────────────────────────────────────────────────────────     │
│                                                                 │
│   P    H    H    W                                             │
│   ↓    ↓    ↓    ↓                                             │
│  15    7    7   22                                             │
│                                                                 │
│ STEP 2: Apply decryption formula P = (C - k) mod 26           │
│ ──────────────────────────────────────────────────────────     │
│                                                                 │
│   For P (C=15):  P = (15 - 3) mod 26 = 12 mod 26 = 12 → M    │
│   For H (C=7):   P = (7 - 3) mod 26 = 4 mod 26 = 4  → E     │
│   For H (C=7):   P = (7 - 3) mod 26 = 4 mod 26 = 4  → E     │
│   For W (C=22):  P = (22 - 3) mod 26 = 19 mod 26 = 19 → T    │
│                                                                 │
│ STEP 3: Convert numbers back to letters                        │
│ ──────────────────────────────────────────────────────────     │
│                                                                 │
│   12   4    4   19                                             │
│   ↓    ↓    ↓    ↓                                             │
│   M    E    E    T                                             │
│                                                                 │
│ ═══════════════════════════════════════════════════════════   │
│                    FINAL RESULT                                 │
│              Ciphertext: PHHW                                  │
│              Plaintext:  MEET                                  │
│ ═══════════════════════════════════════════════════════════   │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

**Why Caesar Cipher is Weak:**

```
┌─────────────────────────────────────────────────────────────────┐
│           BRUTE FORCE ATTACK ON CAESAR CIPHER                   │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│ Ciphertext: PHHW                                                │
│                                                                 │
│ Trying all 25 possible keys:                                   │
│ ──────────────────────────────────                              │
│                                                                 │
│   Key 1:  OGGV  (No - gibberish)                               │
│   Key 2:  NFFU  (No - gibberish)                               │
│   Key 3:  MEET  ✓ YES! Meaningful English word!                │
│   Key 4:  LDDS  (No - gibberish)                               │
│   Key 5:  KCCR  (No - gibberish)                               │
│   ...                                                           │
│   Key 25: QIIX (No - gibberish)                                │
│                                                                 │
│ VULNERABILITIES:                                                │
│ ───────────────                                                 │
│ 1. Only 25 possible keys - can try all in microseconds         │
│ 2. Frequency analysis works (E is most common in English)      │
│ 3. No key management - both sides must agree on shift          │
│                                                                 │
│ MODERN CIPHERS:                                                 │
│ ───────────────                                                 │
│ AES-256 has 2^256 possible keys                                 │
│ = 1.16 × 10^77 keys                                            │
│                                                                 │
│ Even with fastest computer, would take billions of years!      │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

---

#### **2. Monoalphabetic Cipher**

**Definition:** A substitution cipher where each plaintext letter is replaced by a fixed corresponding ciphertext letter throughout the message.

**Characteristics:**
- Uses only **one substitution alphabet**
- Same plaintext letter **always** produces the same ciphertext letter
- Vulnerable to **frequency analysis**

**Example:**
```
Plaintext alphabet:  ABCDEFGHIJKLMNOPQRSTUVWXYZ
Ciphertext alphabet: DFGHIJKLMNOPQRSTUVWXYZABC

Plaintext:  HELLO
Ciphertext: KHOOR
```

---

#### **3. Polyalphabetic Cipher (Vigenère Cipher)**

**Definition:** A substitution cipher that uses **multiple substitution alphabets**, where the replacement depends on a key.

**Characteristics:**
- Uses **more than one** substitution alphabet
- Same plaintext letter can produce **different** ciphertext letters
- More secure than monoalphabetic

**Formula:** C = (P + K) mod 26

**Example Problem:** Encrypt "CRYPTOGRAPHY" with key "HOUSE"

**Step-by-Step Solution:**

```
┌─────────────────────────────────────────────────────────────────┐
│            VIGENÈRE CIPHER ENCRYPTION                           │
│            Plaintext: CRYPTOGRAPHY, Key: HOUSE                  │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│ STEP 1: Repeat key to match plaintext length                   │
│ ──────────────────────────────────────────────────────────     │
│                                                                 │
│   Plaintext: C R Y P T O G R A P H Y                          │
│   Key:       H O U S E H O U S E H O                          │
│                                                                 │
│ STEP 2: Convert to numbers (A=0, B=1, ..., Z=25)              │
│ ──────────────────────────────────────────────────────────     │
│                                                                 │
│   P:  2  17  24  15  19  14   6  17   0  15   7  24           │
│   K:  7  14  20  18   4   7  14  20  18   4   7  14           │
│                                                                 │
│ STEP 3: Apply C = (P + K) mod 26                              │
│ ──────────────────────────────────────────────────────────     │
│                                                                 │
│   C = (2+7) mod 26  = 9   → J                                 │
│   C = (17+14) mod 26 = 31 mod 26 = 5  → F                    │
│   C = (24+20) mod 26 = 44 mod 26 = 18 → S                    │
│   C = (15+18) mod 26 = 33 mod 26 = 7  → H                    │
│   C = (19+4) mod 26  = 23  → X                                 │
│   C = (14+7) mod 26  = 21  → V                                 │
│   C = (6+14) mod 26  = 20  → U                                 │
│   C = (17+20) mod 26 = 37 mod 26 = 11 → L                    │
│   C = (0+18) mod 26  = 18  → S                                 │
│   C = (15+4) mod 26  = 19  → T                                 │
│   C = (7+7) mod 26   = 14  → O                                 │
│   C = (24+14) mod 26 = 38 mod 26 = 12 → M                    │
│                                                                 │
│ ═══════════════════════════════════════════════════════════   │
│                    FINAL RESULT                                 │
│              Plaintext:  CRYPTOGRAPHY                          │
│              Key:        HOUSE                                 │
│              Ciphertext: JFSHXVULSTOM                          │
│ ═══════════════════════════════════════════════════════════   │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

---

### **B. TRANSPOSITION TECHNIQUES**

In transposition techniques, letters are **rearranged** to new positions, not changed.

#### **1. Rail Fence Cipher**

**Definition:** Writes plaintext in a zig-zag pattern across rows (rails) and reads row by row.

**Example Problem:** Encrypt "MEETME" with depth (rails) = 2

**Step-by-Step Solution:**

```
┌─────────────────────────────────────────────────────────────────┐
│            RAIL FENCE CIPHER ENCRYPTION                         │
│            Plaintext: MEETME, Depth: 2 rails                    │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│ STEP 1: Write letters diagonally across 2 rails                │
│ ──────────────────────────────────────────────────────────     │
│                                                                 │
│   Position:  1   2   3   4   5   6                             │
│              ─── ─── ─── ─── ─── ───                           │
│   Rail 1:    M       E       M                                  │
│              ╲     ╱ ╲     ╱ ╲     ╱                           │
│               ╲   ╱   ╲   ╱   ╲   ╱                            │
│                ╲ ╱     ╲ ╱     ╲ ╱                             │
│   Rail 2:        E       T       E                              │
│                                                                 │
│   Visual representation:                                        │
│   ─────────────────────                                         │
│   Rail 1 (top):    M   .   E   .   M   .                        │
│   Rail 2 (bottom): .   E   .   T   .   E                        │
│                                                                 │
│ STEP 2: Read row by row                                        │
│ ──────────────────────────────────────────────────────────     │
│                                                                 │
│   Rail 1 gives: M E M                                          │
│   Rail 2 gives: E T E                                          │
│                                                                 │
│ ═══════════════════════════════════════════════════════════   │
│                    FINAL RESULT                                 │
│              Plaintext:  MEETME                                │
│              Ciphertext: MEMETE                                │
│ ═══════════════════════════════════════════════════════════   │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

**Example Problem:** Decrypt "CTASERPOLSINCYCSI" with depth = 3

**Step-by-Step Solution:**

```
┌─────────────────────────────────────────────────────────────────┐
│         RAIL FENCE CIPHER DECRYPTION                            │
│         Ciphertext: CTASERPOLSINCYCSI, Depth: 3 rails          │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│ Message length: 17 characters                                   │
│                                                                 │
│ STEP 1: Calculate row lengths for 17 chars in 3-rail zigzag   │
│ ──────────────────────────────────────────────────────────     │
│                                                                 │
│   Pattern repeats every 4 positions:                           │
│   Position: 1  2  3  4  5  6  7  8  9 10 11 12 13 14 15 16 17 │
│   Rail:     1  2  3  2  1  2  3  2  1  2  3  2  1  2  3  2  1  │
│                                                                 │
│   Row 1 gets positions: 1, 5, 9, 13, 17 (5 characters)        │
│   Row 2 gets positions: 2, 4, 6, 8, 10, 12, 14, 16 (8 chars)  │
│   Row 3 gets positions: 3, 7, 11, 15 (4 characters)           │
│                                                                 │
│ STEP 2: Distribute ciphertext across rows                     │
│ ──────────────────────────────────────────────────────────     │
│                                                                 │
│   Ciphertext: C T A S E R P O L S I N C Y C S I               │
│               ↓ ↓ ↓ ↓ ↓ ↓ ↓ ↓ ↓ ↓ ↓ ↓ ↓ ↓ ↓ ↓ ↓               │
│               1 2 3 4 5 6 7 8 9                               │
│                                                                 │
│   Row 1 (5 chars):  C T A S E                                 │
│   Row 2 (8 chars):  R P O L S I N C                           │
│   Row 3 (4 chars):  Y C S I                                   │
│                                                                 │
│ STEP 3: Reconstruct the zigzag pattern                        │
│ ──────────────────────────────────────────────────────────     │
│                                                                 │
│   Rail 1: C . . . R . . . Y . . . P . . . T                   │
│   Rail 2: . R . P . O . L . S . I . N . C .                   │
│   Rail 3: . . Y . . . C . . . S . . . I . .                   │
│                                                                 │
│ STEP 4: Read column by column (top to bottom)                 │
│ ──────────────────────────────────────────────────────────     │
│                                                                 │
│   Column 1:  C                                                │
│   Column 2:  R                                                │
│   Column 3:  Y                                                │
│   Column 4:  P                                                │
│   Column 5:  T                                                │
│   Column 6:  O                                                │
│   Column 7:  C                                                │
│   Column 8:  L                                                │
│   Column 9:  A                                                │
│   Column 10: S                                                │
│   Column 11: S                                                │
│   Column 12: I                                                │
│   Column 13: S                                                │
│   Column 14: N                                                │
│   Column 15: I                                                │
│   Column 16: C                                                │
│   Column 17: E                                                │
│                                                                 │
│ ═══════════════════════════════════════════════════════════   │
│                    FINAL RESULT                                 │
│              Ciphertext: CTASERPOLSINCYCSI                     │
│              Plaintext:  CRYPTO CLASS IS NICE                  │
│ ═══════════════════════════════════════════════════════════   │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

---

#### **2. Columnar Transposition Cipher**

**Definition:** Writes plaintext in rows under a key, then reads columns in alphabetical order of the key.

**Example Problem:** Encrypt "SECUREDATA" with key sequence 3 1 4 2

**Step-by-Step Solution:**

```
┌─────────────────────────────────────────────────────────────────┐
│        COLUMNAR TRANSPOSITION CIPHER                            │
│        Plaintext: SECUREDATA, Key: 3 1 4 2                      │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│ STEP 1: Write plaintext in rows under key                      │
│ ──────────────────────────────────────────────────────────     │
│                                                                 │
│   Key:         3   1   4   2                                   │
│              ─── ─── ─── ───                                   │
│   Row 1:      S   E   C   U                                    │
│   Row 2:      R   E   D   A                                    │
│   Row 3:      T   A   .   .   (pad if needed)                  │
│                                                                 │
│ STEP 2: Number columns based on alphabetical order of key     │
│ ──────────────────────────────────────────────────────────     │
│                                                                 │
│   Key values:   3   1   4   2                                  │
│   Alphabetical: 2nd 1st 4th 3rd  (1<2<3<4)                     │
│   Read order:   3rd 1st 4th 2nd  (by original position)        │
│                                                                 │
│   Actually, let's reorder properly:                            │
│                                                                 │
│   Original:     3   1   4   2   ← Key values                   │
│   Position:     1   2   3   4   ← Column numbers               │
│                                                                 │
│   Sort by key value:                                           │
│   Key=1 is at position 2  → Read column 2 first               │
│   Key=2 is at position 4  → Read column 4 second              │
│   Key=3 is at position 1  → Read column 1 third               │
│   Key=4 is at position 3  → Read column 3 fourth              │
│                                                                 │
│   Read order: Column 2, Column 4, Column 1, Column 3          │
│                                                                 │
│ STEP 3: Read columns in order                                  │
│ ──────────────────────────────────────────────────────────     │
│                                                                 │
│   Key:         3   1   4   2                                   │
│              ─── ─── ─── ───                                   │
│              S   E   C   U   ← Column 2: E, E, A              │
│              R   E   D   A   ← Column 4: U, A                 │
│              T   A           ← Column 1: S, R, T              │
│                          ← Column 3: C, D                     │
│                                                                 │
│   Column 2 (key=1): E E A                                      │
│   Column 4 (key=2): U A                                        │
│   Column 1 (key=3): S R T                                      │
│   Column 3 (key=4): C D                                        │
│                                                                 │
│ ═══════════════════════════════════════════════════════════   │
│                    FINAL RESULT                                 │
│              Plaintext:  SECUREDATA                            │
│              Ciphertext: EEAUASRTCD                            │
│ ═══════════════════════════════════════════════════════════   │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

---

### **C. PLAYFAIR CIPHER**

**Definition:** A digraph substitution cipher using a 5×5 matrix of letters.

**Rules of Playfair Cipher:**

```
┌─────────────────────────────────────────────────────────────────┐
│                  PLAYFAIR CIPHER RULES                          │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│ RULE 1: Build 5×5 Matrix                                       │
│ ─────────────────────────                                       │
│ • Use keyword (no duplicate letters)                           │
│ • Fill rest with alphabet (I and J share a box)                │
│                                                                 │
│ RULE 2: Prepare Plaintext                                      │
│ ─────────────────────────                                       │
│ • Split into pairs (digraphs)                                  │
│ • If pair has same letter, insert 'X' between them             │
│ • If odd length, add 'X' at end                                │
│                                                                 │
│ RULE 3: Encryption Rules                                       │
│ ─────────────────────────                                       │
│                                                                 │
│ Case 1: Same Row                                               │
│ ──────────────                                                 │
│ Replace each letter with letter to its RIGHT                   │
│ (wrap around to left if needed)                                │
│                                                                 │
│     [M][O][N][A][R]  →  [O][N][A][R][M]                       │
│                                                                 │
│ Case 2: Same Column                                            │
│ ───────────────                                                │
│ Replace each letter with letter BELOW it                       │
│ (wrap around to top if needed)                                 │
│                                                                 │
│     [M]              [C]                                       │
│     [C]              [E]                                       │
│     [E]       →      [L]                                       │
│     [L]              [P]                                       │
│     [P]              [S]                                       │
│                                                                 │
│ Case 3: Rectangle (Different Row & Column)                    │
│ ──────────────────────────────────                             │
│ Replace each letter with letter on same row at                 │
│ opposite corner of rectangle                                   │
│                                                                 │
│     [H].....[Y]        [Y].....[B]                             │
│       .....            .....                                   │
│       .....     →      .....                                   │
│         .....          .....                                   │
│     [E].....[D]        [D].....[F]                             │
│                                                                 │
│     HE → Rectangle → YD                                        │
│     (H takes Y's column, E takes D's column)                   │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

**Example Problem:** Encrypt "HELLO WORLD" with key "MONARCHY"

**Step-by-Step Solution:**

```
┌─────────────────────────────────────────────────────────────────┐
│          PLAYFAIR CIPHER ENCRYPTION                             │
│          Plaintext: HELLOWORLD, Key: MONARCHY                   │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│ STEP 1: Construct 5×5 Matrix                                   │
│ ──────────────────────────────────────────────────────────     │
│                                                                 │
│   Keyword: MONARCHY (remove duplicates)                        │
│   Remaining alphabet: BDEFGIKLPQSTUVWXZ (I/J combined)         │
│                                                                 │
│   ┌───┬───┬───┬───┬───┐                                       │
│   │ M │ O │ N │ A │ R │  Row 1                                │
│   ├───┼───┼───┼───┼───┤                                       │
│   │ C │ H │ Y │ B │ D │  Row 2                                │
│   ├───┼───┼───┼───┼───┤                                       │
│   │ E │ F │ G │ I │ K │  Row 3     (I/J share cell)          │
│   ├───┼───┼───┼───┼───┤                                       │
│   │ L │ P │ Q │ S │ T │  Row 4                                │
│   ├───┼───┼───┼───┼───┤                                       │
│   │ U │ V │ W │ X │ Z │  Row 5                                │
│   └──────┴──────┴───                                       │
│                                                                 │
│ STEP 2: Prepare Plaintext                                      │
│ ──────────────────────────────────────────────────────────     │
│                                                                 │
│   Original: H E L L O W O R L D                               │
│                                                                 │
│   Split into pairs: (HE) (LL) (OW) (OR) (LD)                   │
│                                                                 │
│   Problem: "LL" has duplicate letters!                         │
│   Solution: Insert 'X' between them                            │
│                                                                 │
│   Final pairs: (HE) (LX) (LO) (WO) (RL) (DX)                   │
│                                                                 │
│ STEP 3: Encrypt Each Pair                                      │
│ ──────────────────────────────────────────────────────────     │
│                                                                 │
│   Pair 1: HE                                                   │
│   ─────────                                                    │
│   H is at (Row 2, Col 2)                                      │
│   E is at (Row 3, Col 1)                                      │
│   → Rectangle case                                             │
│   H → same row, E's column → C                                │
│   E → same row, H's column → F                                │
│   HE → CF                                                      │
│                                                                 │
│   Pair 2: LX                                                   │
│   ─────────                                                    │
│   L is at (Row 4, Col 1)                                      │
│   X is at (Row 5, Col 4)                                      │
│   → Rectangle case                                             │
│   L → same row, X's column → S                                │
│   X → same row, L's column → U                                │
│   LX → SU                                                      │
│                                                                 │
│   Pair 3: LO                                                   │
│   ─────────                                                    │
│   L is at (Row 4, Col 1)                                      │
│   O is at (Row 1, Col 2)                                      │
│   → Rectangle case                                             │
│   L → same row, O's column → P                                │
│   O → same row, L's column → M                                │
│   LO → PM                                                      │
│                                                                 │
│   Pair 4: WO                                                   │
│   ─────────                                                    │
│   W is at (Row 5, Col 3)                                      │
│   O is at (Row 1, Col 2)                                      │
│   → Rectangle case                                             │
│   W → same row, O's column → V                                │
│   O → same row, W's column → N                                │
│   WO → VN                                                      │
│                                                                 │
│   Pair 5: RL                                                   │
│   ─────────                                                    │
│   R is at (Row 1, Col 5)                                      │
│   L is at (Row 4, Col 1)                                      │
│   → Rectangle case                                             │
│   R → same row, L's column → M                                │
│   L → same row, R's column → T                                │
│   RL → MT                                                      │
│                                                                 │
│   Pair 6: DX                                                   │
│   ─────────                                                    │
│   D is at (Row 2, Col 5)                                      │
│   X is at (Row 5, Col 4)                                      │
│   → Rectangle case                                             │
│   D → same row, X's column → B                                │
│   X → same row, D's column → Z                                │
│   DX → BZ                                                      │
│                                                                 │
│ ═══════════════════════════════════════════════════════════   │
│                    FINAL RESULT                                 │
│              Plaintext:  HELLOWORLD                            │
│              Key:        MONARCHY                              │
│              Ciphertext: CF SU PM VN MT BZ                     │
│ ═══════════════════════════════════════════════════════════   │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

---

## 1.12 HILL CIPHER

**Definition:** A polygraphic substitution cipher based on linear algebra (matrix multiplication).

**Formula:** C = (P × K) mod 26

Where:
- P = Plaintext vector (numbers)
- K = Key matrix
- C = Ciphertext vector (numbers)

**Example Problem:** Encrypt "HILLCIPHER" using Hill Cipher with key matrix K = [[3,2],[8,5]]

**Step-by-Step Solution:**

```
┌─────────────────────────────────────────────────────────────────┐
│                HILL CIPHER ENCRYPTION                           │
│        Plaintext: HILLCIPHER, Key Matrix: [3 2]                 │
│                                           [8 5]                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│ STEP 1: Convert Alphabet to Numbers                            │
│ ──────────────────────────────────────────────────────────     │
│                                                                 │
│   A=0, B=1, C=2, D=3, E=4, F=5, G=6, H=7, I=8, J=9           │
│   K=10, L=11, M=12, N=13, O=14, P=15, Q=16, R=17, S=18       │
│   T=19, U=20, V=21, W=22, X=23, Y=24, Z=25                    │
│                                                                 │
│ STEP 2: Split Plaintext into Pairs (2 letters per block)      │
│ ──────────────────────────────────────────────────────────     │
│                                                                 │
│   H I L L C I P H E R                                         │
│   ↓ ↓ ↓ ↓ ↓ ↓ ↓ ↓ ↓ ↓                                         │
│   (HI) (LL) (CI) (PH) (ER)                                    │
│                                                                 │
│   Convert to numbers:                                          │
│   HI → [7, 8]                                                  │
│   LL → [11, 11]                                                │
│   CI → [2, 8]                                                  │
│   PH → [15, 7]                                                 │
│   ER → [4, 17]                                                 │
│                                                                 │
│ STEP 3: Matrix Multiplication C = (K × P) mod 26              │
│ ──────────────────────────────────────────────────────────     │
│                                                                 │
│   Key Matrix K = [3  2]                                        │
│                  [8  5]                                        │
│                                                                 │
│   ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━    │
│   Block 1: HI → [7, 8]                                        │
│   ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━    │
│                                                                 │
│   C = [3  2] × [7]  = [3×7 + 2×8] = [21+16] = [37]           │
│       [8  5]   [8]    [8×7 + 5×8]   [56+40]   [96]           │
│                                                                 │
│   Apply mod 26:                                                │
│   37 mod 26 = 11 → L                                          │
│   96 mod 26 = 18 → S                                          │
│                                                                 │
│   Result: LS                                                   │
│                                                                 │
│   ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━    │
│   Block 2: LL → [11, 11]                                      │
│   ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━    │
│                                                                 │
│   C = [3  2] × [11] = [3×11 + 2×11] = [33+22] = [55]         │
│       [8  5]   [11]   [8×11 + 5×11]   [88+55]   [143]        │
│                                                                 │
│   Apply mod 26:                                                │
│   55 mod 26 = 3 → D                                           │
│   143 mod 26 = 13 → N                                         │
│                                                                 │
│   Result: DN                                                   │
│                                                                 │
│   ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━    │
│   Block 3: CI → [2, 8]                                        │
│   ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━    │
│                                                                 │
│   C = [3  2] × [2]  = [3×2 + 2×8] = [6+16] = [22]            │
│       [8  5]   [8]    [8×2 + 5×8]   [16+40]   [56]           │
│                                                                 │
│   Apply mod 26:                                                │
│   22 mod 26 = 22 → W                                          │
│   56 mod 26 = 4 → E                                           │
│                                                                 │
│   Result: WE                                                   │
│                                                                 │
│   ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━    │
│   Block 4: PH → [15, 7]                                       │
│   ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━    │
│                                                                 │
│   C = [3  2] × [15] = [3×15 + 2×7] = [45+14] = [59]          │
│       [8  5]   [7]    [8×15 + 5×7]   [120+35]  [155]         │
│                                                                 │
│   Apply mod 26:                                                │
│   59 mod 26 = 7 → H                                           │
│   155 mod 26 = 25 → Z                                         │
│                                                                 │
│   Result: HZ                                                   │
│                                                                 │
│   ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━    │
│   Block 5: ER → [4, 17]                                       │
│   ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━    │
│                                                                 │
│   C = [3  2] × [4]  = [3×4 + 2×17] = [12+34] = [46]          │
│       [8  5]   [17]   [8×4 + 5×17]   [32+85]   [117]         │
│                                                                 │
│   Apply mod 26:                                                │
│   46 mod 26 = 20 → U                                          │
│   117 mod 26 = 13 → N                                         │
│                                                                 │
│   Result: UN                                                   │
│                                                                 │
│ ═══════════════════════════════════════════════════════════   │
│                    FINAL RESULT                                 │
│              Plaintext:  HILLCIPHER                            │
│              Key Matrix: [3 2]                                 │
│                          [8 5]                                 │
│              Ciphertext: LSDNWEHZUN                            │
│ ═══════════════════════════════════════════════════════════   │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

### **Attacks on Hill Cipher**

```
┌─────────────────────────────────────────────────────────────────┐
│           KNOWN PLAINTEXT ATTACK ON HILL CIPHER                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│ VULNERABILITY:                                                  │
│ ─────────────                                                   │
│ Hill Cipher is purely linear (matrix multiplication),          │
│ making it vulnerable to Known Plaintext Attack                 │
│                                                                 │
│ ATTACK METHOD:                                                  │
│ ───────────────                                                 │
│                                                                 │
│ 1. Attacker intercepts 'm' plaintext-ciphertext pairs          │
│    (where m is the matrix dimension)                           │
│                                                                 │
│ 2. Sets up matrix equation:                                    │
│                                                                 │
│        Y = X × K   (mod 26)                                   │
│                                                                 │
│    Where:                                                       │
│    • Y = Ciphertext matrix                                     │
│    • X = Plaintext matrix                                      │
│    • K = Secret Key matrix (unknown)                           │
│                                                                 │
│ 3. Calculates inverse of plaintext matrix X⁻¹                  │
│                                                                 │
│ 4. Recovers key by:                                            │
│                                                                 │
│        K = X⁻¹ × Y   (mod 26)                                 │
│                                                                 │
│ EXAMPLE:                                                        │
│ ───────                                                         │
│ If attacker knows:                                              │
│ • Plaintext "HI" → Ciphertext "LS"                             │
│ • Plaintext "LL" → Ciphertext "DN"                             │
│                                                                 │
│ They can set up:                                                │
│                                                                 │
│   [L S]   = [3 2] × [H I]                                     │
│   [D N]     [8 5]   [L L]                                     │
│                                                                 │
│ And solve for the key matrix!                                  │
│                                                                 │
│ DEFENSE:                                                        │
│ ───────                                                         │
│ • Use larger matrix sizes (3×3, 4×4)                           │
│ • Combine with non-linear operations                           │
│ • Use modern ciphers (AES) instead                             │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

---

## 1.13 VERNAM CIPHER & ONE-TIME PAD

### **Vernam Cipher**

**Definition:** Works on binary data using XOR operation.

**Formula:** C = P ⊕ K

Where:
- P = Plaintext bit
- K = Key bit
- C = Ciphertext bit
- ⊕ = XOR operation

**XOR Truth Table:**
```
┌───┬───┬─────┐
│ P │ K │ C=P⊕K│
├──────┼─────
│ 0 │ 0 │  0  │
│ 0 │ 1 │  1  │
│ 1 │ 0 │  1  │
│ 1 │ 1 │  0  │
└──────┴─────
```

---

### **One-Time Pad (OTP)**

**Definition:** The ultimate evolution of Vernam Cipher providing **Perfect Secrecy** (unconditionally secure).

**Three Rules for Perfect Security:**

```
┌─────────────────────────────────────────────────────────────────┐
│            ONE-TIME PAD REQUIREMENTS                            │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  ┌─────────────────────────────────────────────────────────┐   │
│  │  RULE 1: KEY MUST BE TRULY RANDOM                      │   │
│  │  ───────────────────────────────                       │   │
│  │  • Cannot be pseudo-random                             │   │
│  │  • Must use hardware random number generator           │   │
│  │  • No patterns or predictability                       │   │
│  └─────────────────────────────────────────────────────────┘   │
│                                                                 │
│  ┌─────────────────────────────────────────────────────────┐   │
│  │  RULE 2: KEY MUST BE AS LONG AS PLAINTEXT              │   │
│  │  ────────────────────────────────────────              │   │
│  │  • To encrypt 1GB file, need 1GB key                   │   │
│  │  • No key reuse allowed                                │   │
│  │  • Key length = Message length                         │   │
│  └─────────────────────────────────────────────────────────┘   │
│                                                                 │
│  ┌─────────────────────────────────────────────────────────┐   │
│  │  RULE 3: KEY MUST BE USED ONLY ONCE                    │   │
│  │  ──────────────────────────────────                    │   │
│  │  • Destroy key after use                               │   │
│  │  • Never reuse for another message                     │   │
│  │  • "One-Time" = single use only                        │   │
│  └─────────────────────────────────────────────────────────┘   │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

**Perfect Security Definition (Claude Shannon):**

Ciphertext reveals **ZERO** information about plaintext.

Mathematically:
```
Pr[M=m | C=c] = Pr[M=m]
```

Meaning: The probability of message M being 'm' given ciphertext 'c' equals the probability of M being 'm' without seeing the ciphertext.

**Flaw of One-Time Pad:**

```
┌─────────────────────────────────────────────────────────────────┐
│              ONE-TIME PAD PRACTICAL PROBLEM                     │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│ LOGISTICAL NIGHTMARE:                                           │
│ ───────────────────                                             │
│                                                                 │
│ To send a 1GB encrypted file securely:                         │
│                                                                 │
│ 1. Generate 1GB truly random key                               │
│ 2. Securely deliver 1GB key to receiver                        │
│    (requires secure channel)                                   │
│ 3. Encrypt 1GB file using key                                  │
│ 4. Send 1GB ciphertext over insecure channel                   │
│ 5. Receiver decrypts using their copy of key                   │
│ 6. Destroy key on both ends                                    │
│                                                                 │
│ PROBLEM:                                                        │
│ ───────                                                         │
│ If you have a secure channel to send 1GB key,                  │
│ why not just send the 1GB message directly?                    │
│                                                                 │
│ CONCLUSION:                                                     │
│ ──────────                                                      │
│ • Mathematically unbreakable                                   │
│ • Practically impossible for large messages                    │
│ • Used only for extremely sensitive, short messages            │
│   (diplomatic communications, spy networks)                    │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

---

## 1.14 PRODUCT CRYPTOSYSTEM

**Definition:** A cryptographic system that combines **multiple simple transformations** (substitution and transposition) in sequence to produce a stronger cipher.

### **Structure of Product Cryptosystem**

```
                    ┌─────────────┐
                    │  PLAINTEXT  │
                    └──────┬──────┘
                           │
                           ▼
              ┌────────────────────────┐
              │  TRANSFORMATION 1      │
              │  (Substitution)        │
              │                        │
              │  Creates CONFUSION     │
              │  • Hides relationship  │
              │    between key and     │
              │    ciphertext          │
              │  • Replaces symbols    │
              └────────┬───────────────┘
                       │
                       ▼
              ┌────────────────────────┐
              │  TRANSFORMATION 2      │
              │  (Transposition)       │
              │                        │
              │  Creates DIFFUSION     │
              │  • Spreads plaintext   │
              │    statistics across   │
              │    ciphertext          │
              │  • Rearranges symbols  │
              │  • Avalanche Effect    │
              └────────┬───────────────┘
                       │
                       ▼
              ┌────────────────────────┐
              │  MULTIPLE ROUNDS       │
              │  (Repeat above steps)  │
              │                        │
              │  • Hides patterns      │
              │  • Resists             │
              │    cryptanalysis       │
              │  • Strengthens cipher  │
              └────────┬───────────────┘
                       │
                       ▼
                    ┌─────────────┐
                    │ CIPHERTEXT  │
                    └─────────────┘
```

### **Key Components Explained**

```
┌─────────────────────────────────────────────────────────────────┐
│              PRODUCT CRYPTOSYSTEM COMPONENTS                    │
├──────────────┬──────────────────────────────────────────────────┤
│   COMPONENT  │                   EXPLANATION                    │
├──────────────┼──────────────────────────────────────────────────┤
│              │                                                  │
│ SUBSTITUTION │ Replaces plaintext symbols to hide the          │
│ (Confusion)  │ relationship between the key and ciphertext     │
│              │                                                  │
│              │ Purpose:                                         │
│              │ • Makes relationship between key and            │
│              │   ciphertext as complex as possible              │
│              │ • Single-stage ciphers are easy to break        │
│              │ • Substitution obscures patterns                │
│              │                                                  │
│              │ Example: S-boxes in AES, DES                    │
├──────────────┼──────────────────────────────────────────────────┤
│              │                                                  │
│ TRANSPOSITION│ Rearranges positions of symbols to spread       │
│ (Diffusion)  │ plaintext statistics across ciphertext          │
│              │                                                  │
│              │ Purpose:                                         │
│              │ • Dissipates statistical structure of           │
│              │   plaintext over ciphertext                      │
│              │ • One plaintext bit affects many ciphertext     │
│              │   bits (Avalanche Effect)                        │
│              │                                                  │
│              │ Avalanche Effect:                                │
│              │ Change 1 bit in plaintext → 50% of             │
│              │ ciphertext bits change                          │
│              │                                                  │
│              │ Example: P-boxes in DES, ShiftRows in AES       │
├──────────────┼──────────────────────────────────────────────────┤
│              │                                                  │
│ MULTIPLE     │ Repeating substitution and transposition        │
│ ROUNDS       │ transformations multiple times                  │
│              │                                                  │
│              │ Purpose:                                         │
│              │ • Hides patterns more effectively               │
│              │ • Fiercely resists cryptanalysis                │
│              │ • Each round strengthens the cipher             │
│              │                                                  │
│              │ Examples:                                        │
│              │ • DES: 16 rounds                                │
│              │ • AES-128: 10 rounds                            │
│              │ • AES-192: 12 rounds                            │
│              │ • AES-256: 14 rounds                            │
└──────────────┴──────────────────────────────────────────────────┘
```

**Examples of Product Cryptosystems:**
- **DES** (Data Encryption Standard)
- **AES** (Advanced Encryption Standard)
- **Blowfish**
- **Twofish**

---

## 1.15 CRYPTANALYSIS

**Definition:** The science of breaking encryption systems to recover the key or plaintext without knowing the enciphering details.

### **Types of Cryptanalytic Attacks**

```
┌─────────────────────────────────────────────────────────────────┐
│                CRYPTANALYTIC ATTACK TYPES                       │
├──────────────┬──────────────────────────────────────────────────┤
│  ATTACK TYPE │              WHAT ATTACKER KNOWS                 │
├──────────────┼──────────────────────────────────────────────────┤
│              │                                                  │
│ Ciphertext-  │ • Only ciphertext                                │
│ Only Attack  │ • No plaintext information                       │
│              │ • Must use statistical analysis                  │
│              │ • Hardest attack                                 │
│              │                                                  │
│              │ Example: Frequency analysis on Caesar cipher     │
├──────────────┼──────────────────────────────────────────────────┤
│              │                                                  │
│ Known        │ • Ciphertext                                     │
│ Plaintext    │ • Some corresponding plaintext                   │
│ Attack (KPA) │ • Tries to deduce key                            │
│              │                                                  │
│              │ Example: Hill cipher vulnerability               │
│              │          (can solve linear equations)            │
├──────────────┼──────────────────────────────────────────────────┤
│              │                                                  │
│ Chosen       │ • Ciphertext                                     │
│ Plaintext    │ • Can choose plaintext and get ciphertext        │
│ Attack (CPA) │ • Analyzes patterns                              │
│              │                                                  │
│              │ Example: Attacker sends specific messages        │
│              │          to encryption oracle                    │
├──────────────┼──────────────────────────────────────────────────┤
│              │                                                  │
│ Chosen       │ • Ciphertext                                     │
│ Ciphertext   │ • Can choose ciphertext and get plaintext        │
│ Attack       │ • Rare in practice                               │
│              │                                                  │
│              │ Example: Attack on RSA with small exponent       │
├──────────────┼──────────────────────────────────────────────────┤
│              │                                                  │
│ Adaptive     │ • Can adaptively choose plaintexts or           │
│ Attacks      │   ciphertexts based on previous results          │
│              │ • Most powerful                                  │
│              │                                                  │
│              │ Example: Differential cryptanalysis              │
│              │          Linear cryptanalysis                    │
└──────────────┴──────────────────────────────────────────────────┘
```

---

## 1.16 STEGANOGRAPHY

**Definition:** Hiding the **existence** of a message within another file (image, audio, video).

### **Steganography vs Cryptography**

```
┌─────────────────────────────────────────────────────────────────┐
│          STEGANOGRAPHY vs CRYPTOGRAPHY                          │
├────────────────────────────┬────────────────────────────────────┤
│    STEGANOGRAPHY           │     CRYPTOGRAPHY                   │
├────────────────────────────┼────────────────────────────────────┤
│                            │                                    │
│ Hides the EXISTENCE of     │ Hides the MEANING of               │
│ the message                │ the message                        │
│                            │                                    │
│ ┌──────────────┐          │ ┌──────────────┐                  │
│ │ Normal Image │          │ │ HELLO WORLD  │                  │
│ │ (with hidden │          │ │      ↓       │                  │
│ │  message)    │          │ │  ENCRYPT     │                  │
│ └──────────────┘          │ │      ↓       │                  │
│   Looks innocent          │ │ X7#mK9@pL2   │                  │
│   No suspicion            │ │ (Ciphertext) │                  │
│                           │ └──────────────┘                  │
│                           │   Looks scrambled                   │
│                           │   Obviously encrypted               │
├────────────────────────────┼────────────────────────────────────┤
│ ADVANTAGES:                │ ADVANTAGES:                        │
│ • Doesn't attract attention│ • Mathematically secure            │
│ • Passes visual inspection │ • Standardized algorithms          │
│ • Good for covert channels │ • Scalable for large data          │
├────────────────────────────┼────────────────────────────────────┤
│ DISADVANTAGES:             │ DISADVANTAGES:                     │
│ • Low capacity (small      │ • Obvious that data is encrypted   │
│   message in large file)   │ • May be blocked by censors        │
│ • Fragile (compression     │ • Attracts attention               │
│   destroys hidden data)    │                                    │
│ • Once discovered, no      │                                    │
│   protection               │                                    │
└────────────────────────────┴────────────────────────────────────┘
```

### **Example: LSB Steganography**

**LSB (Least Significant Bit)** technique hides data in the least significant bits of image pixels.

```
┌─────────────────────────────────────────────────────────────────┐
│            LSB STEGANOGRAPHY EXAMPLE                            │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│ Original Pixel Values (RGB):                                   │
│ ─────────────────────────                                       │
│ Pixel 1: (154, 235, 127) → Binary:                             │
│          10011010 11101011 01111111                            │
│             ↑        ↑         ↑                               │
│          LSB=0    LSB=1     LSB=1                              │
│                                                                 │
│ Secret Message: "HI" → ASCII: H=72, I=73                       │
│                          Binary: 01001000 01001001             │
│                                                                 │
│ Embedding Process:                                              │
│ ───────────────────                                             │
│                                                                 │
│ Replace LSB of each color channel with message bits:           │
│                                                                 │
│ Pixel 1: 1001101[0] → Change to 1001101[0] (bit 0)            │
│          1110101[1] → Change to 1110101[1] (bit 1)            │
│          0111111[1] → Change to 0111111[0] (bit 0)            │
│                                                                 │
│ New Pixel 1: (154, 235, 126)  ← Almost identical!              │
│                                                                 │
│ Human eye cannot detect this tiny change!                      │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

---

## 1.17 ZERO TRUST SECURITY ARCHITECTURE

**Definition:** A security model based on the principle **"Never trust, always verify"**. No user or device is trusted automatically, whether inside or outside the network perimeter.

### **Old Model vs Zero Trust Model**

```
┌─────────────────────────────────────────────────────────────────┐
│       TRADITIONAL MODEL vs ZERO TRUST MODEL                     │
├────────────────────────────┬────────────────────────────────────┤
│   TRADITIONAL (OLD)        │     ZERO TRUST (NEW)               │
│   "Castle-and-Moat"        │     "Verify Everything"            │
├────────────────────────────┼────────────────────────────────────┤
│                            │                                    │
│  ┌──────────────────┐     │  ┌──────────────────┐             │
│  │   FIREWALL       │     │  │   NO PERIMETER   │             │
│  │  (Moat)          │     │  │   ASSUMPTION     │             │
│  └────────┬─────────┘     │  └─────────────────┘             │
│           │                │           │                        │
│     ══════╪══════          │     ══════╪══════                 │
│    ╱      │      ╲         │    ╱      │      ╲                │
│   ╱   TRUSTED    ╲        │   ╱  VERIFY   ╲                   │
│  ╱    INTERNAL    ╲       │  ╱   EVERY     ╲                  │
│ │     NETWORK      │      │ │    REQUEST    │                 │
│ │                  │      │ │               │                  │
│ │ • Trusted by     │      │ │ • Never trust │                 │
│ │   default        │      │ • Always verify│                  │
│ │ • Free movement  │      │ • Micro-       │                  │
│ │ • Once inside,   │      │   segmentation │                  │
│ │   attacker moves │      │ • Least        │                  │
│ │   freely         │      │   privilege    │                  │
│                    │      │                │                   │
│ WEAKNESS:          │      │ STRENGTH:      │                   │
│ If attacker        │      │ Even if        │                   │
│ breaches firewall, │      │ perimeter      │                   │
│ they own network   │      │ breached,      │                   │
│                    │      │ damage limited │                   │
└────────────────────┴────────────────────────────────────────────┘
```

### **Key Principles of Zero Trust**

```
┌─────────────────────────────────────────────────────────────────┐
│              ZERO TRUST KEY PRINCIPLES                          │
├──────────┬──────────────────────────────────────────────────────┤
│ PRINCIPLE│                    EXPLANATION                       │
├────────────────────────────────────────────────────────────────┤
│          │                                                      │
│    1     │ NEVER TRUST, ALWAYS VERIFY                          │
│          │ ─────────────────────────                           │
│          │ • No user or device trusted by default              │
│          │ • Verify every access request                       │
│          │ • Inside or outside network - same verification     │
│          │ • Assume network is already breached                │
├──────────┼──────────────────────────────────────────────────────┤
│          │                                                      │
│    2     │ LEAST PRIVILEGE ACCESS                              │
│          │ ─────────────────────                               │
│          │ • Grant minimum permissions needed                  │
│          │ • Just-In-Time (JIT) access                         │
│          │ • Just-Enough-Access (JEA)                          │
│          │ • Reduces impact of compromised accounts            │
├──────────┼──────────────────────────────────────────────────────┤
│          │                                                      │
│    3     │ MICRO-SEGMENTATION                                  │
│          │ ───────────────────                                 │
│          │ • Divide network into small secure zones            │
│          │ • Isolate workloads from each other                 │
│          │ • Prevents lateral movement                         │
│          │ • If one segment breached, others safe              │
├──────────┼──────────────────────────────────────────────────────┤
│          │                                                      │
│    4     │ CONTINUOUS MONITORING                               │
│          │ ────────────────────                                │
│          │ • Not just one-time login check                     │
│          │ • Continuously evaluate:                            │
│          │   - Device posture                                  │
│          │   - User behavior                                   │
│          │   - Threat intelligence                             │
│          │ • Real-time risk assessment                         │
├────────────────────────────────────────────────────────────────┤
│          │                                                      │
│    5     │ STRONG AUTHENTICATION                               │
│          │ ─────────────────────                               │
│          │ • Multi-Factor Authentication (MFA)                 │
│          │ • Identity Access Management (IAM)                  │
│          │ • Device health verification                        │
│          │ • Certificate-based authentication                  │
└──────────┴──────────────────────────────────────────────────────┘
```

### **NIST 800-207 Zero Trust Architecture**

```
                    ┌─────────────────────────┐
                    │    CONTROL PLANE        │
                    │                         │
                    │  ┌──────────────────┐  │
                    │  │ Policy Decision  │  │
                    │  │ Point (PDP)      │  │
                    │  │                  │  │
                    │  │ • Policy Engine  │  │
                    │  │ • Policy         │  │
                    │  │   Administrator  │  │
                    │  └─────────────────┘  │
                    │           │             │
                    │           │ Grants/     │
                    │           │ Denies      │
                    │           │ Access      │
                    └───────────┼─────────────┘
                                │
                                ▼
┌─────────┐           ┌─────────────────────────┐           ┌──────────┐
│  USER   │──────────▶│    DATA PLANE           │──────────▶│ RESOURCE │
│         │           │                         │           │ (App/    │
│ (Device)│           │  ┌──────────────────┐  │           │  Data)   │
└─────────           │  │ Policy Enforcement│  │           └──────────┘
                      │  │ Point (PEP)      │  │
                      │  │                  │  │
                      │  │ • Enforces       │  │
                      │  │   decisions      │  │
                      │  │   from PDP       │  │
                      │  └──────────────────┘  │
                      └─────────────────────────┘
```

### **Five Pillars of Zero Trust**

```
┌─────────────────────────────────────────────────────────────────┐
│              FIVE PILLARS OF ZERO TRUST                         │
├──────────┬──────────────────────────────────────────────────────┤
│  PILLAR  │                    FOCUS AREA                        │
├────────────────────────────────────────────────────────────────┤
│    1     │ IDENTITY                                             │
│          │ • Verify user identity                               │
│          │ • Strong authentication (MFA)                        │
│          │ • Identity federation                                │
├──────────┼──────────────────────────────────────────────────────┤
│    2     │ DEVICES                                              │
│          │ • Verify device health                               │
│          │ • Device compliance checks                           │
│          │ • Endpoint security                                  │
├──────────┼──────────────────────────────────────────────────────┤
│    3     │ NETWORKS                                             │
│          │ • Micro-segmentation                                 │
│          │ • Software-defined perimeters                        │
│          │ • Encrypted communications                           │
├──────────┼──────────────────────────────────────────────────────┤
│    4     │ APPLICATIONS/WORKLOADS                               │
│          │ • Application-level access control                   │
│          │ • API security                                       │
│          │ • Container security                                 │
├──────────┼──────────────────────────────────────────────────────┤
│    5     │ DATA                                                 │
│          │ • Data classification                                │
│          │ • Encryption at rest and in transit                  │
│          │ • Data loss prevention (DLP)                         │
└────────────────────────────────────────────────────────────────┘
```

---

