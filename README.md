# 🎯 MASTER CYBERSECURITY STUDY GUIDE: CENTUM EDITION
## Course: 23CYC01 - Cyber Security Essentials
### Target: 100/100 | Target Length: 50+ Pages Equivalent
### Based on: SKCT Regulations 2022 | Semester 3/4 | B.E/B.Tech CSE (Cyber Security)

---

```
┌─────────────────────────────────────────────────────────┐
│  📚 GUIDE STRUCTURE                                     │
├─────────────────────────────────────────────────────────┤
│  UNIT 1: INTRODUCTION TO SECURITY              [~18 pp] │
│  UNIT 2: SECURITY IN OS & DEFENCES             [~18 pp] │
│  UNIT 3: CYBER SECURITY MANAGEMENT             [~18 pp] │
├─────────────────────────────────────────────────────────┤  
└─────────────────────────────────────────────────────────┘
```

---

# 🔷 UNIT 1: INTRODUCTION TO SECURITY
## (Weightage: 15 Marks | Topics: Security Concepts, Attacks, Cryptography, Zero Trust)

---

## 1.1 COMPUTER SECURITY CONCEPTS

### 1.1.1 Definition of Computer Security (NIST Standard)

**Computer Security** is the protection afforded to an automated information system in order to attain the applicable objectives of preserving the **Integrity, Availability, and Confidentiality** of information system resources.

**Resources Protected Include:**
- Hardware (servers, routers, endpoints)
- Software (applications, OS, firmware)
- Data/Information (databases, files, credentials)
- Telecommunications (network channels, protocols)

> 📝 **Exam Integration (CIA1 Q1):** Computer security ensures that only authorized users can access systems, data remains unaltered, and services remain available when needed.

---

### 1.1.2 The CIA Triad: Core Security Goals

```
                    ┌─────────────────┐
                    │   CIA TRIAD     │
                    │  (Security Goals)│
                    └────────┬────────┘
           ┌─────────────────┼─────────────────┐
           ▼                 ▼                 ▼
    ┌────────────┐ ┌────────────┐ ┌────────────┐
    │CONFIDENTIAL│ │ INTEGRITY  │ │AVAILABILITY│
    │   -ITY     │ │            │ │            │
    ├────────────┤ ├────────────┤ ├────────────┤
    │• Prevent   │ │• Prevent   │ │• Ensure    │
    │  unauthorized│ │  unauthorized│ │  authorized│
    │  access    │ │  modification│ │  access  │
    │• Encryption│ │• Hashing  │ │• Redundancy│
    │• Access Ctrl│ │• Digital Sig│ │• Backups │
    └────────────┘ └────────────┘ └────────────┘
```

| Goal | Definition | Attack That Violates | Countermeasure |
|------|-----------|---------------------|----------------|
| **Confidentiality** | Information accessible only to authorized entities | Disclosure/Eavesdropping | Encryption, Access Control |
| **Integrity** | Data cannot be altered without detection | Alteration/Modification | Hashing, Digital Signatures |
| **Availability** | Systems accessible when needed by authorized users | Denial of Service | Redundancy, Load Balancing |

> 📝 **Exam Integration (CIA2 Q1):** When a university's authentication server goes down, blocking staff access, the violated principle is **Availability**—authorized users cannot access the system upon demand.

---

### 1.1.3 The DAD Triad: Failure Counterparts

The **DAD Triad** represents the attack outcomes that directly oppose the CIA goals:

```
    CIA (Defense)          DAD (Attack)
    ─────────────          ────────────
    Confidentiality  ←→   Disclosure
    Integrity        ←→   Alteration  
    Availability     ←→   Denial
```

**Additional Security Properties:**
- **Authenticity**: Verifying that data/users are genuine and not impersonated
- **Accountability/Non-Repudiation**: Ensuring actions can be traced to specific entities; prevents denial of sent messages or performed actions

> 📝 **Exam Integration (CIA1 Q2):** A hacker intercepting a valid message and retransmitting it later performs a **Replay Attack** (Active Attack), violating Integrity and Authentication.

---

### 1.1.4 FIPS 199: Impact Level Classification

When security is breached, impacts are categorized per **FIPS 199**:

| Impact Level | Description | Example Scenario |
|-------------|-------------|-----------------|
| **Low** | Limited adverse effect; minor financial loss | Public website defacement |
| **Moderate** | Serious adverse effect; significant financial harm | Student enrollment data leaked |
| **High** | Severe/catastrophic effect; loss of life or mission | SCADA power grid hacked; patient data altered |

---

## 1.2 CYBERSECURITY THREATS, VULNERABILITIES & ATTACKS

### 1.2.1 Threat Classifications by Sophistication

| Threat Type | Characteristics | Example Actors | Tools Used |
|------------|----------------|---------------|-----------|
| **Unstructured** | Low skill, known exploits, opportunistic | Script kiddies | LOIC, basic scanners |
| **Structured** | Organized, well-funded, targeted attacks | Cybercriminal gangs | Nmap, Metasploit, Shodan |
| **Highly Structured** | Nation-state, zero-days, long-term planning | APT groups, state sponsors | Stuxnet, custom malware |

### 1.2.2 Malware Deep Dive

| Malware Type | Behavior | Propagation | Example |
|-------------|----------|-------------|---------|
| **Virus** | Attaches to legitimate programs; requires user execution | File sharing, email attachments | Melissa, ILOVEYOU |
| **Worm** | Self-replicating; spreads autonomously across networks | Network vulnerabilities | Code Red, Conficker |
| **Trojan** | Disguised as legitimate software; hidden malicious payload | Social engineering, fake downloads | Zeus, Emotet |
| **Botnet** | Network of infected "zombie" machines under attacker control | Worms, drive-by downloads | Mirai, Necurs |
| **Rootkit** | Operates at kernel level; hides its existence | Exploits, privilege escalation | Sony XCP, TDL-4 |
| **Spyware/Keylogger** | Covertly collects user data, keystrokes, browsing habits | Bundled software, exploits | DarkComet, HawkEye |
| **Zero-Day** | Exploits unknown vulnerability; no patch exists | Targeted attacks, APTs | Stuxnet, SolarWinds |

> 📝 **Exam Integration (CIA1 Q7):** Rootkit characteristics: (1) Runs at kernel/root level with full system access, (2) Hides files/processes from OS and antivirus, (3) Persists after reboot via boot sector/kernel hooks, (4) Opens backdoors for remote access, (5) Extremely difficult to remove without hardware-level tools.

---

### 1.2.3 The OSI Security Architecture (X.800 Standard)

#### Security Attacks Classification

```
                    SECURITY ATTACKS (X.800)
                           │
        ┌──────────────────┴──────────────────┐
        ▼                                     ▼
┌───────────────┐                 ┌─────────────────┐
│ PASSIVE ATTACKS│                 │  ACTIVE ATTACKS │
│ • No data modification│         │ • Data altered/blocked│
│ • Hard to detect    │         │ • Easier to detect  │
│ • Breaks Confidentiality│       │ • Breaks Integrity/ │
│                      │         │   Availability/Auth │
├───────────────┤                 ├─────────────────┤
│ Types:        │                 │ Types:          │
│ • Release of  │                 │ • Masquerade    │
│   message     │                 │ • Replay        │
│   contents    │                 │ • Modification  │
│ • Traffic     │                 │ • DoS           │
│   Analysis    │                 │                 │
└───────────────┘                 └─────────────────┘
```

> 📝 **Exam Integration (CIA1 Q2 + CIA2 Q10i):** 
> - **Passive Attack Example**: Eavesdropping on unencrypted HTTP traffic to capture login credentials.
> - **Active Attack Example**: SYN Flood attack filling server connection tables to cause Denial of Service.

#### Security Services (X.800)

| Service | Purpose | Implementation Example |
|---------|---------|----------------------|
| **Authentication** | Verify identity of communicating entities | Digital certificates, Kerberos, MFA |
| **Access Control** | Prevent unauthorized resource usage | ACLs, RBAC, firewalls |
| **Data Confidentiality** | Protect data from unauthorized disclosure | AES encryption, TLS/SSL |
| **Data Integrity** | Detect unauthorized data modification | SHA-256 hashing, HMAC, digital signatures |
| **Non-Repudiation** | Prevent denial of sent/received messages | RSA digital signatures, PKI |

#### Security Mechanisms

**Specific Mechanisms (Layer-Specific):**
- **Encipherment**: Transform plaintext → ciphertext (confidentiality)
- **Digital Signature**: Authenticate source + ensure integrity + non-repudiation
- **Access Control Mechanism**: Enforce authorization rules (ACLs, capabilities)
- **Data Integrity Mechanism**: Detect modification (checksums, MACs)
- **Authentication Exchange**: Verify identity via protocol (challenge-response)
- **Traffic Padding**: Insert dummy data to defeat traffic analysis
- **Routing Control**: Select secure network paths for sensitive data

