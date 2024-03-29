---
cover: >-
  https://images.unsplash.com/photo-1541278107931-e006523892df?crop=entropy&cs=srgb&fm=jpg&ixid=M3wxOTcwMjR8MHwxfHNlYXJjaHwxfHxjYXJkc3xlbnwwfHx8fDE2ODU3MDY4ODV8MA&ixlib=rb-4.0.3&q=85
coverY: 0
---

# ♦ Univariate random variables

**Randomness** play a crucial role in econometrics. This is because econometricians see data as **realizations** (outcomes) of a sequence of **random variables**. Just think about it: if you go out on the streets on Monday and Tuesday and each day ask 100 strangers for their height, you won't get the same 100 outcomes on both days. This is because you obtained two **random samples** which contain information about the **population**, which in this case could be the inhabitants of Amsterdam.&#x20;

This is a very important basis for **statistical sciences:** we draw conclusions about the world around us by studying data and trying to determine (or at least approximate) the underlying process that generated the data. For this, we need knowledge in the field of **probability theory**.

Random variables are often denoted by capital letters, e.g. $$X$$, and their realizations/outcomes by lower case letters, e.g. $$x$$. A random variable has a **probability distribution** that represents the likelihood that any of the possible outcomes occur.&#x20;

> _Example._ Consider a coin and define the outcome "heads" as $$x=0$$ and "tails" as $$x=1$$. If the coin is _fair_, then we should have $$P(X=0) = P(X=1) = \frac{1}{2}$$. That is, both events happen with equal probability. &#x20;

The simple example shows how probability theory can be used to 'model' random events. Let's provide some intuition why this is relevant in statistics and econometrics. To that end, suppose you have a coin at your disposal and you want to know whether it is fair or not. You decide to toss the coin 100 times and you hypothesize that - for the coin to be fair - 50 heads and 50 tails should appear. However, in reality, you find 47 heads and 53 tails. _Does this mean we can conclude the coin is not fair?_

Probability theory and statistics give you a means to answer questions such as the one we just posed. In econometrics, we are often confronted with data and we want to deduce whether it mimics a certain probability distribution. For this reason, concepts such as the **probability distribution function (pdf)** and **cumulative distribution function (cdf)** are vital. They summarize how the random variable assigns probabilities to single outcomes (pdf, $$P(X=1)$$, for example) or to a combination of outcomes (cdf, $$P(X \leq 2)$$, for example).

Other important pieces of information of a random variable is its average value (**mean**), its dispersion/spread (**variance**), the symmetry of its distribution (**skewness**) and the fatness of the tails of the distribution (**kurtosis**). They all give extremely relevant information.&#x20;

> _Example._ Suppose we are looking at the random variable 'wage' in the Netherlands. The mean tells you the average wage of a worker in the Netherlands. However, this does not tell you whether almost all Dutch workers earn a wage close to the average or whether the individual wages lie far apart. The variance provides information on that. If the distribution of wage is very asymmetric, there might be a large difference between poor and rich. If the tails of the distribution are 'fat', there might be many workers with extreme wages (both extremely low and high wages).

Another way to characterize the distribution of a random variable is to look at its **quantiles**. We then chop the distribution in intervals with equal probability, e.g. in parts of four such that each part represents 25%. If we now obtain data, we could order the values from low to high, which represents the distribution of the sample. We could now chop this distribution in the same way in intervals with equal probability to see whether the distribution of our data/sample coincides with the distribution of the random variable.

> _Example._ Suppose you collect a data on the height of adults in Amsterdam. You hypothesize that height is probably normally distributed. This distribution looks nicely bell-shaped curved, which could fit 'height' very well. Overall, there are not a lot of very short people or very tall people, and most adults have a height close to the average. This is an example in which you can investigate whether your **sample distribution** is close to the **theoretical distribution** you expect (a normal distribution, in this case). To make this comparison, a **QQ-plot** is a useful graphical tool.&#x20;

So far, we have only talked about a single random variable (therefore, **univariate**) or sequences of this random variable. However, often we want to link one random variable to another. For example, we are not just interested in 'wage', but we want to know whether years of education has an important impact on wage. Or maybe whether the combination of years of education _and_ the type of education affect wages. To study these type of relations, we need **multivariate random variables**.
