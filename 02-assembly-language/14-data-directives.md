Sahi Option Hai: **db**

---

### **Concept (Samajhne ke liye):**

NASM Assembly language mein memory mein space reserve/define karne ke liye Data Directives istemaal hoti hain. Numbers ka size bit-length par depend karta hai:

* **1 Byte = 8 Bits**
* **`db` (Define Byte):** Memory mein **8 bits (1 byte)** reserve ya initialize karne ke liye use hota hai.

---

### **NASM Data Directives Summary (Exam Ke Liye):**

| Directive | Full Form | Size in Bytes | Size in Bits | Example |
| --- | --- | --- | --- | --- |
| **`db`** | **Define Byte** | **1 Byte** | **8 Bits** | `var1 db 0xAA` |
| **`dw`** | **Define Word** | **2 Bytes** | **16 Bits** | `var2 dw 0xFFFF` |
| **`dd`** | **Define Double word** | **4 Bytes** | **32 Bits** | `var3 dd 0x12345678` |
| **`dq`** | **Define Quad word** | **8 Bytes** | **64 Bits** | `var4 dq 0x123456789ABCDEF0` |

---

> **Exam Tip:**
> * **8 bits** $\rightarrow$ **`db`** (Define Byte)
> * **16 bits** $\rightarrow$ **`dw`** (Define Word)
> * **32 bits** $\rightarrow$ **`dd`** (Define Double-word)
> 
>
