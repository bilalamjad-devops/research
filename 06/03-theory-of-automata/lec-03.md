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

**Method 3 (Regular Expressions)**

Now consider another language L, consisting of all possible strings, defined over Σ = {a, b}. This language can
also be expressed by the regular expression (a + b)*. 

Now consider another language L, of strings having exactly one a, defined over Σ = {a, b}, then it’s regular
expression may be `b*ab*`.

Now consider another language L, of even length, defined over Σ = {a, b}, then it’s regular expression may be
((a+b)(a+b))*

Now consider another language L, of odd length, defined over Σ = {a, b}, then it’s regular expression may be
`(a+b)((a+b)(a+b))* or ((a+b)(a+b))*(a+b). `





22-Nov-2026
