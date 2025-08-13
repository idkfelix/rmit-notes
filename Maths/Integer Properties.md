## The Division Algorithm
- The division algorithm is not an algorithm at all but a statement of mathematical fact.
- Let $x$ and $y$ be two integers. Then $x$ divides $y$ (denoted $x\mid{y}$ ) if and only if $x\neq{0}$ and there is an integer $k$ such that $y=kx$
- $x$ does not divide $y$ is denoted by $x\nmid{y}$ if $x$ divides $y$, then $y$ is said to be a multiple of $x$, and $x$ is a **factor** or **divisor** of $y$
- If a number $x$ divides two different numbers, $y$ and $z$, then $x$ divides any linear combination of $y$ and $z$. 
	- A **linear combination** of two numbers is the sum of multiples of those numbers. For example $3x-7y$ and $-2x+4y$ are both linear combinations of $x$ and $y$.
	- let $x$, $y$, and $z$ be integers. if $x\mid{y}$ and $x\mid{z}$, then $x\mid{(sy+tz)}$ for any integers $s$ and $t$
## Quotients and Remainders
- If $x$ does not divide $y$, then dividing $x$ is into $y$ results in a nonzero remainder. The division algorithm states that the result of the division (the **quotient**) and the **remainder** are unique.
- Let $n$ be an integer and let $d$ be a positive integer. Then, there are unique integers $q$ and $r$, with $0\le{r}\le{d-1}$, such that $n=qd+r$
- In the division algorithm, the number $q$ is called the **quotient**, and the number $r$ is called the **remainder**. The operations $\text{div}$ and $\text{mod}$ produce the quotient and the remainder as a function of $n$ and $d$
	- $q=n\,\text{div}\,d$
	- $r=n\,\text{mod}\,d$
- Most languages include the $\text{div}$ and $\text{mod}$ operations. Where $n$ is positive the result of $n\,\text{mod}\,d$ is straight forward, however if $n$ is negative, different languages may return different values
	- A language may return $-3$ for $-7\,\text{mod}\,4$. However the definition of the $\text{mod}$ operation according to the division algorithm requires that the result of $-7\,\text{mod}\,4$ be an integer in the range of $0$ through $3$
	- Since $-7=-2\cdot4+1$, the division algorithm says that $-7\,\text{div}\,4=-2$ and $-7\,\text{mod}\,4=1$
## Division Procedural Definition
$$
\begin{align*}
	&\text{Input: Integers}\,n\,\text{and}\,d\gt0\\
	&\text{Output: }q=n\,\text{div}\,d\,\text{and}\,r=n\,\text{mod}\,d\\\\
	
	&\text{Case 1}:n\lt0\\
	&q:=0\\
	&r:=n\\\\
	&\text{While}(r\lt{d})\\
	&\quad q:=q+1\\
	&\quad r:=r-d\\
	&\text{End-While}\\\\
	
	&\text{Case 2}:n\lt0\\
	&q:=0\\
	&r:=n\\\\
	&\text{While}(r\lt{d})\\
	&\quad q:=q-1\\
	&\quad r:=r+d\\
	&\text{End-While}\\\\
\end{align*}
$$
## Modular Arithmetic
- Given the set $\set{0,1,2,3,4}$, addition and multiplication are defined on the elements in this set in the usual way, except hat the $\text{mod}\,5$ function is applied afterwards to ensure that the result is again from $\set{0,1,2,3,4}$
- The operation defined by adding two numbers and applying $\text{mod}\,m$ to the result is called $\text{addition}\,\text{mod}\,m$. Similarly the operation defined by multiplying two numbers and applying $\text{mod}\,m$ to the result is called $\text{multiplication}\,\text{mod}\,m$
- The set $\set{0,1,2,\dots,m-1}$ with addition and multiplication $\text{mod}\,m$ defines a closed mathematical system with $m$ elements called a **ring**.
	- The ring $0,1,2,\dots,m-1$ with addition and multiplication $\text{mod}\,m$ is denoted by $\mathbb{Z}_m$
