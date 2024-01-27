** Bayesian Model ** 

Abstractly, naive Bayes is a conditional probability model: it assigns probabilities $p(C_k \mid x_1, \ldots, x_n)$ for each of the $K$ possible outcomes or ''classes'' $C_k$ given a problem instance to be classified, represented by a vector $\mathbf{x} = (x_1, \ldots, x_n)$ encoding some $n$ features (independent variables).

The problem with the above formulation is that if the number of features $n$ is large or if a feature can take on a large number of values, then basing such a model on probability tables is infeasible. The model must therefore be reformulated to make it more tractable. Using Bayes' theorem, the conditional probability can be decomposed as:

: $p(C_k \mid \mathbf{x}) = \frac{p(C_k) \ p(\mathbf{x} \mid C_k)}{p(\mathbf{x})} \,$


**The Cauchy-Schwarz Inequality**
$$\left( \sum_{k=1}^n a_k b_k \right)^2 \leq \left( \sum_{k=1}^n a_k^2 \right) \left( \sum_{k=1}^n b_k^2 \right)$$

** Hidden Markov Model **

$$\Pi_{i=0}^N \left( P(X_i \mid X_{i-1}) \right) $$

== Definition ==
Let $X_n$ and $Y_n$ be discrete-time stochastic processes and $n\geq 1$. The pair $(X_n,Y_n)$ is a ''hidden Markov model'' if

* $X_n$ is a Markov process whose behavior is not directly observable ("hidden");
* $\mathbf{P}\bigl(Y_n \in A\ \bigl|\ X_1=x_1,\ldots,X_n=x_n\bigr)=\mathbf{P}\bigl(Y_n \in A\ \bigl|\ X_n=x_n\bigr),$ 

:for every $n\geq 1,$ $x_1,\ldots, x_n,$ and every Borel set set $A$.

Let $X_t$ and $Y_t$ be continuous-time stochastic processes. The pair $(X_t,Y_t)$ is a ''hidden Markov model'' if

* $X_t$ is a Markov process whose behavior is not directly observable ("hidden");
* $\mathbf{P}\bigl(Y_{t_0} \in A\ \bigl|\ \[X_t \in B_t \]_{t \leq t0} \bigr)$


 ㅤㅤ= $\mathbf{P}\bigl(Y_{t_0} \in A\ \bigl|\ X_{t_0} \in \[B_{t_0}\bigr)$

:for every $t_0,$ every Borel set $A,$ and every family of Borel sets $\[B_t\]_{t \leq t_0}.$
