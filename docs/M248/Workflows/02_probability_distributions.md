# Probability Distributions

## Checking the validity of a probability distribution

We are given some probability distribution (either a p.m.f. or a p.d.f.), and we are asked to confirm it is valid.

**Workflow:**
Check if the properties of a p.m.f. or p.d.f. hold true.

### Discrete

1. $\sum_x p(x) = 1$
2. $p(x) \in (0,1]$

### Continuous

1. $\int f(x) = 1$, over the range of $x$
2. $f(x) \in (0,1)$

## Calculating a normalising constant

We are given a p.d.f. $f(x)$, and asked to calculate the normalising constant $k$ so the p.d.f. is valid.

**Workflow:**
Solve $k = \int_{a}^{b} f(x) \> dx$

**Rationale:**
We know by the definition of the c.d.f. that

$$
1 = \int_{a}^{b} f(x) \> dx.
$$

Therefore, if the p.d.f. is $\frac{1}{k} f(x)$, then it must be that

$$
\begin{aligned}
    1 &= \int_{a}^{b} \frac{1}{k} f(x) \> dx \\
    &= \frac{1}{k} \int_{a}^{b} f(x) \> dx \\
    k &= \int_{a}^{b} f(x) \> dx.
\end{aligned}
$$

## Confirming the use of a normalising constant

We are given some p.d.f. $\frac{1}{k} f(x)$, and asked to confirm the validity.

**Workflow:**
See *Checking the validity of a probability distribution > Continuous.*

## Population quantiles

We are given a robability distribution, and asked to calculate some $\alpha-$quantile of the distribution.

### Discrete

**To add.**

### Continuous

**Workflow:**

1. **Find the c.d.f.** (if it is not given in the question)
2. **Convert the quantile to** $\alpha \in (0,1)$, if it is given as a percentage or description (e.g., lower sampler quartile)
3. **Solve** $q_{\alpha} = F^{-1}(\alpha)$ by rearranging $F(q_{\alpha}) = \alpha$

**Example.** Find the lower quartile of the continuous rv $X$ with p.d.f.

$$
f(x) = x^{2}, \hspace{3mm} x \in ( 0,\sqrt[3]{3} ).
$$

The c.d.f. of $X$ is given by

$$
\begin{aligned}
    F(x) = \int_{0}^{x} y^{2} \> dy &= \bigg[ \frac{1}{3} y^{3} \bigg]_{0}^{x} \\ &= \frac{1}{3} x^{3} - \frac{1}{3} (0^{3})
    \\ &= \frac{1}{3} x^{3}.
\end{aligned}
$$

Let $q_{\alpha}$ be the value of $X$ that corresponds to the $\alpha-$quantile of $X$.
The lower quartile is the 0.25-quantile, so

$$
\begin{aligned}
    F(q_{0.25}) &= 0.25 \\
    \frac{1}{3} q_{0.25}^{3} &= 0.25 \\
    q_{0.25}^{3} &= 0.75 \\
    q_{0.25} &= \sqrt[3]{0.75} \simeq 0.909.
\end{aligned}
$$

## Using Standard Probability Models

We are given a scenario, and asked to calculate the probability of some event.

**Workflow:**

1. **Identify the distribution.** (If it is not given in the question.)
2. **Map the parameters.**
3. **Parse the probability.** 9Translate it into some form involving either $p(x), f(x)$, or $F(x)$.
4. **Solve the equation(s).**

Note, do not forget to state any approximation in the final statement.
