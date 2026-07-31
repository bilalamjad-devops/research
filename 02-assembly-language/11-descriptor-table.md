Sahi Option Hai: **IDTR (Interrupt Descriptor Table Register)**

---

### **Concept (Samajhne ke liye):**

Protected Mode mein CPU interrupts handle karne ke liye **IDT (Interrupt Descriptor Table)** ka istemaal karta hai.

* **IDT (Table):** RAM/Memory ke andar bani hui ek table hoti hai jisme interrupt handlers ke address hotay hain.
* **IDTR (Register):** CPU ke andar ek special 48-bit register hota hai jo **IDT ka physical base address** aur uski limit (size) apne paas save rakhta hai.

CPU jab bhi kisi interrupt ko process karta hai, toh woh sab se pehle **IDTR** register se IDT ka memory address dhoondta hai.

---

### **Quick Comparison (CS401 Exam Ke Liye):**

| Register Name | Full Form | Purpose |
| --- | --- | --- |
| **IDTR** | **Interrupt Descriptor Table Register** | **IDT** ka base physical address aur limit hold karta hai. |
| **GDTR** | **Global Descriptor Table Register** | **GDT** (Global Descriptor Table) ka address hold karta hai. |
| **LDTR** | **Local Descriptor Table Register** | **LDT** (Local Descriptor Table) ka address hold karta hai. |

---

> **Exam Tip:**
> * **IDT** $\rightarrow$ Memory mein pari table.
> * **IDTR** $\rightarrow$ Register jo IDT ka physical address rakhta hai.

40. The physical address of IDT (Interrupt Descriptor Table) is stored in
- DTR
- IDTR (Page 182) rep
- IVT
- IDTT


70. The physical address of Interrupt Descriptor Table (IDT) is stored in
- GDTR
- IDTR (Page 182) rep
- IVT
- IDTT


98.8088 is a...........................
- 16 bit processor (Page 14)
- 32 bit processor
- 64 bit processor
- 128 bit processor

99. The table index (TI) is set to to access the GDT (Global Descriptor Table).
- 1
- 0 (Page 175)
- -1
- -2



