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

---
---
---


**Equivalent Regular Expressions**

Definition

Two regular expressions are said to be equivalent if they generate the same language.

Example

Consider the following regular expressions

r1 = (a + b)* (aa + bb)

r2 = (a + b)*aa + ( a + b)*bb then both regular expressions define the language of strings ending in aa or bb.

Note

If r1 = (aa + bb) and r2 = ( a + b) then

r1+r2 = (aa + bb) + (a + b)

r1r2 = (aa + bb) (a + b)

= (aaa + aab + bba + bbb)

(r1)* = (aa + bb)* 

---
---
---





23-Nov-2026
