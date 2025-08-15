## Predicates
- A logical statement with a truth value that is a function of one or more variables is called a **predicate**
- Predicates differ from propositions as they do not have a well defined truth value until the value of the variables are specified
    - The statement "$\large x$ is an odd number" is not a proposition because the statement does not have a well defined truth value until the value of $\large x$ is specified. If $\large x=5$ the statement is true, however if $\large x=4$ then it is false.
- These statements can be expressed as a function $\large{p}$ of the variable $\large{x}$, as in $\large{P(x)}$ read as $\large{P}$ of $\large{x}$.
- If the **predicate** $\large{P(x)}$ is defined to be the statement "$\large{x}$ is an odd number," then $\large{P(5)}$ corresponds to the statement "$\large{5}$ is an odd number". This is considered a **proposition** as $\large{P(5)}$ has a well-defined truth value

## Variable Domains
- The **domain** of a variable in a predicate is the set of all possible values for the variable. 
- For example, a natural domain for the variable $\large{x}$ in the predicate "$\large{x}$ is an odd number" is the set of all integers or $\large{\mathbb{Z}}$
- If the domain of a variable in a predicate is not clear from the context, the domain should be given as a part of the definition of the predicate
- A statement $\large{P(x)}$ may be true for all values in the domain, however if the statement contains a variable it is still considered to be a predicate not a proposition.

## Universal Quantifier ($\large \forall$)
- The universally quantified statement $\large \forall xP(x)$, using the universal quantifier $\large \forall$, is read as "for all $\large x,P(x)$" or "for every $\large x,P(x)$". This logical statement asserts that $\large P(x)$ is true for every possible value of $\large x$ in its domain.
    - $\large \forall{xP(x)}=P(a_1)\land P(a_2)\land\dots\land P(a_k)$
- A universally quantified statement $\large \forall xP(x)$ turns the predicate $\large P(x)$ into a proposition as it is now either true or false.
    - The statement is true if and only if $\large P(n)$ is true for every $\large n$ in the domain of variable $\large x$. This can be proven by showing the predicate holds for an arbitrary element in the domain of variable $\large x$, 
        - "arbitrary" indicating that nothing is assumed about the element except for its inclusion in the domain
    - A single counterexample of an element in the domain of variable $\large x$ where $\large P(x)$ is false is enough to prove the universally quantified statement $\large \forall xP(x)$ to be false.
- If the domain for variable $\large x$ is empty, then the statement $\large \forall xP(x)$ is true because there are no elements in the domain for which $\large P(x)$ is false.

## Existential Quantifier ($\large \exists$)
- The existentially quantified statement $\large \exists xP(x)$, using the existential quantifier $\large \exists$, is read as "there exists an $\large x$ such that $\large P(x)$". This logical statement asserts that $\large P(x)$ is true for at least one possible value for $\large x$ in its domain.
    - $\large \forall{xP(x)}=P(a_1)\lor P(a_2)\lor\dots\lor P(a_k)$
- A existentially quantified statement $\large \exists xP(x)$ turns the predicate $\large P(x)$ into a proposition as it now either true or false.
    - The statement is true if there is an element in the domain of variable $\large x$ for which $\large P(x)$ is true.
    - In order to prove the existentially quantified statement false one must show that for every element in the domain of variable $\large x$ $\large P(x)$ is false.
        - Some statements can be shown to be false for an arbitrary element in the domain of variable $\large x$. For example $\large \exists x(x+1\lt x)$ can be shown false because no positive integer satisfies the expression $\large x+1\lt x$ .
- If the domain for variable $\large x$ is empty, then the statement $\large \exists xP(x)$ is false because there is no element in the domain for which $\large P(x)$ is true.

## De Morgan's Law for Quantified Statements
 - The negation operation can be applied to a quantified statement, such as $\large \neg\forall{xP(x)}$ or $\large \neg\exists{xP(x)}$. The following statements show the logical equivalence of this negation:
     - $\large \neg\forall{xP(x)}\equiv\exists{x\neg P(x)}$
     - $\large \neg\exists{xP(x)}\equiv\forall{x\neg{P(x)}}$
- This can be used similarly to De Morgan's Law for propositions in order to simplify quantified statements.

## Nested Quantifiers
- If a predicate has more than one variable, each variable must be bound by a separate quantifier. A logical expression with more than one quantifier that binds different variables in the same predicate has nested quantifiers.
- $$
\begin{align*}
&\forall{x\,\exists{y\,P(x,y)}} & x \text{ and } y \text{ are both bound.}\\
&\forall{x\,P(x,y)} & x \text{ is bound and } y \text{ is free.}\\
&\exists{y\,\exists{z\,T(x,y,z)}} & y \text{ and } z \text{ are bound. } x \text{ is free.}
\end{align*}
$$
- A logical expression is only a proposition if all of its variables are bound by a quantifier, otherwise it is still considered a predicate.
- Nested quantifiers are always evaluated **left to right** so by switching the order of the quantifiers in the proposition $\large \exists{x\forall{yP(x,y)}}$ to $\large \forall{x\exists{yP(x,y)}}$ the meaning of the proposition is changed.
    - For the proposition $\large \forall{x\exists{yP(x,y)}}$ to be true there must a $\large y$ for every possible value of $\large x$ such that the predicate is true.
    - For the proposition $\large \exists{x\forall{yP(x,y)}}$ to be true there must be an $\large x$ for which every possible value of $\large y$ will make the predicate true.

## Expressing Uniqueness
- 