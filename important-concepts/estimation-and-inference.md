---
cover: >-
  https://images.unsplash.com/photo-1600267147646-33cf514b5f3e?crop=entropy&cs=srgb&fm=jpg&ixid=M3wxOTcwMjR8MHwxfHNlYXJjaHw2fHx0ZXN0aW5nfGVufDB8fHx8MTY4NTcwOTAyOHww&ixlib=rb-4.0.3&q=85
coverY: 0
---

# 🧪 Estimation and inference

Econometricians build models for various reasons, as outlined on the page [What is econometrics?](what-is-econometrics.md). Up until now, we have discussed random variables and their statistical properties. However, in most cases, we do not know these (exact) properties. For example, you might have data at your disposal and by plotting the data as a histogram, it looks like it's normally distributed. Even though you cannot know the distribution for sure, assume you have convinced yourself that the normal distribution is accurate. In that case, you still do not know the mean $$\mu$$ and variance $$\sigma^{2}$$, also called **distributional parameters**, of this distribution. Thus, we have to **estimate** these parameters.

As another example, suppose that the econometrician hypothesizes that two random variables $$X$$and $$Y$$are related in the following way:

$$Y = \beta_{0} + \beta_{1}X + u$$,

where $$Y$$is the **dependent variable**, $$X$$the **independent variable** and $$u$$ the **error term**. This model is called the **linear regression model**, as it assumes that the two random variables are linearly related. The error term $$u$$ takes into account that the relationship between $$X$$and $$Y$$is not perfectly linear (i.e. if we collect data, it does not lie perfectly on a line), but is rather scattered around a line. The only quantities we did not yet discuss are $$\beta_{0}$$and $$\beta_{1}$$, which we call **model parameters** or **model coefficients**. They are almost always unknown to the econometrician and thus have to be estimated.

To estimate both types of parameters mentioned above, we can employ estimation methods such as **ordinary least squares**, **maximum likelihood** and **methods of moments**. These estimation methods are derived under specific sets of assumptions, which makes them appropriate in different contexts. During the minor Applied Econometrics, you will learn more about this.

Using our estimates of the parameters and their corresponding standard errors, we can perform **inference**. This typically consists of performing statistical tests on coefficients. Revisiting the example of the linear regression model, we might want to test the null hypothesis $$H_{0}: \beta_{1}=0$$ (i.e. there is no relation between$$X$$and $$Y$$) versus the alternative hypothesis that there is a relationship, i.e. $$H_{1}: \beta_{1} \neq 0$$. This is called **hypothesis testing**.

Statistical tests can be interpreted in different ways. An econometrician typically sets a **significance level** beforehand (usually $$\alpha = 1\%, \ 5\%$$or $$10\%$$). To draw conclusions on whether to "reject" or "fail to reject" the null hypothesis, one has to compare the significance level to the **p-value** of the test. As an alternative to testing, we can also compute **confidence intervals** (around coefficients), which represents a range of estimates for an unknown parameter.&#x20;
