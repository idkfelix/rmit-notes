## Functions
- A function $f$ that maps elements of a set $X$ to elements of a set $Y$ is a subset of $X\times{Y}$ such that for every $x\in{X}$, there is exactly one $y\in{Y}$ for which $(x,y)\in{f}$
- $f:X \rightarrow Y$ is the notation to express the fact that $f$ is a function from $X$ to $Y$
- The set $X$ is called the **domain** of $f$, and the set $Y$ is called the **target** of $f$. Another term for target is **co-domain**
- The fact that $f$ maps $x$ to $y$ (or $(x,y)\in{f}$) can also be denoted as $f(x)=y$
- If $f$ maps an element of the domain to zero elements or more than one element, then $f$ is not well-defined
## Function Properties
- A function is **one-to-one** or **injective** if $x_{1}\neq x_2$ implies that $f(x_1)\neq{f(x_2)}$. That is $f$ maps different elements in $X$ to different elements in $Y$
- A function is **onto** or **surjective** if the range of $f$ is equal to the target $Y$. That is for every $y\in{Y}$, there is an $x\in{X}$ such that $f(x)=y$
- Information about the sizes of the **domain** and **target** sets can be inferred based on whether the function is one-to-one or onto
	- if $f:D\rightarrow T$ is onto, then $|D|\geq{|T|}$
	- if $f:D\rightarrow T$ is one-to-one, then $|D|\leq{|T|}$
	- if $f:D\rightarrow T$ is a bijection, then the function is onto and one-to-one, which implies $|D|={|T|}$ 
## Range
- For function $f:X\rightarrow Y$, an element $y$ is in the range of $f$ if and only if there is an $x\in{X}$ such that $(x,y)\in{f}$
	- Range of $f=\set{y:(x,y)\in{f},\text{for some }x\in{X}}$
- The range of $f$ is a subset of the target, but not necessarily equal to the target.
- This can be found with an arrow diagram between the domain and target sets where any elements in the target set that do not have an arrow from the domain set are not included in the range
```tikz
\usepackage{tikz}
\usetikzlibrary{shapes.geometric,fit}
\begin{document}
\begin{tikzpicture}[scale=2.5]
    \foreach[count=\i] \lseti/\lsetmi in {X/{$w$,$x$,$y$,$z$},Y/{$a$,$b$,$c$,$d$}} {
        \begin{scope}[local bounding box=\lseti, x=2cm, y=0.5cm]
        \foreach[count=\j] \lj in \lsetmi {
            \node[minimum width=1em,anchor=base,text height=1.4ex,text
            depth=0.25ex] (n-\j-\lseti) 
            at (\i,-\j) {\lj};
        }
        \end{scope}
        \node[ellipse, draw, fit=(\lseti), 
        label={[name=l-\lseti]above:$\lseti$}] {};
    }
    \draw[->] (n-1-X) -- (n-4-Y);
    \draw[->] (n-2-X) -- (n-4-Y);
    \draw[->] (n-3-X) -- (n-1-Y);
    \draw[->] (n-4-X) -- (n-2-Y);
    \draw[->] (l-X) -- node[above]{$f$}(l-Y);
\end{tikzpicture}
\end{document}
```
## Floor & Ceiling Functions
- A **floor** function maps a real number to the nearest integer in the downward direction.
- $floor:\mathbb{R}\rightarrow\mathbb{Z}, \text{where }floor(x)=\text{the largest integer } y \text{ such that } t \leq x$
- Floor functions are common enough they have their own notation:
	- $floor(x)=\lfloor{x}\rfloor$
- The **ceiling** function rounds a real number to the nearest integer in the upward direction
- $ceiling:\mathbb{R}\rightarrow\mathbb{Z}, \text{where }ceiling(x)=\text{the smallest integer } y \text{ such that } t \leq x$
- The ceiling function also has its own notation:
	- $ceiling(x)=\lceil{x}\rceil$
## Absolute
- The absolute value of a real number is denoted with $|x|$, similarly to the cardinality of a set $|A|$
- The absolute value of a negative number drops the leading sign leaving just the positive value.
## Inverse Function
- If a function $f:X\rightarrow Y$ is a bijection, then the **inverse** of $f$ is obtained by exchanging the first and second entries in each pair in $f$.
	- The inverse of $f$ is denoted by $f^{-1}$ 
	- $f^{-1}=\set{(y,x):(x,y)\in{f}}$
- Reversing each pair in a function $f$ does not always result in a well defined function. Therefore, some functions do not have an inverse.
- A function $f:X\rightarrow Y$ has an inverse if and only if it is also **one-to-one** and **onto** which implies it is a **bijection**
## Composition of Functions
- $f$ and $g$ are two functions, where $f:X\rightarrow Y$ and $g:Y\rightarrow Z$. the composition of $g$ with $f$, denoted as $g \circ f$, is the function $(g\circ{f}:X\rightarrow Z)$, such that for all $x\in{X},(g\circ{f})(x)=g(f(x))$
- More than two functions can be composed. As composition is associative, the order in which one composes the functions does not matter:
	- $f\circ{g}\circ{h}=(f\circ{g})\circ{h}=f\circ(g\circ{h}))$
## The Exponential Function
- The exponential function $exp_b:\mathbb{R}\rightarrow \mathbb{R}^+$ is defined as:
	- $exp_b(x)=b^x$
- Where $b$ is a positive number and $b\neq1$. The parameter $b$ is referred to as the base of the exponent in the expression $b^x$, with $x$ being referred to as the exponent
- Properties of exponents:
	- $b^xb^y=b^{x+y}$
	- $(b^x)^y=b^{xy}$
	- $\frac{b^{x}}{b^{y}}=b^{x-y}$
	- $(bc)^{x}=b^xc^x$
## The Logarithm Function
- The logarithm function for a real number $b>0$ and $b\neq1$, $\log_b:\mathbb{R}^+\rightarrow \mathbb{R}$ is defined as:
	- $\large b^{x=y}\Leftrightarrow \log_{b}y=x$
- The parameter $b$ is referred to as the base of the logarithm in the expression
- Properties of logarithms:
	- $\log_b(xy)=\log_bx+\log_by$
	- $\log_b(\frac{x}{y})=\log_b{x}-\log_b{y}$
	- $\log_b(x^y)=y\log_b{x}$ 
	- $\log_c{x}=\frac{\log_b{x}}{\log_b{c}}\text{ where }c\neq1$
## Population Growth
- The growth of a population is often modelled mathematically by an exponential function:
	- $\large n=p\cdot{b^t}\Leftrightarrow\frac{n}{p}=b^t$
- The initial population size is represented by $p$, and after $t$ days the population will increase / decrease as described by some number $b$
- The prior equation is used to show how many days ($t$) it will take to reach a population size of $n$ from an initial population $p$ at a rate of $b$
- The value of $t$ in this equation is $\log_b{(\frac{n}{p})}$
- As this equation uses real numbers its result will almost always be approximate as the population size must be an integer