
> [!Definition] Partition of a Set
> Let $A$ be a finite set, $A_i$, $i=1, 2, ... , n$ has the property that $A_{i} \cap A_{j}= \emptyset$ and $\cup_{i=1}^n A_{i} = A$, then $A_{1}, A_{2} ,\dots, A_{n}$ is a partition of A

Essentially, for every element $a \in A$, $a \in A_{i}$ for a **unique** $i$.  In other words, we are assigning the *colour* to every element in $A$

This allows us to have the following equality
$\sum_{x\in A} x = \sum_{i=1}^n \sum_{x \in A_{i}}x$

The equality says that **we can sum elements in $A$ in any order we desire**

> How to prove partition?

If we have $A_{i}'s$ such that $\cup_{i=1}^n A_{i} = A$, then all we have to do it to prove disjoint. Assume not, if there exist $i, j$ such that $A_i$ has common element with $A_j$, then what happens.....

> Trick

For any set $A$, one **common partition is**, partitioning $A$ into *the parts that are in $B$,* and *the parts that are not in $B$ *  