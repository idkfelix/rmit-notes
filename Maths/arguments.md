## Arguments
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
