Aao isay aik bilkul aam zindagi ki misaal se samjhte hain!

Aap apne phone ka tasawwur karein:

---

### **Real Life Example: Smart Phone**

Maan lijiye aapke paas ek phone hai. Aap chahte hain ke usme sirf **safe aur zaroori apps** chalain, koi virus ya faltu app na aaye.

Iske liye aap ek **List (Inventory)** banate hain:

1. **WhatsApp** (Version 2.24)
2. **Zoom** (Version 5.12)
3. **MS Office** (Version 16.0)

Aapne sirf inhi specific apps aur unke versions ko permission di hui hai. Is list ko kehte hain: **"Authorized Software and Version List"**.

---

### **Iska Security Mein Kya Faida Hai?**

1. **Ghalat Apps Se Bachao (Unauthorized Software Block):**
Agar koi Banda ya Hacker aapke PC mein koi ghalat game ya virus app install karne ki koshish karega, toh system check karega ke *"Kya yeh app meri List mein hai?"* Jawab milega **"Nahi"**, toh system use **block** kar dega.
2. **Purane Versions Ka Pata Chalna (Version Tracking):**
Maan lijiye news aati hai ke *Zoom version 5.10 mein ek hacker ka bug aaya hai*. Agar aapke paas exact **version number** likha hua hoga, toh aapko foran pata chal jayega ke aapko Zoom update karne ki zaroorat hai.

---

### **MCQ Ki Summary:**

Jab Control kehta hai ke **"Authorized and Unauthorized Software ki Inventory (List) banao"**, toh iska matlab yeh hota hai ke:

> **"Aapke paas un tamaam APPROVED / AUTHORIZED software aur unke EXACT VERSIONS ki list honi chahiye jo aapke systems par chalne ki ijazat rakhte hain."**

Isi waja se **Option C (Authorized software and version)** sahi jawab hai!

Ab clear hua? Agar koi confusion ho toh poochein!

---

Yeh **CIS Critical Security Controls** (jise pehle **SANS Top 20 Controls** kaha jata tha) ke andar aata hai.

CS205 ke course curriculum mein security hardening aur inventory controls ke liye **CIS Controls Framework** ko follow kiya jata hai.

---

### **CIS Controls Ke Pehle 2 Major Controls:**

CIS Controls framework mein assets aur software ki list rakhne ke liye 2 foundational controls hain:

1. **CIS Control 1: Inventory and Control of Enterprise Assets**
* Organizations ke saare **Hardware / Devices** (laptops, servers, routers) ki list rakhna.


2. **CIS Control 2: Inventory and Control of Software Assets**
* (Yeh aapka MCQ tha!) Enterprise mein chalne wale saare **Authorized Software aur unke exact Versions** ki list rakhna taake unauthorized software ko block kiya ja sake.



---

### **Parent Umbrella / Category Chart:**

```text
               [ CIS Critical Security Controls ]
                               |
       -------------------------------------------------
       |                                               |
 [ CIS Control 1 ]                               [ CIS Control 2 ]
 Hardware Inventory                              Software Inventory
 (Devices / Laptops)                             (Authorized Software & Version)

```

---

### **One-Line Answer for Exam:**

> "Inventory of Authorized and Unauthorized Software" **CIS Critical Security Controls (CIS Controls)** framework ke **Control 2 (Software Asset Management)** ke andar aata hai.

Ab poori baat samajh aa gayi? Jab aap ready hon, agla MCQ share karein!

29-July-2026


Yeh diagram **CIS Critical Security Controls (Center for Internet Security Controls)** ke **sab se pehle 2 basic rules (foundational controls)** ko dikha raha hai.

In short: **Security ka pehla aur sab se buniyadi asool yeh hai ke pehle pata toh ho ke organization mein KYA KYA chal raha hai!**

---

### Iska Simple Matlab Kya Hai?

Jab bhi aap kisi organization ki cyber security tight karte hain, toh pehle do kaam sab se pehle kiye jaate hain:

1. **CIS Control 1: Enterprise Hardware Inventory (Devices Ka Hisab-Kitaab)**
* **Sawal:** Aapke network par kitne physical devices connect hain?
* **Details:** Laptops, Desktops, Servers, Routers, Mobile devices.
* **Maqsad:** Agar kisi device ka pata hi nahi hoga (unauthorized laptop), toh aap use secure kaise karenge?


2. **CIS Control 2: Software Assets Inventory (Software & Versions Ka Hisab-Kitaab)**
* **Sawal:** Un sabhi devices par kaun kaun se software aur unke kaunse versions chal rahe hain?
* **Details:** Approved/Authorized Apps (jaise MS Office v16, Chrome v120) vs Unapproved Apps (Torrent, Cracked Games).
* **Maqsad:** Purane software versions aur ghalat apps mein sab se zyada security bugs (vulnerabilities) hotay hain. Unhe block aur update karna!



---

### Real-Life Analogy (Ghar Ki Security):

* **CIS Control 1 (Hardware):** Ghar ke saare **Darwazay aur Khidkiyaan (Entry Points)** ginna taake sab par taala lagaya ja sake.
* **CIS Control 2 (Software):** Ghar ke andar **kaun kaun se log (Software)** reh rahe hain aur unke paas **chabiyaan (Versions/Permissions)** konsi hain unka hisab rakhna.

---

### Exam Summary:

Yeh dono **CIS Top 18 / Top 20 Controls** ke **Basic/Foundational Controls** hain jo har security model ki **Buniyaad (Foundation)** hote hain.

---

Aao isay step-by-step simple words mein samjhte hain taake yeh hamesha ke liye clear ho jaye!

---

### 1. **Qualys Kya Hai? (The Tool)**

Qualys ek **Automated Software Tool** hai jo poore network ko scan karta hai.

* **Sochien:** Qualys ek **Digital Security Guard** ya **Inspector** ki tarah hai jo aap ke hazaron computers aur servers ko automated check karta hai.

---

### 2. **CIS aur DISA Kya Hain? (The Rules / Standards)**

Qualys ek Inspector zaroor hai, lekin jab tak aap inspector ko **"Security Rules / Checklist"** nahi denge, use kaise pata chalega ke computer secure hai ya nahi?

Yeh **Rules** pehle se security experts ne banaye hain:

* **CIS (Center for Internet Security):** Global industry ke sab se best rules (Checklist). Jaise: *"Windows 11 ka password kam se kam 12 characters ka hona chahiye"*, ya *"Unused WiFi networks ko block karna chahiye"*.
* **DISA (Defense Information Systems Agency):** Army aur Military-grade high security rules (Checklist).

---

### 3. **Qualys Ko CIS aur DISA Ki Kyun Zaroorat Hai? (Why Built-in Library?)**

Maan lijiye aapki company mein **5,000 Computers** hain. Agar aapko check karna ho ke un sab par security rules apply hue hain ya nahi, toh:

1. **Agar Built-in Rules NA HO (Without CIS/DISA Library):**
Aapko manually 5,000 rules likhne parenge, jismein mahino lag jayenge aur ghalti ka chance hoga.
2. **Built-in CIS/DISA Library Ka Faida (With Built-in Library):**
Qualys ke andar yeh saare rules **pehle se bane hue** (built-in) hain!
Aap bas Qualys mein **"CIS Benchmark Policy"** select karte hain aur **Start Scan** dabate hain. Qualys foran 5,000 computers ko scan karke ek minute mein report de deta hai ke:
* *"Computer 12 me Password policy ghalat hai"*
* *"Computer 45 me Windows Firewall OFF hai"*



---

### **Simple Summary for Exam:**

> **Qualys** = Scanning Tool (Inspecting Engine)
> **CIS / DISA** = Rules & Security Checklists (Standard Books)
> **Qualys ke andar CIS aur DISA ki built-in policies isliye hoti hain taake aapko khud se security rules na likhne paren, aur aap international security standards ke mutabiq 1-click scanning kar sakein.**

Clear ho gaya? Jab aap ready hon, agla MCQ share karein!