**Pervasive Mechanisms (System-Wide):**
- **Trusted Functionality**: Ensure components operate per security policy
- **Security Labels**: Tag data with classification levels (Unclassified, Secret)
- **Event Detection**: Monitor for security violations (IDS/SIEM)
- **Security Audit Trail**: Maintain tamper-proof logs for forensics
- **Security Recovery**: Restore operations after security failure (backups, DRP)

> 📝 **Exam Integration (CIA1 Q11i + CIA2 Q10ii):** For an online banking system:
> 1. **Prevent Unauthorized Access**: Authentication (MFA) + Access Control (RBAC) + Confidentiality (TLS encryption)
> 2. **Detect Suspicious Activity**: Integrity (HMAC on transactions) + Event Detection (IDS monitoring) + Audit Trail (logging all actions)
> 3. **Recover from Breaches**: Security Recovery (isolated backups) + Redundant infrastructure for availability

---

### 1.2.4 Model for Network Security

```
                    NETWORK SECURITY MODEL
┌─────────────────────────────────────────────────┐
│                                                 │
│  [SENDER] → [ENCRYPTION] ===(Ciphertext)=== → [DECRYPTION] → [RECEIVER] │
│              ↑                    ↑                    ↑              │
│         [Secret Key]    [INSECURE CHANNEL]    [Secret Key]           │
│                                   │                                  │
│                          [OPPONENT/SNIFFER]                         │
│                                   │                                  │
│              [TRUSTED THIRD PARTY - Key Distribution]               │
│                                                 │
└─────────────────────────────────────────────────┘
```

**Four Basic Tasks in Designing Security Services:**
1. **Design Algorithm**: Create secure encryption/decryption transformation
2. **Generate Secret Key**: Produce cryptographically strong keys
3. **Distribute Trust**: Securely share keys via trusted third party (CA, KDC)
4. **Specify Protocol**: Define rules for secure communication exchange

> 📝 **Exam Integration (CIA1 Q3 + CIA2 Q3):** The network security model ensures that even if an opponent intercepts ciphertext on an insecure channel, they cannot understand it without the secret key, which is distributed securely via a trusted third party.

---

## 1.3 CLASSICAL ENCRYPTION TECHNIQUES

### 1.3.1 Steganography vs. Cryptography

| Aspect | Steganography | Cryptography |
|--------|--------------|--------------|
| **Goal** | Hide the *existence* of the message | Hide the *meaning* of the message |
| **Method** | Embed data in cover medium (image LSBs, audio) | Transform plaintext via algorithm + key |
| **Security** | Security through obscurity; fails if discovered | Mathematical security; secure even if algorithm known |
| **Overhead** | High (large cover file for small secret) | Low (ciphertext ≈ plaintext size) |
| **Weakness** | Fragile to compression/modification; detectable via steganalysis | Vulnerable to cryptanalysis if key weak or algorithm flawed |

> 📝 **Exam Integration (CIA1 Q3 + CIA2 Q10ii):** Steganography's main drawback: once the hidden message is discovered via steganalysis, it can be read directly because there's no key protecting it. Encryption protects content even if intercepted.

---

### 1.3.2 Substitution Techniques

#### Caesar Cipher (Monoalphabetic)

**Formula**: `C = (P + k) mod 26` where P=plaintext letter position (A=0), k=key shift, C=ciphertext

**🔴 Exam Numerical: Encrypt "DATA" with key k=5**
```
D(3) + 5 = 8 → I
A(0) + 5 = 5 → F  
T(19) + 5 = 24 → Y
A(0) + 5 = 5 → F
Ciphertext: IFYF
```

**🔴 Exam Numerical: Decrypt "IFMMP" with key k=3**
```
Decryption: P = (C - k) mod 26
I(8) - 3 = 5 → F
F(5) - 3 = 2 → C  ❌ Wait, let's recalculate properly:

I(8) - 3 = 5 → F? No: A=0,B=1,C=2,D=3,E=4,F=5,G=6,H=7,I=8
So: I(8)-3=5=F, F(5)-3=2=C, M(12)-3=9=J, M(12)-3=9=J, P(15)-3=12=M
Result: FCJJM? That's not meaningful.

Let me use the standard example from materials:
Decrypt "PHHW" with k=3:
P(15)-3=12=M, H(7)-3=4=E, H(7)-3=4=E, W(22)-3=19=T → "MEET" ✓
```

**Why Caesar Cipher is Weak:**
- Only 25 possible keys → brute force trivial
- Preserves letter frequency → vulnerable to frequency analysis
- No key management security

#### Vigenère Cipher (Polyalphabetic)

**Formula**: `C_i = (P_i + K_i) mod 26` where key repeats cyclically

**🔴 Exam Numerical: Encrypt "SECURITY" with key "KEY"**
```
Plaintext:  S  E  C  U  R  I  T  Y
Position:  18  4  2 20 17  8 19 24
Key:        K  E  Y  K  E  Y  K  E
Key Pos:    10  4 24 10  4 24 10  4

C = (P+K) mod 26:
S: (18+10)=28 mod26=2 → C
E: (4+4)=8 → I
C: (2+24)=26 mod26=0 → A
U: (20+10)=30 mod26=4 → E
R: (17+4)=21 → V
I: (8+24)=32 mod26=6 → G
T: (19+10)=29 mod26=3 → D
Y: (24+4)=28 mod26=2 → C

Ciphertext: CIAEVGDC
```

> 📝 **Exam Integration (CIA1 Q6):** Vigenère is polyalphabetic—same plaintext letter can map to different ciphertext letters depending on key position, making frequency analysis harder than monoalphabetic ciphers.

---

### 1.3.3 Playfair Cipher (Digram Substitution)

**Rules:**
1. Create 5×5 matrix using keyword (omit duplicate letters; I/J share cell)
2. Split plaintext into digrams (pairs); insert 'X' between duplicate letters; add 'X' if odd length
3. **Same Row**: Replace each letter with the one to its right (wrap around)
4. **Same Column**: Replace each letter with the one below it (wrap around)  
5. **Rectangle**: Replace each letter with the one on its row at the opposite corner

**🔴 Exam Numerical: Encrypt "HELLO WORLD" with key "MONARCHY"**

**Step 1: Build Matrix**
```
M  O  N  A  R
C  H  Y  B  D
E  F  G  I/J K
L  P  Q  S  T
U  V  W  X  Z
```

**Step 2: Prepare Plaintext**
```
HELLOWORLD → HE LL OW OR LD
Duplicate L in "LL" → insert X: HE LX LO WO RL DX
```

**Step 3: Encrypt Each Digram**
```
HE: Rectangle → H(row2,col2), E(row3,col1) → opposite corners: C(row2,col1), F(row3,col2) → CF
LX: Rectangle → L(row4,col1), X(row5,col4) → opposite: S(row4,col4), U(row5,col1) → SU  
LO: Rectangle → L(row4,col1), O(row1,col2) → opposite: P(row4,col2), M(row1,col1) → PM
WO: Rectangle → W(row5,col3), O(row1,col2) → opposite: V(row5,col2), N(row1,col3) → VN
RL: Rectangle → R(row1,col5), L(row4,col1) → opposite: M(row1,col1), T(row4,col5) → MT
DX: Rectangle → D(row2,col5), X(row5,col4) → opposite: B(row2,col4), Z(row5,col5) → BZ

Final Ciphertext: CF SU PM VN MT BZ
```

> 📝 **Exam Integration (CIA1 Q4 + CIA2 Q10i):** Playfair uses digram substitution, making frequency analysis harder than single-letter ciphers. The matrix structure and rectangle rule provide confusion.

---

### 1.3.4 Transposition Techniques

#### Rail Fence Cipher (Depth=2)

**Method**: Write plaintext in zigzag across rows, then read row-by-row

**🔴 Exam Numerical: Encrypt "MEETME" with depth=2**
```
Write diagonally:
Rail 1: M   E   M
Rail 2:   E   T   E

Read rows: Rail1 + Rail2 = MEM + ETE = MEMETE
Ciphertext: MEMETE
```

**🔴 Exam Numerical: Decrypt "CTASERPOLSINCYCSI" with depth=3**
```
Length=17 chars, depth=3 zigzag pattern:
Row1 positions: 1,5,9,13,17 → 5 chars: C T A S E
Row2 positions: 2,4,6,8,10,12,14,16 → 8 chars: R P O L S I N C  
Row3 positions: 3,7,11,15 → 4 chars: Y C S I

Reconstruct zigzag reading column-wise:
C R Y P T O C L A S S I S N I C E
Plaintext: CRYPTO CLASS IS NICE
```

#### Columnar Transposition

