# Probability Distributions

## Checking the validity of a probability distribution

We are given some probability distribution (either a p.m.f. or a p.d.f.), and we are asked to confirm it is valid.

Check if the properties of a p.m.f. or p.d.f. hold true.

**Propertis of discrete random variables:**

1. $\sum_x p(x) = 1$
2. $p(x) \in (0,1]$

**Propertis of continuous random variables:**

1. $\int f(x) = 1$, over the range of $X$
2. $f(x) \in (0,1)$

## Normalising constants

### Calculating a normalising constant

We are given a p.d.f. $f(x)$, and asked to calculate the normalising constant $\dfrac{1}{k}$ so the p.d.f. is valid.

1. Solve $k = \int_{a}^{b} f(x) \> dx$

### Confirming the use of a normalising constant

We are given some p.d.f. $\frac{1}{k} f(x)$, and asked to confirm the validity.

See *Checking the validity of a probability distribution > Continuous.*

## Using standard probability models

We are given a scenario, and asked to calculate the probability of some event.

1. **Identify the distribution.** (If it is not given in the question.)
2. **Map the parameters.**
3. **Parse the probability.** Translate it into some form involving either $p(x), f(x)$, or $F(x)$.
4. **Solve the equation(s).**

Note do not forget to state any approximation in the final statement.

## Expected value and variance

We are asked to calculate the expected value or variance of some probability distribution by hand.

Note to find the the standard deviation $S(X)$, take the square root of $V(X)$.

### Discrete

**Expected value:**
$E(X) = \sum_{x} x \> p(x)$.

1. **Calculate** $xp(x)$ for each element of $X$.
2. **Sum the values.**

**Variance:**
$V(X) = E(X^{2}) - E(X)^{2}$.

1. **Calculate** $x^{2} p(x)$ for each element of $X$.
2. **Sum the values of** $x^{2} p(x)$. This gives $E(X^{2})$
3. **Calculate** $E(X)$. *See above.*
4. **Calculate** $E(X^{2}) - E(X)^{2}$.

### Continuous

**Expected value:**
$E(X) = \int_{a}^{b} x \> f(x)$.

1. **Integrate** $\int_{a}^{b} x \> f(x)$, where $a, b$ are the boundaries of $X$.

**Variance:**
$V(X) = E(X^{2}) - E(X)^{2}$.

1. **Integrate** $\int_{a}^{b} x^{2} \> f(x)$, where $a, b$ are the boundaries of $X$. This gives $E(X^{2})$.
2. **Calculate** $E(X)$. *See above.*
3. **Calculate** $E(X^{2}) - E(X)^{2}$.

## Linear transformations

We are given a random variable $Y$ expressed as a linear transformation of some other random variable $X$, such that $Y = aX + b$, and $a, b$ are known constants.

**Expected value:**
Calculate $E(Y) = aE(X) + b$.

**Variance:**
Calculate $V(Y) = a^{2} E(X)$.

Note to find the the standard deviation $S(Y)$, take the square root of $V(Y)$.

## Population quantiles

We are given a probability distribution, and asked to calculate some $\alpha-$quantile of the distribution.

### Discrete

**To add.**

### Continuous

1. **Find the c.d.f.** (if it is not given in the question)
2. **Convert the quantile to** $\alpha \in (0,1)$, if it is given as a percentage or description (e.g., lower sampler quartile)
3. **Solve** $q_{\alpha} = F^{-1}(\alpha)$ by rearranging $F(q_{\alpha}) = \alpha$
