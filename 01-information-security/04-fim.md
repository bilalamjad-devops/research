

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
