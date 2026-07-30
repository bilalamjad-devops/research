Koi baat nahi, tension bilkul mat lein! DevOps context thoda high-level ho sakta hai. Chalein saaf aur simple urdu mein step-by-step clear karte hain.

---

### **Bus 2 Batein Yaad Rakhein:**

#### **1. Normal Code (Jo Hum Likhte Hain):**

Jab hum CPU ko koi kaam dene ke liye instruction likhte hain, jaise:

* `MOV AX, 5` (AX mein 5 daalo)
* `INT 21h` (Screen par kuch print karo)

Yeh sab **hum khud code mein likhte hain**.

---

#### **2. Automatic Accident / Event (Jo CPU Khud Karta Hai):**

Sochein aap gari chala rahe hain. Agar engine overheat ho jaye, toh gari ka dash-board par **Red Warning Light khud hi on ho jati hai**. Aap ko manually koi button nahi dabana parta.

CPU mein jab **Zero ($0$) se division** hoti hai (jaise $10 \div 0$), toh yeh maths mein possible nahi hai.

* Yeh **CPU ke liye ek accident / error** hai.
* Is error aate hi CPU **khud-ba-khud (Automatically)** ek warning signal generate kar deta hai jise **`INT 0`** kehte hain.
* Programmer ko code mein `INT 0` likhne ki **kisi qism ki zaroorat nahi hoti**.

---

### **Sawal Ka Seedha Jawab:**

MCQ puch raha hai ke *'Divide by 0'* hone par **kon si instruction use hoti hai?**

Jawab hai: **Koi instruction use nahi hoti, yeh AUTOMATICALLY trigger hota hai!**

---









---
---
---


Sahi sawal! Simple lafzon mein: **`INT` ka matlab Interrupt hota hai**, aur aage jo number ($0, 1, 2$) likha hai, wo **Interrupt Ka ID / Type Number** hota hai.

Jaise Police ka emergency number **15** hota hai, Fire Brigade ka **16**, aur Ambulance ka **1122**—har number ka apna ek specific kaam fix hota hai.

Bilkul waise hi CPU ke paas bhi pehle se fixed **Interrupt Numbers** hote hain:

---

### **1. `INT 0` — Divide by Zero (Ghalat Maths Error)**

* **Kyun Aata Hai?** Jab bhi aapka program kisi number ko **Zero ($0$)** se divide karne ki koshish karta hai (jaise $10 \div 0$).
* **Kaise Trigger Hota Hai?** Yeh **CPU Khud / Automatically** trigger karta hai.

---

### **2. `INT 1` — Single Step (Debugging Mode)**

* **Kyun Aata Hai?** Jab aap Debugger software (jaise AFD ya GDB) mein code ko **ek ek line karke run (step-by-step)** check karte hain.
* **Kaise Trigger Hota Hai?** Har ek single assembly line execute hone ke baad CPU yeh interrupt generate karta hai taake aap registers ki values check kar sakein.

---

### **3. `INT 2` — Non-Maskable Interrupt / NMI (Hardware Emergency)**

* **Kyun Aata Hai?** Jab computer ke hardware mein koi severe issue aaye—jaise RAM corrupt hona, Power supply mein Masla, ya Memory parity error.
* **Khas Baat:** Isay CPU ignore (mask) **nahi** kar sakta. Chahe CPU kitna bhi busy ho, isay baqi sab kaam chor kar pehle handles karna padta hai.

---

### **Quick Summary Table (Exam Ke Liye):**

| Interrupt | Dedicated Name | Kab Trigger Hota Hai? | Kon Trigger Karta Hai? |
| --- | --- | --- | --- |
| **`INT 0`** | **Divide by Zero** | Zero से divide hone par | **CPU (Automatic)** |
| **`INT 1`** | **Single Step / Trap** | Code ko 1-1 line check karne par | **CPU (Debugging)** |
| **`INT 2`** | **NMI (Hardware Fault)** | RAM / Power supply fault hone par | **Motherboard / Hardware** |

---

> **Aasan Baath:** Yeh teeno $0, 1, 2$ CPU ke **built-in emergency / special signals** hain jo specific conditions par trigger hotay hain!
