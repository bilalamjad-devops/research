Sahi Option Hai: **Source**

---

### **Concept (Samajhne ke liye):**

NASM / Intel Assembly Language syntax mein instruction ka structure hamesha yeh hota hai:

$$\text{Instruction} \quad \text{Destination}, \quad \text{Source}$$

Instruction **`mov ax, 5`** mein:

* **`mov`:** Opcode (Operation code - move/copy ka action).
* **`ax`:** **Destination** operand (jahan value copy hakar jani hai - ek Register).
* **`5`:** **Source** operand (jo value copy honi hai - ek Constant/Immediate value).

Is instruction ka matlab hai: Constant value `5` ko **Source** se utha kar **Destination** register `AX` mein daal do.

---

### **Operand Types (CS401 Exam Ke Liye):**

| Instruction Part | Role in `mov ax, 5` | Operand Category |
| --- | --- | --- |
| **`ax`** | **Destination** | Register Operand |
| **`5`** | **Source** | Immediate / Constant Value |

---

> **Exam Tip:**
> Comma (`,`) ke **daayein (right)** taraf **Source** hota hai, aur **baayein (left)** taraf **Destination** hota hai!
