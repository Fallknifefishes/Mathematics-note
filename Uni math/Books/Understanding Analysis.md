
# Chapter 1: The Real Numbers

> [!Definition] Definition: Sets
> Sets are a collection of objects

> [!thm] Theorem 1.1
> $x \in A\cup B \text{  if and only if } x\in A \text{ or } x \in B$
> $x \in A\cap B \text{  if and only if } x\in A \text{ and } x \in B$

> [!definition] Definition: Function
> Given two sets $A$ and $B$, a function $f$ takes each $x \in A$ and maps it to a **unique** element in $B$, denoted by $f(x)$ .
> $A$ is the **domain** of $f$ and $B$ is the **codomain**. The set formed by the values of $f(x)$ is called the **image set, or range**.
> The image set is a **subset** of the codomain.

## 1.1 Axiom of Completeness 
> **Axiom of Completeness**. Every nonempty set of real numbers that is bounded above has a least upper bound.

Below we introduce the mathematcial definition of bounded. 


> [!Definition] Definition: Upper Bounds and Supremum 
> Let $A \subseteq \mathbb{R}$ be a nonempty set.
> - The set $A$ is **bounded above** if there exists a number $b \in \mathbb{R}$ such that $a \le b$ for all $a \in A$. The number $b$ is called an **upper bound**  for $A$.
> - A real number $s$ is the **least upper bound**  or **supremum** (上确界) for $A$ (denoted by $s = \sup A$) if it meets two conditions:
>   1. $s$ is an upper bound for $A$.
>   2. If $b$ is any upper bound for $A$, then $s \le b$.

> [!Definition] Definition: Lower Bounds and Infimum 
> Let $A \subseteq \mathbb{R}$ be a nonempty set.
> - The set $A$ is **bounded below** if there exists a number $l \in \mathbb{R}$ such that $l \le a$ for all $a \in A$. The number $l$ is called a **lower bound**  for $A$.
> - A real number $i$ is the **greatest lower bound** or **infimum** for $A$ (denoted by $i = \inf A$) if it meets two conditions:
>   1. $i$ is a lower bound for $A$.
>   2. If $l$ is any lower bound for $l$, then $l \le i$.

Another equivalent (though more frequently used version) is stated below

> [!thm]  Lemma 1.1.1: Alternative Characterization of Supremum
> Assume $s \in \mathbb{R}$ is an upper bound for a set $A \subseteq \mathbb{R}$. Then, $s = \sup A$ if and only if, for every $\epsilon > 0$, there exists an element $a \in A$ such that $s - \epsilon < a$.

**Intuition:** The AoC ensures that they are no 'gaps' in the real number line. It garentees $SupA$ or $Inf(A)$ exists in $\mathbb{R}$ given a real bounded set $A$. 
As a *mathematical tool*, it **proves existance.** 
	More specifically, if we want to prove $s$ exists, then we can construct a sequence $(a_{n})$ which (is known to us) to have $\sup a_{n} = s$, and so $s$ exists.


> [!NOTE] Archimedean Property
> For any real number $x$ and $y$, there exists a natural number $n$ such that $nx>y$

**Intuition**: What the Archimedean Property ensures is that there are no real 'infinitly large or small'. However large $y$ is and however small $x$ can be, a finite $x$ can surpass $y$.

Tigger/summary: System with AP mean the *finite sum of arbitrarly small number can be arbitrarily large (in the system).*

> **Counterexample**: If we consider the system of fractional polynomials with $x$ tending to infinity. We can have $\frac{2x^3 +6x-4}{7x^3+1} = \frac{2}{7}$, however $1+1+1 \dots^\text{n times} = n <x$ for every $n$, hence in this system AP does not hold. (sum of finite small number cannot be arbitrarily large).
>*What breaks it?* There is a '*infinitly large*' number in this system, namely $x$.




## 1.2 Consequences of Completeness

> [!Theorem] Theorem 1.2.1 (Nested Interval Property)
> For each $n \in \mathbb{N}$, define the closed interval $I_n = [a_n, b_n] = a_n\leq x \leq b_n$ be non-emply intervals satisfying the following 
> $$
> I_{1} \supseteq I_{2} \supseteq I_{3} \dots \supseteq I_{n} \dots
> $$
> Then $\cap_{n=1}^\infty I_{n} \neq \emptyset$

> This is a consequence of AoC. For a solid stick (the complete real number system), no matter how small you go, there has to be somthing left.
> Sketch of proof: Let $s = sup(a_{n})$, show that $s\in I_{n}$ for every $n \in \mathbb{N}$.


**Remark 1:** If $I_{n} = (a_{n}, b_{n})$ is open, and $sup(a_{n})<inf{({b_{n}})}$, then the NIP still hold.
**Remark 2:** If $|I_k|$ is can be arbitrarily small, then $\cap_{n=1}^\infty I_{n} = s$ for a single element $s$

## 1.3 Cantor's theorem

