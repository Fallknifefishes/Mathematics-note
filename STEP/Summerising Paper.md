
## 2021 Step 2

### Q 1
*Trigger*: The hinted formula $\cos a\cos 3a= \frac{1}{2}(\cos 4a + \cos 2a)$. 
*What does it do*: This turns **multiplication** into **summation** and change the angle.

*Crux:* Not really, the difficulty is uniformly distributed. **only point** is a factorisation trick: Keep trying.
 
*Trap:* Messy thinking.  May incorrectly count root/miss root

*Takeaway:* 
1. When counting the root of **trig**, or things in general. **Draw a diagram** to prevent messy working.
2. Wen factorising, 1. Check previous work and think '**does this definitly factorise**'. 2. It it does, KEEP trying.

### Q 2
Trigger: Symmetry. Thing in the form of $a+b$, $a^2+b^2$, $a^3 + b^3$. We can process using Vieta.

*Crux:* Veita Veita Veita
 
 Trap: Aritgmetic slip 
 
*Takeaway*: Recognise Vieta


### Q 3

Trigger: [x] is an integer and {x} is positive

*Crux:* Be careful about cases

*Trap:* Arithmetic slip

*Takeaway:* Slow and clear arithmetic working

### Q 4 
revisit

Trigger: Looking at the graph of $xe^x$ 

*Crux*: Relate functions to the desired form (i.e **substitution to solve equation**)

*Trap:* Ensure the substitution is **bijective**, and be carful about the **values x can take(domain)** and the **values y can take (range)**

*Takeaway*:* Method of **relating, and solving equations by varible substitution.** When substituting, ensure the value which the new varible can take generates all the possible values old varible can take. And **bijectivity** (if not at least some kind of relations)

### Q 5

Trigger: Just Sub

Crux: Sub correctly 

Trap: Don't make mistake

Takeaway: Do arithmetic slowly and *ensure to get all easy marks*

### Q 6
Trigger: Just math

Crux: Read and understand 

Trap: Read and understand PROPERLY

Takeaway: STEP problem are not that hard if you READ properly. And think NEATLY. And
> [!Theorem] Conservation of difficulty
> Very wordy problems and lengthy problems tend to be simple, and a part of it's difficulty is converted into reading and length



### Q 7

Trigger: Equating entries of the matrix

Crux: **Repeatedly applying a formula**

Trap: Arithmetic slip, and computational slip (Especially when matracies is involved)

Takeaway: Write with clearity 

### Q 8
Ez


## 2021 STEP 3

### Q 1
Trigger: Copying the instructed, use the formula $$
d=\frac{|ax_{0}+by_{0}+c|}{\sqrt{ a^2+b^2 }}
$$
To work out that the perpendicular distance to the normal line from $(0,0)$ is always $1$. This means that 'maybe' the independent curve is a circle. 
Try to varify....

Crux: Don't make mistake and things work out fine 

Trap: ez

Takeaway: No rushing (even im behind). Think clearly.

### Q 2
Trigger: **Learn and summerise** from the previous part.

Crux: Apply the 'summery' of the previous parts. (i.e What (i) did was using determinant=0 to obtain an equality) so for (ii), one needs to satisfy det = 0. 

Trick!! : We need to prove, for positive integers $a, b \text{ and } c$
$$
\frac{a}{b+c}+\frac{c}{a+b}+\frac{b}{c+a} \ge 1
$$

We can see that $$
\frac{a}{b+c}+\frac{c}{a+b}+\frac{b}{c+a}\ge\frac{a}{b+c+a}+\frac{c}{a+b+c}+\frac{b}{c+a+b} \ge 1
$$
The idea is **making the denominator the same so that fractions can be summed**
Or 
**exploiting symmetry**
##### **Symmetry!!!!!!!!!!**


### Q 3
Trigger: Hinted process by (i)

Crux: Two main points
1. Seek for what needed. In 'following tutorial' problems, **seek for whats needed** instead of strictly following 
2. Compare with $0$ whenever you can.
- When comparing sizes, a good thing to do is **make one side zero or constant**, it is way harder to try to compare the size of two changing varible.
Trap: Unable to think of the crux.

Takeaway: The general idea of '**making one side constant**'. And **think with flexibility**.

### Q 4
Trigger: bro just understand the problem

Crux: expand things well and think clearly
Trap: **a** and **b** are fuckin unit vectors
	for the record i ignored this condition and wasted 5 minutes on it and got mad so blew my nose really hard, trying to blame my reading issues on hayfever and got an nosebleed 
		never do that again. Always be calm in a step exam


Takeaway: Fuck hayfever aint going to effect me.


### Q 5
Polar curve scetch is a scam


### Q 6
Trigger: Oberve the form of the given function $$
f_{a}(x) = \tan^{-1}(\frac{x\tan \alpha+1}{\tan \alpha-x})
$$
This looks crazily similar to the **double angle formula of tan** but the other way around.

$$
\tan(a\pm b) = \frac{\tan a \pm \tan b}{1\mp \tan a \tan b}
$$
With $a=\alpha$ and $b=\tan^{-1}x$
Therefore $f_{a}(x) = \tan^{-1}(\cot(\alpha-\tan^{-1}x ))$
Using 奇变偶不变，符号看象限。we can say that $\cot(t)=\tan\left( \frac{\pi}{2}-t \right)$
So $$
f_{a}(x) = \tan^{-1}(\cot(\alpha-\tan^{-1}x )) = \tan^{-1}(\tan{(\frac{\pi}{2}-\alpha+\tan^{-1}x)})
$$
Crux: Realising this identity

Note : $\tan(\arctan x)= x$ holds for all x but $\arctan(\tan x) = x$ only hold for $x\in \left( -\frac{\pi}{2}, \frac{\pi}{2} \right)$ and more generally $\arctan(\tan x) = x+k\pi$

Trap: The ones who did not spot this transformation cant do it. **And $\sqrt{x^2}=|x|$ for god sake!**

Takeaway: 
1. I should be able to spot a path under 3 min after understanding the problem. If not, the i'm probabily missing things from earlier. So look back. **think about. 1: hinted methods 2: SUS structure and relations. 3: Clarify goals and conditions** 
2. Be **very sensitive about structures**