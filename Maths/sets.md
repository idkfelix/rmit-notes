## Common Sets
- $\mathbb{N}$ set of **Natural Numbers** / positive integers including $0$
- $\mathbb{Z}$ set of **All Integers** positive or negative including $0$
- $\mathbb{Q}$ set of **Rational Numbers** / real numbers that can be expressed as $\large\frac{a}{b}$
- $\mathbb{P}$ set of **Irrational Numbers** / real numbers that cannot be expressed as $\large\frac{a}{b}$
- $\mathbb{R}$ set of **All Real Numbers**
- $\emptyset$ is an empty set with **No Elements**
## Set Superscripts ($+ -$)
- Common sets can be used with a positive or negative superscript to only include the positive or negative elements of said set
- Neither positive sets or negative sets include the integer zero
	- $\mathbb{Z}^{+} = \set{1,2,3,4,\ldots}$ 
## Set Builder Notation
- Used to define a set that includes all elements in a larger set that also satisfy certain conditions.
- $A = \set{x \in S :P(x)}$ where $S$ is a larger set from which the elements of $A$ are taken given they satisfy the the condition $P(x)$.
- The $:$ symbols is read as "such that", hence the prior set builder reads as "all $x$ in $S$ such that $P(x)$".
- $S$ is often one of the common sets $\mathbb{N}\,\mathbb{Z}\,\mathbb{Q}\,\mathbb{P}\,\mathbb{R}$
	- $C=\set{x\in{\mathbb{Z}} : 0<x<100\text{ and }x\text{ is prime}}$
## Cardinality
- The cardinality of of a set is the number of distinct elements in said set
- This is denoted as $|A|$ for set $A=\set{1,1,2,3,4}$ and given the set only contains four distinct elements $|A|=4$
## Subsets & Proper Subsets
- A subset is a set of which all its elements can be found within another set
- $A\subseteq{B}$ indicates that $A$ is a subset of $B$ and if $A$ contains an element that's not found in set $B$ the opposite is indicated with $A\nsubseteq{B}$
- If $A\subseteq{B}$ and there is any element of $B$ that set $A$ does not contain, $A$ is considered to be a **Proper Subset** of $B$ and can be denoted as $A\subset{B}$
## Power Sets ($P(A)$)
- $2\in{A}$ shows that $2$ is an element in $A$
- A power set is a set created with the with the function $P(A)$ that contains all possible subsets of $A$ as elements.
- The cardinality of this set can be determined with  $2$ to the power of the input sets cardinality such that if $|A|=5$ then $|P(A)|=2^5$ 
- For Example $P(\set{1,2,3}) = \set{1,2,3,\set{1,2},\set{1,3},\set{2,3},\set{1,2,3},\emptyset}$
	- $\emptyset$ represents the empty subset of the input rather than $\set{}$
## Union and Intersection ($\cup \cap$)
- The **Intersection** of sets $A$ and $B$ is denoted as $A\cap{B}$ and forms a set of all elements that are elements of **both** sets $A$ and $B$
- The **Union** of sets $A$ and $B$ is denoted as $A\cup{B}$ and forms a set of all elements that are elements of sets $A$ or $B$. As elements in a set are unique an element in both sets will not be repeated
## Difference and Symmetric Difference ($-$ $\oplus$)
- The difference of set $A$ from set $B$ or $A-B$ shows all elements in set $A$ that are not in set $B$ or $\set{x:x\in{A}\text{ and }x\notin{B}}$
- The symmetrical difference of two set is denoted as $A \oplus B$ and combines both differences of the sets to create a set containing all elements in set $A$ or $B$ that are not contained in the other or $\set{x:x\in{A-B}\text{ or }x\in{B-A}}$
## Complement Sets ($\bar{A}$)
- The complement of set $A$ is all elements not contained within set $A$ , this operation is denoted as $\bar{A}$ and can be found with the builder $\set{x:x\notin{A}}$
## Set Identities
- ## Idempotent Laws
	- $A\cup{A}=A$
	- $A\cap{A}=A$
- ## Associative Laws
	- $(A\cup{B})\cup{C}=A\cup{(B\cup{C})}$
	- $(A\cap{B})\cap{C}=A\cap{(B\cap{C})}$
- ## Commutative Laws
	- $A\cup{B}=B\cup{A}$
	- $A\cap{B}=B\cap{A}$
- ## Distributive Laws
	- $A\cup{(B\cap{C})}=(A\cup{B})\cap{(A\cup{C})}$
	- $A\cap{(B\cup{C})}=(A\cap{B})\cup{(A\cap{C})}$
- ## Identity Laws
	- $A\cup{\emptyset}=A$
	- $A\cap{U}=A$
- ## Domination Laws
	- $A\cap{\emptyset}=\emptyset$
	- $A\cup{U}=U$
- ## Double Complement Law
	- $\bar{\bar{A}}=A$
- ## Complement Laws
	- $A\cap{\bar{A}}=\emptyset$
	- $\bar{U}=\emptyset$
	- $A\cup{\bar{A}}=U$
	- $\bar{\emptyset}=U$
- ## De Morgans Law
	- $\overline{A\cup{B}}=\bar{A}\cap{\bar{B}}$
	- $\overline{A\cap{B}}=\bar{A}\cup{\bar{B}}$
- ## Absorption Law
	- $A\cup{(A\cap{B})}=A$
	- $A\cap{(A\cup{B})}=A$
## Cartesian Products
- The product of two sets creates a set containing ordered pairs of values that can be plotted on a Cartesian plane
- Unlike sets which use curly braces, indicating the order of the elements does not matter, elements in a Cartesian product are surrounded with parentheses to indicate $(x,y)\neq{(y,x)}$
- The product of a previous product can be found, creating tuple elements with three ordered elements $(x,y,z)$, etc.
- $$
\begin{align*}
A\times{B}&= \set{(a,b):a\in{A\text{ and }b\in{B}}}\\\\
A&=\set{1,2} \quad B=\set{a,b,c}\\
&\begin{array} {|r|r|r|}
  \hline (1,a) & (1,b) & (1,c) \\
  \hline (2,a) & (2,b) & (2,c) \\
  \hline
\end{array}\\\\
A\times{B}=&\set{(1,a),(1,b),(1,c),(2,a),(2,b),(2,c)}
\end{align*}
$$
- The elements of a Cartesian product can be represented as string instead of tuples by concatenating each nested element in order, for example the element $(1,2,3)$ can be represented as $123$ 
## Partitions
- Two sets, $A$ and $B$ are **disjoint** if the intersection of the two sets is empty or $\emptyset$
- A sequence of sets, $A_{1},A_{2},\dots,A_{n}$ , is **pairwise disjoint** if every pair of distinct sets in the sequence is disjoint.
- A **partition** of non-empty set $A$ is a collection of non-empty subsets of $A$ such that each element of $A$ is in exactly one of the subsets