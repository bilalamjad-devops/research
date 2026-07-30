The thread registration code initializes the PCB and adds it to the linked list so that the ___ will give it a turn.

- Assembler
- Scheduler (Page 141)
- linked
- Debugger

Sahi Option Hai: **Scheduler**

---

### **Concept (Samajhne ke liye):**

Is question mein pucha gaya hai ke jab bohot saare **Threads** ya **Processes** chal rahe hote hain, toh run-time par unhe CPU ka time slot (baari/turn) kaun deta hai?

* **Scheduler (Operating System ka hissa):** Iska kaam yeh hota hai ke yeh faisla kare ke kis thread ko abhi CPU milega aur kitni der ke liye milega. Yeh har thread ko ek ek karke uski **turn (baari)** deta hai.

---

### **Baqi Options Galat Kyun Hain?**

* **Assembler:** Yeh Assembly Code (e.g., `MOV AX, BX`) ko Machine Code (`0s` aur `1s`) mein convert karta hai. Iska execution timing se koi lena dena nahi.
* **Linker:** Yeh multiple code files/object files ko mila kar ek executable (`.exe`) file banata hai.
* **Debugger:** Yeh code mein se errors (bugs) dhoondne ke liye use hota hai (jaise `DEBUG` ya `AFD`).

---

> **Exam Tip:**
> Jab bhi **"turn"**, **"CPU allocation"**, ya **"multitasking timing"** ka question aaye, toh uska answer hamesha **Scheduler** hota hai.

Agla MCQ paste karein!