> [!NOTE] Definition
> The sets $A$ and $B$ are said to have the same cardinality if there exists bijective function $f$ from $A$ to $B$ 
> $$
> f: A \rightarrow B
> $$

 **Intuition**: Method to compare of size in infinite setting. 'if there exists a bijective mapping between set, then they are equivalant in size'.


> [!NOTE] Theorem (Schroder-Bernstein Theorem)
> For sets $X$ and $Y$, if there exist a injective mapping $g:X\rightarrow Y$ and an injective mapping $h : Y\rightarrow X$. Then $X\sim Y$ ($X$ and $Y$ have the same cardinality)


**Idea of the proof:**
Due to injectivity, an element can only be mapped by at most one element (or non) from the opposing set by the injective function. For $x \in X$, we can trace up the element that is mapped to it by the function in $Y$, and repeat the process until it ends (or never end), therefore;
 For every element $x \in X$ and $y \in Y$, they fall into the following $4$ cases;
 	1. Part of the $x$-origin chain; Tracing up, it's chain ends in an element in $X$
 	2. Part of the $y$-origin;
 	3. Part of a loop; The tracing up repeats itself in loops
 	4. Part of an infinite chain
 For each of these $4$ parts, they are internally bijective, and hence $X$ and $Y$ has the same cardinality.


# Sequence and Series

> [!NOTE] Definition (Convergence)
> A sequence $(a_{n})$ is said to converge to a limit $L$ if 
> $\forall \epsilon >0, \exists N \in \mathbb{N} \text{ such that } \forall n> N \text{ we have } |a_{n}- L|<\epsilon$
> We write $\lim_{ n \to \infty } a_{n} = L$

> Intuition: This is essentially a translation of 'for any small number we can image, the distance between the sequence and the limit is smaller then the number'.


> [!NOTE] $\epsilon$ - Neighbourhood
> For the parametre $\epsilon>0$, the $\epsilon$ - Neighbourhood of a point $x$ is the interval $V_{\epsilon}(x) = (x-\epsilon, x+\epsilon)$

> [!NOTE] Topological definition of convergence
> A sequence $(a_{n})$ converges to $L$ if and only if for each $\epsilon>0$, only a **finite number** of terms is outside of $V_{\epsilon}(x)$


---

> [!NOTE] Algebraic limit theorem 
> **Given** $\lim_{ n \to \infty } a_{n} = a$ and $\lim_{ n \to \infty }b_{n} = b$
> Then
> 1. $\lim_{ n \to \infty } ca_{n} = ca$ for all $c\in \mathbb{R}$
> 2. $\lim_{ n \to \infty } (a_{n} \pm b_{n}) = a\pm b$
> 3. $\lim_{ n \to \infty }a_{n}b_{n} = ab$
> 4. $\lim_{ n \to \infty } \frac{a_{n}}{b_{n}} = \frac{a}{b}$ provided $b \neq 0$

All of these can be proven by **unpacking and packing limits** using the $\epsilon -N$ language.

It is saying that, given limit of $(a_{n})$ and $(b_{n})$ **exist**, they behave normally under basic algebra.


> [!NOTE] Order limit theorem
> Given $\lim_{ n \to \infty }a_{n}=a$ and $\lim_{ n \to \infty }b_{n} = b$.
> 1. If $a_{n}<b_{n}$ for all $n \in \mathbb{N}$, then $a\leq b$
> 2. If there exists $c \in \mathbb{R}$ for which $c\leq b_{n}$ for all $n \in N$, then $c\leq b$
> Similarlly when we swich $\leq \rightarrow \ge$

**What does it say?**
Limit of a sequence respects size properties of finite terms

**Idea linked with it:** An $\epsilon$ of room.
When we want to study $(x_{\infty}, S_{\infty})$ or $(x_{0}, S_{0})$, we first study $(x_{n}, S_{n})$ for $(x_{\epsilon}, S_{\epsilon})$ and for every $n$ and $\epsilon$ and push $


---

> [!NOTE] Monotone Convergence Theorem (MCT)
> If a sequence $(a_{n})$ is monotonically increasing (decreasing) and has an upper (lower) bound, then it converges. $\lim_{ n \to \infty } a_{n}$ exists.

**Idea of proof:** We say that, by **AOC**, $L = \sup(a_{n})$ is the limit of $(a_{n})$. **For every** $\epsilon>0$, **there exists** $N$ such that $L-\epsilon < a_{N}$. Because monotonic, **for all**  $n>N$, we have $a_{n}> a_{N}$, so $L-\epsilon < a_{n}$ and hence $|L-a_{n}| = L-a_{n} < \epsilon$. Which goes in to the box of definition of convergence. 

 > **Intuition**: If one continues to 'step up', and has a ceiling, then it must stop/tend to somewhere 

> **trigger:** When the proof of convergence is needed, monotone and bounded are given (Or can be interpreted).

> **Idea:** 
> Because we study the infinite process, a finite term of an infinite process does not matter that much (ie it is very easy to control). So we can have the following version.

> [!NOTE] MCT but slightly stronger
> If a sequence $(a_{n})$ is **eventually** monotonically increasing (decreasing) and has an upper (lower) bound, then it converges.  $\lim_{ n \to \infty } a_{n}$ exists.


