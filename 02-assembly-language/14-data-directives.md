Sahi Option Hai: **db**

---

### **Concept (Samajhne ke liye):**

NASM Assembly language mein memory mein space reserve/define karne ke liye Data Directives istemaal hoti hain. Numbers ka size bit-length par depend karta hai:

* **1 Byte = 8 Bits**
* **`db` (Define Byte):** Memory mein **8 bits (1 byte)** reserve ya initialize karne ke liye use hota hai.

---

### **NASM Data Directives Summary (Exam Ke Liye):**

| Directive | Full Form | Size in Bytes | Size in Bits | Example |
| --- | --- | --- | --- | --- |
| **`db`** | **Define Byte** | **1 Byte** | **8 Bits** | `var1 db 0xAA` |
| **`dw`** | **Define Word** | **2 Bytes** | **16 Bits** | `var2 dw 0xFFFF` |
| **`dd`** | **Define Double word** | **4 Bytes** | **32 Bits** | `var3 dd 0x12345678` |
| **`dq`** | **Define Quad word** | **8 Bytes** | **64 Bits** | `var4 dq 0x123456789ABCDEF0` |

---

> **Exam Tip:**
> * **8 bits** $\rightarrow$ **`db`** (Define Byte)
> * **16 bits** $\rightarrow$ **`dw`** (Define Word)
> * **32 bits** $\rightarrow$ **`dd`** (Define Double-word)

---
---
---
**NASM** ka matlab **Netwide Assembler** hota hai.

---

### **NASM Kya Hai?**

NASM x86 architecture (Intel aur AMD processors) ke liye ek bohot popular, free, aur open-source **Assembler** tool hai.

* **Assembler Ka Kaam:** Yeh aap ke likhe huay human-readable Assembly Code (jaise `MOV`, `ADD`, `INT 21h`) ko Machine Code (`0s` aur `1s` / Binary Code) mein convert karta hai jise computer ka CPU direct samajh kar execute kar sakta hai.

---

### **CS401 Mein NASM Kyun Use Hota Hai?**

1. **Intel Syntax:** Is mein code likhna clean aur aasan hota hai (pehle destination operand, phir source operand—e.g., `mov ax, bx`).
2. **Modular Directives:** Is mein file modularity ke liye `EXTERN`, `GLOBAL`, aur data declare karne ke liye `db`, `dw`, `dd` jaisi directives milti hain.
3. **Versatile Output:** Yeh multiple binary formats output kar sakta hai (jaise `.COM` files, `.EXE` files, ya ELF/COFF object files).

---

### **NASM Code Execution Flow:**

```text
[Assembly Code (.asm)] ──(NASM Assembler)──> [Object File (.obj / .com)] ──(Execution)──> [CPU Runs Program]

```

> **Exam Tip:** Paper mein jab bhi `.asm` file ko compile/assemble karne ki baat ho ya Assembly language directives (`db`, `dw`, `EXTERN`, `GLOBAL`) aayein, toh wo **NASM (Netwide Assembler)** ki bat ho rahi hoti hai!
