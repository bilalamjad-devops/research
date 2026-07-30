Sahi Option Hai: **CS register**

---

### **Concept (Samajhne ke liye):**

Assembly language mein subroutine (function) se wapas aane ke liye do tarah ke return instructions hotay hain:

1. **`RET` / `RETN` (Near Return):**
* Yeh farz karta hai ke caller aur subroutine **dono same code segment** mein hain.
* Isliye yeh stack se sirf 16-bit **Offset Address (IP)** pop karta hai.


2. **`RETF` (Far Return):**
* Yeh tab use hota hai jab subroutine kisi **doosre Code Segment (Far Call)** mein hoti hai.
* Isliye yeh stack se **do (2) values** pop karta hai:
1. Pehle **Offset Address** $\rightarrow$ **IP (Instruction Pointer)** register mein.
2. Phir **Segment Address** $\rightarrow$ **CS (Code Segment)** register mein.





---

### **Near Return vs Far Return (Quick Comparison):**

| Instruction | Return Type | Stack Operations (Pops) | Registers Updated |
| --- | --- | --- | --- |
| **`RET`** | Near Return | Pops 1 word (2 bytes) | **IP** |
| **`RETF`** | Far Return | Pops 2 words (4 bytes) | **IP** and **CS** |

---

> **Exam Tip:**
> * **`RET`** $\rightarrow$ Updates **IP** (Instruction Pointer)
> * **`RETF`** $\rightarrow$ Updates **IP** AND **CS** (Code Segment)

15. RETF will pop the segment address in the
 CS register (Page 72)
 DS register
 SS register
