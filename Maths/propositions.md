## Order of Operations
- Parentheses work the same as normal algebra
- Without parentheses the order of operations are:
	1. Not ($\neg{}$) or Negation
	2. And ($\land$) or Conjunction
	3. Or ($\lor$) or Disjunction
## Truth Tables
- Truth tables show all the possible truth value combinations of a proposition
- There are $2^n$ rows where $n$ is the number of variables
- The values chosen for each column of a truth table follow a set methodology
	- Each column begins its first row with a value of $T$
	- The rightmost variable column should alternate $T$ and $F$ every row
	- Following on, the second rightmost should alternate $TT$ and $FF$
	- The next column $TTT$ and $FFF$, so on and so forth
## Conditional Operation ($\rightarrow$)
- $p \rightarrow q$, read as "if $p$, then $q$"
- The hypothesis is denoted as $p$, and the proposition as $q$
- $p \rightarrow q$ is false if and only if $p=T$ and $q=F$
- A proposition $p \rightarrow q$ will have three related statements:
	- **Converse** $q \rightarrow p$
	- **Inverse** $\neg{p}\rightarrow \neg{q}$
	- **Contrapositive $\neg{q}\rightarrow \neg{p}$
## Biconditional Proposition ($\leftrightarrow$)
- $p \leftrightarrow q$, read as "$p$ if and only if $q$"
- A biconditional is only true if both $p$ and $q$ have the same truth value
- The abbreviation "iff" can be used in place of "if and only if"
## Tautology & Contradiction
- A compound proposition is a **Tautology** if the proposition evaluates to **T** regardless of the variable values
	- An example of a tautology is $p \lor \neg{p}$ where when $p$ has a value of either $T$ or $F$ it will evaluate to $T$
- Similarly a compound proposition that will only evaluate to $F$ is referred to as a contradiction.
	- An example of a contradiction is $p \land \neg{p}$ where $p$ and $\neg{p}$ can never have the same value required to evaluate as $T$
## Logical Equivalence ($\equiv$)
  - Two propositions are logically equivalent if they both have the same truth value regardless of the regardless of their variable values
  - This is denoted with the symbol $\equiv$ where $s \equiv r$ indicates propositions $s$ and $r$ are logically equivalent
  - Propositions $s$ and $r$ are logically equivalent if and only if $s \leftrightarrow r$ is a tautology
## De Morgans Law
- A pair of rules that relate conjunctions and disjunctions through negation
- The negation of a conjunction is equivalent to the disjunction of the negations and vice versa
- $\neg{(p \lor q)} \equiv (\neg{p}\land \neg{q})$
- $\neg{(r \land s)} \equiv (\neg{r}\lor \neg{s})$
## Law of Conditional identities
- Conditional operations can be transformed into a disjunction with a negated hypothesis
	- $p \rightarrow q \equiv \neg{p} \lor q$
- Biconditional operations can be transformed into a disjunction between the conditional operation of both elements
	- $p \leftrightarrow q \equiv (p \rightarrow q) \lor (q \rightarrow p)$
## Laws of propositional logic
- **Associative**
	- $(p \lor q)\lor r \equiv p \lor (q \lor r)$
	- $(p \land q)\land r \equiv p \land (q \land r)$
- **Distributive**
	- $p \lor (q \land r)\equiv(p \lor q)\land (p \lor r)$
	- $p \land (q \lor r)\equiv(p \land q)\lor (p \land r)$
- **Identity & Domination**
	- $p \lor F \equiv p \qquad p \land F \equiv F$
	- $p \land T \equiv p \qquad p \lor T \equiv T$
- **Absorption**
	- $p \lor (p \land q) \equiv p$
	- $p \land (p \lor q) \equiv p$
## Argument
- An argument is a sequence of propositions, called **hypotheses**, followed by a final proposition, called the **conclusion**.
- An argument is valid if the conclusion is true when all propositions / hypotheses that make up the argument are also true or $(h_{1}\land h_{2}\land...\land h_{n})\rightarrow c$
- Arguments are denoted in the following format where each $h$ is a hypothesis and $c$ is the conclusion:
	- $$
\begin{align*}
&h_{1}\\
&h_{2}\\
&...\\
&\underline{h_{n}}\\
&\therefore c
\end{align*}
$$
- Reordering the hypotheses of an argument does not change whether it is valid or not. Two arguments with hypotheses in different orders are considered to be the same argument
## Rules of Inference
- The rules of inference are a set of **known valid arguments** used to simplify the process of proving an arguments validity
- $\newcommand{\Conclusion}[1]{ \hline\therefore\,#1 }$ $\newcommand{\Argument}[2]{ \begin{array}{l}#1\end{array}&&\text{#2} }$ $$
\begin{array}{l,l}
\Argument{p\\ p\to{q}\\ \Conclusion{q}}{Modus ponens}\\\\
\Argument{\neg{q}\\ p\to{q}\\ \Conclusion{\neg{p}}}{Modus tollens}\\\\
\Argument{p\\ \Conclusion{p\lor q}}{Addition}\\\\
\Argument{p\land q\\ \Conclusion{p}}{Simplification}\\\\
\Argument{p\\ q\\ \Conclusion{p\land q}}{Conjunction}\\\\
\Argument{p\to{q}\\ q\to{r}\\ \Conclusion{p\to{r}}}{Hypothetical syllogism}\\\\
\Argument{p\lor q\\ \neg{p}\\ \Conclusion{q}}{Disjunctive syllogism}\\\\
\Argument{p\lor q\\ \neg{p}\lor{r}\\\Conclusion{q\lor r}}{Resolution}\\\\
\end{array}
$$
