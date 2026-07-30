61. In STOSW instruction, When DI is cleared, SI is
- Incremented by 1
- Incremented by 2 (Page 92)
- Decremented by 1
- Decremented by 2






Sahi Option Hai: **Incremented by 2**

---

### **1-Line Memory Trick:**

1. **`STOSW` (W = Word):** Word ka matlab **2 Bytes** hota hai.
2. **DF Cleared (DF = 0):** Direction flag clear ka matlab **Forward (Increment)** hota hai.

Toh: **Cleared (Increment) + Word (2) = Incremented by 2**

---

> **Exam Fast Cheat Sheet:**
> * `STOSB` + Cleared = **Incremented by 1**
> * `STOSW` + Cleared = **Incremented by 2**
> * `STOSW` + Set = **Decremented by 2**


*(Note: Phele bataye gaye MCQ ki tarah, handout mein `DI` ki jagah generic term `SI` likha hota hai, lekin rule same rehta hai!)*

In 8086 Assembly language, **`STO`** stands for **STORE**.

---

### **Fast Context:**

* **`STOS`** = **STO**re **S**tring
* **`STOSB`** = **STO**re **S**tring **B**yte (Store 1 Byte from `AL` into memory)
* **`STOSW`** = **STO**re **S**tring **W**ord (Store 2 Bytes from `AX` into memory)

> **Shortcut Rule:**
> * **`STO`** = **Store** (Data ko CPU register se nikalkar **Memory/RAM mein store karna**)
> * **`LOD`** = **Load** (Data ko Memory/RAM se nikalkar **CPU register mein lana**)
> 
>
