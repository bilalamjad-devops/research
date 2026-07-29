CS205 ke course handout ke mutabiq, yeh chaaro components **Security Assessment Framework** (ya **Security Assessment Domain**) ke andar aate hain.

Agah CS205 handouts mein dekha jaye, toh in chaaro ko ek umbrella term ke andar rakha jata hai:

## **Security Assessment Techniques / Evaluation Methods**

CS205 Handouts mein **Chapter / Section 5: Security Assessment & Auditing** ya **Security Assurance Domain** ke tehat in chaaro methods ko divide kiya gaya hai.

---

### In Chaaro Ka Classification Chart (Handbook Context):

Security evaluation ko 4 alag angles se test karne ke liye yeh chaar tools / techniques use ki jaati hain:

```text
               [ Security Assessment Framework ]
                               |
  -----------------------------------------------------------
  |                |                   |                    |
[ Audit ]  [ Vulnerability ]  [ Penetration ]     [ Security ]
            Assessment           Testing             Review

```

---

### Main Points Jo CS205 Key Syllabus Mein Hain:

1. **Security Domain:**
Yeh sab **Information Security Management & Testing Domain** ka hissa hain.
2. **Assessment Objective (Maqsad):**
Security System ko **Assure (Yaqeeni)** karna ke system har lihaz se secure hai:
* **Compliance** check karne ke liye $\rightarrow$ **Audit**
* **Flaws/Bugs** dhoondne ke liye $\rightarrow$ **Vulnerability Assessment**
* **Real Attack** test karne ke liye $\rightarrow$ **Penetration Testing**
* **Controls Review** ke liye $\rightarrow$ **Security Review**



---

### **One-Line Paper Answer:**

> Agar paper mein aaye ke *"Audit, Vulnerability Assessment, Pen Testing, and Security Review come under which umbrella?"*
> Toh sahi term hai: **Security Assessment Techniques** (ya **Security Assurance & Evaluation Methods**).

Clear ho gaya? Agla MCQ paste karein jab aap ready hon!

---
---

Yeh chaaron security testing aur evaluation ke primary methods hain. Teeno/Chaaro ka maqsad, tareeqa-e-kaar (approach), aur output bilkul alag hota hai.

Teeno ko ek jagah asani se samajhne ke liye yeh breakdown dekhein:

---

## 1. Security Audit (Grievance / Compliance Check)

* **Main Purpose:** Yeh check karna ke aapka system kisi **Standard, Baseline Policy, ya Regulation** (jaise ISO 27001, PCI-DSS, CIS Benchmarks) ko **follow/comply** kar raha hai ya nahi.
* **Approach:** Checklist-based verification (Formal comparison).
* **Question Answered:** *"Kya hum pehle se tay shuda security rules aur standards par poora utar rahe hain?"*
* **Example:** Check karna ke sabhi 100 computers par antivirus installed aur updated hai ya nahi (Rule ke mutabiq).

---

## 2. Vulnerability Assessment (Bug Hunting & Discovery)

* **Main Purpose:** System mein jitne bhi **known flaws, bugs, misconfigurations, aur kamzoriyaan (vulnerabilities)** hain, unko automated scanners (jaise Nessus, Qualys) se dhoondna aur unhe priority wise **patch/fix** karna.
* **Approach:** Automated Scanning + Prioritization.
* **Question Answered:** *"Hamare system mein kahan kahan kamzoriyaan (loopholes) hain jinhe patch karne ki zaroorat hai?"*
* **Example:** Automated scanner chala kar yeh report nikalna ke kaunse 15 servers mein outdated software chal raha hai.

---

## 3. Penetration Testing (Simulated Goal-Oriented Attack)

* **Main Purpose:** Ek real-world attacker ki tarah system par attack karke yeh dekhta ke **kya koi hacker kisi specific goal ko achieve kar sakta hai** (e.g., Database se data churaana) aur aapki current security posture kitni strong hai.
* **Approach:** Exploitation & Objective-driven (Hacking test).
* **Question Answered:** *"Agar koi hacker hamare system par attack kare, toh wo kitna andar tak ja sakta hai aur kya nuksan pohncha sakta hai?"*
* **Example:** Software ki vulnerability ko exploit karke Admin access hasil karne ki koshish karna.

---

## 4. Security Review (Control Verification)

* **Main Purpose:** Un security controls, architecture, ya configurations ko re-examine aur verify karna jise **pehlay se secure maan liya gaya tha (assumed to be secure)**.
* **Approach:** Code review, architecture analysis, aur setup re-verification.
* **Question Answered:** *"Jo security controls humne pehle se lagaye hue hain, kya wo waqai expected tarike se kaam kar rahe hain?"*
* **Example:** Firewall ki complex ruleset ya source code ko dobara parhna taake dekha ja sake ke koi hidden logic flaw toh nahi reh gaya.

---

### **Quick Summary Table (Exam & Concept Memory):**

| Method | Main Goal / Keyword | Output |
| --- | --- | --- |
| **Audit** | **Compliance & Standards** se comparison | Compliance Report (Pass / Fail / Gap) |
| **Vulnerability Assessment** | **Identify & Fix** as many bugs as possible | List of Vulnerabilities to Patch |
| **Penetration Testing** | Achieve **Specific Goals** via simulated attack | Proof of Concept / Risk Impact Report |
| **Security Review** | Verify controls **assumed to be secure** | Architecture / Code Quality Review |

---

Agla MCQ paste karein jab aap ready hon!

---
---


Is concept ko **Penetration Testing Types** ya **Security Assessment Approaches** (Target Access / Knowledge Levels) kehte hain.

Jab testing ki baat hoti hai, toh hum specific tester ke **Knowledge Level** (White, Grey, Black Box) ki buniyad par access define karte hain:

---

### **1. Types of Testing / Knowledge Levels**

Is specific concept ko **Box Testing Methods** ya **Access Levels in Penetration Testing** bhi kaha jata hai:

* ⚪ **White Box:** Full Access & Internal Info (Source Code, Network Diagrams)
* 🔘 **Grey Box:** Partial Access & Limited Info (User Credentials)
* ⬛ **Black Box:** Zero Access & No Prior Info (External Hacker Perspective)

---

### **2. CS205 Context Mein Main Hierarchy (Boht Important)**

Ab tak jo humne 3 major concepts parhe hain, inki **Parent-Child Hierarchy** yeh banti hai taake aapke mind mein koi confusion na rahe:

```text
                  [ Security Evaluation / Assurance ]
                                  |
              ------------------------------------------
              |                                        |
    [ Assessment Types ]                    [ Knowledge Levels / Approaches ]
    (Kya check karna hai?)                   (Tester ke paas kitni info hai?)
              |                                        |
     ├── 1. Audit                             ├── 1. White Box (Full Info)
     ├── 2. Vulnerability Assessment          ├── 2. Grey Box (Partial Info)
     ├── 3. Penetration Testing               └── 3. Black Box (Zero Info)
     └── 4. Security Review

```

---

### **Quick Summary for Paper:**

* **White Box / Black Box / Grey Box** $\rightarrow$ **Knowledge Levels / Penetration Testing Types**
* **Audit / VM / Pen Testing / Security Review** $\rightarrow$ **Security Assessment Techniques**

Clear ho gaya? Jab bhi ready hon, agla MCQ paste karein!
