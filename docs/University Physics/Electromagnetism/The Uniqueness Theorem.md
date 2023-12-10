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
  
- [[The Uniqueness Theorem#The Theorem|The Theorem]]  
- [[The Uniqueness Theorem#Proof|Proof]]  
  
# The Uniqueness Theorem  
  
## The Theorem  
  
> **The Uniqueness Theorem**  
>  
> Consider a volume $V$ containing charge distribution $\rho$ (may be infinite). If $\partial V$ are all conductor surface, then the electric field is **uniquely** determined if the charge on each conductor is given.  
  
## Proof  
  
Suppose that there are two fields $\vec{E}_1$, $\vec{E}_2$ satisfying the conditions. Then in volume $V$:  
  
$$  
\vec{\nabla}\cdot\vec{E}_1=\vec{\nabla}\cdot\vec{E}_2=\rho.  
$$  
  
Assume that $\partial V$ is made up of conductor surfaces $S_i$, that is, $\partial V=\sum S_i$. Assume that $S_i$ has charge $Q_i$.  
  
$$  
\oint_{S_i}\vec{E}_1\cdot d\vec{A}=\oint_{S_i}\vec{E}_2\cdot d\vec{A}=\frac{Q_i}{4\pi\varepsilon_0}.  
$$  
  
Now consider an electric field $\vec{E}_3=\vec{E}_1-\vec{E}_2$. It's indeed an electric field, as long as you negate $\rho_2$ and add it to $\rho_1$. $\vec{E}_3$ will obey that in $V$:  
  
$$  
\vec{\nabla}\cdot\vec{E}_3=0,  
$$  
  
on $S_i$:  
  
$$  
\oint_{S_i}\vec{E}_3\cdot d\vec{A}=0.  
$$  
  
Now there's a trick, consider $\vec{\nabla}\cdot(V_3\vec{E}_3)$, where $V_3$ is the potential of $\vec{E}_3$, with arbitrary zero potential points.  
  
$$  
\vec{\nabla}\cdot(V_3\vec{E}_3)=V_3(\vec{\nabla}\cdot\vec{E}_3)+\vec{E}_3\cdot(\vec{\nabla}V_3)=-(E_3)^2.  
$$  
  
And consider:  
  
$$  
\int_{V}\vec{\nabla}\cdot(V_{3}\vec{E}_{3})d\tau=\oint_{\partial V}V_{3}\vec{E}_{3}\cdot d\vec{A}=-\int_{V}(E_{3})^{2}d\tau.  
$$  
  
But consider the middle one. On each conductor surface $V_3$ must be constant (This comes from $V_1$ and $V_2$ are constant.), thus:  
  
$$  
\begin{aligned}  
\oint_{\partial V}V_{3}\vec{E}_{3}\cdot d\vec{A}  
&=\sum\oint_{S_i}V_{3}\vec{E}_{3}\cdot d\vec{A}\\  
&=\sum V_{3}\oint_{S_i}\vec{E}_{3}\cdot d\vec{A}\\  
&=0.  
\end{aligned}  
$$  
  
Thus:  
  
$$  
\int_{V}(E_{3})^{2}d\tau=0.  
$$  
  
What does this mean? The integral of a non negative function is zero, which means that   
  
$$  
\vec{E}_3\equiv 0.  
$$  
  
This means that $\vec{E}_1$ and $\vec{E}_2$ are the same field. Q.E.D.  
