---  
share: true  
lev: 3  
categories:  
  - FLA  
tags:  
  - math  
  - FLA  
---  
  
  
# Table of Contents  
  
- [[Regular Expr & Lang#Regular Language|Regular Language]]  
- [[Regular Expr & Lang#Regular Expression|Regular Expression]]  
	- [[Regular Expr & Lang#Regular Expression|The language of RE]]  
- [[Regular Expr & Lang#Algebraic Laws for RE|Algebraic Laws for RE]]  
	- [[Regular Expr & Lang#Algebraic Laws for RE|Basic laws:]]  
		- [[Regular Expr & Lang#Basic laws:|Associativity & commutativity]]  
		- [[Regular Expr & Lang#Basic laws:|Identities & annihilators]]  
		- [[Regular Expr & Lang#Basic laws:|Distributive laws]]  
	- [[Regular Expr & Lang#Algebraic Laws for RE|Test for a RE algebraic law]]  
  
  
# Regular Expr&Lang   
## Regular Language  
  
>[!definition]  
>***Regular language (RL)*** on [[./The basic definitions in FL&A#Alphabet|alphabet]] $\Sigma$ is defined by induction:  
>- **Basis:**  
>   1. $\{\varepsilon\}$, $\emptyset$ are RL;  
>   2. For any $a\in\Sigma$, $\{a\}$ is RL;  
>- **Induction:** suppose $L$ and $R$ are RL:  
>  1. $L\cup R$ is RL;  
>  2. $L\cdot R$ is RL;  
>  3. $L^*$ is RL;  
  
## Regular Expression  
  
>[!definition]  
>***Regular expression (RE)*** on [[./The basic definitions in FL&A#Alphabet|alphabet]] $\Sigma$ is defined by induction:  
>- **Basis:**  
>   1. $\varepsilon$, $\emptyset$ are RE;  
>   2. Any $a\in\Sigma$ is RE;  
>   3. Any variable $L$ is RE.  
>- **Induction:** suppose $E$ and $F$ are RE:  
>  1. $E+F$ is RE;  
>  2. $EF$ is RE;  
>  3. $E^*$ is RE;  
>  4. $(E)$ is RE.  
  
>[!info]- The precedence of operators:  
>1. $*$  
>2. $\cdot$  
>3. $+$  
  
### The language of RE  
  
>[!definition]  
>Define the [[./The basic definitions in FL&A#Language|language]] of an RE on $\Sigma$ by induction:  
>- **Basis:**  
>   1. $L(\varepsilon)=\{\varepsilon\}$, and $L(\emptyset)=\emptyset$.  
>   2. For $a\in \Sigma$, $L(a)=\{a\}$.  
>- **Induction:** suppose $E$ and $F$ are RE:  
>  1. $L(E+F)=L(E)\cup L(F)$;  
>  2. $L(EF)=L(E)\cdot L(F)$;  
>  3. $L(E^*)=L(E)^*$;  
>  4. $L((E))=L(E)$.  
  
As you can see, there are some correspondence between RE and RL, in fact, you can define RL with RE:  
  
>[!definition]- **Alternative definition of regular language**  
>A language $R$ on $\Sigma$ is a regular language iff there exists a regular expression $E$ on $\Sigma$ such that $L(E)=R$  
  
## Algebraic Laws for RE  
  
The reason for the existence of variables in the definition of RE is that, RE gives us a specific structure, regardless of symbols used.  
  
Moreover, the structure remains true even if you substitute a symbol with a set of strings, that is, a language.  
  
>[!definition]   
>**Equivalence between REs:** suppose $E$ and $F$ are RE:  
>- If $E$ and $F$ don't contain variables, then we say $E=F$ iff $L(E)=L(F)$.  
>- If $E$ and $F$ contain variables, then $E=F$ iff whatever language we substitute for the variables in them, they represent the same language.  
  
>[!info]  
>You can skip to [[Regular Expr & Lang#Test for a RE algebraic law|Test for a RE algebraic law]] directly for more on equivalence between REs.  
  
### Basic laws:  
  
Suppose $L$, $M$ and $N$ are variables.  
  
#### Associativity & commutativity  
  
One can easily prove that:  
- $L+M=M+L$;  
- $(L+M)+N=L+(M+N)$;  
- $(LM)N=L(MN)$;  
  
#### Identities & annihilators  
  
- Identity: $\varepsilon$;  
- Annihilator: $\emptyset$;  
  
#### Distributive laws  
  
- $L(M+N)=LM+LN$;  
- $(M+N)L=ML+NL$.  
  
### Test for a RE algebraic law  
  
In our definition of equivalence between REs, we distinguished RE without variables and with variables, but now we are going to see that, you don't need to consider the latter case.  
  
>[!theorem]  
>If RE $E$ and $F$ have variables, substitute each variable with a single symbol from $\Sigma$ to get $C$ and $D$, then:  
>$$E=F\iff C=D.$$  
  
>[!proof]-  
>This theorem indeed comes from the fact that RE just represents a structure, let's start with a lemma which describes this.  
>>[!lemma]  
>>Set $E$ is an RE purely with variables $L_1,L_2,\ldots,L_m$. Substitute $L_i$ with $a_i\in\Sigma$ to get $C$. If we consider each variable $L_i$ to represent an arbitrary language $L_i$, then $w\in L(E)$ iff:  
>> - $\exists w_1,w_2,\ldots,w_k$, where $w_i\in L_{j_i}$, $s.t.\ w=w_1w_2\cdots w_k$.  
>> - Moreover, $a_{j_1}a_{j_2}\cdots a_{j_k}\in L(C)$.  
>  
>The proof is just structural induction, which is left as exercise : )  
>  
>The rest of the proof is trivial, try yourself : )  
  