**🔴 Exam Numerical: Encrypt "SECUREDATA" with key sequence 3-1-4-2**
```
Key: 3 1 4 2 → Alphabetical order: 1(B), 2(D), 3(A), 4(C)
So read columns in order: Column2, Column4, Column1, Column3

Write plaintext in rows of 4 columns:
Col1 Col2 Col3 Col4   [Key: 3  1  4  2]
 S    E    C    U     [    A  B  C  D  ]
 R    E    D    A
 T    A    (pad)

Read by key order (B→D→A→C = Col2→Col4→Col1→Col3):
Col2: E, E, A → EEA
Col4: U, A → UA  
Col1: S, R, T → SRT
Col3: C, D → CD

Ciphertext: EEAUASRTCD
```

> 📝 **Exam Integration (CIA1 Q11ii):** Double transposition applies two separate key-based rearrangements, making cryptanalysis exponentially harder because the attacker must reverse both permutations without knowing intermediate state.

---

### 1.3.5 Hill Cipher (Matrix-Based Substitution)

**Formula**: `C = (K × P) mod 26` where K=key matrix, P=plaintext vector, C=ciphertext vector

**🔴 Exam Numerical: Encrypt "HILLCIPHER" with key K = [[3,2],[8,5]]**

**Step 1: Convert to Numbers (A=0...Z=25)**
```
HI → [7,8], LL → [11,11], CI → [2,8], PH → [15,7], ER → [4,17]
```

**Step 2: Matrix Multiplication mod 26**
```
For HI [7,8]:
C = [[3,2],[8,5]] × [7,8] = [3×7+2×8, 8×7+5×8] = [37, 96]
37 mod 26 = 11 → L, 96 mod 26 = 18 → S → "LS"

For LL [11,11]:
C = [3×11+2×11, 8×11+5×11] = [55, 143]  
55 mod 26 = 3 → D, 143 mod 26 = 13 → N → "DN"

For CI [2,8]:
C = [3×2+2×8, 8×2+5×8] = [22, 56]
22 mod 26 = 22 → W, 56 mod 26 = 4 → E → "WE"

For PH [15,7]:
C = [3×15+2×7, 8×15+5×7] = [59, 155]
59 mod 26 = 7 → H, 155 mod 26 = 25 → Z → "HZ"

For ER [4,17]:
C = [3×4+2×17, 8×4+5×17] = [46, 117]
46 mod 26 = 20 → U, 117 mod 26 = 13 → N → "UN"

Final Ciphertext: LSDNWEHZUN
```

**🔴 Vulnerability: Known Plaintext Attack**
Because Hill cipher is linear algebra, if attacker knows m plaintext-ciphertext pairs for an m×m key matrix, they can solve:
`K = C × P⁻¹ mod 26`
Thus, Hill cipher is broken if any known plaintext is available.

> 📝 **Exam Integration (CIA2 Q11ii):** The primary attack on Hill cipher is Known Plaintext Attack—intercepting plaintext-ciphertext pairs allows solving linear equations to recover the key matrix.

---

### 1.3.6 Perfect Security & Information Theory

**Perfect Security (Shannon)**: Ciphertext reveals ZERO information about plaintext:
`Pr[M=m | C=c] = Pr[M=m]` for all messages m and ciphertexts c

**One-Time Pad (OTP)**: Only system achieving perfect security
- **Requirements**: 
  1. Key truly random
  2. Key length = plaintext length  
  3. Key used ONLY ONCE, then destroyed
- **Flaw**: Logistically impossible to securely distribute massive keys

**Vernam Cipher**: Binary XOR operation `C = P ⊕ K`; OTP is its perfect-security evolution

> 📝 **Exam Integration (CIA1 Q7):** Perfect security means ciphertext gives no information about plaintext; only One-Time Pad achieves this mathematically, but key distribution challenges make it impractical for most uses.

---

### 1.3.7 Product Cryptosystem & Modern Foundations

**Product Cryptosystem**: Combines multiple transformations sequentially for stronger security:
```
[Plaintext]
    │
    ▼
┌─────────────┐
│Substitution │ → Creates CONFUSION (hide key-ciphertext relationship)
└──────┬──────┘
       ▼
┌─────────────┐  
│Transposition│ → Creates DIFFUSION (spread plaintext statistics)
└──────┬──────┘
       ▼
   [Multiple Rounds]
       │
       ▼
[Ciphertext]
```

**Avalanche Effect**: Changing 1 bit of plaintext/key changes ~50% of ciphertext bits—critical for modern ciphers like AES.

**Cryptanalysis Purpose**: Recover key or plaintext without prior knowledge by exploiting:
- Statistical patterns (frequency analysis)
- Mathematical weaknesses (linear/differential cryptanalysis)
- Implementation flaws (side-channel attacks)

> 📝 **Exam Integration (CIA1 Q8):** Cryptanalysis aims to break encryption by recovering keys/plaintext; cryptography aims to create secure transformations. They are adversarial disciplines driving security evolution.

---

## 1.4 ZERO TRUST SECURITY ARCHITECTURE

### 1.4.1 Core Principle: "Never Trust, Always Verify"

**Traditional Model (Castle-and-Moat)**: Trust internal network; perimeter defense only. Once breached, attacker moves freely.

**Zero Trust Model**: Assume network already compromised. Verify EVERY request regardless of source location.

```
                    ZERO TRUST ARCHITECTURE (NIST 800-207)
┌─────────────────────────────────────────────────┐
│                                                 │
│  [CONTROL PLANE]                                │
│  ┌─────────────────────┐                        │
│  │ Policy Decision     │                        │
│  │ Point (PDP)         │                        │
│  │ • Policy Engine     │                        │
│  │ • Policy Admin      │                        │
│  └────────┬────────────┘                        │
│           │ Grants/Denies Access                │
│           ▼                                     │
│  [DATA PLANE]                                   │
│  ┌─────────────────────┐                        │
│  │ Policy Enforcement  │                        │
│  │ Point (PEP)         │                        │
│  │ • Intercepts ALL    │                        │
│  │   requests          │                        │
│  └────────┬────────────┘                        │
│           │                                     │
│  [User] → [PEP] → [Resource]                   │
│           │                                     │
│  [Continuous Monitoring & Analytics]           │
│                                                 │
└─────────────────────────────────────────────────┘
```

### 1.4.2 Five Pillars of Zero Trust

| Pillar | Implementation | Security Benefit |
|--------|---------------|-----------------|
| **Identity** | MFA, IAM, behavioral analytics | Prevents credential theft attacks |
| **Devices** | Device posture checking, MDM | Blocks compromised endpoints |
| **Network** | Micro-segmentation, encryption | Limits lateral movement |
| **Applications** | API security, runtime protection | Protects app-layer vulnerabilities |
| **Data** | Classification, encryption, DLP | Prevents data exfiltration |

### 1.4.3 Key Principles in Practice

1. **Least Privilege Access**: Grant minimum permissions needed; Just-In-Time access
2. **Micro-segmentation**: Divide network into isolated zones; breach in one zone doesn't spread
3. **Continuous Monitoring**: Evaluate user/device behavior in real-time; detect anomalies
4. **Strong Authentication**: MFA mandatory; certificate-based where possible
5. **Assume Breach**: Design defenses assuming attacker is already inside

> 📝 **Exam Integration (CIA2 Q12i):** Zero Trust enhances security by eliminating implicit trust, enforcing least privilege, segmenting networks to contain breaches, and continuously verifying all access requests—critical for cloud and remote work environments.

---

# 🔷 UNIT 2: SECURITY IN OPERATING SYSTEMS AND DEFENCES
## (Weightage: 15 Marks | Topics: OS Security, Rootkits, Network Attacks, Countermeasures, Databases)

---

## 2.1 SECURITY IN OPERATING SYSTEMS

### 2.1.1 OS Protection Functions

The OS enforces security through:
1. **Enforced Sharing**: Table lookups ensure safe resource sharing between processes
2. **IPC & Synchronization**: Secure bridges for inter-process communication
3. **Guaranteed Fair Service**: Hardware clocks prevent process starvation
4. **Memory Protection**: Prevent Process A from overwriting Process B or OS

### 2.1.2 Hardware Memory Protection Mechanisms

#### Base and Bounds Registers (Most Important for Exams)

```
                    MEMORY PROTECTION WITH BASE/BOUNDS
┌─────────────────────────────────────────────────┐
│                                                 │
│  [OS Memory]                                    │
│  ─────────                                      │
│  [User Process A Sandbox]                       │
│  Base Register = 0x1000  ← Start address        │
│  Bounds Register = 0x5000 ← End address         │
│                                                 │
│  Hardware Check for EVERY memory access:        │
│  IF (Base ≤ Address ≤ Bounds) → ALLOW          │
│  ELSE → TRAP to OS (Access Violation)          │
│                                                 │
│  Context Switch to Process B:                  │
│  Simply update Base/Bounds registers            │
│                                                 │
└─────────────────────────────────────────────────┘
```

