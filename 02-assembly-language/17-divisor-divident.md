16. For the execution of the instruction “DIV BL”, the implied dividend will be stored in
- AX (Page 85)
- BX
- CX
- DX

Sahi Option Hai: **AX**

---

### **Concept (Samajhne ke liye):**

`DIV` (Division) instruction mein divisor (division karne wala number) toh instruction mein specify hota hai (jaise yahan `BL`), lekin **dividend** (jis number ko divide karna hai) CPU automatic pehle se fixed register se uthata hai. Isay **Implied Dividend** kehte hain.

Dividend ka size hamesha Divisor ke size se **double (2x)** hota hai:

1. **8-bit Division (`DIV reg8`):**
* **Divisor:** 8-bit register (jaise `BL`)
* **Implied Dividend:** 16-bit **`AX`** register
* **Result:** Quotient `AL` mein aur Remainder `AH` mein store hota hai.


2. **16-bit Division (`DIV reg16`):**
* **Divisor:** 16-bit register (jaise `BX`)
* **Implied Dividend:** 32-bit **`DX:AX`** pair
* **Result:** Quotient `AX` mein aur Remainder `DX` mein store hota hai.



---

### **`DIV` Instruction Working Summary (CS401 Exam Ke Liye):**

| Instruction | Divisor Size | Implied Dividend | Quotient Stored In | Remainder Stored In |
| --- | --- | --- | --- | --- |
| **`DIV BL`** | 8-bit (`BL`) | **`AX` (16-bit)** | `AL` | `AH` |
| **`DIV BX`** | 16-bit (`BX`) | **`DX:AX` (32-bit)** | `AX` | `DX` |

---

> **Exam Tip:**
> Jab divisor 8-bit ka ho (`BL`, `CL`, `AL`), toh dividend hamesha **`AX`** hota hai!
