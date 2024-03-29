**Mathematical foundations of NLP**
Objective: Reasonably deep understanding of classic to mainstream nlp techniques. Interview preparation, revision reference.


**Bayes theorem and bayesian classifiers**

Abstractly, naive Bayes is a conditional probability model: it assigns probabilities $p(C_k \mid x_1, \ldots, x_n)$ for each of the $K$ possible outcomes or ''classes'' $C_k$ given a problem instance to be classified, represented by a vector $\mathbf{x} = (x_1, \ldots, x_n)$ encoding some $n$ features (independent variables).

The problem with the above formulation is that if the number of features $n$ is large or if a feature can take on a large number of values, then basing such a model on probability tables is infeasible. The model must therefore be reformulated to make it more tractable. Using Bayes' theorem, the conditional probability can be decomposed as:

: $$p(C_k \mid \mathbf{x}) = \frac{p(C_k) \ p(\mathbf{x} \mid C_k)}{p(\mathbf{x})} \,$$

Now Bayes classifiers assume that the features $x = (x_1 ... x_n)$ are independent so:
$$p(\mathbf{x} \mid C_k) = p(x_{1} \mid C_k) \cdot p(x_{2} \mid C_{k}) \cdot ... \cdot p(x_n \mid C_k)$$

Advantages:
– Fast to train (single scan). Fast to classify 
– Not sensitive to irrelevant features
– Handles real and discrete data
– Handles streaming data well

Disadvantages:
– Assumes independence of features

**The Cauchy-Schwarz Inequality**
$$\left( \sum_{k=1}^n a_k b_k \right)^2 \leq \left( \sum_{k=1}^n a_k^2 \right) \left( \sum_{k=1}^n b_k^2 \right)$$

The Cauchy-Schwarz inequality has various applications in machine learning. This inequality provides an upper bound on the absolute value of the inner product of two vectors, and it is a fundamental tool in mathematical analysis. Here are some applications of the Cauchy-Schwarz inequality in the context of machine learning:

    Feature Selection:
        In feature selection problems, where the goal is to choose a subset of relevant features, the Cauchy-Schwarz inequality can be used to establish bounds on the correlation or similarity between different features. This can guide the selection of features that contribute the most to the model's performance.

    Kernel Methods:
        The Cauchy-Schwarz inequality is used in the analysis of kernel methods, such as Support Vector Machines (SVMs). It provides insights into the relationships between input data points in the feature space induced by the kernel function.

    Bounding Loss Functions:
        In the analysis of machine learning algorithms, particularly those involving loss functions, the Cauchy-Schwarz inequality can be employed to derive bounds on the expected value of a product of random variables. This is useful in proving convergence rates and generalization bounds.

    Optimization:
        The Cauchy-Schwarz inequality is often utilized in optimization problems related to machine learning. For instance, it can be applied in the derivation of update rules for optimization algorithms, helping to establish convergence properties.

    Covariance Matrix Inequalities:
        The Cauchy-Schwarz inequality is fundamental in establishing inequalities involving covariance matrices. In machine learning, this can be relevant when dealing with multivariate distributions and is useful in understanding the relationships between different variables.

    Information Theory:
        In the context of information theory, the Cauchy-Schwarz inequality is used to establish bounds on the correlation between different random variables. This is relevant when dealing with entropy, mutual information, and other information-theoretic quantities.

    Probabilistic Bounds:
        The Cauchy-Schwarz inequality is applied in deriving probabilistic bounds and concentration inequalities, which are crucial in understanding the behavior of random variables and in establishing confidence intervals for certain machine learning algorithms.

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

Question: What is Markov assumption/property?
The Markov assumption states that the future state of a system depends only on its current state and is independent of how the system arrived at its current state. In other words, given the present state of the system, the future behavior of the system is not influenced by the sequence of events that preceded the current state.

Vocabulary, word, document, and corpus:
Corpus: set of unique words used in the text corpus is referred to as the vocabulary. When processing raw text for NLP, everything is done around the vocabulary.
*character based vocabulary
*word-based vocabularies
*word: item from vocabulary indexed by {1...V}. Which is represented as unit-basis vectors. 
*document: sequence of n words
*corpus: Collection of M documents