**Advantages**: Perfect process isolation; hardware-enforced; efficient context switching

#### Other Mechanisms Comparison

| Mechanism | Concept | Advantage | Limitation |
|-----------|---------|-----------|-----------|
| **Fence Register** | Single boundary between OS and user | Simple | Only protects OS, not user-user isolation |
| **Base/Bounds** | Two registers define sandbox | Perfect isolation | Requires hardware support |
| **Tagged Architecture** | Every memory word has access tags | Fine-grained control | Expensive custom hardware |
| **Segmentation** | Logical divisions (code/data) | OS can assign different rights per segment | External fragmentation |
| **Paging** | Fixed-size page frames | Eliminates fragmentation; efficient | Pages lack logical unity for security policies |
| **Paged Segmentation** | Segments divided into pages | Combines logical security + memory efficiency | Complex address translation |

> 📝 **Exam Integration (CIA1 Q9 + CIA2 Q12ii):** Memory segmentation provides two key security benefits: (1) Logical isolation allows different access rights per segment (e.g., code=execute-only, data=read-write), enforcing integrity; (2) Hardware-enforced bounds prevent buffer overflows from corrupting other segments or the OS.

---

### 2.1.3 Rootkits: Subverting the OS Core

**Definition**: Malicious code operating at highest privilege level (Ring 0/kernel) that actively conceals its existence from OS, antivirus, and users.

#### How Rootkits Evade Detection: API Hooking/Splicing

```
                    ROOTKIT API INTERCEPTION
┌─────────────────────────────────────────────────┐
│                                                 │
│  Normal Program (e.g., Antivirus) calls:       │
│  FindNextFile() → List files in directory      │
│                    │                            │
│                    ▼                            │
│  [OS Kernel API]                                │
│         │                                       │
│         │  ROOTKIT HAS MODIFIED THIS POINTER   │
│         ▼                                       │
│  [Rootkit Interceptor] ← Hooked function        │
│         │                                       │
│         │ 1. Call original OS function         │
│         │ 2. Get file list                     │
│         │ 3. FILTER OUT malicious files        │
│         │ 4. Return "clean" list to antivirus  │
│         ▼                                       │
│  Antivirus sees: "System is clean" ❌          │
│                                                 │
└─────────────────────────────────────────────────┘
```

#### Famous Rootkit Case Studies

| Rootkit | Year | Technique | Impact |
|---------|------|-----------|---------|
| **Sony XCP** | 2005 | Hooked OS to hide files starting with `$sys$` | Malware writers used `$sys$` prefix to hide their own viruses; Sony's DRM rootkit became universal malware cloak |
| **TDL-4/Alureon** | 2008-2010 | Infected Master Boot Record (MBR); created hidden encrypted filesystem | Bypassed Windows driver signature checks; loaded before OS, achieving total stealth |
| **Mobile Rootkits** | Research | Silently activated GPS/mic; drained battery via Bluetooth | Demonstrated smartphones vulnerable to undetectable surveillance and denial-of-service |

> 📝 **Exam Integration (CIA1 Q7 + CIA2 Q8):** Rootkits differ from other malware by operating at kernel level (Ring 0), intercepting system calls to hide their presence, and persisting through reboots—making them extremely difficult to detect or remove without specialized offline tools.

---

## 2.2 NETWORK SECURITY ATTACKS & WIRELESS THREATS

### 2.2.1 Threats to Network Communications

| Threat Type | Description | Security Property Violated | Example |
|------------|-------------|---------------------------|---------|
| **Interception** | Unauthorized eavesdropping on data | Confidentiality | Packet sniffing on unencrypted Wi-Fi |
| **Modification** | Altering data in transit | Integrity | MITM changing bank transfer amount |
| **Fabrication** | Inserting fake data/messages | Integrity/Authentication | Spoofed login requests |
| **Interruption** | Blocking/denying service | Availability | DoS/DDoS attacks |

#### Advanced Network Attacks

**Port Scanning (Reconnaissance)**:
- Tools: Nmap, Shodan
- Purpose: Map open ports, services, OS versions to identify vulnerabilities
- Defense: Firewalls, IDS, minimize exposed services

**Session Hijacking (TCP)**:
1. Attacker monitors TCP 3-way handshake
2. Spoofs source IP and guesses sequence/acknowledgment numbers
3. Takes over established session, kicking out legitimate user
- Defense: Encryption (TLS), sequence number randomization, short session timeouts

**DNS Cache Poisoning**:
1. Attacker floods DNS server with fake IP resolutions
2. If query ID guessed correctly, server caches malicious mapping
3. All future users redirected to attacker's fake site
- Defense: DNSSEC, randomized query IDs, minimal cache TTL

---

### 2.2.2 Denial of Service (DoS) Attacks

#### Specific DoS Attack Mechanisms

```
┌─────────────────────────────────────────────────┐
│  SYN FLOOD ATTACK (Exploits TCP Handshake)     │
├─────────────────────────────────────────────────┤
│                                                 │
│  Normal TCP 3-Way:                             │
│  Client → SYN → Server                         │
│  Client ← SYN-ACK ← Server                     │
│  Client → ACK → Server [Connection Established]│
│                                                 │
│  SYN Flood Attack:                             │
│  Attacker → SYN (spoofed IP) → Server          │
│  Attacker ← SYN-ACK ← Server [NO ACK SENT]    │
│  Server allocates RAM for "half-open" connection│
│  Repeat millions of times → RAM exhausted     │
│  Server crashes or rejects legitimate users   │
│                                                 │
└─────────────────────────────────────────────────┘
```

| Attack | Mechanism | Target Resource | Defense |
|--------|-----------|----------------|---------|
| **Ping of Death** | Oversized ICMP packets causing buffer overflow | System memory/stack | Packet size filtering, OS patches |
| **Smurf Attack** | Spoof victim IP, ping broadcast address → entire network replies to victim | Bandwidth | Disable directed broadcasts, ingress filtering |
| **Echo-Chargen** | Create infinite loop between echo/chargen services | CPU/bandwidth | Disable unused services |
| **Teardrop** | Send fragmented packets with overlapping offsets causing reassembly crash | OS kernel | Packet reassembly validation, OS patches |
| **SYN Flood** | Exhaust connection table with half-open connections | Server memory/CPU | SYN cookies, rate limiting, firewalls |

---

### 2.2.3 Distributed Denial of Service (DDoS) & Botnets

**Botnet Architecture**:
```
                    BOTNET DDoS ATTACK FLOW
┌─────────────────────────────────────────────────┐
│                                                 │
│  [ATTACKER]                                     │
│       │                                         │
│       ▼                                         │
│  [Command & Control Server]                    │
│       │  (Encrypted commands via Push/Pull)    │
│       ▼                                         │
│  [Handler Machines - Tier 2]                   │
│       │                                         │
│       ▼                                         │
│  [Bots/Zombies - Tier 3]                       │
│  • Thousands of infected PCs, IoT devices      │
│  • Each sends attack traffic simultaneously    │
│       │                                         │
│       ▼                                         │
│  [TARGET SERVER]                               │
│  • Bandwidth/CPU/memory exhausted              │
│  • Legitimate users blocked                    │
│                                                 │
└─────────────────────────────────────────────────┘
```

**Why IP Blocking Fails Against DDoS**:
1. **Massive Scale**: Botnets contain 10,000-1,000,000+ IPs; blocking all is impossible
2. **IP Spoofing**: Attackers forge source IPs; blocking "attack IPs" harms innocent parties
3. **Dynamic IPs**: Home IoT devices use DHCP; blocked bots reconnect with new IPs
4. **Legitimate-Looking Traffic**: Application-layer DDoS mimics real user requests

**Real-World Examples**:
- **Mirai (2016)**: 600,000 IoT devices → 1.2 Tbps attack on Dyn DNS → Twitter/Netflix/Reddit down
- **GitHub (2018)**: 1.35 Tbps memcached amplification attack
- **AWS (2020)**: 2.3 Tbps attack (largest recorded) mitigated by AWS Shield

> 📝 **Exam Integration (CIA2 Q13i):** Blocking IPs is ineffective against DDoS because of botnet scale, IP spoofing, dynamic addressing, and application-layer attacks that mimic legitimate traffic—requiring multi-layered defenses like traffic scrubbing, CDNs, and behavioral analysis.

---

### 2.2.4 Wireless Network Security (IEEE 802.11)

#### Why WEP Failed Completely

| Flaw | Technical Reason | Consequence |
|------|-----------------|-------------|
| **Short IV (24-bit)** | Initialization Vector repeats quickly on busy networks | IV collisions allow RC4 key recovery via statistical attacks |
| **Static Keys** | Same encryption key used for all sessions, rarely changed | Compromise one session → all sessions vulnerable |
| **No Authentication** | Relies only on SSID/MAC (easily spoofed) | Rogue APs and clients can join freely |
| **Broken Integrity (CRC-32)** | Linear checksum allows bit-flipping without detection | Attacker can modify encrypted packets and adjust CRC to match |

