The protocol address of the next hop must be __ to an equivalent hardware address before a packet can be sent.

Translated


**Haan, bilkul 100%!** Aap ke ghar ka **Wi-Fi router / modem** hi aap ke computer ya mobile ke liye pehla **Next Hop** hota hai.

---

### **Yeh Process Kaise Kam Karta Hai?**

1. **Aapka Device (Mobile/Laptop):** Jab aap apne mobile par koi website (e.g., `google.com`) kholte hain.
2. **First Stop (Next Hop):** Aapka mobile dekhta hai ke Google ka server ghar se bahar internet par hai. Toh mobile data ko sab se pehle aap ke **Wi-Fi Router / Modem** ke paas bhejta hai.
$\rightarrow$ Yahan **Wi-Fi Modem = Next Hop**.
3. **Translating Address:** Mobile ko Wi-Fi modem ki IP address (jaise `192.168.1.1`) pata hoti hai. Lekin Wi-Fi signal/Ethernet par data bhejne ke liye mobile pehle us IP ko modem ke **MAC Address (Hardware Address)** mein **Translate** karta hai.
4. **Agla Safar:** Jab data modem tak pohanch jata hai, toh modem usay aage internet provider (PTCL, StormFiber, etc.) ke agle router par bhej deta hai (jo modem ke liye *agla* Next Hop ban jata hai).

---

### **Summary (Exam Mindset):**

> **Local Network:** Aap ke computer ke liye **Next Hop = Aapka Wi-Fi Modem / Default Gateway**.
> **Data Transfer Rule:** Packet Wi-Fi modem tak phonchane se pehle modem ki IP address ko uske **Hardware (MAC) address mein Translate** karna zaroori hota hai.
