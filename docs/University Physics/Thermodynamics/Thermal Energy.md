---  
tags:  
  - physics  
  - thermodynamics  
lev: 4  
share: true  
categories:  
  - University Physics  
  - Thermodynamics  
---  
  
  
# Table of Contents  
  
- [[Thermal Energy#Thermal energy and heat|Thermal energy and heat]]  
- [[Thermal Energy#Heat capacity|Heat capacity]]  
- [[Thermal Energy#Work|Work]]  
- [[Thermal Energy#Internal energy|Internal energy]]  
	- [[Thermal Energy#Internal energy|Experiment]]  
	- [[Thermal Energy#Internal energy|Derivation]]  
- [[Thermal Energy#Relationship between 2 heat capacities|Relationship between 2 heat capacities]]  
  
# Thermal Energy  
## Thermal energy and heat  
  
Temperature is related to the internal energy or thermal energy of the thermal system.  
  
- A system can transfer its internal (thermal) energy by changing the temperature (or phase) of another system,   
- It can also use its internal energy to do mechanical work on its surroundings, or both.  
  
Heat is a kind of energy. Heat is not conserved but can be converted into other forms of energy. The thermal energy flow is called the heat flow $Q$.  
  
## Heat capacity  
  
Where $dQ$ is the heat flow required to bring about a temperature change $dT$ , defines the heat capacity $C$. In other words, $dQ=CdT$.  
  
- Specific heat capacity: the heat capacity of 1g of a specified material $c_g=C/m$,  
- Molar heat capacity: the heat capacity of 1 mole of a specified material $c_m=C/n$.  
  
## Work  
  
The work done by a thermal system on its environment is:  
  
$$  
dW=\vec{F}\cdot d\vec{x}=PAdx=PdV,  
$$  
  
so,  
  
$$  
W=\int_{V_1}^{V_2}PdV.  
$$  
  
Actually the $P$ here is only defined for reversible process. In reversible processes, $P_{sys}=P_{surr}\pm dP$, so whether in case the system does work on environment or the environment does work on the system, we can use $P_{sys}$ for calculation.  
  
In irreversible processes, $P_{sys}$ is not well defined, we can only use $P_{surr}$ for calculation.  
  
- In compression: $\displaystyle W_{irrev}=-\int_{V_s}^{V_l}P_{surr}dV$, and we know $P_{surr}>P_{sys}$, here $P_{sys}$ is the pressure of an **analogous** reversible process, so $W_{irrev}<W_{rev}$ (analogous reversible process).  
- In expansion: $\displaystyle W_{irrev}=\int_{V_s}^{V_l}P_{surr}dV$, and we know $P_{surr}<P_{sys}$, so $W_{irrev}<W_{rev}$ (analogous reversible process).  
  
So we always have $W_{irrev}<W_{rev}$, regardless of signs.  
  
*After learning this, let's go to [[./Thermodynamic Processes#Three basic processes|3 examples of thermaldynamic processes]].*  
  
## Internal energy  
  
In an [[./Thermodynamic Processes#Adiabatic process|adiabatic transformation]] a system has no thermal contact with its surroundings. There are only work done, it's actually a mechanic system. As stated above, we define this energy to be ***thermal energy*** (or ***internal energy***) $U$. So in adiabatic transformation $dU=-dW$, and $\Delta U=-W$.  
  
What about other processes, in other processes where $Q\ne 0$, can we establish a relationship between $U$ and $Q$, $W$ ? This introduces [[./The 1st Law of Thermodynamics|The 1st Law of Thermodynamics]].  
  
  
>[!WARNING]  
>The following discussion requires [[./The 1st Law of Thermodynamics|The 1st Law of Thermodynamics]].  
  
### Experiment  
  
In 1845, Joule performed an experiment to study the internal energy for ideal gas. He demonstrated that *for ideal gas, the internal energy is a function of temperature alone:* $U=U(T)$.   
  
His experiment is actually an adiabatic free expansion of gas. The experiment result showed that during the process, temperature doesn't change. Also, there's no work done nor heat flow, so $\Delta U=0$. But there's volume change, so $U$ must be independent of $V$.  
  
### Derivation  
  
In the analysis of isochoric process, we have $dW=0$ and $dQ=C_VdT$. Thus $dU=dQ-dW=C_VdT$, we have:  
  
$$U(T)=\int_0^TC_VdT+Constant.$$  
  
We just care about changes in $U$, so actually we can set the constant to zero.  
  
Furthermore, if $C_V$ is independent of temperature, then:  
  
$$U(T)=C_VT.$$  
  
## Relationship between 2 heat capacities  
  
In the analysis of isobaric process:  
  
$$dU=dQ-dW=C_pdT-pdV=C_pdT-nRdT.$$  
  
Combine this with isochoric process:  
  
$$dU=C_VdT.$$  
  
We know $C_VdT=(C_p-nR)dT$, which means:  
  
$$C_V=C_p-nR$$  
  
This result only applies to ideal gas. Actually it works in some real cases.  
  
*Why can we say that RHS of the two equations equal just because LHS is both $dU$? It's because $U$ is a state function! It's easy to construct an isochoric process and an isobaric process that both goes from $T_1$ to $T_2$.*  
  
---  
Ahead:  
- [[./Statistical Mechanics|Statistical Mechanics]]  
- [[./Heat Engines|Heat Engines]]