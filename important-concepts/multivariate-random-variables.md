---
cover: >-
  https://images.unsplash.com/photo-1551288049-bebda4e38f71?crop=entropy&cs=srgb&fm=jpg&ixid=M3wxOTcwMjR8MHwxfHNlYXJjaHw0fHxlY29ub21pY3N8ZW58MHx8fHwxNjg1NzA4OTg4fDA&ixlib=rb-4.0.3&q=85
coverY: 0
---

# ♠ Multivariate random variables

As alluded to on the previous page, econometricians are often interested in the relationship between two or more random variables. Therefore, we need measures that give us insight into the **joint probability distribution** of these random variables.&#x20;

An important quantity is the **covariance**, which is a measure of joint variability between two random variables. The sign of the covariance (i.e. + or -) indicates whether the random variables generally move in the same or opposite direction. The interpretation of a covariance is generally not straightforward, because the values it can take are not bounded. For that reason, the measure **correlation** which only takes values between -1 and +1  is often preferred.

Whereas the previous measures are useful, they only tell part of the story. More specifically, they only provide information on how two random variables are related **linearly**. Correlation is however just one way for random variables to be **dependent**. Note for example that it is possible for two random variables to be uncorrelated, yet dependent.

> _Example._ Suppose we have two random variables $$X$$and $$Y$$, such that $$Y=X^2$$. Assume that $$X$$can only take values -1, 0 and 1 each with equal probability $$\frac{1}{3}$$(alternatively, we say that $$X$$is uniformly distributed on $$\{ -1, 0 , 1\}$$). Note that, using elementary results from probability theory:
>
> * $$\mathbb{E}(X) = (-1) \cdot \frac{1}{3} + 0 \cdot \frac{1}{3} + 1 \cdot \frac{1}{3} = -\frac{1}{3} + \frac{1}{3} = 0$$,
> * $$\mathbb{E}(XY) = \mathbb{E}(X^{3}) = (-1)^3 \cdot \frac{1}{3} + 0^3 \cdot \frac{1}{3} + 1^3 \cdot \frac{1}{3} = -\frac{1}{3} + \frac{1}{3} = 0 = \mathbb{E}(X)\mathbb{E}(Y)$$.
>
> Because $$\mathbb{E}(XY) = \mathbb{E}(X)\mathbb{E}(Y)$$,$$X$$and $$Y$$are _uncorrelated_. We can however show that they are dependent:
>
> * $$\mathbb{P}(X = -1 \text{ and } Y=1) = \mathbb{P}( X = -1) = \frac{1}{3}$$,
> * $$\mathbb{P}(X=-1)\mathbb{P}(Y=1) = \frac{1}{3} \cdot \frac{2}{3} = \frac{2}{9}$$.
>
> Because (for example) $$\mathbb{P}(X=-1,Y=1) \neq \mathbb{P}(X=-1)\mathbb{P}(Y=1)$$, $$X$$and $$Y$$ are _dependent_.

So far we have focused on the relation between only two random variables. However, often we deal with (many) more random variables. The multivariate generalizations of the concepts we discussed above are the **covariance matrix** and the **correlation matrix**. We characterize one of these in the example below.&#x20;

> _Example._ Suppose we are given three random variables $$X,Y,Z$$. Then we can define the covariance matrix of these three random variables as
>
> $$\begin{pmatrix} \mathbb{V}\text{ar}(X) & \mathbb{C}\text{ov}(X,Y) & \mathbb{C}\text{ov}(X,Z) \\ \mathbb{C}\text{ov}(Y,X) & \mathbb{V}\text{ar}(Y) & \mathbb{C}\text{ov}(Y,Z) \\ \mathbb{C}\text{ov}(Z,X) & \mathbb{C}\text{ov}(Z,Y) & \mathbb{V}\text{ar}(Z) \end{pmatrix}$$.&#x20;
>
> In words: the matrix has the respective variances of the three random variables on the diagonal, while the off-diagonal elements consist of the covariances.

Thus, in the case of multivariate random variables we often use **vectors** and **matrices** to "summarize" the relationships between random variables. More generally, we use concepts from **linear algebra** to investigate the properties of statistical quantities. For example, one could check whether the covariance matrix above has full rank (which is a necessary condition for the matrix to be invertible).

Let us now go back to the concept of **joint distribution**. Consider the case of two random variables $$X$$and $$Y$$. The joint distribution, denoted $$f_{X,Y}(x,y)$$, then determines the probability distribution on _all pairs of outcomes._ Simply said, it considers all possible combinations of outcomes of $$(X,Y)$$and assigns a probability to all of these outcomes. However, the random variables $$X$$and $$Y$$also still have their own, separate distributions, denoted $$f_{X}(x)$$ and$$f_{Y}(y)$$ which we call **marginal distributions.**

The joint and marginal distributions are related through **conditional distributions**. The concept of **conditioning** plays a central role in econometrics and allows us to ask questions such as "What is the probability of $$Y$$ given that $$X$$takes on a certain value $$x$$?". That is, knowledge of the outcome of a related variable $$X$$might influence the likelihood of $$Y$$. It is generally not straightforward to work with **conditional distributions, conditional means** and **conditional variances**. But despair not, there are useful theorems out there, such as the **law of total expectation** and the **law of total variance,** that aid in simplifying difficult computations. &#x20;

&#x20;&#x20;
