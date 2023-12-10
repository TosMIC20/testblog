---  
tags:  
  - physics  
  - thermodynamics  
lev: 4  
categories:  
  - University Physics  
  - Thermodynamics  
share: "true"  
---  
  
# Table of Contents  
  
- [[Thermodynamic Processes#Reversible and irreversible processes|Reversible and irreversible processes]]  
	- [[Thermodynamic Processes#Reversible and irreversible processes|Reversible process:]]  
	- [[Thermodynamic Processes#Reversible and irreversible processes|Irreversible process:]]  
	- [[Thermodynamic Processes#Reversible and irreversible processes|Characteristics:]]  
- [[Thermodynamic Processes#Three basic processes|Three basic processes]]  
	- [[Thermodynamic Processes#Three basic processes|Isobaric process]]  
	- [[Thermodynamic Processes#Three basic processes|Isochoric process]]  
	- [[Thermodynamic Processes#Three basic processes|Adiabatic process]]  
- [[Thermodynamic Processes#More on processes|More on processes]]  
	- [[Thermodynamic Processes#More on processes|Isothermal process]]  
	- [[Thermodynamic Processes#More on processes|Adiabatic process]]  
  
# Thermodynamic Processes  
  
## Reversible and irreversible processes  
  
### Reversible process:  
  
Thermodynamic variables vary sufficiently slowly such that approximate thermal equilibrium is always maintained. (Quasistatic process)  
  
### Irreversible process:   
  
Thermodynamic variables vary too fast and the system goes out of equilibrium, including so-called Spontaneous processes.  
  
### Characteristics:  
  
For a reversible process, the thermodynamic equations of state for the system never differ by more than an infinitesimal amount from those of the surroundings. eg.  
  
- reversible expansion: $P_{sys}=P_{surr}+dP$.  
- reversible compression: $P_{sys}=P_{surr}-dP$.  
  
In reversible processes, the thermodynamic variables **can** be returned to their original values by reversing the external conditions that caused the change.   
  
While in irreversible processes, the thermodynamic variables **cannot** be returned to their original values.  
  
Whenever you see a curve on $P$-$V$ graph, it must represent a **reversible** process. If the system is not in equilibrium, the pressure of the system is not well defined, so it cannot be represented by a dot on $P$-$V$ graph.  
  
*In our discussion afterwards, if not stated, we are always discussing reversible processes.*  
  
  
## Three basic processes  
  
>[!INFO]  
>The following analysis requires some content in note [[./Thermal Energy|Thermal Energy]] ([[./Thermal Energy#Thermal energy and heat|heat]], [[./Thermal Energy#Heat capacity|heat capacity]] and [[./Thermal Energy#Work|work]]) but not including [[./Thermal Energy#Internal energy|internal energy]].   
  
### Isobaric process  
  
We can carefully control the temperature and the volume of the gas during compression or expansion so that $\frac{dT}{T}=\frac{dV}{V}$ always stands, we will have $p$ as a constant:  
  
$(p+dp)(V+dV)=nR(T+dT)\implies dp\equiv0$.  
  
Under this condition:  
  
- Work: $\displaystyle W=\int_{V_1}^{V_2}pdV=p\Delta V$.  
- Heat flow: $\displaystyle dQ=C_pdT=\frac{C_pT}{V}dV=\frac{C_p}{nR}pdV=\frac{C_p}{nR}dW$, so $\displaystyle Q=C_p\Delta T=\frac{C_p}{nR}W$. (Assuming $C_p$ is constant.)  
  
### Isochoric process  
  
This is easy to understand, as long as we fix the size of the container, we can have such a process with $dV\equiv0$. In this case, we have $\frac{dT}{T}=\frac{dp}{p}$, so:  
  
- Work: $dW=pdV\equiv 0$, $W=0$.  
- Heat flow: $\displaystyle dQ=C_VdT=\frac{C_VT}{p}dp=\frac{C_VV}{nR}dp$, $\displaystyle Q=C_V\Delta T=\frac{C_VV}{nR}\Delta p$. (Assuming $C_V$ is constant.)  
  
### Adiabatic process  
  
A reversible process with no heat flow, ie. $dQ=0$.  
  
If there's no heat flow, work-energy theorem tells us that there's some sort of energy in the gas changing when work is being done. And that introduces [[./Thermal Energy#Internal energy|internal energy]].  
  
## More on processes  
  
>[!WARNING]  
>The following analysis requires [[./Thermal Energy#Internal energy|internal energy]].  
  
### Isothermal process  
  
In isothermal process, temperature is constant, thus $dU=0$.  
  
- Work: $\displaystyle W=\int_{V_1}^{V_2}pdV=\int_{V_1}^{V_2}\frac{nRT}{V}dV=nRT\ln\frac{V_2}{V_1}.$  
- Heat flow: $Q=W$.  
  
### Adiabatic process  
  
In order to better analyze it, we construct an isochoric path that has the same temperature change with the adiabatic process, so:  
  
$dU=-pdV=C_VdT$.  
  
According to $pV=nRT$, we have:  
  
$pdV+Vdp=nRdT$.  
  
Combine the two, we know that:  
  
$\displaystyle Vdp=nRdT-pdV=-\frac{nR}{C_V}pdV-pdV=-\frac{C_V+nR}{C_V}pdV=-\frac{C_p}{C_V}pdV$.  
  
We call $\gamma=\frac{C_p}{C_V}$ adiabatic index, and there are:  
  
$\displaystyle \frac{dp}{p}=-\gamma\frac{dV}{V}$.  
  
This gives $PV^\gamma=Constant$.  
  
Thus work done can be described by:  
  
$\displaystyle \begin{aligned}W=\int_{V_1}^{V_2}pdV&=\int_{V_1}^{V_2}\frac{p_1V_1^\gamma}{V^\gamma}dV\\ &=(\gamma-1)p_1V_1^\gamma(\frac{1}{V_1^{\gamma-1}}-\frac{1}{V_2^{\gamma-1}})\\ &=(\gamma-1)(p_1V_1-p_2V_2)\\ &=-(\gamma-1)nR\Delta T.\end{aligned}$  
  
The result is within expectation, since we defined internal energy to be work done in adiabatic process.  
  
---  
Ahead:  
- [[./Statistical Mechanics|Statistical Mechanics]]  
- [[./Heat Engines|Heat Engines]]