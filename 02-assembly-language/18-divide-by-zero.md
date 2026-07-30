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
