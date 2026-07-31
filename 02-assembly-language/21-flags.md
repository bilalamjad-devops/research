26. Which flags are NOT used for mathematical operations?
- Carry, Interrupt and Trap flag.
- Direction, Interrupt and Trap flag. (Page 133)
- Direction, Overflow and Trap flag.
- Direction, Interrupt and Sign flag

Sahi Option Hai: **Direction, Interrupt and Trap flag.**

---

### **Concept (Samajhne ke liye):**

8086 CPU ke Flags Register mein **16-bits** hotay hain jinhe **2 categories** mein baata jata hai:

1. **Status / Math Flags (Jo Maths Operations Se Change Hotay Hain):**
* **Carry Flag (CF):** Math mein overflow/borrow ke liye.
* **Zero Flag (ZF):** Jab result $0$ aaye.
* **Sign Flag (SF):** Jab result negative ho.
* **Overflow Flag (OF):** Signed math ke overflow ke liye.
* **Parity Flag (PF)** aur **Auxiliary Carry Flag (AF)**.


2. **Control Flags (Jo CPU Ke Behaviour Ko Control Karte Hain — Math Se Koi Lagaao Nahi):**
* **Direction Flag (DF):** Controls string processing direction (Forward `0` ya Backward `1`).
* **Interrupt Flag (IF):** External hardware interrupts ko enable/disable karta hai (`STI`/`CLI`).
* **Trap Flag (TF):** Single-step debugging mode ko enable karta hai.



---

### **Quick Table (Exam Summary):**

| Flag | Category | Mathematical Operations Se Effect Hota Hai? |
| --- | --- | --- |
| **Carry, Zero, Sign, Overflow** | **Status Flags** | **YES** |
| **Direction, Interrupt, Trap** | **Control Flags** | **NO** |

---

> **Exam Shortcut Tip:**
> Jab bhi pucha jaye ke **Maths ke liye kon se flags use NAHI hotay**, toh **`DIT`** (Direction, Interrupt, Trap) ko dhoondein!

---

102. When a 32 bit number is divided by a 16 bit number, the quotient is of
- 32 bits
- 16 bits (Page 85)
- 8 bits
- 4 bits


Crisp Bottom Line:

Maths mein answer 2 ata hai. Lekin CPU mein wo answer jis dabba/register (AX) mein save hota hai, us dabba ki capacity 16 bits hoti hai!