**Tools that Break WEP**: Aircrack-ng can recover keys in minutes with ~50,000 captured packets.

#### IEEE 802.11i (WPA2) - The Solution: 5 Phases

```
┌─────────────────────────────────────────────────┐
│  IEEE 802.11i RSN OPERATION PHASES             │
├─────────────────────────────────────────────────┤
│                                                 │
│  Phase 1: DISCOVERY                            │
│  • AP broadcasts Beacon with RSN IE            │
│  • Station & AP agree on cipher suite (AES-CCMP)│
│                                                 │
│  Phase 2: AUTHENTICATION                       │
│  • PSK (WPA2-Personal) or 802.1X/EAP (Enterprise)│
│  • RADIUS server verifies credentials          │
│                                                 │
│  Phase 3: 4-WAY HANDSHAKE (Key Generation)    │
│  • AP sends ANonce → Station computes PTK      │
│  • Station sends SNonce+MIC → AP verifies     │
│  • AP sends GTK encrypted → Station confirms  │
│  • Result: Unique session keys per connection │
│                                                 │
│  Phase 4: PROTECTED DATA TRANSFER              │
│  • AES-CCMP encryption + 64-bit MIC           │
│  • 48-bit Packet Number prevents replay      │
│                                                 │
│  Phase 5: CONNECTION TERMINATION              │
│  • Secure deauthentication frame              │
│  • Session keys destroyed (forward secrecy)  │
│                                                 │
└─────────────────────────────────────────────────┘
```

**Key Innovations in WPA2**:
- **Dynamic Keys**: 4-way handshake generates unique PTK/GTK per session
- **Strong Encryption**: AES-CCMP replaces broken RC4
- **Message Integrity**: 64-bit MIC (Michael algorithm) prevents bit-flipping
- **Replay Protection**: Packet numbers ensure frames processed in order

> 📝 **Exam Integration (CIA2 Q13ii):** IEEE 802.11i's five phases provide layered security: discovery negotiates strong ciphers, authentication verifies identity, 4-way handshake creates unique session keys, AES-CCMP protects data integrity/confidentiality, and secure termination prevents key reuse—fixing all WEP vulnerabilities.

---

## 2.3 SECURITY COUNTERMEASURES

### 2.3.1 Cryptography in Network Security

#### Symmetric vs. Asymmetric Cryptography

| Feature | Symmetric (Secret Key) | Asymmetric (Public Key) |
|---------|----------------------|------------------------|
| **Keys Used** | Same key for encryption & decryption | Mathematically linked public/private key pair |
| **Speed** | Very fast (ideal for bulk data) | 100-1000× slower (computationally heavy) |
| **Key Distribution** | Problem: Securely share secret key beforehand | Solution: Public key published openly; private key kept secret |
| **Non-Repudiation** | ❌ Cannot prove who encrypted | ✅ Digital signatures provide non-repudiation |
| **Algorithms** | AES, 3DES, ChaCha20 | RSA, ECC, Diffie-Hellman |
| **Use Cases** | Encrypting files, database, TLS bulk data | Key exchange, digital signatures, certificates |

#### Hybrid Cryptosystems (How HTTPS/TLS Works)

```
                    HYBRID CRYPTO IN PRACTICE
┌─────────────────────────────────────────────────┐
│                                                 │
│  Step 1: Asymmetric Key Exchange               │
│  Client & Server use RSA/Diffie-Hellman to    │
│  securely agree on a temporary "Session Key"  │
│                                                 │
│  Step 2: Symmetric Bulk Encryption            │
│  Once Session Key established, switch to AES  │
│  for encrypting actual webpage/data transfer  │
│                                                 │
│  Result: Best of both worlds                  │
│  • Secure key distribution (asymmetric)       │
│  • Fast bulk encryption (symmetric)           │
│                                                 │
└─────────────────────────────────────────────────┘
```

#### 🔴 RSA Numerical Example (Most Important Exam Problem)

**Given**: p=5, q=11, e=3, message M=7  
**Find**: n, φ(n), d, encrypt, decrypt

**Step-by-Step Solution**:
```
1. Compute n = p × q = 5 × 11 = 55
2. Compute φ(n) = (p-1)(q-1) = 4 × 10 = 40
3. Find d such that: (e × d) mod φ(n) = 1
   (3 × d) mod 40 = 1
   Try d=27: 3×27=81; 81 mod 40 = 1 ✓ → d=27
4. Public Key: (e,n) = (3,55); Private Key: (d,n) = (27,55)
5. Encrypt: C = M^e mod n = 7^3 mod 55 = 343 mod 55 = 13
6. Decrypt: M = C^d mod n = 13^27 mod 55
   Use modular exponentiation:
   13^2=169 mod55=4; 13^4=4^2=16; 13^8=16^2=256 mod55=36;
   13^16=36^2=1296 mod55=31; 13^27=13^16×13^8×13^2×13^1
   =31×36×4×13 mod55 = (31×36=1116 mod55=16) ×4=64 mod55=9 ×13=117 mod55=7 ✓
   Decrypted M=7 (original message recovered)
```

#### 🔴 Diffie-Hellman Key Exchange Numerical

**Given**: p=23 (prime), g=5 (generator), A's secret=6, B's secret=15  
**Find**: Shared secret key

**Step-by-Step**:
```
1. A computes public value: A_pub = g^a mod p = 5^6 mod 23
   5^2=25 mod23=2; 5^4=2^2=4; 5^6=5^4×5^2=4×2=8 mod23 → A_pub=8
2. B computes public value: B_pub = g^b mod p = 5^15 mod 23
   5^1=5; 5^2=2; 5^4=4; 5^8=4^2=16; 5^15=5^8×5^4×5^2×5^1=16×4×2×5=640 mod23
   640÷23=27×23=621, remainder 19 → B_pub=19
3. A computes shared key: K = B_pub^a mod p = 19^6 mod 23
   19^2=361 mod23=16; 19^4=16^2=256 mod23=3; 19^6=19^4×19^2=3×16=48 mod23=2
4. B computes shared key: K = A_pub^b mod p = 8^15 mod 23
   8^2=64 mod23=18; 8^4=18^2=324 mod23=2; 8^8=2^2=4; 8^15=8^8×8^4×8^2×8^1=4×2×18×8=1152 mod23
   1152÷23=50×23=1150, remainder 2 → K=2 ✓
Both compute same shared key K=2 without ever transmitting it!
```

#### 🔴 Modular Exponentiation Practice
**Compute**: 3^45 mod 11
```
Use repeated squaring:
3^1 = 3 mod11
3^2 = 9 mod11  
3^4 = 9^2 = 81 mod11 = 4
3^8 = 4^2 = 16 mod11 = 5
3^16 = 5^2 = 25 mod11 = 3
3^32 = 3^2 = 9 mod11

45 = 32 + 8 + 4 + 1
3^45 = 3^32 × 3^8 × 3^4 × 3^1 = 9 × 5 × 4 × 3 mod11
= (9×5=45 mod11=1) × (4×3=12 mod11=1) = 1×1 = 1 mod11
Answer: 1
```

> 📝 **Exam Integration (Question Bank Q8-9):** RSA and Diffie-Hellman are high-probability numerical questions. Practice key generation, encryption/decryption steps, and modular arithmetic. Always show work for partial credit.

---

### 2.3.2 Firewalls

#### Firewall Types & Architecture

```
                    SCREENED SUBNET (DMZ) ARCHITECTURE
┌─────────────────────────────────────────────────┐
│                                                 │
│  [INTERNET]                                     │
│       │                                         │
│       ▼                                         │
│  ┌─────────────────┐                           │
│  │ EXTERNAL FIREWALL│                          │
│  │ (Less strict rules)│                        │
│  └────────┬────────┘                           │
│           │                                     │
│           ▼                                     │
│  ┌─────────────────┐                           │
│  │ DMZ (Public Servers)│                       │
│  │ • Web Server    │                           │
│  │ • Email Server  │                           │
│  │ • DNS Server    │                           │
│  └────────┬────────┘                           │
│           │                                     │
│           ▼                                     │
│  ┌─────────────────┐                           │
│  │ INTERNAL FIREWALL│                          │
│  │ (Very strict rules)│                        │
│  └────────┬────────┘                           │
│           │                                     │
│           ▼                                     │
│  ┌─────────────────┐                           │
│  │ INTERNAL LAN    │                           │
│  │ • HR Workstations│                          │
│  │ • Internal DB   │                           │
│  └─────────────────┘                           │
│                                                 │
└─────────────────────────────────────────────────┘
```

