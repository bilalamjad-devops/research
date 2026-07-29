Isko bilkul simple tariqay se samajhte hain!

Yeh **OSI Model** ki alag-alag layers par kaam karne wale **Firewalls / Proxies** ki types hain.

Jab internet se traffic aata ya jaata hai, toh security tools (Firewalls) use alag-alag level par check karte hain. Inhe computer networking mein **Firewall Technologies / Proxy Types** kaha jata hai.

---

### 1. Network Layer Filtering Proxy (Packet Filter)

* **OSI Layer:** **Layer 3 (Network Layer)**
* **Kaam Kya Hai?** Yeh sirf basic details dekhta hai—jaise **Source IP, Destination IP, aur Port Number**.
* **Misaal:** Yeh ek Security Guard ki tarah hai jo sirf aapka **CNIC / ID Card** dekhta hai, lekin aapke bag ke andar kya hai wo check nahi karta.

---

### 2. Transport / Session Layer Filtering Proxy (Circuit-Level Gateway)

* **OSI Layer:** **Layer 4 & 5 (Transport & Session Layer)**
* **Kaam Kya Hai?** Yeh check karta hai ke do devices ke beech **TCP Handshake / Connection** sahi tariqay se bana hai ya nahi.
* **Misaal:** Yeh guard check karta hai ke aapka aane ka **time aur pass (session)** valid hai ya nahi, lekin content phir bhi read nahi karta.

---

### 3. Application Layer Proxy (Application Firewall / Proxy Firewall)

* **OSI Layer:** **Layer 7 (Application Layer - Top Level)**
* **Kaam Kya Hai?** Yeh sab se **smart aur secure** filtering hoti hai. Yeh poore packet ke **andar ke content / data** ko khol kar inspect karta hai (jaise HTTP, HTTPS, FTP, Emails) aur user ko authenticate bhi karta hai.
* **Misaal:** Yeh wo guard hai jo aapka ID check karne ke baad aapka **bag khol kar scanner se guzarta hai** taake andar koi virus ya harmful item na ho.

---

### Summary Table (Paper Tip):

| Proxy / Filter Type | OSI Layer | Main Focus | Speed vs Security |
| --- | --- | --- | --- |
| **Network Layer** | Layer 3 | IP Address & Ports | Tezz (Fast), kam security |
| **Session Layer** | Layer 5 | Handshake / Connection session | Medium |
| **Application Layer** | Layer 7 | Deep Data Inspection & User Auth | Thora slow, **Sab se high security** |

> **Summary:**
> In sab ko **Firewall Filtering Types** ya **Proxy Technologies** kaha jata hai.

---

If you want a quick visual overview of how proxy firewalls inspect traffic at layer 7, check out this video:

[What Is a Proxy Firewall? Application-Layer Security Explained](https://www.youtube.com/watch?v=3OxGSZBNX7U)

This video explains how proxy firewalls break connection paths at the application layer to deeply inspect data packets.

19-July-2026
