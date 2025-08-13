## Reflexive
- Suppose that $R$ is a binary relation on set $A$. $R$ is **reflexive** if an only if for every $x\in{A}$, $xRx$
- The definition of reflexive is a universal statement. In order for a binary relation to be reflexive, every element must be related to itself.
- To show that a relation is not reflexive, one must only show that a particular $x\in{A}$ exists such that $xRx$ is not true.
## Anti-Reflexive
- $R$ is **anti-reflexive** if and only if for every $x$ in the domain of $R$, it is not true that $xRx$
- Irreflexive is an alternate term for anti-reflexive
- The definition of anti-reflexive is a universal statement. In order for a binary relation to be anti-reflexive, every element must not be related to itself.
## Symmetric
- Suppose that $R$ is a relation on set $A$. $R$ is **symmetric** if and only if for every pair, $x$ and $y\in{A}$, $xRy$ if and only if $yRx$
- A relation is symmetric if for every pair in the domain one of the following situations is true:
	- $xRy$ and $yRx$ are both true
	- Neither $xRy$ nor $yRx$ is true
## Anti-Symmetric
- Suppose that $R$ is a relation on set $A$. $R$ is **anti-symmetric** if and only if for every pair, $x$ and $y\in{A}$, if $x\neq{y}$ then $xRy$ and $yRx$ cannot both be true
- A relation is anti-symmetric if for every pair of distinct elements in the domain one of the following situations holds:
	- $xRy$, but $yRx$ is not true
	- $yRx$, but $xRy$ is not true
	- Neither $xRy$ nor $yRx$ is true
## Transitive
- Suppose $R$ is a relation on set $A$. $R$ is **transitive** if any only if for every three elements $x,y,z\in{A}$, if $xRy$ and $yRz$, then $xRz$ must also be true.
- In the definition of transitive relation, the elements, $x$, $y$, and $z$ do not necessarily have to be distinct.
- The definition of transitive is a universal statement. If any $x$, $y$, and $z$ in the domain have the forbidden pattern of $xRy$, $yRz$, but not $xRz$, then the relation is not transitive.
## Directed Graphs
- A **directed graph**, or **digraph** for short, consists of a pair $(V,E)$. $V$ is a set of vertices, and $E$, a set of directed edges, is a subset of $V\times{V}$.
- An individual element of $V$ is called a **vertex** . A vertex is pictured as a labelled point on the graph.
- An edge, $(u,v)\in{E}$, is pictured as an arrow going from the vertex labelled $u$ to the vertex labelled $v$. The vertex $u$ is the **tail** of the edge, with $v$ being the **head**
- The **in-degree** of a vertex is the number of edges pointing into it and the **out-degree** is the number of edges pointing out of it.
- $$
  \begin{align*}
    \text{in-degree}(u)&= |v|(v,u)\in{E}|\\
	\text{out-degree}(u)&= |v|(u,v)\in{E}|
  \end{align*}
  $$
## Walks
- A **walk** from $v_0$ to $v_1$ in a directed graph $G$ is a sequence of alternating vertices and edges that starts and ends with a vertex
	- $\langle v_0,(v_0,v_1),v_1,\dots,v_{l-1},(v_{l-1},v_l),v_l\rangle$
- The length of a walk is $l$, the number of edges in the walk.
- Each edge in the sequence appears after its tail and before its head
- Since the edges in a walk are determined by the vertices, a walk can also be denoted by the sequence of vertices:
	- $\langle v_0,v_1,\dots,v_l\rangle$
- An **open walk** is a walk which the first and last vertices are not the same. 
- A **closed walk** is a walk in which the first and last vertices are the same
- Special types of walks:
	- A **trail** is a walk in which no edge occurs more than once.
	- A **path** is an open walk in which no vertex occurs more than once.
	- A **circuit** is a closed trail.
	- A **cycle** is a circuit of length at least $1$ in which no vertex occurs more than once, except the first and last vertices which are the same.