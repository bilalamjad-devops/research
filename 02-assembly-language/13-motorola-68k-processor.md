Sahi Option Hai: **32bit**

---

### **Concept (Samajhne ke liye):**

Motorola **68000 (68K)** processor family ek 16/32-bit CISC architecture par mabni CPU series hai.

* **Program Counter (PC):** 68K processor mein Program Counter **32-bit** ka hota hai, jo current execution address ko hold karta hai. Is 32-bit PC ki madad se processor up to **4 Gigabytes ($2^{32}$ bytes)** ki memory area ko directly address kar sakta hai.

---

### **68K Processor Ke Main Registers (CS401 Summary):**

| Register Type | Size | Quantity / Details |
| --- | --- | --- |
| **Program Counter (PC)** | **32-bit** | Holds the address of current executing instruction |
| **Data Registers ($D0 - D7$)** | **32-bit** | Total 8 General Purpose Data Registers |
| **Address Registers ($A0 - A7$)** | **32-bit** | Total 8 Address Registers ($A7$ is Stack Pointer) |
| **Status Register (SR)** | **16-bit** | Flags aur condition codes hold karta hai |

---

> **Exam Tip:**
> Motorola 68K processor mein Data Registers, Address Registers, aur **Program Counter (PC)** teeno **32-bit** ke hotay hain.
