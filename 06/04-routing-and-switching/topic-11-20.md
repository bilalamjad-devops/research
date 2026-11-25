## Topic 012

Is video (**CS407_Topic011** — Virtual University of Pakistan) ka short aur asaan **Roman English** summary niche diya gaya hai:

### **Topic: Cisco IOS Modes Mein Navigate Karna** [[00:01](https://www.youtube.com/watch?v=Cby3hmjFUwk&t=1)]

Jab technician router ya switch se connect hota hai, to security aur access control ke liye **Cisco IOS** kaam ko mukhtalif **modes** mein taqseem karta hai [[00:22](https://www.youtube.com/watch?v=Cby3hmjFUwk&t=22), [00:36](https://www.youtube.com/watch?v=Cby3hmjFUwk&t=36)].

---

### **1. Main IOS Modes** [[00:36](https://www.youtube.com/watch?v=Cby3hmjFUwk&t=36)]

* **User EXEC Mode (`Router>` / `Switch>`):** [[01:20](https://www.youtube.com/watch?v=Cby3hmjFUwk&t=80), [01:43](https://www.youtube.com/watch?v=Cby3hmjFUwk&t=103)]
* Sab se limited (read-only / view-only) mode hai [[01:28](https://www.youtube.com/watch?v=Cby3hmjFUwk&t=88), [01:36](https://www.youtube.com/watch?v=Cby3hmjFUwk&t=96)].
* Symbol **`>`** hota hai [[01:49](https://www.youtube.com/watch?v=Cby3hmjFUwk&t=109)]. Sirf basic check commands (jaise `ping`) chalti hain [[04:55](https://www.youtube.com/watch?v=Cby3hmjFUwk&t=295)].


* **Privileged EXEC Mode (`Router#` / `Switch#`):** [[00:51](https://www.youtube.com/watch?v=Cby3hmjFUwk&t=51), [02:21](https://www.youtube.com/watch?v=Cby3hmjFUwk&t=141)]
* Symbol **`#`** hota hai [[02:21](https://www.youtube.com/watch?v=Cby3hmjFUwk&t=141)].
* Is mein monitoring, management, aur administrative commands chal sakti hain [[02:32](https://www.youtube.com/watch?v=Cby3hmjFUwk&t=152), [02:49](https://www.youtube.com/watch?v=Cby3hmjFUwk&t=169)].


* **Global Configuration Mode (`Router(config)#`):** [[03:06](https://www.youtube.com/watch?v=Cby3hmjFUwk&t=186), [03:32](https://www.youtube.com/watch?v=Cby3hmjFUwk&t=212)]
* Poore router ya switch ki overall settings ke liye hota hai [[04:24](https://www.youtube.com/watch?v=Cby3hmjFUwk&t=264)].
* Prompt mein **`(config)`** aata hai [[03:32](https://www.youtube.com/watch?v=Cby3hmjFUwk&t=212)].


* **Sub-Configuration Modes (`Router(config-if)#`):** [[03:50](https://www.youtube.com/watch?v=Cby3hmjFUwk&t=230), [04:11](https://www.youtube.com/watch?v=Cby3hmjFUwk&t=251)]
* Kisi khas hisse (jaise kisi ek **interface** / port) ki setting ke liye hota hai [[04:04](https://www.youtube.com/watch?v=Cby3hmjFUwk&t=244), [04:36](https://www.youtube.com/watch?v=Cby3hmjFUwk&t=276)].
* Prompt mein hyphen ke saath naam aata hai, jaise **`(config-if)#`** [[04:11](https://www.youtube.com/watch?v=Cby3hmjFUwk&t=251)].



---

### **2. Modes Change Karne Ki Main Commands** [[06:04](https://www.youtube.com/watch?v=Cby3hmjFUwk&t=364)]

* `enable` $\rightarrow$ `>` se **`#`** (Privileged EXEC) mein jane ke liye [[06:10](https://www.youtube.com/watch?v=Cby3hmjFUwk&t=370)].
* `disable` $\rightarrow$ `#` se wapas **`>`** (User EXEC) mein aane ke liye [[06:29](https://www.youtube.com/watch?v=Cby3hmjFUwk&t=389)].
* `configure terminal` $\rightarrow$ `#` se **`(config)#`** (Global Config) mein jane ke liye [[03:18](https://www.youtube.com/watch?v=Cby3hmjFUwk&t=198), [05:24](https://www.youtube.com/watch?v=Cby3hmjFUwk&t=324)].
* `exit` $\rightarrow$ Ek step peeche jane ke liye.

Yehi tareeqa router aur switch dono par same kaam karta hai [[05:45](https://www.youtube.com/watch?v=Cby3hmjFUwk&t=345)].

**Video Link:** [http://www.youtube.com/watch?v=Cby3hmjFUwk](http://www.youtube.com/watch?v=Cby3hmjFUwk)

---
---
---

## Topic 012 

<img width="1600" height="900" alt="image" src="https://github.com/user-attachments/assets/23cd2d17-975f-4ca7-a8d4-733547bfc46c" />


Koi baat nahi! Chalein isay bilkul **mobile ya WhatsApp / Google search ki misal** se samajhte hain, taake bilkul asaan lage.

Sochhein aap router ke andar baithe hain aur usay command de rahe hain.

---

### **1. Command Likhne Ka Tareeqa**

Jis tarah aap WhatsApp par kisi ko msg bhejte waqt likhte hain:

* **Kis ko bhejna hai (`ping` / `show`)** $\rightarrow$ yeh **Command** hai.
* **Kis cheez par / kis address par (`192.168.1.1`)** $\rightarrow$ yeh **Argument / Target** hai.

Misal: `ping 192.168.1.1` = *"Check karo ke `192.168.1.1` tak raabta ho raha hai ya nahi."*

---

### **2. Jab Aap Ko Samajh Na Aaye ya Ghalti Ho (`?` aur Errors)**

* **`?` (Sawal ka Nishan) = Madad Mangna:**
* Jis tarah Google mein aadha word likhne par suggestions aatay hain, waise hi router mein `clock set ?` likh dein to woh khud bata deta hai ke aage kya likhna hai.


* **Ambiguous Command = "Bohot Saare Option Hain":**
* Agar aap sirf `c` likh dein, to router kahega: *"Bhai `c` se to `clock` bhi aata hai aur `clear` bhi—poora to likho!"*


* **Incomplete Command = "Baat Adhoori Hai":**
* Agar aap sirf `clock set` likh kar ruk jayein, to router kahega: *"Time to batao kitna set karna hai!"*


* **Invalid Input (`^`) = "Yahan Ghalti Hai":**
* Agar aap galat word likh dein, to router niche `^` ka teer laga kar bata deta hai ke ghalti kahan hai.



---

### **3. Shortcut Keys (Kaam Tez Karne Ke Liye)**

* **`Tab`** = Aadha lafz likh kar `Tab` dabayein to router khud poora kar dega (bilkul phone ki auto-complete ki tarah).
* **Up Arrow (`↑`)** = Pichli command wapas laane ke liye (jaise pichla msg dobara bhejna ho).
* **`Ctrl + Shift + 6`** = Agar koi check/process lamba chal raha ho (jaise lamba `ping`) aur aap ko beech mein rokna ho, to is se rok lete hain.
* **`Ctrl + C`** = Us waqt ki command ko cancel/band karne ke liye.

---

### **4. `show` Commands (Router Ki Report Card Dekhna)**

Jab aap router ki haalat check karna chahein to `show` likh kar poochte hain:

* **`show running-config`** = **Abhi Live Kya Chal Raha Hai** (RAM mein mojood settings — aise samjhein jaise table par rakha khula register).
* **`show startup-config`** = **Save Kya Hua Hai** (NVRAM mein mehfooz backup settings — aise samjhein jaise almari mein lock register).
* **`show interfaces`** = Router ki **ports/taaron** ki haalat (kaun si port on hai, off hai, ya IP kya laga hai).
* **`show version`** = Router ke **OS ka version** aur woh kab on/reboot hua tha.
* **`show flash`** = Router ki **Flash memory** mein konsi files pari hain.

---

### **Sirf 3 Cheezein Yaad Rakhein:**

1. **`?`** = Madad lena
2. **`Tab`** = Lafz poora karna
3. **`running-config` vs `startup-config**` = Live (RAM) vs Saved (NVRAM)

Ab kaisa laga? Agar kisi aik hisse ko aur zyada simple karna ho to us ka naam bata dein!


25-Nov-2026
