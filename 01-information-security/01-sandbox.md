
## 🟢 B. Sandboxing ✅

### What is it?

Sandboxing creates a **fake computer** to safely run suspicious files.

If the file is malicious...

It infects only the fake computer.

Your real computer remains safe.

---

### DevOps Example

Suppose an employee receives:

```
Salary_Increment.pdf.exe
```

Looks like PDF.

Actually ransomware.

Instead of opening it on the employee's PC...

The email gateway first opens it inside a sandbox.

Inside sandbox:

✔ Encrypts files
✔ Creates registry keys
✔ Contacts hacker server

Immediately...

🚫 Block Email

Employee never receives it.

---

### Think Like Docker

This is why DevOps students remember it quickly.

A sandbox is like:

```
docker run suspicious-file
```

The malicious program runs inside an isolated environment.

If it destroys everything...

Destroy container.

Host machine stays safe.

Exactly the same idea.

Isolation.

---

### Memory Trick

**Sandbox = Children's sandbox**

Kids play inside the box.

Sand stays inside.

Doesn't spread everywhere.

Similarly...

Malware stays inside the sandbox.

---
