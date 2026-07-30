77. Which bit of the attributes byte represents the red component of foreground color?
- 5
- 4
- 3
- 2 (Page 81)

Sahi Option Hai: **2**

---

### **Concept (Video Attribute Byte Structure):**

Video memory mein text mode par ek character ka Attribute Byte (8 bits: Bit 0 se Bit 7) is tarah split hota hai:

```
 Bit 7     Bit 6  Bit 5  Bit 4     Bit 3     Bit 2  Bit 1  Bit 0
[ Blink ] [   Background RGB   ]  [ Intensity ] [   Foreground RGB   ]
                                                  R      G      B

```

Foreground Colors (**Bits 0–2**):

* **Bit 0:** Blue
* **Bit 1:** Green
* **Bit 2:** **Red**

---

### **Exam Cheat Sheet (Video Attribute Bits):**

| Bit Position | Component |
| --- | --- |
| **Bit 0** | Foreground Blue |
| **Bit 1** | Foreground Green |
| **Bit 2** | **Foreground Red** |
| **Bit 3** | Foreground Intensity (Bright/Light) |
| **Bit 4** | Background Blue |
| **Bit 5** | Background Green |
| **Bit 6** | Background Red |
| **Bit 7** | Blink / Background Intensity |

---

> **1-Line Memory Trick:**
> Order hamesha **RGB** (Red, Green, Blue) ki jagah bit order mein **BGR** hota hai: Bit 0 = Blue, Bit 1 = Green, Bit 2 = Red!
