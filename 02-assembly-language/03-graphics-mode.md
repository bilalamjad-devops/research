Aao isay ek simple screen aur picture ki example se samajhte hain!

### **Real-Life Example: TV ya Mobile Screen**

Mobile ya Computer screen chote chote **dots** (jinko hum **Pixels** bolte hain) se mil kar bani hoti hai.

1. **Text Mode (Likhai waala mode):**
Is mode mein screen ko chote chote **Character Boxes** mein baanta jata hai. Ek location par poora ka poora **letter** (jaise 'A', 'B', 'C') aata hai.
2. **Graphics Mode (Drawing/Gaming waala mode):**
Is mode mein screen ka har ek chota **Dot** direct memory ke saath connect hota hai.
* Agar memory mein $1$ likhein, toh screen ka wo **Dot** chamak jayega (Light on).
* Agar $0$ likhein, toh wo **Dot** dark ho jayega (Light off).



Jab bohot saare **Dots** ek sath milte hain, tabhi mil kar Line, Circle, ya koi Photo banti hai.

---

### **Bas Yeh Table Yaad Rakhni Hai Exam Ke Liye:**

| Screen Mode | Memory Location Kya Represent Karti Hai? |
| --- | --- |
| **Graphics Mode** | **Dot** (Pixel) |
| **Text Mode** | **Character** (Letter) |

Question mein **Graphics mode** poocha tha, isliye sahi answer **Dot** hai!

Ab clear hua? Agla MCQ paste karein!

30-July-2026


---

28. Value of AH in the write Graphics pixel service is
 ► 0Ch (Page 152)
 ► 0Bh
 ► 1Ch
 ► 2Ch


Sahi Option Hai: **0Ch**

---

### **Concept (Samajhne Ke Liye):**

Video screen par kaam karne ke liye hum **`INT 10h`** (Video Services) ka istemal karte hain.

Jab aap graphics mode mein screen par ek **akela pixel (Chota sa Dot)** draw ya write karna chahte hain:

1. Service Number **`0Ch`** ko **`AH`** register mein rakhte hain (`mov ah, 0Ch`).
2. Pixel ka rang (color) **`AL`** register mein daalte hain.
3. Pixel ki position ($X, Y$ coordinates) **`CX`** (Column) aur **`DX`** (Row) mein daalte hain.
4. Phir **`INT 10h`** call karte hain.

---

### **INT 10h Video Services Cheat Sheet (Exam Ke Liye Important):**

| Service (`AH`) | Purpose (Kaam) |
| --- | --- |
| **`00h`** | Set Video Mode (Text vs Graphics Mode) |
| **`02h`** | Set Cursor Position (Text mode mein cursor move karna) |
| **`0Ch`** | **Write Graphics Pixel (Screen par pixel draw karna)** |
| **`0Dh`** | Read Graphics Pixel (Pixel ka color read karna) |

---

> **Exam Shortcut:**
> Screen par Pixel **Write** karne ke liye `AH` mein **`0Ch`** rakha jata hai!
