---  
tags:  
  - math  
  - FLA  
categories: FLA  
share: true  
lev: 3  
---  
  
  
# Table of Contents  
  
- [[The Basics in FLA#Alphabet:|Alphabet:]]  
- [[The Basics in FLA#String:|String:]]  
	- [[The Basics in FLA#String:|Empty String:]]  
	- [[The Basics in FLA#String:|Length of Strings:]]  
	- [[The Basics in FLA#String:|Concatenation of Strings:]]  
- [[The Basics in FLA#Powers of an Alphabet:|Powers of an Alphabet:]]  
- [[The Basics in FLA#Language:|Language:]]  
- [[The Basics in FLA#Operations on Language:|Operations on Language:]]  
	- [[The Basics in FLA#Operations on Language:|Union:]]  
	- [[The Basics in FLA#Operations on Language:|Concatenation:]]  
	- [[The Basics in FLA#Operations on Language:|Power and Closure:]]  
  
  
# The Basics in FLA  
  
## Alphabet:  
  
An ***alphabet*** is a **finite**, **nonempty** set of symbols (usually denoted $\Sigma$ ), eg.  
  
- English alphabet: $\Sigma=\{a,b,\ldots,z\}$.  
- Binary alphabet: $\Sigma=\{0,1\}$.  
  
## String:  
  
A ***string*** is a **finite** sequence of symbols chosen from some alphabet.  
  
### Empty String:  
  
Empty string is the string with zero occurrence of symbols (usually denoted $\epsilon$ ). It is a string that can be chosen from any alphabet.  
  
### Length of Strings:  
  
Number of occurrences of symbols in a string, eg. $|010|=3$, $|\epsilon|=0$.  
  
### Concatenation of Strings:  
  
Set $x=a_1a_2\ldots a_n$ and $y=b_1b_2\ldots b_m$, then define $xy:=a_1a_2\ldots a_nb_1b_2\ldots b_m$. Some properties of concatenation for example:  
  
- $x(yz)=(xy)z$.  
- $\epsilon x=x\epsilon$.  
- $|xy|=|x|+|y|$.  
  
## Powers of an Alphabet:  
  
If $\Sigma$ is an alphabet, define $\Sigma^k$ to be the set of all strings of length $k$ from it.  
  
Note that the set of all strings over $\Sigma$ is: ($*$ closure)  
  
$$\Sigma^*=\bigcup\limits_{i=0}^\infty \Sigma^i=\Sigma^0\cup \Sigma^1\cup \Sigma^2\cup\cdots$$  
  
The set of all nonempty strings over $\Sigma$: ($+$ closure)  
  
$$\Sigma^+=\bigcup\limits_{i=1}^\infty \Sigma^i=\Sigma^1\cup \Sigma^2\cup \Sigma^3\cup\cdots$$  
  
We have $\Sigma^*=\Sigma^+\cup\{\epsilon\}$.  
  
## Language:  
  
If $\Sigma$ is an alphabet and $L\subseteq \Sigma^*$, then $L$ is a ***language*** over $\Sigma$. In other words, $L$ is an arbitrary set of strings from $\Sigma$ (can be empty!). The language $\emptyset$ and $\{\epsilon\}$ are not the same language!  
  
## Operations on Language:  
  
Set $L$, $M$ to be languages on $\Sigma$.  
  
### Union:  
  
$$L\cup M=\{w|w\in L\lor w\in M\}$$  
  
### Concatenation:  
  
$$L\cdot M=\{w_1w_2|w_1\in L\land w_2\in M\}$$  
  
### Power and Closure:  
  
$$L^k=\begin{cases}\{\epsilon\},&k=0\\L^{k-1}L,&k\geq 1\end{cases}$$  
  
$$L^*=\bigcup\limits_{i=0}^\infty L^i=L^0\cup L^1\cup L^2\cup\cdots$$  
  
$$L^+=\bigcup\limits_{i=1}^\infty L^i=L^1\cup L^2\cup L^3\cup\cdots$$  
  
---  
Ahead:  
- [[./Context-Free Grammar|Context-Free Grammar]]