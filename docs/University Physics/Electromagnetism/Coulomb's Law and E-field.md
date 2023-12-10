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
  
- [[Coulomb's Law and E-field#Coulomb's law|Coulomb's law]]  
	- [[Coulomb's Law and E-field#Coulomb's law|Notes]]  
- [[Coulomb's Law and E-field#E-field|E-field]]  
	- [[Coulomb's Law and E-field#E-field|Notes]]  
	- [[Coulomb's Law and E-field#E-field|E-field lines]]  
  
# Coulomb's Law and E-field  
  
## Coulomb's law  
  
The force between 2 point charges:  
  
> $$\vec{F}_{12}=\frac{1}{4\pi \varepsilon_0}\frac{q_1q_2}{r^2_{12}}\hat{r}_{12}.$$  
  
### Notes  
  
- $\hat{r}$ (read r-hat) is the unit vector pointing from $q_1$ to $q_2$.  
- $q_1$ and $q_2$ are signed.  
- $\varepsilon_0\overset{\sim}{=} 8.854\times 10^{-12}\:\mathrm{C^2/N\cdot m^2}$ is called the *permittivity* of free space. It is defined with the speed of light, which will be discussed in later notes.   
- Write $k=\frac{1}{4\pi\varepsilon_0}$ for simplicity, and it has value ~$8.988\times10^9\:\mathrm{N\cdot m^2/C^2}$.  
  
If there are more than two charges, the ***principle of superposition*** applies, which means:  
  
$$  
\vec{F}=\sum_{i=1}^N\vec{F}_i=\frac{q}{4\pi\varepsilon_0}\sum_{i=1}^N\frac{q_i}{r_i^2}\hat{r}_i.  
$$  
  
For continuous charge distribution, the sum becomes integral:  
  
$$  
\vec{F}=\frac{q}{4\pi\varepsilon_{0}}\int\frac{dq}{r^{2}}\hat{r}.  
$$  
  
The integral is a vector integral. In principle, you should integrate for $F_x$, $F_y$ and $F_z$. But in practice, the problems always contain some sort of symmetry, which will simplify the calculation.  
  
*The charge is quantized, why we can take integral?*   
  
## E-field  
  
The ***electric field*** at a point is defined as follows:  
  
> $$\vec{E}=\lim_{q_0\to0}\frac{\vec{F}}{q_0}.$$  
  
### Notes  
  
The calculation of E-field is similar as above.  
  
### E-field lines  
  
Electric field lines are continuous lines in space constructed in the following way:  
  
1. Lines start and terminate **only** on charges, never in empty space.  
2. Lines originate on and run outward from **positive** charges. They terminate on and run toward **negative** charges.  
3. The **tangent** to the field line at each point specifies the **direction** of the electric field $\vec{E}$ at that point.  
4. The **density** in space of the electric field lines around a particular point is proportional to the **strength** of the electric field at that point.  
5. Lines are parallel in a small enough region.  
6. Two field lines never cross. (why?)  
  
---  
Ahead:  
- [[./Ex of E-field Calculations|Ex of E-field Calculations]]  
- [[./Electric Dipole#Classic dipole|Classic Electric Dipole]]  
