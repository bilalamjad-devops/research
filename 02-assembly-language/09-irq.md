**IRQ** ka matlab **Interrupt Request** hota hai.

Isay aik simple real-life example se samajhte hain!

---

### **Real-Life Example: Office Desk**

Maan lein aap apne room mein baith kar gehri parhai (work) kar rahe hain.

* Jab tak koi doorbell nahi bajata, aap apna kaam karte rehte hain.
* Jaise hi doorbell bajti hai, aap apna kaam **temporarily pause** karte hain, darwaza kholte hain (guest ko deal karte hain), aur wapas aakar wahan se parhai start kar dete hain jahan chhodi thi.

Is example mein:

* **CPU** = Aap
* **Doorbell Signal** = **IRQ (Interrupt Request)**
* **Guest Ko Deal Karna** = Interrupt Service Routine (ISR)

---

### **Technical Definition:**

**IRQ (Interrupt Request)** aik hardware signal hota hai jo computer ke devices (jaise Keyboard, Mouse, Disk, ya Timer) **CPU ko bhejte hain**.

Jab kisi device ko CPU ki urghant attention chahiye hoti hai (jaise jab aap keyboard par key press karte hain), toh woh IRQ pin par signal bhej kar CPU ko bolta hai: **"Mera kaam pehle karo, apna current kaam do minute roko!"**

---

### **Computer Mein IRQs Kaise Kaam Karte Hain?**

1. CPU apna normal program chala raha hota hai.
2. Aap keyboard par `A` press karte hain.
3. Keyboard Controller **IRQ 1** line par signal bhejta hai.
4. **PIC (Programmable Interrupt Controller)** is signal ko receive karta hai aur CPU ko bolta hai ke Keyboard se input aaya hai.
5. CPU apna current code temporary save karta hai, `A` key ko screen par show karta hai, aur wapas apne purane kaam par laut jata hai.

---

### **CS401 Exam Ke Liya 3 Key Points:**

* **IRQ = Hardware Signal** (Device se CPU ki taraf jata hai).
* **IRQ 0:** System Timer (Clock ticks).
* **IRQ 1:** Keyboard (Key press/release).

---
---
---

Sahi Option Hai: **IRQ 1**

---

### **Concept (Samajhne ke liye):**

Computer mein jab bhi aap keyboard par koi key press karte hain ya chorhte hain, toh keyboard CPU ko ek **Hardware Interrupt (IRQ)** bhejta hai taake CPU ko pata chale ke koi input aaya hai.

Hardware Interrupts (IRQs) ke fixed channels hotay hain:

* **IRQ 0:** System Timer (Clock) ke liye dedicated hota hai.
* **IRQ 1:** **Keyboard** ke liye reserved hota hai.
* **IRQ 2:** Cascade IRQ (SND 8259 PIC controller ko connect karne ke liye).

---

### **Important IRQs List (CS401 Exam Ke Liye):**

| IRQ Number | Associated Hardware Device |
| --- | --- |
| **IRQ 0** | System Timer |
| **IRQ 1** | **Keyboard** |
| **IRQ 2** | Cascaded Interrupt Controller (PIC 2) |
| **IRQ 3** | COM2 / COM4 (Serial Ports) |
| **IRQ 4** | COM1 / COM3 (Serial Ports) |
| **IRQ 6** | Floppy Disk Controller |
| **IRQ 7** | LPT1 (Parallel Port / Printer) |

---

> **Exam Tip:**
> Keyboard ka IRQ hamesha **IRQ 1** hota hai aur iska Interrupt Vector **INT 9** hota hai.

30-July-2026
