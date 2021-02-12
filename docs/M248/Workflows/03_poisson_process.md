# The Poisson Process

## Using the Poisson process

We are given some process that occurs in real time with a rate $\lambda$, and asked to identify the probability of some event occuring within some time interval.

### Number of events

**Workflow:**

1. **Formalise the rate.** Pay attention to the *unit of time.*
2. **Determine the rate in question.** Is the time interval in the question the same as that of that for the rate given in (1)? If it is *not,* then use $\lambda t$, where $t$ is the conversion factor between the units of time.
3. **Parse the probability.** Express it in terms involving either $p(x)$ or $F(x)$, using Use $X \sim \text{Poisson}(\lambda t)$.
4. **Solve the equation.**

### Waiting time between events

**Workflow:**

1. **Formalise the rate.** Pay attention to the *unit of time.*
2. **Parse the probability.** Express it in terms involving of $F(t)$. Use $T \sim M(\lambda)$ (do not use $\lambda t$).
3. **Solve.**

## Confirming the Poisson process is a good model

**Use case:** We are presented with some data, and asked to confirm if the data conforms to the Poisson process

**Workflow:** Perform the following visual checks:

1. **Rate of occurrence is linear.** Plot a scatterplot of Events against Time.
2. **Number of events $\to$ Poisson distribution.** Plot a bar chart of Number of Events per Time Interval *(same time interval as rate).*
3. **Waiting time between events $\to$ exponential distribution.** Plot a frequency histogram of Waiting Times.

Also check that for the

- **Number of events**: $E(X) = V(X)$ (see properties of the Poisson distribution)
- **Waiting time between events**: $E(T) = S(T)$ (see properties of the exponential distribution)
