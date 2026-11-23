**The Language EVEN-EVEN**

Language of strings, defined over Σ={a, b} having even number of a’s and even number of b’s. i.e.

EVEN-EVEN = {Λ, aa, bb, aaaa,aabb,abab, abba, baab, baba, bbaa, bbbb,…}, its regular expression can be
written as `(aa+bb+(ab+ba)(aa+bb)*(ab+ba))* `

---
---
---

Note

It is important to be clear about the difference of the following regular expressions

r1 = a*+b*

r2 = (a+b)*

Here r1 does not generate any string of concatenation of a and b, while r2 generates such strings. 

example: 

r1 can create this: aaaaa, bbbbb 

we can create abbba using r2 but not using r1. 

23-Nov-2026
