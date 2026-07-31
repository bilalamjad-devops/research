**Ji bilkul sahi!**

Aap ne exact concept pakad liya hai. **Process Control Block (PCB)** wohi block / data structure hai jahan Operating System kisi bhi process ki **poori information** save rakhta hai.

---

### **PCB ke andar kya kya information hoti hai?**

Jab computer aik process se doosre process par switch karta hai (jisay **Context Switching** kehte hain), toh woh purane process ki sari state PCB mein save kar deta hai:

* **Process State:** Process abhi kya kar raha hai (Running, Waiting, ya Ready).
* **Program Counter (`IP` / `PC`):** Code ki konsi line par execution ruki thi taake wahan se wapas start ho sake.
* **CPU Registers:** `AX`, `BX`, `CX`, `DX` wagera mein kya values parhi thi.
* **Memory Management:** Process ko kitni RAM aur kon kon se memory addresses mile hue hain.
* **I/O Information:** Konsi files open hain ya kon se devices use ho rahe hain.

---

> **Simple Analogy:**
> Jab aap game khel rahe hon aur game ko **Pause** kar dein, toh game aapka score, location, aur health save kar leta hai. Phir jab aap **Resume** karte hain, toh game waise hi wahan se start hoti hai. PCB computer ke liye bilkul isi **Pause/Save State** ka kaam karta hai!

30-July-2026


132. PCB stands for?

- Select correct option:
- Process Control Block (Page 140)
- Process Clearing Block
- Programmable Counter Block

