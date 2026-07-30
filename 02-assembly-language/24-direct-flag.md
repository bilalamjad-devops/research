35. In STOSB instruction, when DF is clear, SI is
- Incremented by 1 (Page 92)
- Incremented by 2
- Decremented by 1
- Decremented by 2

Wait, is sentence mein ek choti si **mistake / twist** hai jo aapke quiz file mein ho sakti hai! Pehle sahi answer dekh lete hain aur phir ghalati samajhte hain:

### **Correct Option:** **Incremented by 1**

---

### **1. Pehle Iska Concept Samjhein (DF: Direction Flag):**

String instructions (jaise `STOSB`, `MOVSB`, `LODSB`) mein **Direction Flag (DF)** decide karta hai ke memory mein aage barhna hai ya peeche:

* **DF = 0 (Clear):** **Forward direction** $\rightarrow$ Pointer **Increment** (+1 ya +2) hota hai.
* **DF = 1 (Set):** **Backward direction** $\rightarrow$ Pointer **Decrement** (-1 ya -2) hota hai.

**Byte vs Word:**

* **`STOSB` (Byte - 1 Byte):** Change **1** se hota hai.
* **`STOSW` (Word - 2 Bytes):** Change **2** se hota hai.

Lekin jab **DF clear (0)** hai, toh pointer **Increment** hoga! Isliye sahi option **Incremented by 1** hai.

---

### **2. Handout / Question Ki Choti Si Ghalati:**

In reality / CS401 Architecture:

* `STOSB` (Store String Byte) register **`AL`** ki value ko **`ES:DI`** par store karta hai. Toh actually register **`DI`** increment hota hai (`SI` nahi).
* Lekin CS401 ke paper/quiz mein generic string instruction ki wajah se **Incremented by 1** ko hi sahi option mana jata hai.

---

### **Cheat Sheet (Exam Tip):**

| Instruction | Flag Status (DF) | Register Pointer Effect |
| --- | --- | --- |
| **`STOSB` / `LODSB**` | **DF = 0 (Clear)** | **Incremented by 1** |
| **`STOSB` / `LODSB**` | **DF = 1 (Set)** | **Decremented by 1** |
| **`STOSW` / `LODSW**` | **DF = 0 (Clear)** | **Incremented by 2** |
| **`STOSW` / `LODSW**` | **DF = 1 (Set)** | **Decremented by 2** |


LODSB (Load String Byte)

STOSB (Store String Byte)
