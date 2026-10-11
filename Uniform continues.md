> [!definition] Uniform continues
> A function $f : A \to B$ is uniformly continues iff $\forall \epsilon>0$, $\exists \delta >0$ such that $\forall x, y\in A$, $|x-y|<\delta$, there is $|f(x)-f(y)|<\epsilon$

If we compare the definition of *pointwise continues*
> [!Definiton] Pointwise continues
> $f:A\to B$ is pointwise continues at $c$ iff $\forall \epsilon>0$, $\exists \delta>0$ such that $\forall x \in (c-\delta, c+\delta)$ we have $|f(x)-f(c)|<\epsilon$

The only different is the fixed point $c$ is changed to a variying point $y$. 
In *UC*, the value of $\delta$ is only dependent on $\epsilon$ and $A$, whereas in *PC*, It is also dependent on $c$.

So, *UC* ensures that given a $\epsilon$, there is a close enough distance $\delta$ which restricts the whole domain. Whereas PC only restrict the point $c$ on discussion.


> [!Theorem] Sequential characterisaion of non-uniform continues
> A function $f: A\to B$ is non-uniform continues on $A$ iff there exists $\epsilon_{0}>0$ and sequences $(x_{n}), (y_{n}) \subset A$ such that $|x_{n} - y_{n}|\to 0$ and $|f(x_{n}) - f(y_{n}) | \ge \epsilon_{0}$ for all $n \in \mathbb{N}$.

> "Suffice" of a domain means that the output of the $x$'s in the small domain is not further then given $\epsilon$

Intuition: Uniform continues says that 'for any given small output, one can find a small input space which suffice in all of $A$'
This is basically saying 'Exists $\epsilon_{0}$ (an output range), there is a range which does not suffice in $A$.'