Here, eventually means there **exist a (finite)** $N$ such that **for all** $n>N$ we have $a_{n}$ is monotonic.

> Analysis studies the behaviour of **thing approaching infinity**, so if a behaviour  is only limited to finite amount of terms, it can be **controlled** or **diluted** though infinite behaviour, so is *shouldn't matter much*

---

> [!NOTE] Definition (Boundedness of sequence)
> A sequence $(a_n)$ is said to be **bounded** if and only if there exists $M > 0$ such that $\forall n \in \mathbb{N}$ we have $|a_{n}| < M$

> [!NOTE] Bolzano-Weierstrass theorem
> Every bounded sequence has a convergent subsequence

**Idea of the proof:**  Given $(a_{n})$ is bounded, we have infinite terms in the interval $[-M, M]$. Therefore at least one of $[-M, 0]$ and $[0, M]$ contains infinite terms of $(a_{n})$, pick that and name it $I_{1}$. WLOG it is $[0, M]$, we repeat the process, at least one of $[0, \frac{M}{2}]$ and $[\frac{m}{2}, M]$ contains infinite terms of $(a_{n})$, pick that and define it to be $I_{2}$. Repeat the process and get $I_{3}$, $I_{4}$ and so on. Since $I_{k} \supseteq I_{k+1}$ is satisfies for all $k$, because $I_{k}$ is getting arbitrarily small, by NIP, $\cap_{n=1}^{\infty} I_{n} = s$. 
We **pick** $a_{n_{k}} \in I_{k}$ for each $k$ and we can show that $(a_{n_{k}})$ converge to $s$ by the definition of convergence **using the arguement that $I_{k}$ is arbitrarily small** $a_{n_{k}}$ and $s$ are both in $I_{k}$.


> **Intuition**:  This is essentially pigeohole principle in approaching-infinity setting. Consider if we divide $[-M, M]$ into intervals length of $\epsilon$, at least one of the intervals will contain infinite terms. This holds for **each** $\epsilon>0$ and therefore, BW holds.


> [!NOTE] Cauchy sequence
> A sequence $(a_{n})$ is cauchy if $\forall \epsilon>0$, $\exists N \in \mathbb{N}$ s.t $\forall m>n>N$, we have $|a_{m}-a_{n}|<\epsilon$

So essentially cauchy sequence are infinitly close to eachother at infinitly. This look very converging (out of intuition), and so we have the following theorem


> [!NOTE] Lemma
> Cauchy sequence are bounded 

**Proof**: Choose $\epsilon = 1$ and there exist a $N$ such that for all $m$, $|a_{m} - a_{N}|<1$, because $N$ is finite, let $M = \max{|a_{1}|, |a_{2}|,\dots, |a_{N-1}|, |a_{N}+1|, |a_{n}-1|}$, and so for all $n \in \mathbb{N}$ we have $|a_{n}|\leq M$, hence $(a_{n})$ is bounded.

> **Core idea**
> Seporate infinite sequence in **two part**, one finite and one infinite. Controll infinite by **limit behaviours** and finite controll it self.
> As an example, $\lim_{ n \to \infty }(a_{n}) = l$, we can find $N$ such that for all $n>N$, $a_{n}$ is an epsilon room from $l$ (controlled infinite behaviour). And we take care of $a_1, a_2 ... a_N$ seporatly.





> [!NOTE] Theorem: Cauchy Criterion
> A sequence $(a_{n})$ converges if and only if it's a Cauchy sequence.

**Idea of the proof**
$\rightarrow$
The intuition behind this seems very obvious, if $(a_{n})$ converges, then it's forever stuck in the $\epsilon$ neighbourhood of the limit from some point forward, and so will the difference of terms past that point


$\leftarrow$
This way is a little bit harder, intuitionally, it makes sence, as for some point onward, the sequence will be stuck in the $\epsilon$ interval of some $a_{n}$. And so it should converge


The **problem** is, we do not have a **proposed limit** to proof it's convergence *(we have no idea what the limit is*). In this case, we use the **Bolzano-Weierstrass theorem** to argue that it's subsequence converge to a limit, and because **the other terms are eventuall very close to the subsequence**, they converge to the same limit

A **rigours proof** is just unpacking there idea into formal $\epsilon - N$ language and packing them again.

> **Tool:** This provides another way of showing a sequence is convergent without knowing  the limit. It converts the chain of 
> Want to proof convergence -> Propose a limit -> Show that $(a_{n})$ is eventually infinitly close to the proposed limit ($\epsilon -N$)
> 
> Which studies the relationship between **the term and the proposed limit**, to ;
> Want to proof convergence -> Study the relationship between terms -> Show that the terms of $(a_{n})$ gets arbitrarly close 
> If shift the focus from **a fixed limit (external to $a_{n}$ )** to **relationship between terms of $(a_{n})$ (Internal to $a_{n}$)** 

> **Trigger:** The **limit is unrelated or unguessable**


---
