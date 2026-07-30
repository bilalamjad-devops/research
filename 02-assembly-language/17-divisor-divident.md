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


Aap ka logic bilkul sahi direction mein hai! **Dividend hamesha Divisor se double size ka hota hai** taake division ke baad remainder aur quotient bina overflow ke fit aa sakein.

Lekin yeh $8$-bit ya $16$-bit hai, yeh kaise pata chalta hai? **Yeh aap instruction mein diye gaye Divisor ke register ke size se pehchante hain!**

---

### **Rule: Divisor ka Size Dekho, Dividend Mil Jayega**

Assembly language mein x86 registers ka size fixed hota hai:

* **$8$-bit Registers:** `AL`, `AH`, `BL`, `BH`, `CL`, `CH`, `DL`, `DH`
* **$16$-bit Registers:** `AX`, `BX`, `CX`, `DX`, `SI`, `DI`, `BP`, `SP`

---

### **Pehchanne Ka Tariqa (2 Scenarios):**

#### **Case 1: Jab Divisor $8$-bit Ka Ho**

Instruction dekhein: **`DIV BL`**

1. **Step 1:** Divisor pehchanein $\rightarrow$ `BL` ek **$8$-bit** register hai.
2. **Step 2:** Dividend nikalne ke liye size double karein $\rightarrow 8 \text{ bits} \times 2 = 16 \text{ bits}$.
3. **Conclusion:** $16$-bit ke liye CPU fixed **`AX`** register ko dividend maanta hai.

$$\text{Operation: } \frac{\mathbf{AX} \text{ (16-bit)}}{\mathbf{BL} \text{ (8-bit)}} \implies \text{Quotient} = \mathbf{AL}, \text{ Remainder} = \mathbf{AH}$$

---

#### **Case 2: Jab Divisor $16$-bit Ka Ho**

Instruction dekhein: **`DIV BX`**

1. **Step 1:** Divisor pehchanein $\rightarrow$ `BX` ek **$16$-bit** register hai.
2. **Step 2:** Dividend nikalne ke liye size double karein $\rightarrow 16 \text{ bits} \times 2 = 32 \text{ bits}$.
3. **Conclusion:** $16$-bit registers mein $32$-bit number fit nahi aata, isliye CPU do $16$-bit registers ko milakar **`DX:AX`** pair ko dividend banata hai.

$$\text{Operation: } \frac{\mathbf{DX:AX} \text{ (32-bit)}}{\mathbf{BX} \text{ (16-bit)}} \implies \text{Quotient} = \mathbf{AX}, \text{ Remainder} = \mathbf{DX}$$

---

### **Quick Cheat Sheet (Exam Ke Liye):**

| Instruction | Divisor Size | Double Rule ($2\times$) | Implied Dividend |
| --- | --- | --- | --- |
| **`DIV CL`** | $8$-bit | $16$-bit | **`AX`** |
| **`DIV CX`** | $16$-bit | $32$-bit | **`DX:AX`** |

> **Aasan Lafzon Mein:** Bas `DIV` ke aage likha register dekhein. Agar uske aakhri mein **`L`** ya **`H`** hai (`BL`, `CL`), toh dividend **`AX`** hai. Agar aakhri mein **`X`** hai (`BX`, `CX`), toh dividend **`DX:AX`** hai!

---

Why not BX, CX, DX?

### **Simple Real-Life Analogy:**

Sochein aapke kitchen mein:

* **`AX` = Main Cooking Stove (Chulha)** — Saari cooking (arithmetic) yahin hogi.
* **`BX` = Spice Rack (Masalay)**
* **`CX` = Timer (Ghadhi)**

Jab bhi `DIV` (Khana pakana) chalega, CPU hamesha **Main Stove (`AX`)** ko hi use karega. Aap Masalay wale dabba (`BX`) par sidha khana nahi pakayein ge!

---