| Firewall Type | OSI Layer | How It Works | Pros | Cons |
|--------------|-----------|--------------|------|------|
| **Packet Filtering (Stateless)** | L3/L4 | Checks IP/port/protocol per packet | Fast, low resource | No connection state; vulnerable to spoofing |
| **Stateful Inspection** | L3/L4 + state table | Tracks connection state (SYN/ACK); allows return traffic | More secure; prevents many spoofing attacks | State table memory; vulnerable to SYN flood |
| **Application/Proxy** | L7 | Acts as intermediary; inspects application payload | Highest security; understands app context | Slow; may break non-proxy-aware apps |
| **Next-Generation (NGFW)** | Multi-layer | Combines stateful + DPI + IPS + app awareness + malware filtering | Comprehensive protection | Complex configuration; higher cost |

#### 🔴 Firewall Rule Evaluation Example
**Rule Set**:
1. Allow TCP port 80 (HTTP) from any source
2. Deny all other traffic

**Packet**: Source IP=192.168.1.100, Dest Port=443 (HTTPS), Protocol=TCP  
**Evaluation**: 
- Rule 1: Port 443 ≠ 80 → No match
- Rule 2: "Deny all" → Packet blocked  
**Result**: Denied (HTTPS not allowed by policy)

> 📝 **Exam Integration (Question Bank):** Firewalls enforce access control by filtering traffic based on rules. Stateful firewalls track connection state for better security; NGFWs add deep packet inspection and application awareness.

---

### 2.3.3 Intrusion Detection & Prevention Systems (IDPS)

#### IDS vs. IPS: Critical Differences

| Feature | IDS (Detection) | IPS (Prevention) |
|---------|----------------|-----------------|
| **Placement** | Out-of-band (SPAN port/tap); receives copy of traffic | In-line; all traffic passes through |
| **Action** | Generates alerts; cannot block traffic | Can block/drop packets, reset connections in real-time |
| **Risk** | No impact on network performance/availability | False positives can block legitimate traffic (availability risk) |
| **Use Case** | Monitoring, forensics, threat intelligence | Active defense, critical infrastructure protection |

#### Detection Methodologies

| Method | How It Works | Pros | Cons | Best For |
|--------|-------------|------|--------|----------|
| **Signature-Based** | Compare traffic against database of known attack patterns | Fast, accurate for known threats, low false positives | Blind to zero-day attacks; requires constant updates | Known malware, exploit patterns |
| **Anomaly-Based** | Build baseline of "normal" behavior; flag significant deviations | Can detect zero-days, insider threats, novel attacks | High false positives; requires training period; complex tuning | APTs, insider threats, novel attacks |

**🔴 Exam Case**: Sudden traffic spike detected  
- **IDS**: Alerts administrators to investigate potential DDoS  
- **IPS**: Can automatically rate-limit or block suspicious source IPs  
- **Decision**: Critical networks prefer IPS for automatic response; research networks may prefer IDS to avoid blocking legitimate traffic spikes

> 📝 **Exam Integration (CIA2 Q2 + Question Bank):** Intrusion prevention is preferred over detection in critical networks because IPS can block attacks in real-time, preventing damage rather than just alerting after the fact—though false positive risk requires careful tuning.

---

### 2.3.4 Network Management & SNMP Security

#### SNMP Architecture & Security Evolution

```
                    SNMP MANAGER-AGENT MODEL
┌─────────────────────────────────────────────────┐
│                                                 │
│  [SNMP Manager - Central Server]               │
│         │                                       │
│         │ GET/SET requests                      │
│         ▼                                       │
│  [Network: UDP Port 161/162]                  │
│         │                                       │
│         ▼                                       │
│  [SNMP Agent - Router/Switch/Firewall]        │
│         │                                       │
│         │ TRAP notifications (async alerts)    │
│         ▼                                       │
│  [Manager processes responses/updates MIB]    │
│                                                 │
└─────────────────────────────────────────────────┘
```

| SNMP Version | Security Features | Vulnerability |
|-------------|------------------|---------------|
| **SNMPv1/v2c** | Community string (password) sent in cleartext | Packet sniffers can capture community string → full device control |
| **SNMPv3** | • Authentication: HMAC-MD5/SHA<br>• Privacy: AES/DES encryption<br>• VACM: Granular access control | Complex configuration; performance overhead |

**Best Practice**: Always use SNMPv3 with authentication AND privacy enabled for production networks.

---

## 2.4 DATABASES: SECURITY & INTEGRITY

### 2.4.1 Security Requirements of Databases

| Requirement | Definition | Example Threat | Countermeasure |
|------------|-----------|---------------|---------------|
| **Physical Integrity** | Immunity to hardware failures, disasters | Disk crash, power failure | RAID, backups, UPS |
| **Logical Integrity** | Structure preserved during crashes/transactions | Partial transaction commit | ACID properties, 2PC |
| **Element Integrity** | Individual data values accurate and valid | SQL injection altering values | Input validation, parameterized queries |
| **Semantic Integrity** | Business rules enforced (e.g., age ≥ 18) | Application bug allowing invalid data | Database constraints, triggers |
| **Referential Integrity** | Foreign keys map to valid primary keys | Deleting parent record leaves orphaned child | Foreign key constraints |
| **Access Control** | Granular permissions (row/column level) | Employee viewing CEO salary | RBAC, row-level security |
| **Auditability** | Tamper-proof logs of all access/modifications | Insider deleting audit trails | Write-once storage, SIEM integration |

---

### 2.4.2 Reliability & Integrity: ACID Properties (CRITICAL FOR EXAMS)

**ACID** ensures database transactions are processed reliably:

| Property | Meaning | Example Scenario | Failure Consequence |
|----------|---------|-----------------|-------------------|
| **Atomicity** | "All or nothing": transaction completes fully or not at all | Money transfer: deduct from A, add to B | If crash after deducting from A but before adding to B → money lost |
| **Consistency** | Transaction moves DB from one valid state to another | Salary cannot be negative; foreign keys valid | Invalid data corrupts business logic, reports |
| **Isolation** | Concurrent transactions don't interfere; result = serial execution | Two users booking last seat on flight | Lost update: both think they booked, overbooking |
| **Durability** | Committed transactions persist despite crashes | Power failure after "Transaction Complete" | Lost sales, inconsistent inventory |

#### 🔴 Exam Case: Identify Failed ACID Property
**Scenario**: During fund transfer, system crashes after deducting from Account A but before adding to Account B.  
**Analysis**: Atomicity failed—transaction was not treated as indivisible unit; partial completion caused data inconsistency.  
**Solution**: Use transaction logs and rollback mechanisms to ensure atomicity.

---

### 2.4.3 Two-Phase Commit Protocol (2PC) for Distributed Databases

```
                    TWO-PHASE COMMIT PROTOCOL
┌─────────────────────────────────────────────────┐
│                                                 │
│  [Coordinator]      [Node 1]      [Node 2]     │
│        │                │             │         │
│        │ PHASE 1: PREPARE PHASE                │
│        │---------------->│             │         │
│        │ "Prepare to Commit"                  │
│        │                │---------------->│     │
│        │                │ "Prepare to Commit" │ │
│        │                │             │         │
│        │                │ (Check local state, │ │
│        │                │  acquire locks)    │ │
│        │<----------------│             │         │
│        │ "VOTE: READY" │             │         │
│        │<-----------------------------│         │
│        │                │ "VOTE: READY"│         │
│        │                │             │         │
│        │ PHASE 2: COMMIT PHASE (if ALL voted READY)│
│        │---------------->│             │         │
│        │ "Global Commit"│             │         │
│        │                │---------------->│     │
│        │                │ "Global Commit"│     │
│        │                │             │         │
│        │                │ (Write to disk)│     │
│        │<----------------│             │         │
│        │ "ACK: Committed"│            │         │
│        │<-----------------------------│         │
│        │                │ "ACK: Committed"│    │
│        │                │             │         │
│        ▼                ▼             ▼         │
│  [Transaction Complete - All nodes consistent]│
│                                                 │
│  If ANY node voted ABORT or timed out:        │
│  Coordinator sends "Global Rollback" to all   │
│                                                 │
└─────────────────────────────────────────────────┘
```

> 📝 **Exam Integration (CIA2 Q3 + Question Bank):** Database reliability and integrity are crucial for enterprise systems because financial transactions, inventory, and customer data must remain consistent even during failures—ACID properties and protocols like 2PC ensure this.

---

### 2.4.4 Database Disclosure & Inference Attacks

#### Types of Disclosure

