76. SP is associated with.................By default
- SS (Page 34)
- DS
- CS
- ES

Sahi Option Hai: **SS**

---

### **1-Line Memory Trick:**

* **`SP`** = **S**tack **P**ointer
* **`SS`** = **S**tack **S**egment

**Rule:** `SP` (Stack Pointer) hamesha by default **`SS`** (Stack Segment) ke sath hi pair banta hai!

---

### **Fast Recall Table (Segment & Offset Default Pairs):**

| Offset Register | Default Segment Register | Main Purpose |
| --- | --- | --- |
| **`IP`** (Instruction Pointer) | **`CS`** (Code Segment) | Agli instruction ka address |
| **`SP` / `BP**` (Stack/Base Pointer) | **`SS`** (Stack Segment) | Stack memory access |
| **`SI` / `BX**` | **`DS`** (Data Segment) | Normal Data Access |
| **`DI`** (Destination Index) | **`ES`** (Extra Segment) | String Operations Destination |
