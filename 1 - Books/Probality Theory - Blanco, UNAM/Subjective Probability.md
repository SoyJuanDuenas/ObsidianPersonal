#probability 
# Definition

Subjective probability is a perspective within probability theory that applies to any situation involving uncertainty, beyond just the outcomes of repeated experiments (as [[Frequentist Probability]]). For example, predictions about tomorrow’s weather, which are not based on repeated [[random experiment]]s, also fall under this category. Importantly, subjective probability does not imply arbitrary assignment; probabilities must adhere to [[Probability axioms]] and [[conditional probability]] to avoid inconsistencies. This is called Coherent Behavior.

This interpretation of the probability expresses an individual's personal belief or degree of confidence about the occurrence of a particular [[event]]. Subjective probability is not based on long-run frequencies or objective data but on personal judgment, experience, or intuition. Calling the probabilities “subjective” does not imply that they may be assigned without regard to the axioms of probability.

## Example

Let Y a binary variable with Y = 1 if a coin toss results in a head and 0 otherwise, and let:

$$\begin{align} \left\{ \begin{array}{l} P(Y = 1) = \theta  \\ P(Y = 0) = 1 - \theta \\  \end{array} \right. \end{align}$$

which is assumed to be constant for each trial. In this model, $\theta$ is a parameter and the value of $Y$ is the data (realization $y$ ).

Under these assumptions, $Y$ is said to have the Bernoulli distribution, written as

$$Y \sim Be (\theta)$$
We consider a [[i.i.d sample]] of variables $(Y_1, \dots ,Y_n )$ that corresponds to $n$ repeated experiments. The realization is denoted by $(y_1, \dots  , y_n )$. 

| Frequentist Approach                                                                                                        | Subjetive Approach                                                  |
| --------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------- |
| The parameter $\theta$ is an unknown number between zero and one                                                            | The parameter $\theta$ is a [[random variable]]                     |
| Because $\theta$ is a constant, do not have a distribution, it's important remember $\theta$ is different to $\hat{\theta}$ | The parameter $\theta$ has a distribution "ad hoc" called [[prior]] |
## Statistical Implications

The subjective view of probability requires that subjective probabilities adhere to the standard axioms of probability to maintain coherence and avoid certain losses. This perspective emphasizes that while probabilities are subjective, they are not arbitrary and must be consistently set in accordance with probability theory. Also subjetive probabilities open the door for [[Bayesian inference]] with a direct relationship with the concepts of [[prior]] and [[posterior]] distributions

