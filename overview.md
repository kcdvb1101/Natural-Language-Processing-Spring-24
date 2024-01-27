**The Cauchy-Schwarz Inequality**
$$\left( \sum_{k=1}^n a_k b_k \right)^2 \leq \left( \sum_{k=1}^n a_k^2 \right) \left( \sum_{k=1}^n b_k^2 \right)$$

$$ \section*{Hidden Markov Model}

\subsection*{State Transition Probabilities:}
\[
  P(S_t|S_{t-1}) =
  \begin{bmatrix}
    P(S_1|S_1) & P(S_2|S_1) & P(S_3|S_1) \\
    P(S_1|S_2) & P(S_2|S_2) & P(S_3|S_2) \\
    P(S_1|S_3) & P(S_2|S_3) & P(S_3|S_3) \\
  \end{bmatrix}
\]

\subsection*{Emission Probabilities:}
\[
  P(O_t|S_t) =
  \begin{bmatrix}
    P(O_1|S_1) & P(O_2|S_1) & P(O_3|S_1) \\
    P(O_1|S_2) & P(O_2|S_2) & P(O_3|S_2) \\
    P(O_1|S_3) & P(O_2|S_3) & P(O_3|S_3) \\
  \end{bmatrix}
\]

$$
