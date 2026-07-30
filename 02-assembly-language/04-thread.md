Thread ko simple real-life example se samajhte hain!

### **Simple Real-Life Example:**

Maan lein **Microsoft Word** ek poora **Process (Program)** hai. Jab aap Word kholte hain, toh ek sath kayi kaam ho rahe hote hain:

1. Aap keyboard se typing kar rahe hote hain.
2. Background mein spelling errors check ho rahe hote hain.
3. File automatically auto-save ho rahi hoti hai.

Yeh saare alag-alag chote kaam jo ek hi program ke andar ek sath chal rahe hain, inko **Threads** bolte hain!

---

### **Technical Definition (Assembly / OS ke mutabiq):**

* **Thread** kisi bhi Program/Process ke andar **sabse chota execution path (sub-task)** hota hai.
* Continuous/Parallel working ke liye computer ek hi process ko chote chote **Threads** mein baant deta hai taake CPU fast kaam kar sake.

---

### **Thread "Dynamic" Kyun Hota Hai?**

Jab aap typing shuru karte hain, toh computer ek naya thread **banata** hai (create karta hai). Jab aap typing rok dete hain, toh wo thread **khatam** ho jata hai.

Kyunki yeh threads program chalne ke dauran (Runtime par) zaroorat ke hisab se bante aur mit-te rehte hain, isliye inki creation ko **Dynamic** kaha jata hai!

---

> **Key Points for CS401 Exam:**
> * **Process:** Main Program (e.g., MS Word, Game).
> * **Thread:** Program ke andar ka Chota Task (e.g., Typing, Sound play hona).
> * **Creation:** **Dynamic** (Run-time par bante hain).

---
---
---

Sahi Option Hai: **Dynamic**

---

### **Concept (Samajhne ke liye):**

Assembly Language aur Operating System ke context mein threads **Dynamic** hote hain:

1. **Dynamic Creation:** Jab program chal raha hota hai (Run-time par), tab zaroorat ke mutabiq naye threads create kiye jaate hain aur jab unka kaam khatam ho jata hai toh unhe destroy/kill kar diya jata hai.
2. Kyunki threads program ke dauran kabhi bhi bante aur khatam hote rehte hain, isliye inki creation **Dynamic** hoti hai (static nahi).

---

> **Exam Tip:**
> Jab bhi Threads ya Processes ki creation ka question aaye, toh CS401 ke mutabiq iska answer **Dynamic** hota hai.

Agla MCQ paste karein!

Ab Thread ka concept clear ho gaya? Agla question paste karein!

---
---
---


29. Threads can have function calls, parameters and _ variables.
- Global
- Local (Page 141)
- Legal
- Illegal

Asaan alfaz mein samjhte hain!

Aap **DevOps / Programming** mein **Multithreading** ya Functions to zaroor use karte honge. Bilkul wahi concept hai!

---

### **Real-Life Example (Chef / Kitchen):**

Sochein ek kitchen (Process) hai jisme **2 Chefs (Threads)** kaam kar rahe hain:

1. **Global Variables (Shared):** Kitchen ka **Main Fridge ya Stove**. Dono chefs isse aapas mein share karte hain.
2. **Local Variables (Private):** Har chef ka apna **Katne wala Board (Cutting Board) ya Pocket**. Chef 1 ke board par jo pyaz rakha hai, wo Chef 2 ke board par nahi hota!

---

### **Computer Mein Kya Hota Hai?**

Jab ek **Thread** chalta hai:

* Uske apne **Functions** hote hain.
* Un functions ke **Parameters** hote hain.
* Aur unke andar banne wale **Local Variables** us thread ke apne private hote hain (uske apne Stack mein hote hain).

---

### **Aapke Sawal Ka Direct Answer:**

> Threads ke paas apne function calls, parameters aur **Local** variables hote hain.

*(Kyunke local variables har thread ke apne private hote hain, baki threads ke sath share nahi hote).*
