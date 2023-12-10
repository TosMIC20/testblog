---  
tags:  
  - physics  
  - electromagnetism  
lev: 4  
categories:  
  - University Physics  
  - Electromagnetism  
share: "true"  
---  
  
  
# Table of Contents  
  
- [[Capacitors#Definition|Definition]]  
- [[Capacitors#Capacitance|Capacitance]]  
- [[Capacitors#Common capacitors|Common capacitors]]  
	- [[Capacitors#Common capacitors|Parallel plates capacitor]]  
	- [[Capacitors#Common capacitors|Coaxial cable]]  
- [[Capacitors#Capacitor Energy|Capacitor Energy]]  
  
  
# Capacitors  
  
## Definition  
  
A ***Capacitor*** is a pair of conductors. Usually it's 2 conductors, but in some cases the other one may be at $\infty$.  
  
## Capacitance  
  
The ***capacitance*** $C$ of a capacitor is defined to be the ratio of the charge on **each** of the conductor of a capacitor and the potential difference between them. Take the sign potential difference to make $C$ positive.  
  
> $$C=\frac{Q}{\Delta V}.$$  
  
  
For a special case, consider a charged sphere shell with radius $R$ . Another conductor is at infinity, so:  
  
$$  
C=\frac{Q}{\Delta V}=\frac{Q}{\frac{1}{4\pi \varepsilon_0}\frac{Q}{R}}=4\pi \varepsilon_0 R.  
$$  
>[!INFO] Why is $C$ well-defined?  
>You may argue that, the definition of capacitance is correct only when $\Delta V$ is proportional to $Q$, but is this true for any two conductors?  
>  
> [[./The Uniqueness Theorem|The Uniqueness Theorem]] could help us out.  
  
What is the relation between the uniqueness theorem and our intended conclusion $\Delta V\propto Q$ ?   
  
Now consider a capacitor. Assume that conductors have charge $\vec{Q}$, where the $i$-th coordinate of $\vec{Q}$ is the charge on $i$-th conductor, and for capacitor, $|Q_i|=Q$. The charge density function on each conductor surface is $\sigma_i$, and we write $\vec{\sigma}$ in the same way.  
  
Consider the volume surrounded by the conductors (may be infinite). The potential difference between two conductor surface is given by the electric field. The uniqueness theorem tells us that electric field is determined by $\vec{Q}$.   
  
Consider a charge density $k\vec{\sigma}$, assume that it corresponds to charge $\vec{Q}'$.  
$$  
Q'_i=\oint_{S_i}k\sigma_idS_i=k\oint_{S_i}\sigma_idS_i=kQ_i.  
$$  
Thus $\vec{Q}'=k\vec{Q}$. The uniqueness theorem tells us that the electric field with $k\vec{Q}$ is unique. It must corresponds to the field given by $k\vec{\sigma}$. Since:  
$$  
\Delta V=\sum\oint_{S_i}\frac{\sigma_i}{\|\vec{x}-\vec{r}\|}dS_i.  
$$  
We know that:  
$$  
\Delta V'=\sum\oint_{S_i}\frac{k\sigma_i}{\|\vec{x}-\vec{r}\|}dS_i=k\sum\oint_{S_i}\frac{\sigma_i}{\|\vec{x}-\vec{r}\|}dS_i=k\Delta V.  
$$  
Therefore, we have arrived at what we want.  
  
## Common capacitors  
  
Now that we know that $\Delta V\propto Q$ for any capacitors. The coefficient is only decided by shape, which is the meaning of capacitance. Let's take a look at the capacitance of some common capacitors.  
  
*From now on, for the sake of simplicity, we will write $V$ in place of $\Delta V$ for potential difference between conductors of a capacitor.*  
  
### Parallel plates capacitor  
  
Consider two parallel plates, one of them has charge $Q$, another has $-Q$, and they both has area $A$. Put them at a distance $d$ from each other.  
  
For small enough $d$, we can approximate the electric field with that of infinitely large plates. Thus, the electric field between two plates are constant, and equals to $\frac{\sigma}{\varepsilon_0}$. And the potential difference will be $\frac{\sigma d}{\varepsilon_0}=\frac{Qd}{A\varepsilon_0}$. Thus:  
$$  
C=\frac{Q}{V}=\frac{\varepsilon_0 A}{d}.  
$$  
  
### Coaxial cable  
  
Coaxial cable consists of two concentric conductor pipes with radii $a<b$. They have charge $Q$ and $-Q$. The length $L$ is much larger than $b$, so we can approximate its electric field as if it's infinitely long.   
  
Then we can use Gauss' law. It can be easy drawn that the electric field is always perpendicular to the axis. The strength $E$ is a function of distance $r$ to the axis:  
$$  
E=  
\begin{cases}  
0, &r>b,\\  
\frac{\lambda}{2\pi\varepsilon_0 r},&a\leq r\leq b,\\  
0,&0\leq r<a.  
\end{cases}  
$$  
Where $\lambda=\frac{Q}{L}$. Then:  
$$  
\displaystyle V=\left|\int_a^b\pm \frac{\lambda}{2\pi\varepsilon_0 r}dr\right|=\frac{\lambda}{2\pi\varepsilon_0}\ln\frac{b}{a}.  
$$  
And we have:  
$$  
C=\frac{Q}{V}=\frac{2\pi\varepsilon_0 L}{\ln\frac{b}{a}}.  
$$  
  
## Capacitor Energy  
  
In terms of capacitor energy, let's assume that we have two neutral plates. How many work is needed to move an amount of charge $Q$ from one conductor to another, to make one charged $Q$, and another charged $-Q$.   
  
In terms of 1 conductor capacitor, let's consider moving charges from infinity to it.  
  
Consider an intermediate state, where the potential difference between two conductors is $V_q$, and we intend to move $dq$ charge from one to another. The work needed will be $V_qdq$. Thus the total work is given by:  
$$  
W=\int_0^QV_qdq=\int_0^Q\frac{q}{C}dq=\frac{1}{C}\int_0^Qqdq=\frac{Q^2}{2C}.  
$$  
This is true for any capacitor.   
  
An understanding for $\frac{1}{2}$ there is think of $W=\frac{Q^2}{2C}=\frac{1}{2}QV$. Think of what we derived in the discussion of [[./Electric Potential#Electric Field Energy|electric field energy]]. The capacitor is a special case for continuous distribution, which is a generalization from sum to integral.  
  
*Try calculate with energy density, and find out why the integration zone can be within the two plates.*  
  
---  
Ahead:  
- [[./Dielectrics|Dielectrics]]