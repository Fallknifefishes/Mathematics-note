### Mixed products
> [!Definition] Definition: Mixed product
> Give vectors $\vec{a}$, $\vec{b}$ and $\vec{c}$, the mixed product is defined to be $\vec{c}.(\vec{a} \times \vec{b}).$
> Let $[\vec{a},\vec{b},\vec{c}]$ denote $\vec{c}.(\vec{a} \times \vec{b}).$

This has geometric meaning. By the definition of cross products, $|\vec{a} \times \vec{b}|$ represents the **area of the parallelgram** with $\vec{a}$ and $\vec{b}$ as the two sides
 $\vec{c}.(\vec{a} \times \vec{b})$ then takes $\vec{c}$ and resolve in the direction **the perpendicular to the plane OAB**. in other words, the **height** of the parallelepiped with $\vec{a}$, $\vec{b}$ and $\vec{c}$ as the three non-parallel sides. This value is multiplied by the base area, give **volume of the parallelpiped**.

 
![[Pasted image 20260504164321.png]]

> [!Thm] Geometric interpretation of mixed product
> The value of $[\vec{a}, \vec{b}, \vec{c}]$ is the signed value of the **parallelpiped** formed with $\vec{a}$, $\vec{b}$ and $\vec{c}$ as the three non-parallel sides.

This meaning that any shift the the mixed product does **not change the actual value**, but only the sign. In fact, we have the following theorem

> [!Thm] Theorem 1.1
> For any **cyclic shifts** of the mixed product, the signs are preserved;
> $[\vec{a}, \vec{b}, \vec{c}] = [\vec{c}, \vec{a}, \vec{b}]= [\vec{b}, \vec{c}, \vec{a}]$ 
> And for any **non-cylic shifts**, the signs negates.

> [!proof]
> Left as an exercise


 Anothor application (very commen in step) is to use mixed product to proof thing are (or aren't) coplaner.

If $\vec{a}$ , $\vec{b}$ and $\vec{c}$ are on the same plane, then the parallelpiped formed has area 0. Conversly, if the parallelpiped has area 0, then they have to be on the same plane. Hence
> [!Thm] Theorem 1.2 
> $\vec{a}$ , $\vec{b}$ and $\vec{c}$ are on the same plane if and only if $[\vec{a}, \vec{b}, \vec{c}] = 0$

### BAC-CAB identity

We have the following identity 
> [!thm] BAC-CAB identity
> For $\vec{a}$, $\vec{b}$ and $\vec{c}$
> $\vec{a} \times (\vec{b} \times \vec{c}) = (\vec{b}(\vec{a}.\vec{c}) - \vec{c}(\vec{a}.\vec{b}))$

**Proof**
Let $\vec{d} =\vec{a} \times (\vec{b} \times \vec{c})$ . Then $\vec{d} \perp \vec{a}$ and $\vec{d} \perp (\vec{b} \times \vec{c})$

Hence $\vec{d}$ is coplaner with the plane $BOC$. We can then write $$
\vec{d} = x\vec{b} + y \vec{c}
$$
For scalar $x$ and $y$.  And therefore $$
\vec{a}.\vec{d} = x \vec{b} \vec{a} + y \vec{a} \vec{c} = 0
$$
Hence $\frac{x}{\vec{a}\vec{c}} = - \frac{y}{\vec{b} \vec{a}} = \lambda$ for some value of $\lambda$.  This $\lambda$ is universally constant.

## Plane equation