**The Cauchy-Schwarz Inequality**
$$\left( \sum_{k=1}^n a_k b_k \right)^2 \leq \left( \sum_{k=1}^n a_k^2 \right) \left( \sum_{k=1}^n b_k^2 \right)$$

** Hidden Markov Model **

== Definition ==
Let $X_n$ and $Y_n$ be discrete-time [[stochastic processes]] and $n\geq 1$. The pair $(X_n,Y_n)$ is a ''hidden Markov model'' if

* $X_n$ is a [[Markov process]] whose behavior is not directly observable ("hidden");
* $\mathbf{P}\bigl(Y_n \in A\ \bigl|\ X_1=x_1,\ldots,X_n=x_n\bigr)=\mathbf{P}\bigl(Y_n \in A\ \bigl|\ X_n=x_n\bigr),$ 

:for every $n\geq 1,$ $x_1,\ldots, x_n,$ and every [[Borel set|Borel]] set $A$.

Let $X_t$ and $Y_t$ be continuous-time stochastic processes. The pair $(X_t,Y_t)$ is a ''hidden Markov model'' if

* $X_t$ is a Markov process whose behavior is not directly observable ("hidden");
* $\mathbf{P}\bigl(Y_{t_0} \in A\ \bigl|\ \[X_t \in B_t \]_{t \leq t0} \bigr)=$
  $ \indent \mathbf{P}\bigl(Y_{t_0} \in A\ \bigl|\ X_{t_0} \in \[B_{t_0}  \bigr)$

:for every $t_0,$ every Borel set $A,$ and every family of Borel sets $\[B_t\]_{t \leq t_0}.$