| Type | Description | Example |
|------|-------------|---------|
| **Exact Data Disclosure** | Attacker learns precise sensitive value | Query reveals Alice's salary = $125,500 |
| **Bounds Disclosure** | Attacker determines value range | Average salary queries reveal Alice's salary is $120K-$130K |
| **Negative Result Disclosure** | Attacker learns what value is NOT | "List employees >$150K" excludes Alice → Alice earns <$150K |
| **Probabilistic Disclosure** | Attacker infers likelihood of value | Knowing Alice is Senior Engineer + 90% of Seniors earn >$100K → probable inference |

#### Inference Attack Defense: Polyinstantiation

**Problem**: In multilevel secure databases (Unclassified/Secret/Top Secret), users can infer classified data from unclassified queries.

**Solution**: Allow multiple rows with same primary key but different classification levels.

```
                    POLYINSTANTIATION EXAMPLE
┌─────────────────────────────────────────────────┐
│                                                 │
│  Database Table: SHIP_LOCATIONS                │
│                                                 │
│  Ship_ID | Destination      | Classification  │
│  --------|------------------|----------------│
│  ENT-01  | War Zone Alpha   | TOP SECRET    │
│  ENT-01  | Training Exercise| UNCLASSIFIED  │ ← Returned to unclassified users
│                                                 │
│  Unclassified User Query: "Where is USS Enterprise?"│
│  → Returns: "Training Exercise" (fake data)  │
│  → User cannot infer secret mission exists  │
│                                                 │
│  Top Secret User Query: Same question        │
│  → Returns: "War Zone Alpha" (real data)     │
│                                                 │
└─────────────────────────────────────────────────┘
```

> 📝 **Exam Integration (CIA2 Q10i + Question Bank):** Database disclosure occurs via direct queries or inference attacks. Polyinstantiation prevents inference by providing classification-appropriate data versions, hiding the existence of sensitive information from lower-clearance users.

---

# 🔷 UNIT 3: CYBER SECURITY MANAGEMENT
## (Weightage: 15 Marks | Topics: Planning, BCP, Incident Response, Risk, Industrial Security, Ethics)

---

## 3.1 SECURITY PLANNING & GOVERNANCE

### 3.1.1 Hierarchical Security Documentation

```
                    SECURITY DOCUMENT HIERARCHY
┌─────────────────────────────────────────────────┐
│                                                 │
│  [POLICIES] - "What & Why" (CEO/Board Level)   │
│  • High-level management intent                │
│  • Mandatory, organization-wide              │
│  • Example: "All sensitive data must be      │
│    protected from unauthorized access"       │
│           │                                     │
│           ▼                                     │
│  [STANDARDS] - "Musts" (Technical Requirements)│
│  • Specific, mandatory rules to enforce policies│
│  • Example: "All laptops must use AES-256   │
│    full-disk encryption"                     │
│           │                                     │
│           ▼                                     │
│  [GUIDELINES] - "Shoulds" (Best Practices)    │
│  • Recommendations, not mandatory            │
│  • Example: "Users should use password      │
│    managers for credential storage"         │
│           │                                     │
│           ▼                                     │
│  [PROCEDURES] - "How" (Step-by-Step Instructions)│
│  • Detailed implementation guides            │
│  • Example: "10-step manual for IT admin   │
│    to configure BitLocker on new laptop"   │
│                                                 │
└─────────────────────────────────────────────────┘
```

> 📝 **Exam Integration (Question Bank Q31):** Security planning components include policies (strategic intent), standards (technical mandates), guidelines (recommendations), and procedures (implementation steps)—ensuring consistent, auditable security practices across the organization.

---

## 3.2 BUSINESS CONTINUITY & DISASTER RECOVERY

### 3.2.1 BCP vs. DRP: Scope & Focus

| Aspect | Business Continuity Planning (BCP) | Disaster Recovery Planning (DRP) |
|--------|-----------------------------------|---------------------------------|
| **Scope** | Entire organization: people, processes, facilities | IT infrastructure only: servers, networks, data |
| **Goal** | Keep critical business functions operating during/after disaster | Restore IT systems and data to operational state |
| **Timeline** | Immediate response through long-term recovery | Focused on technical recovery within RTO |
| **Example** | Activate alternate office; manual order processing | Restore database from backups; rebuild servers |

### 3.2.2 Critical Recovery Metrics (EXAM ESSENTIALS)

| Metric | Definition | Formula/Example | Exam Application |
|--------|-----------|-----------------|-----------------|
| **RTO (Recovery Time Objective)** | Maximum allowable downtime before unacceptable business impact | "E-commerce site RTO=4 hours" → IT must restore within 4h | Determines backup/redundancy strategy |
| **RPO (Recovery Point Objective)** | Maximum acceptable data loss measured in time | "RPO=1 hour" → backups must run at least hourly | Determines backup frequency |
| **MTD (Maximum Tolerable Downtime)** | Absolute maximum survival time before business failure | "MTD=72 hours" for critical system | RTO must always be < MTD |

**Relationship**: `RTO ≤ MTD` and `Backup Interval ≤ RPO`

> 📝 **Exam Integration (CIA2 Q12i + Question Bank Q33):** Business Continuity Planning includes components like risk assessment, strategy development, plan documentation, training/testing, and maintenance. In a data center loss scenario, BCP activates alternate sites while DRP restores systems within RTO/RPO targets.

---

## 3.3 INCIDENT RESPONSE & MANAGEMENT

### 3.3.1 PICERL Incident Response Lifecycle

```
                    PICERL FRAMEWORK
┌─────────────────────────────────────────────────┐
│                                                 │
│  1. PREPARATION (Before Incident)              │
│  • Train IR team; establish communication plans│
│  • Prepare forensic toolkits; draft policies  │
│                                                 │
│  2. IDENTIFICATION (Detection & Triage)       │
│  • Monitor IDS/SIEM alerts                    │
│  • Confirm true incident vs. false positive  │
│  • Classify severity; activate response team │
│                                                 │
│  3. CONTAINMENT (Stop the Bleeding)          │
│  • Isolate compromised systems from network │
│  • ⚠️ DO NOT power off if volatile RAM data │
│    needed for forensics                     │
│  • Preserve evidence; document actions      │
│                                                 │
│  4. ERADICATION (Remove the Threat)          │
│  • Identify root cause; patch vulnerability│
│  • Delete malware; disable compromised accounts│
│  • Verify threat completely removed        │
│                                                 │
│  5. RECOVERY (Restore Operations)            │
│  • Restore from clean backups; test functionality│
│  • Gradually bring systems back online    │
│  • Monitor closely for reinfection        │
│                                                 │
│  6. LESSONS LEARNED (Post-Mortem)           │
│  • Meeting within 2 weeks of incident      │
│  • Document: What happened? Why defenses failed?│
│  • Update policies/tools to prevent recurrence│
│                                                 │
└─────────────────────────────────────────────────┘
```

**🔴 Exam Case: Malware Detected – Immediate Actions**
1. **Contain**: Disconnect affected machine from network (but keep powered for memory forensics)
2. **Identify**: Capture RAM dump; collect logs; determine malware type and entry point
3. **Notify**: Alert IR team, management, legal/compliance per policy
4. **Preserve**: Document chain of custody for potential legal action
5. **Contain Further**: Block malicious IPs/domains at firewall; reset compromised credentials

> 📝 **Exam Integration (CIA2 Q5 + Question Bank Q34):** Incident handling follows PICERL: Preparation (training/tools), Identification (detection/triage), Containment (isolate systems), Eradication (remove threat), Recovery (restore operations), Lessons Learned (improve defenses).

---

## 3.4 RISK ANALYSIS (HIGH-PROBABILITY NUMERICALS)

### 3.4.1 Quantitative Risk Analysis Formulas

```
RISK = THREAT × VULNERABILITY × IMPACT
```

**Key Metrics & Formulas**:
1. **AV (Asset Value)**: Monetary worth of asset  
   Example: Database AV = ₹100,000

2. **EF (Exposure Factor)**: % of asset lost in single incident  
   Example: Fire destroys 50% of database → EF = 0.50

3. **SLE (Single Loss Expectancy)**: Loss from one incident  
   `SLE = AV × EF`  
   Example: ₹100,000 × 0.50 = ₹50,000

4. **ARO (Annualized Rate of Occurrence)**: Expected incidents per year  
   Example: Fire once per 10 years → ARO = 0.1

5. **ALE (Annualized Loss Expectancy)**: Expected annual loss  
   `ALE = SLE × ARO`  
   Example: ₹50,000 × 0.1 = ₹5,000/year

**Decision Rule**: Do not spend more than ALE on countermeasures.  
If fire suppression costs ₹10,000/year but ALE=₹5,000 → cheaper to accept risk.

---

### 🔴 Exam Numerical Practice Set

**Problem 1**: Asset value = ₹50,000; Exposure factor = 0.4  
**Find SLE**:
```
SLE = AV × EF = ₹50,000 × 0.4 = ₹20,000
```

