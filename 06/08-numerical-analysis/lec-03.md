
<img width="1600" height="900" alt="image" src="https://github.com/user-attachments/assets/e521d364-f4e0-4d96-bfb9-60ea57e9ef0e" />


f(x) = x^3 - 9x + 1 = 0 

Put x = 2

f(2) = 8 - 18 + 1 

= -10 + 1

= -9


Put x = 4 

f(4) = 64 - 36 + 1

= 29 

Mid Point = 2 + 4/2 = 6/2= 3 

Put x = 3 

f(3) = 27 - 27 + 1

= 1

Mid Point = 2 + 3/2 =5/2 = 2.5 

Put 2.5 in f(x) = x^3 - 9x + 1 = 0 

f(2.5) = (2.5)^3 - 9(2.5) + 1

= 15.635 - 22.5 + 1

= -5.865 

Mid Point = 2.5 + 3 /2 = 

Bilkul pareshan na hon, shuru mein ye thora confusing lagta hai lekin jab aap iske **2–3 main rules** pakar lete hain to bohot asaan ho jata hai [[12:04](https://www.youtube.com/watch?v=g59AM_8AYGI&t=724)].

Video link: [http://www.youtube.com/watch?v=g59AM_8AYGI](http://www.youtube.com/watch?v=g59AM_8AYGI)

---

### 1. Linear vs. Non-Linear Equations (Buniyaadi Farq)

* **Linear Equation:** Jis mein variables ki power **1** hoti hai (jaise $2x + cy - c = 5$) [[00:33](https://www.youtube.com/watch?v=g59AM_8AYGI&t=33)]. Iska graph **straight line** banta hai [[01:23](https://www.youtube.com/watch?v=g59AM_8AYGI&t=83)].
* **Non-Linear Equation:** Jis mein variable ki power **1 se zyada** hoti hai (jaise $x^3 - 9x + 1 = 0$ — transcript mein auto-caption ne $x^3$ ko "x" likh diya hai, lekin aage $3^3 = 27$ solve kiya gaya hai) [[00:52](https://www.youtube.com/watch?v=g59AM_8AYGI&t=52), [02:13](https://www.youtube.com/watch?v=g59AM_8AYGI&t=133), [04:22](https://www.youtube.com/watch?v=g59AM_8AYGI&t=262)]. Iska graph **curve** hota hai [[01:28](https://www.youtube.com/watch?v=g59AM_8AYGI&t=88)].

---

### 2. Bisection Method Kya Hai?

Ek interval ko baar-baar aadha ($2$ hisson) mein divide kar ke equation ka approximate root/solution nikalne ka method hai, jab tak consecutive midpoints aapas mein qareeb/approximately equal na aa jayein [[06:25](https://www.youtube.com/watch?v=g59AM_8AYGI&t=385), [12:26](https://www.youtube.com/watch?v=g59AM_8AYGI&t=746)].

---

### 3. Step-by-Step Kaise Solve Karte Hain? (Video Ki Example)

Function: $f(x) = x^3 - 9x + 1$, initial interval $[2, 4]$ [[02:19](https://www.youtube.com/watch?v=g59AM_8AYGI&t=139), [02:34](https://www.youtube.com/watch?v=g59AM_8AYGI&t=154), [02:38](https://www.youtube.com/watch?v=g59AM_8AYGI&t=158)]:

* **Step 1 — Endpoints par function ki values check karein:**
* $f(2) = -9$ (**negative**) [[02:49](https://www.youtube.com/watch?v=g59AM_8AYGI&t=169), [02:59](https://www.youtube.com/watch?v=g59AM_8AYGI&t=179)]
* $f(4) = 29$ (**positive**) [[03:03](https://www.youtube.com/watch?v=g59AM_8AYGI&t=183), [03:07](https://www.youtube.com/watch?v=g59AM_8AYGI&t=187)]
* Signs opposite hain ($-9$ aur $+29$), is liye interval valid hai [[03:13](https://www.youtube.com/watch?v=g59AM_8AYGI&t=193), [03:58](https://www.youtube.com/watch?v=g59AM_8AYGI&t=238)].


* **Step 2 — Midpoint nikalein:**
* $\text{Midpoint} = \frac{2 + 4}{2} = 3$ [[03:45](https://www.youtube.com/watch?v=g59AM_8AYGI&t=225), [04:13](https://www.youtube.com/watch?v=g59AM_8AYGI&t=253)]


* **Step 3 — Midpoint par $f(x)$ ki value nikalein:**
* $f(3) = 27 - 27 + 1 = 1$ (**positive**) [[04:18](https://www.youtube.com/watch?v=g59AM_8AYGI&t=258), [04:29](https://www.youtube.com/watch?v=g59AM_8AYGI&t=269)]


* **Step 4 — Naya interval banayein (Opposite signs rule):**
* Nayi value $f(3) = +1$ (positive) aayi hai [[05:06](https://www.youtube.com/watch?v=g59AM_8AYGI&t=306)].
* Ab pichli values mein se **negative** wali value ($f(2) = -9$) uthayein ge [[05:16](https://www.youtube.com/watch?v=g59AM_8AYGI&t=316), [05:24](https://www.youtube.com/watch?v=g59AM_8AYGI&t=324)].
* Naya interval ban gaya $[2, 3]$ [[05:30](https://www.youtube.com/watch?v=g59AM_8AYGI&t=330)].


* **Step 5 — Repeat (Iterations):**
* $[2, 3]$ ka midpoint $\frac{2+3}{2} = 2.5$ aaya, phir $f(2.5) = -5.875$ (negative) [[05:49](https://www.youtube.com/watch?v=g59AM_8AYGI&t=349), [06:11](https://www.youtube.com/watch?v=g59AM_8AYGI&t=371)].
* Ab negative ($2.5$) ke saath positive ($3$) ka interval $[2.5, 3]$ banega, aur ye cycle chalta rahega [[06:54](https://www.youtube.com/watch?v=g59AM_8AYGI&t=414), [07:15](https://www.youtube.com/watch?v=g59AM_8AYGI&t=435)].
* Video mein aage midpoints $2.75$, $2.875$, $2.9375$, aur $2.96875$ aate hain aur $2.9$ ke qareeb stop kar diya jata hai [[07:28](https://www.youtube.com/watch?v=g59AM_8AYGI&t=448), [09:04](https://www.youtube.com/watch?v=g59AM_8AYGI&t=544), [10:22](https://www.youtube.com/watch?v=g59AM_8AYGI&t=622), [11:28](https://www.youtube.com/watch?v=g59AM_8AYGI&t=688), [11:45](https://www.youtube.com/watch?v=g59AM_8AYGI&t=705)].



---

### Sabse Zaroori Baat (Shortcut Rule)

Har naye midpoint par $f(\text{mid})$ nikalne ke baad:

1. Agar answer **minus** aaye $\rightarrow$ is naye midpoint ko pichle **plus** wale point ke saath pair karein [[06:54](https://www.youtube.com/watch?v=g59AM_8AYGI&t=414)].
2. Agar answer **plus** aaye $\rightarrow$ is naye midpoint ko pichle **minus** wale point ke saath pair karein [[05:06](https://www.youtube.com/watch?v=g59AM_8AYGI&t=306), [05:20](https://www.youtube.com/watch?v=g59AM_8AYGI&t=320)].

Kya aapko **naya interval choose karne** wale part mein zyada uljhan ho rahi hai, ya **calculation/midpoint** wale hisse mein?

28-nov-2026
