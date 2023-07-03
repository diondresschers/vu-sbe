---
cover: >-
  https://images.unsplash.com/photo-1454165804606-c3d57bc86b40?crop=entropy&cs=srgb&fm=jpg&ixid=M3wxOTcwMjR8MHwxfHNlYXJjaHwxfHxkYXRhJTIwY29sbGVjdGlvbnxlbnwwfHx8fDE2ODU3MDkxNDV8MA&ixlib=rb-4.0.3&q=85
coverY: 0
---

# ♾ Asymptotics

Econometricians do not just want to _use_ existing estimation and testing methods, but also _investigate their properties_ or even _develop new ones_. In particular, there are some characteristics that are desirable. For estimators of parameters, we might want them to be **consistent** and **asymptotically normally distributed**. For tests, we want them to correctly "fail to reject" or "reject" the null hypothesis (given that we know the truth). Intuitively, the performance of the estimator or test should become "better" when we have more data at our disposal. Therefore, econometricians typically study the properties of estimators/tests, as sample size goes to infinity (or in mathematical terms, as $$n \rightarrow \infty$$). This is what **asymptotics** is all about.&#x20;

There are a couple of concepts that are very useful when we do asymptotic analysis:

* **Convergence in probability**, which is often used when we want to show that a sequence of random variables (typically a sequence of estimators) _converges to a specific value_ when sample size grows large.
* **Convergence in distribution**, which is often used when we want to show that a sequence of random variables (typically a sequence of a rescaled version of the estimators) _converges to a specific distribution._
* **Central limit theorem**, which is a key concept in probability theory. There are various versions of the theorem, but it essentially states that if we multiply the ratio consisting of the sample mean $$\overline{X}$$ minus the real mean $$\mu$$, divided by the standard deviation $$\sigma$$ by $$\sqrt{n}$$ (i.e. the square root of sample size), then we obtain a standard normal distribution as $$n \rightarrow \infty$$. This is even true when the random variables $$X_{1},...,X_{n}$$ which make up $$\overline{X}$$are themselves _not normally distributed._

Before starting the minor Applied Econometrics, it might help to read more about the important concepts that were listed and intuitively explained in the last pages. You can use the references mentioned at [Literature](../literature.md). It can give you a swift start into the minor program!

No worries if you do not master everything in complete (mathematical or statistical) detail. Of course, the more you know already, the better; but the most important is that you understand why the concepts are crucial and useful to the field of econometrics. We hope you'll enjoy the program!
