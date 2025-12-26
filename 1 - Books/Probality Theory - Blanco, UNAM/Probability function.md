#probability 

We have two types of probability functions, discrete and continuous: 

# Discrete probability function

Let be $X$ a discrete [[random variable]] with values in $x_1, x_2, x_3, \dots$ and probabilities:

- $P_1 = P(X = x_1)$
- $P_2 = P(X = x_2)$
- $P_3 = P(X = x_3)$
- $\dots$

The discrete probability function of the [[random variable]] $X$ will be:

$$f(x): \mathbb{R} \rightarrow \mathbb{R}$$
Where:

$$f(x) = \begin{cases} P(X = x) & \text{if } x = x_1, x_2, \dots \\ 0 & \text{on another case } \end{cases}$$

This can also be expressed as $f_x(x)$ and if we want to see in a graphical view we visualize it as follows:

![[Pasted image 20240818164059.png]]

This function should follow this properties:

- $f(x) \geq 0$
- $\sum _x f(x) = 1$

And if we want to calculate the probabilities, then:

If $A \subseteq \mathbb{R}$, then:

$$P(X \in A) = \sum_{x \in A} f(x) $$
## Example

Let consider the following probability function:

$$f(x) = \begin{cases} 1/4 & \text{if } x = 1 \\ 1/2 & \text{if } x = 2 \\ 1/4 & \text{if } x = 3 \\ 0 & \text{On another case } \end{cases}$$

Then:

- $P(X \in [1,2]) = \frac{1}{4} +  \frac{1}{2} = \frac{3}{4}$
- $P(X \in [3,\infty)) = \frac{1}{4}$
- $P(X \in \{1,3\}) = \frac{1}{4} + \frac{1}{4} = \frac{1}{2}$
- $P(X \in \{-1,0,1\}) = \frac{1}{4}$

# Continuous probability function

Let be $X$ a continous [[random variable]], if a function $f(x): \mathbb{R} \rightarrow \mathbb{R}$ is no negative, and can be integrable and for all interval $(a,b) \subseteq \mathbb{R}$ then can be a continuous probability function:

$$P(X \in (a,b)) = \int_a^b f(x) dx$$
This function should follow this properties:

- $f(x) \geq 0$
- $\int_{-\infty}^{\infty} f(x) dx = 1$

We can visualize it as follows:

![[Pasted image 20240818174559.png]]