**Problem 2**: SLE = ₹20,000; ARO = 0.5  
**Find ALE**:
```
ALE = SLE × ARO = ₹20,000 × 0.5 = ₹10,000/year
```

**Problem 3**: Compare risk before/after control  
- Before: ALE = ₹10,000/year  
- Control cost: ₹3,000/year  
- New ARO after control: 0.1 (reduced from 0.5)  
- New ALE = ₹20,000 × 0.1 = ₹2,000/year  
- Net benefit: (₹10,000 - ₹2,000) - ₹3,000 = ₹5,000/year savings → Control justified

> 📝 **Exam Integration (Question Bank Q38-40):** Risk analysis numericals are high-probability exam questions. Master SLE=AV×EF and ALE=SLE×ARO formulas. Always show units (₹) and interpret results for business decisions.

---

## 3.5 DEALING WITH DISASTER

### 3.5.1 Disaster Classification & Mitigation

| Disaster Type | Examples | Primary Mitigation Strategies |
|--------------|----------|------------------------------|
| **Natural** | Earthquake, flood, hurricane | Geographic redundancy; offsite backups; structural hardening |
| **Technical** | Power failure, hardware crash, software bug | UPS/generators; RAID; clustering; patch management |
| **Human** | Insider threat, accidental deletion, sabotage | Access controls; audit logs; training; separation of duties |

**🔴 Exam Case: Power Failure Mitigation**
- **Immediate**: UPS provides short-term power for graceful shutdown
- **Short-term**: Backup generators kick in for extended outages
- **Long-term**: Geographic redundancy (failover to secondary data center)
- **Data Protection**: Frequent backups with RPO-aligned intervals; transaction logs for point-in-time recovery

---

## 3.6 CYBER SECURITY IN INDUSTRIAL CONTEXTS

### 3.6.1 Information Governance: IT vs. OT Priorities

```
                    CIA vs. AIC TRIAD PRIORITY SHIFT
┌─────────────────────────────────────────────────┐
│                                                 │
│  CORPORATE IT Priority Order:                  │
│  1. Confidentiality (protect data secrecy)    │
│  2. Integrity (ensure data accuracy)         │
│  3. Availability (keep systems running)      │
│                                                 │
│  INDUSTRIAL OT Priority Order:                 │
│  1. Availability & Safety (systems must run  │
│     24/7; milliseconds matter for physical  │
│     processes; human safety paramount)      │
│  2. Integrity (commands to machines must be│
│     accurate; wrong valve command = explosion)│
│  3. Confidentiality (reading boiler temp   │
│     rarely matters if attacker can't alter it)│
│                                                 │
└─────────────────────────────────────────────────┘
```

> 📝 **Exam Integration (CIA2 Q12ii + Question Bank Q41):** Information governance in industry prioritizes availability and safety over confidentiality because industrial control system failures can cause physical damage, environmental disasters, or loss of life—unlike IT breaches which primarily cause financial/data loss.

---

### 3.6.2 Securing the Industrial Internet of Things (IIoT)

#### Purdue Enterprise Reference Architecture (PERA)

```
                    PURDUE MODEL FOR OT SECURITY
┌─────────────────────────────────────────────────┐
│                                                 │
│  LEVEL 5: Enterprise Network                  │
│  • Internet access, corporate VPNs, email    │
│                                                 │
│  LEVEL 4: Site Business Planning              │
│  • ERP systems, business analytics           │
│                                                 │
│  ═══════════════════════════════════════     │
│  [IT/OT DMZ - "Air Gap" Equivalent]          │
│  • Jump servers, patch management, strict  │
│    firewalls; NO direct L4↔L3 traffic      │
│  ═══════════════════════════════════════     │
│                                                 │
│  LEVEL 3: Site Operations                     │
│  • Plant-wide SCADA, historian databases     │
│                                                 │
│  LEVEL 2: Area Supervisory Control           │
│  • HMI (Human-Machine Interface) screens    │
│                                                 │
│  LEVEL 1: Basic Control                      │
│  • PLCs (Programmable Logic Controllers),  │
│    RTUs (Remote Terminal Units)            │
│                                                 │
│  LEVEL 0: Physical Process                  │
│  • Motors, valves, pumps, sensors          │
│                                                 │
└─────────────────────────────────────────────────┘
```

**Security Principle**: Strict segmentation prevents IT breach from reaching OT. Attacker compromising HR email (L4) cannot directly access turbine controllers (L1).

#### IIoT Threats & Challenges

| Threat | Why Critical in OT | Mitigation |
|--------|-------------------|------------|
| **Legacy Protocols** (Modbus, DNP3) | No encryption/authentication; commands in cleartext | Protocol gateways; network segmentation; monitoring |
| **Patching Difficulties** | Cannot reboot nuclear reactor for Windows Update | Virtual patching (IPS); scheduled maintenance windows; compensating controls |
| **State-Sponsored Attacks** (Stuxnet) | Target physical processes; cause kinetic damage | Air-gapping where possible; behavioral monitoring; supply chain security |
| **Insider Threats** | Operators with physical access can cause catastrophic harm | Least privilege; dual-control for critical actions; continuous monitoring |

---

### 3.6.3 Intrusion Detection in OT Environments

**Why Traditional IPS Fails in OT**:
- **Availability Risk**: False positive blocking a legitimate valve command could cause explosion
- **Timing Sensitivity**: OT protocols require millisecond response; IPS inspection adds latency
- **Proprietary Protocols**: Commercial IDS don't understand Modbus, Profibus, etc.

**OT-Appropriate Solution: Passive Specialized IDS**
```
                    PASSIVE IDS FOR OT
┌─────────────────────────────────────────────────┐
│                                                 │
│  [OT Network Traffic]                          │
│         │                                       │
│         ▼                                       │
│  [Network Tap/SPAN Port] → Copy of traffic only│
│         │                                       │
│         ▼                                       │
│  [Specialized OT-IDS]                          │
│  • Trained on industrial protocols            │
│  • Builds baseline of "normal" process behavior│
│  • Alerts on anomalies (e.g., valve command  │
│    at unusual time/parameter)                │
│         │                                       │
│         ▼                                       │
│  [Human Operator Review] ← Final safety decision│
│  • IDS alerts; human decides to intervene    │
│  • Prevents automated false-positive blocking│
│                                                 │
└─────────────────────────────────────────────────┘
```

> 📝 **Exam Integration (Question Bank Q44):** Traditional IDS fails in industrial systems because automated blocking risks physical safety. OT environments use passive, protocol-aware IDS that alert human operators—who make final safety-critical decisions.

---

### 3.6.4 Compliance Standards

| Standard | Scope | Key Focus | Industry Application |
|----------|-------|-----------|---------------------|
| **IEC 62443** | Industrial Automation & Control Systems (IACS) | Security zones/conduits; security levels for OT | Manufacturing, energy, utilities |
| **ISO/IEC 27001** | General Information Security Management System (ISMS) | Policies, risk management, continuous improvement | All sectors; foundational framework |
| **NIST Cybersecurity Framework (CSF)** | Critical infrastructure | Identify, Protect, Detect, Respond, Recover functions | US critical infrastructure; widely adopted globally |

**Implementation Tip**: Map controls across standards to avoid duplication—e.g., IEC 62443 zone segmentation supports NIST "Protect" function.

---

### 3.6.5 Computer Ethics in Industrial Contexts

#### RFC 1087: Ethics and the Internet (IAB)

Unethical activities include any that:
1. Seek unauthorized access to Internet resources
2. Disrupt intended Internet use
3. Waste resources (people, capacity, computers)
4. Destroy integrity of computer-based information
5. Compromise user privacy

#### Ten Commandments of Computer Ethics (Computer Ethics Institute)

1. Thou shalt not use a computer to harm other people  
2. Thou shalt not interfere with other people's computer work  
3. Thou shalt not snoop around in other people's computer files  
4. Thou shalt not use a computer to steal  
5. Thou shalt not use a computer to bear false witness  
6. Thou shalt not copy or use proprietary software without payment  
7. Thou shalt not use other people's computer resources without authorization  
8. Thou shalt not appropriate other people's intellectual output  
9. Thou shalt think about social consequences of programs/systems you design  
10. Thou shalt use computers with consideration and respect for fellow humans  

**🔴 Exam Case: Employee Leaks Industrial Data**  
- **Ethical Violation**: Commandments #3 (snooping), #4 (theft of IP), #7 (unauthorized resource use)  
- **Industrial Impact**: Could enable sabotage of physical processes → safety/environmental risk  
- **Prevention**: Ethics training; clear policies; technical controls (DLP, access logs); whistleblower channels  

> 📝 **Exam Integration (CIA2 Q8 + Question Bank Q46):** Computer ethics are paramount in industrial contexts because cyber attacks can cause kinetic damage. RFC 1087 and the Ten Commandments provide moral frameworks for security professionals managing life-critical systems.

---


