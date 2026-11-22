**Regular Expression**

As discussed earlier that 

a* generates Λ, a, aa, aaa, … 

and 

a+ generates a, aa, aaa, aaaa, …, 

so 

the language L1 = {Λ, a, aa, aaa, …} 

and 

L2 = {a, aa, aaa, aaaa, …} can simply be expressed by a* and a+, respectively.

a* and a+ are called the regular expressions (RE) for L1 and L2 respectively.

`Note a+, aa* and a*a generate L2.*`

---
---
---


**Recursive definition of Regular Expression(RE)**

Step 1: Every letter of Σ including Λ is a regular expression.

Step 2: If r1 and r2 are regular expressions then
- (r1)
- r1 r2
- r1 + r2 and
- r1*
are also regular expressions.

Step 3: Nothing else is a regular expression. 

---
---
---



22-Nov-2026
