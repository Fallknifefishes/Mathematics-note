### Problem 1
> [!example] Problem 1
![[Pasted image 20260506164828.png]]
##### Partial solution
We first translate the conditions
$LM \perp PQ \iff l-m = ki (p-q)$ for some real number $k$

The points are on the same circle, means that they have the same modulus, and hence
$\bar{l}l = \bar{m}m = \bar{p} p = \bar{q}q = a^2$, where $a$ is the radium of the circle [[Understanding Analysis]]

> [!thinkingprocess]  thought process
> Aim: We **want** expressions concerning ml and pq.
> Problem: We now have **conjuates**, so how do we deal with them?
> Take conjugates both side of $l-m = ki (p-q)$ to generate another expression with conjugate, and see how these two link 

> [!bug] Why I had no thoughts
> When I was doing the problem, I though of the condition $l-m = ki (p-q)$, and I spotted the problem of involvement of complex number. Did not move on from there.

> [!Success] What should I improve?
> What can I do better.
> 1. Read all of the problem without missing condition. I could of read $\bar{l}l = \bar{m}m = \dots$ condition and had a inspirations
> 2. Do try to **activly analyse** the problem instead of hiding away. (ie ask **how to deal with the k and $i$**)


Taking conjugate both side of $l-m = ki (p-q)$, we obtain $\bar{l}-\bar{m} = -ki (\bar{p}-\bar{q})$

> [!Thinkingprocess] thought process 
> There are three (essentially two) conditions, and we want to **link** the conditions in some way thats **Losses lest infomation(as it should be if and only if)**
> 
 > Maybe its good to get rid of $k$ somehow? Trying: Multiplying or dividing the two expressions does nothing. 
 > 
> We need to use the **length condition**. Otherwise the (amount of) information is insufficient to prove desired condition.
> 
> We could use the length condition to link the structures $l-m$ and $\bar{l} - \bar{m}$ together 

$ml \bar{l} = la^2$ and $m l \bar{m} = ma^2$, Subtracting the two, we obtain 
$$ml(\bar{l} - \bar{m})=a^2 (l-m)$$

By similar process 
$$pq(\bar{p}-\bar{q})= a^2 (q-p)
$$
And rest is ez~

> [!example] Problem 2
> ![[Pasted image 20260509182511.png]]

The key point to this problem is to identify(or work out) the centre of $\omega$
First if we substitute $z =\frac{1}{\bar{\omega}}$, we get the equation 
$$
(|a|^2 - r^2)\bar{\omega}\omega - a \omega - \bar{a}\bar{\omega} + 1 = 0
$$
Our **aim** is to prove the locus of $\omega$ is a circle, and find it's centre. ***looking back***

We have shown that if **some z** satisfies 

$$\bar{z}z - \bar{a}z - a\bar{z} + a \bar{a} - r^2= 0 (1)$$

Then the locus of $z$ is a circle with centre  $a$ and radius $r$ . 

Then maybe we can use this for $w$, and find some $a'$, $r'$ in which $w$ satisfies (1), notice that (1) is monic. So we divide by $|a|^2 - r^2$. Resulting in.

$$
\bar{\omega}\omega - \frac{a}{|a|^2 - r^2} \omega - \frac{\bar{a}}{|a|^2-r^2}\bar{\omega} + \frac{1}{|a|^2-r^2} = 0
$$

Then compare the coefficients, let $a' = \frac{\bar{a}}{|a|^2 - r^2}$, and so on. Things work out fine.
> [!thoughtprocess] Reflection
> In this question, to inspire the key step, we must
> 1. have a very good appreciation of what the first part mean. Maybe translate in words if stuck Translate in the stucture of **condition** leading to **property**.
> 2. In further sections, look at the **property derived above** and see and any approach can be inspired.
> 3. Have a **versatile** understanding. (1) does not only hold for $z$, but for **any complex number in general.** Even if **this complex number** $\omega$ is a transformation of $z$.

> [!success] To improve
> Think about whether a condition holds for **all**, or for **certain**. If for **all**, what is the most requiring and infomation rich thing that you could plug in.
> View conditions in a **versatile** manner.
> (e.g) $\cos(a e^x) = \cos(e^b e^x)$ for $a>0$.







## Methods of Complex number 
> [!method] Conjugates
> These are very fun! They have the following property
### 1 Conjugates

For complex numbers $w$ we have 
$$
|w|^2 = w \bar{w}
$$
So the **conjugate** and **modulus** of complex numbers are linked. Further, this links **complex numbers** to **real numbers**
Especially, if $w$ has unit length, then 
$$
\frac{1}{w} = \bar{w}
$$
Another very fun property is that, the complex numbers are **automorphic** (whatever that means). 
$$
(wz)^{*} =w^{*}z^{*}
$$
$$
(\frac{w}{z})^{*} = \frac{w^{*}}{z^{*}}
$$
$$
(w\pm z)^{*} = w^{*}\pm z^{*}
$$

### 2 Arguments

let $arg(z)$ denote the arguement of complex number $z$, then 
$$
arg( \frac{z}{w}) = arg(z)-arg(w)
$$

this $arg(z)$ can take any value, not $mod (2\pi)$

And 
$$
arg(z^{*}) = -arg(z)
$$
### 3
When $LM \perp PQ$, and let complex number $l$ denote $L$ on the plane, the rest adapting similar definition. Then 
$$
l-m = k i (p-q)
$$

### 4
When the points $P, Q, R, S$ are cyclic, (similarlly let $p$ denote the complex number which represents $P$, and rest the same). Then 
$$
\frac{\frac{r-s}{r-p}}{\frac{q-s}{q-p}}\in \mathbb{R}
$$



