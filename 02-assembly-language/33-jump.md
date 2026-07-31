Sahi Option Hai: **Short, near, far**

---

### **1-Line Memory Trick:**

* **`Short Jump`:** $-128$ se $+127$ bytes ke andar jump (1-Byte offset).
* **`Near Jump`:** Usi segment ($CS$) ke andar jump (2-Byte offset, $\pm32\text{KB}$).
* **`Far Jump`:** Dusre segment mein jump (4-Byte: $CS + IP$ dono change hote hain).

---

> **Exam Shortcut:**
> Assembly mein Total **3 Types** ke Jump hotay hain: **Short, Near, Far**.

128. Every bit of line status in serial port conveys information.

- different (Page 171)
- same
- partial
- full

129. There are total bytes in a standard floppy disk.

- 1444k
- 1440k (Page 155)
- 1280k
- 2480k

Here are the answers for both questions:

---

### **128. Every bit of line status in serial port conveys ... information.**

Sahi Option Hai: **different**

> **Memory Trick:** Line Status Register ki **har bit alag-alag signal / condition** show karti hai (e.g., Data Ready, Overrun Error, Parity Error, Framing Error, Transmit Buffer Empty).

---

### **129. There are total ... bytes in a standard floppy disk.**

Sahi Option Hai: **1440k**

> **Memory Trick:** Standard 3.5-inch High-Density Floppy Disk ki capacity **$1.44\text{ MB} = 1440\text{ KB}$** hoti hai.

---

### **Floppy Disk Size Calculation:**

* $2 \text{ Sides} \times 80 \text{ Tracks} \times 18 \text{ Sectors} \times 512 \text{ Bytes} = 1,474,560 \text{ Bytes}$
* $1,474,560 \div 1024 = \mathbf{1440\text{ KB}}$
