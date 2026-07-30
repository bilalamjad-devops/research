Sahi Option Hai: **External directive, Global directive**

---

### **Concept (Samajhne ke liye):**

NASM Assembly language mein jab hum code ko multiple files mein baant-te (modular programming) hain, toh symbols (labels / functions / variables) ko share karne ke liye do directives istemaal hoti hain:

1. **`EXTERN` (Imported Symbol):**
* Jab kisi doosri file ka function ya variable aap apni current file mein **import / use** karna chahte hain, toh aap **`EXTERN`** directive use karte hain.
* Yeh assembler ko batata hai ke "yeh symbol yahan nahi, kisi aur file mein bana hua hai".


2. **`GLOBAL` (Exported Symbol):**
* Jab aap apni current file ke kisi label ya function ko **export / public** karna chahte hain taake baqi files bhi usay access kar sakein, toh aap **`GLOBAL`** directive use karte hain.



---

### **Code Example:**

```assembly
; File 1: Math functions
GLOBAL add_numbers      ; Is function ko export kar rahe hain taake doosri files use kar sakein

add_numbers:
    add ax, bx
    ret

; File 2: Main Program
EXTERN add_numbers      ; File 1 ke function ko import kar rahe hain

main:
    call add_numbers

```

---

> **Exam Tip:**
> * **Import** karna $\rightarrow$ **`EXTERN`** (ya `EXTERNAL`)
> * **Export** karna $\rightarrow$ **`GLOBAL`**
> 
>
