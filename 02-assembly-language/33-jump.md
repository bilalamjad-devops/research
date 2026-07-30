Sahi Option Hai: **Short, near, far**

---

### **1-Line Memory Trick:**

* **`Short Jump`:** $-128$ se $+127$ bytes ke andar jump (1-Byte offset).
* **`Near Jump`:** Usi segment ($CS$) ke andar jump (2-Byte offset, $\pm32\text{KB}$).
* **`Far Jump`:** Dusre segment mein jump (4-Byte: $CS + IP$ dono change hote hain).

---

> **Exam Shortcut:**
> Assembly mein Total **3 Types** ke Jump hotay hain: **Short, Near, Far**.
