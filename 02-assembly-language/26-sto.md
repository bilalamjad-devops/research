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
> 
> 

*(Note: Phele bataye gaye MCQ ki tarah, handout mein `DI` ki jagah generic term `SI` likha hota hai, lekin rule same rehta hai!)*
