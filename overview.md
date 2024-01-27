**The Cauchy-Schwarz Inequality**
$$\left( \sum_{k=1}^n a_k b_k \right)^2 \leq \left( \sum_{k=1}^n a_k^2 \right) \left( \sum_{k=1}^n b_k^2 \right)$$

** Hidden Markov Model **

Let $X_t$ and $Y_t$ be continuous-time stochastic processes. The pair $(X_t,Y_t)$ is a ''hidden Markov model'' if
* $X_t$ is a Markov process whose behavior is not directly observable ("hidden");

  $\textbf{P}(Y_{t_0} \in A |$ $\[X_t \in B_t\]_{ t\leq t_0} ) = \textbf{P}(Y_{t_0} \in A |$ $\[X_{t_0} \in B_t\]_{ t\leq t_0} )$

:for every $t_0,$ every Borel set $A,$ and every family of Borel sets $\{B_t\}_{t \leq t_0}.$
