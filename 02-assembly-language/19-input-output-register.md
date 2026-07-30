18. INT 21 service 01H is used to read character from standard input with echo. It returns the
result in
Register.
- AL (Page 152)
- BL
- CL
- BH


### **Analogy (Dukaan Wali Example):**

* **`AH = 01h`** $\rightarrow$ Aapne dukandar ko bola: *"Mujhe 1 Aam (Mango) chahiye"*.
* **`INT 21h`** $\rightarrow$ Aapne dukandar ko paise diye.
* **`AL`** $\rightarrow$ Dukandar ne Aam utha kar aap ki **Right Hand (AL)** mein thama diya!

Toh key press ka result hamesha **`AL`** register mein hi wapas milta hai.

---

### **Sawal Aur Jawab:**

* **Sawal:** INT 21h Service 01h character read karne ke baad result kis register mein wapas degi?
* **Jawab:** **`AL`** register mein!


### **Yeh Concept Kya Hai?**

Jab bhi hum OS / System se koi kaam karwate hain (jaise Keyboard input), CPU registers ke do fixed role hote hain:

1. **Input Register (`AH`):**
Aap System ko batate hain ke **kya kaam karna hai** (`AH = 01h` matlb: *keyboard input le kar aao*).
2. **Return / Output Register (`AL`):**
System kaam khatam karne ke baad **natija (result) kis register mein wapas rakhega** (`AL` register mein).

---
