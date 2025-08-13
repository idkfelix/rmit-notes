## The Bijection Rule
- A bijection is where every element in one set matches up to one of every element in another set
- The bijection rule says that if there is a bijection from one set to another then the two sets have the same cardinality
- Let $S$ and $T$ be two finite sets. If there is a bijection from $S$ to $T$ then $|S|=|T|$
## The $k$-to-$1$ Rule
- The $k$-to-$1$ rule shows that one element in a set corresponds to $k$ elements in another set, such as two shoes from a set to each person in another set
- A $1$-to-$1$ correspondence is another term for a bijection
- Let $X$ and $Y$ be finite sets. The function $f:X\rightarrow{Y}$ is a $k$-to-$1 correspondence if for every $y\in{Y}$, there are exactly $k$ different $x\in{X}$ such that $f(x)=y$
- Suppose there is a $k$-to-$1$ correspondence from a finite set $A$ to a finite set $B$, then $|B|=|A|/{k}$
## The Product Rule
- The product rule provides a way to count sequences using the product of each sets cardinality instead of the cardinality of the product of all the sets
- $$$|D\times M \times S|=|D|\cdot |M|\cdot |S|=2\cdot 2\cdot 3=12$$
## The Generalised Product Rule
- The generalised product rule states that in selecting an item from a set, if the number of choices at each step does not depend on previous choices made, then the number of items in the set is the product of the number of choices in each step.
- A set of $S$ of sequences of $k$ items where there are $n_1$ choices for the first item: 
	- For any choice of first item, $n_2$ choices are available for the second item
	- For any choice of first and second item, $n_3$ choices are available for the third
	- $\dotsb$
	- For any choice for the first $k-1$ items,  the $k^\text{th}$ item has $n_k$ choices available
- This describes the following implementation of the generalised product rule:
	- $\large{|S|=n_{1} \cdot n_{2} \cdot \dots n_{k}}$
## $n$ Choose $r$ Notation
- There is a dedicated formula for counting subsets that has its own notation and terminology called "$n$ choose $r$ notation"
- $$
\begin{gathered}
\small\text{The number of ways of selecting an }r\text{-subset from a set of size }n\text{ is:}\\\\
{n \choose r} =  \frac{n!}{r!(n-r)!}\\\\
\small{n \choose r} \text{ is read as "n choose r". The notation }C(n,r)\text{ is sometimes used for }{n \choose r}\\\\
\small\text{Additionally } r \text{ in } {n\choose{r}} \text{ can be replaced with } n-r \text{ to create }{n\choose{n-r}} \\\\
{n\choose{n-r}}=\frac{n!}{(n-r)!(n-(n-r))!}=\frac{n!}{(n-r)!r!}={n\choose{r}}
\end{gathered}
$$
- An equation is called an **identity** if the equation holds for all values for which the expressions in the equation are well defined
- The equation ${n\choose{r}}={n\choose{n-r}}$ is an identity because the equality holds for any non-negative integer $n$ and any integer $r$ in the range $0\dots{n}$ 
- An Identity means that for any set $S$ with $n$ elements, the number of $r$-subsets from $S$ is equal to the number of $(n-r)$-subsets from $S$
