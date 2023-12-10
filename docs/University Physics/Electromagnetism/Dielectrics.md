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
  
- [[Dielectrics#Introduction|Introduction]]  
- [[Dielectrics#Dipole theory of dielectrics|Dipole theory of dielectrics]]  
- [[Dielectrics#Modified Gauss' law|Modified Gauss' law]]  
  
# Dielectrics  
  
## Introduction  
  
What are dielectrics? ***Dielectrics*** are basically insulators, characterized by lack of free-moving charge.  
  
Experiment showed that, when you plug in dielectrics between a parallel plate capacitor, its capacitance changes. Moreover, it changes by a constant ratio for the same dielectric. That is:  
$$  
C=\kappa C_0.  
$$  
  
And for all dielectrics, $\kappa>1$.   
  
Meantime, the strength of electric field also changes:  
$$  
E=\frac{1}{\kappa}E_0.  
$$  
To explain this phenomenon, dipole theory is introduced.  
  
[[./Electric Dipole|Electric Dipole]]  
  
## Dipole theory of dielectrics  
  
This theory is basically viewing the dielectrics as a bunch of dipoles. In an electric field, dipole is tended to align with the electric field. However, not all of them will align with the electric field, because of thermodynamic factor.  
  
Taking into account all the factors, we consider a not too small, but not too large volume $\Delta V$ in dielectrics. The volume is not too small, so we can still take average in statistical mechanics. It's not large, so we can do integrals, and we define the ***polarization density*** $\vec{P}$ to be:  
$$  
\vec{P}=\lim_{\Delta V\to 0}\frac{\sum\vec{p}}{\Delta V}.  
$$  
Where $\sum\vec{p}$ is the sum of dipole momentum in that volume. Although we write limit, but the $\Delta V$ should not actually go to $0$.  
  
For *isotropic* materials, empirical results show that, the polarization density is proportional to external electric field, which is:  
$$  
\vec{P}=\varepsilon_0\chi_e \vec{E}_{ext}.  
$$  
$\chi_e$ is called ***electric susceptibility***.  
  
Now we can take into account the influence of these dipoles. Let's consider every dipole chunk as an independent dipole. Assume that we can use the approximation:  
$$  
V(\vec{x})=\frac{1}{4\pi\varepsilon_0}\frac{(\vec{x}-\vec{r})\cdot\vec{p}}{\|\vec{x}-\vec{r}\|^3}.  
$$  
Where $\vec{r}$ is the location of this dipole chunk, then the influence would be:  
$$  
V'(\vec{x})=\frac{1}{4\pi\varepsilon_0}\int_{\mathcal{V}}\frac{(\vec{x}-\vec{r})\cdot\vec{P}}{\|\vec{x}-\vec{r}\|^3}dV.  
$$  
Set $\vec{\eta}=\vec{x}-\vec{r}$, and $\eta=\|\vec{x}-\vec{r}\|$ now we use a trick. Notice that $\vec{\nabla}(\frac{1}{\eta})=\frac{\vec{\eta}}{\eta^3}$, and:  
$$  
\vec{\nabla}\cdot\left(\frac{1}{\eta}\vec{P}\right)=\vec{\nabla}\left(\frac{1}{\eta}\right)\cdot\vec{P}+\frac{1}{\eta}\left(\vec{\nabla}\cdot\vec{P}\right).  
$$  
We know that:  
$$  
\begin{aligned}  
V'(\vec{x})  
&=\frac{1}{4\pi\varepsilon_0}\int_{\mathcal{V}}\vec{\nabla}\left(\frac{1}{\eta}\right)\cdot\vec{P}dV\\  
&=\frac{1}{4\pi\varepsilon_0}\left(\int_{\mathcal{V}}\vec{\nabla}\cdot\left(\frac{1}{\eta}\vec{P}\right)dV-\int_{\mathcal{V}}\frac{1}{\eta}\left(\vec{\nabla}\cdot\vec{P}\right)dV\right)\\  
&=\frac{1}{4\pi\varepsilon_0}\left(\int_{\partial\mathcal{V}}\frac{1}{\eta}\vec{P}\cdot d\vec{S}+\int_{\mathcal{V}}\frac{1}{\eta}\left(-\vec{\nabla}\cdot\vec{P}\right)dV\right).  
\end{aligned}  
$$  
Think about it yourself that the first term is equivalent to a surface charge $\sigma'=\vec{P}\cdot\hat{n}$ on $\partial\mathcal{V}$ (where $\hat{n}$ is unit outward pointing normal vector), and the second term is equivalent to a charge density $\rho'=-\vec{\nabla}\cdot\vec{P}$ in $\mathcal{V}$. Also, you can verify it that the same is true for calculation of electric field.  
  
Thus, the effect of $\vec{P}$ can be think of these two parts. $\sigma'$ are called *induced surface charge density*, and $\rho'$ are called *induced volume charge density*.  
  
Moreover, if we have $\vec{P}=\varepsilon_0\chi_e \vec{E}_{ext}$, then the change can be quantized. (Think of the reason that we use $\vec{E}$ to calculate $\vec{P}$, instead of $\vec{E}_0$)  
$$  
\begin{aligned}  
\vec{E}  
&=\vec{E}'+\vec{E}_0\\  
&=\frac{\chi_e}{4\pi}\left(\int_{\partial\mathcal{V}}\frac{\vec{\eta}}{\eta^3}\vec{E}\cdot d\vec{S}+\int_{\mathcal{V}}\frac{\vec{\eta}}{\eta^3}(-\vec{\nabla}\cdot\vec{E})dV\right)+\vec{E}_0\\  
&=\frac{\chi_e}{4\pi}\left(\int_{\partial\mathcal{V}}\frac{\vec{\eta}}{\eta^3}(-\frac{\sigma}{\varepsilon_0})dS+\int_{\mathcal{V}}\frac{\vec{\eta}}{\eta^3}(-\frac{\rho}{\varepsilon_0})dV\right)+\vec{E}_0\\  
&=-\chi_e \vec{E}+\vec{E}_0.  
\end{aligned}  
$$  
Thus,  
$$  
\vec{E}=\frac{1}{\chi_e+1}\vec{E}_0.  
$$  
We define $\varepsilon_r=\chi_e+1$ to be the ***relative permittivity*** of the dielectric. Associating this with the formula at the very beginning, we know $\kappa=\varepsilon_r$.  
  
## Modified Gauss' law  
  
In the presence of dielectrics, the original Gauss' law needs to be modified. In terms of isotropic dielectrics, we know that $\vec{E}=\frac{1}{\varepsilon_r}\vec{E}_0$, so we can directly modify it:  
$$  
\oint_A\vec{E}\cdot d\vec{A}=\frac{Q_{in}}{\varepsilon_0\varepsilon_r}=\frac{Q_{in}}{\varepsilon}.  
$$  
Where $\varepsilon=\varepsilon_0\varepsilon_r$ is called ***permittivity*** of the dielectric.  
  
In general, we can define ***electric displacement*** $\vec{D}=\varepsilon_0\vec{E}+\vec{P}$. Since:  
$$  
\begin{aligned}  
\rho&=\rho_0+\rho'\\  
\varepsilon_0\vec{\nabla}\cdot\vec{E}&=\varepsilon_0\vec{\nabla}\cdot\vec{E}_0-\vec{\nabla}\cdot\vec{P}\\  
\vec{\nabla}\cdot\vec{D}&=\varepsilon_0\vec{\nabla}\cdot\vec{E}_0.  
\end{aligned}  
$$  
We have:  
$$  
\begin{aligned}  
\oint_A\vec{D}\cdot d\vec{A}&=\int_V \vec{\nabla}\cdot\vec{D}dV\\  
&=\varepsilon_0\int_V\varepsilon_0\vec{\nabla}\cdot\vec{E}_0dV\\  
&=\varepsilon_0\oint_A\vec{E}\cdot d\vec{A}\\  
&=Q_{in}.  
\end{aligned}  
$$  
  
This formula:  
$$  
\oint_A\vec{D}\cdot d\vec{A}=Q_{in},  
$$  
is true for any setup, no matter how complicated the system is, how many dielectrics there are, whatever charge distribution it is, and for any surface $A$.  
  
$\vec{D}$ has no actual physical meaning, but it's useful in calculations.  
  
## Energy  
  
Let's take a look at what happens when you put a dielectric into a capacitor. The energy before is $\frac{1}{2}CV^2$, after putting in the dielectric, it becomes $\frac{1}{2}C'V'^2=\frac{1}{2\kappa}CV^2$ (here set $Q=Constant$).   
  
Since $\kappa>1$, the energy has dropped! Where has it gone?   
  
Actually, when you insert a dielectric, it will be subject to a force exerted by the plates, which drags it in.   
  
Let's recall [[./Electric Dipole#The electric force on dipole|electric force on dipole]], there are force on dielectric if the electric field is not constant, and there are so called *fringe effect* which says that at the edge of a capacitor, the electric field is not constant.   
  
There's actually a formula of force on the dielectrics in an electric field. It can be given by:   
$$  
\vec{F}_V=(\vec{P}\cdot\vec{\nabla})\vec{E}.  
$$  
Where $\vec{F}_V$ is force in a unit volume.