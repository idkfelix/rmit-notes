## Disjunctive / Conjunctive Normal Form (DNF / CNF)
- A disjunctive normal form expression or DNF expression is the sum of one or many terms with no addition within each term.
- A conjunctive normal form expression or CNF expression is the product of one or many clauses with no multiplication within each clause
- The complement of a variable is denoted with a bar over said term, for example the complement of $\large x$ is represented as $\large\bar{x}$.
- Complements can only be applied to single variables in both DNF and CNF expressions.
- $$
\begin{align}
&\mathrm{Disjunctive\ Normal\ Form\ (DNF)}
&&\large{\bar{x}y\bar{z}+xy+\bar{w}+y \bar{z} w}\\ \\
&\mathrm{Conjunctive\ Normal\ Form\ (CNF)}
&&\large{(\bar{x}+y+\bar{z})(x+y)(w)(y+\bar{z}+w)}
\end{align}
$$
##  Boolean Satisfiability (SAT)
- The boolean satisfiability problem or SAT takes a boolean expression as input and asks whether the values of the variables can be set so that the expression evaluate
- Showing that an expression is unsatisfiable by considering all possible assignments for the variables takes time proportional to $\large{2^n}$ for an expression with $\large{n}$ variables
- No provably efficient method to solve SAT has been found as of yet, many in the field believe that no such method exists