

## 🟢 D. FIM

Full Form

File Integrity Monitoring

---

Purpose

Checks whether important files have been modified.

Example

Linux server

Yesterday

```
/etc/passwd
```

Today

```
/etc/passwd
```

changed.

Who changed it?

FIM immediately alerts.

---

DevOps Example

Suppose someone hacks your EC2 instance.

They modify

```
nginx.conf
```

or

```
/etc/shadow
```

FIM immediately says

⚠ Important system file modified!

Examples

Tripwire

Wazuh

OSSEC

---

Think Like Git

Git tells you

```
Modified
```

```
Deleted
```

```
Added
```

FIM does something similar for operating system files.

---

# Quick Comparison (Exam Revision)

| Option                   | Purpose                                          | DevOps Analogy                              |
| ------------------------ | ------------------------------------------------ | ------------------------------------------- |
| **Enterprise Antivirus** | Detects known malware                            | Windows Defender on employee PCs            |
| **Sandboxing** ✅         | Runs suspicious files in an isolated environment | Docker container for unknown programs       |
| **SIEM**                 | Collects and analyzes security logs              | Central logging dashboard (like ELK/Splunk) |
| **FIM**                  | Detects changes to important files               | Git showing file modifications on servers   |

---

# 🎯 VU Exam Shortcut

If the question contains...

* **Email attachment**
* **Unknown file**
* **Behavior analysis**
* **Safe environment**
* **Isolated execution**

👉 **Answer = Sandboxing**

If it says...

* **Collect logs** → **SIEM**
* **Virus detection** → **Antivirus**
* **File modified** → **FIM**

---

From now on, I'll teach every MCQ this way:

* ✅ VU exam perspective
* ☁️ AWS/Cloud perspective
* ⚙️ DevOps perspective
* 🧠 Memory tricks
* 🎯 MCQ elimination techniques

This approach will help you not only pass **CS205 Information Security** but also build concepts useful in **DevOps interviews**.


28-July-2026


### Correct Answer: **D. File integrity monitoring tool**

---

### Concept Samjhen:

Sawal yeh pooch raha hai ke **kisi critical system file mein koi tabdeeli (alteration/change) na hui ho, yeh check karne ke liye konsa tool use hota hai?**

---

### File Integrity Monitoring (FIM) Kya Hota Hai?

**File Integrity Monitoring (FIM)** ek aisa security control / tool hai jo aapki critical files (jaise operating system files, application config files, system logs) ka **hash / digital fingerprint** bana kar save kar leta hai.

1. **Kaise Kaam Karta Hai?**
FIM tool continuously baseline files ko monitor karta hai. Agar koi hacker, malware, ya unauthorized banda kisi important file ko change, modify, ya delete karne ki koshish karega, toh FIM instantly alert generate kar deta hai ke *"File Alter Ho Gayi Hai!"*
2. **Common Tools:** Tripwire, OSSEC, Microsoft Defender for Cloud FIM.

---

### Baki Options Kyun Nahi Sahi?

* **A. CIS Cat Pro:** Yeh system configuration ko CIS Benchmarks ke mutabiq audit/benchmark karne ka tool hai.
* **B. Qualys Vulnerability Scanner:** Yeh system mein bugs aur security vulnerabilities dhoondhta hai.
* **C. SIEM Tools (Security Information and Event Monitoring):** Yeh mukhtalif devices ke logs jama kar ke analysis karta hai.

---

> **Key Memory Tip:**
> Whenever you see the words **"critical system files altered / changed"**, the answer is always **File Integrity Monitoring (FIM)**!

---

Agla MCQ paste karein!
