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


24. When two devices in the system want to use the same IRQ line then what will happen?
- An IRQ Collision
- An IRQ Conflict (Page 114)
- An IRQ Crash
- An IRQ Blockage

### **Question 24 Answer:**

**Sahi Option:** **An IRQ Conflict**

#### **Concept (Samajhne ke liye):**

`IRQ` (Interrupt Request) ek hardware line hoti hai jisse devices (jaise Keyboard, Mouse, Sound Card) CPU ka dhyan apni taraf khinchte hain.

* Agar do alag devices (jaise Sound Card aur Network Card) **ek hi IRQ line** ko use karne ki koshish karein, toh ise hardware terminology mein **IRQ Conflict** kehte hain.
* Iski wajah se dono devices crash ya properly kaam karna band kar sakti hain.

---

37. IRQ is referred to
- `Eight input signals`
- One output signal
- One input signals
- Eight output signals

38. Which of the following IRQs is derived by a key board?
- IRQ 0
- IRQ 1 (Page 113) rep
- IRQ 2
- IRQ 3

39. Which of the following IRQs is connected to serial port COM 1?
- IRQ 4 (page 114)
- IRQ 5
- IRQ 6
- IRQ 7

---
---
---

56. IRQ 0 has priority
- Low
- High
- Highest (Page 114)
- Medium




## 2. Sawal 56: IRQ 0 Priority (V.I.P Line)

Computer ke andar boht saari cheezein ek sath CPU ka dhyan khainchti hain (Keyboard, Mouse, Disk, Timer). Isliye CPU ne ek **Priority List (VIP List)** banayi hui hai:

* **IRQ 0 (System Timer):** Yeh Prime Minister ki tarah hai — iski priority sab se **Highest (Sab Se Pehle)** hoti hai. CPU baaki sab kaam chhor kar pehle Timer ki baat sunta hai.
* **IRQ 7:** Iski priority sab se **Lowest (Sab Se Aakhir)** hoti hai.

> **Ratta / Shortcut Rule:**
> **IRQ 0** = Sab se pehla number = **Highest Priority**.

---

Tension mat lo, agar koi MCQ ajeeb lage toh mujhe bol do, hum usko simple real-life example mein tod lenge!

---



64. IRQ referred as
- Eight Input signals (Page 113 ) rep
- One Input signal
- Eight Output signals
- One output signal

65. IRQ for keyboard is
1 (Page 114)

- Timer IRQ (Page 114)
- Sound Card
- Floppy Disk

