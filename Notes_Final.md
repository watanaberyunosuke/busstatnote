# Business Statistic Notes

Week 1 is missing due to inrelevancy.

## Week 2

Numerical Descriptive Measures:

Central Tendency:

1. Arithmetic Mean
2. Median
3. Mode

### Mean

$$\overline{X}=\frac { \sum_{i=1}^{n}X_i }{ n } = \frac{ X_1+X_2+\ldots+X_n } { n }$$

### Median

In an ordered array, the median is the 'middle' number (50% above, 50% below).

Its main advantage over the arithmetic mean is that it is not affected by extreme values

$$Median=\frac{ n+1 }{ 2 }\qquad$$

### Mode

- A measure of central tendency
- Value that occurs **most often** (the most frequent)
- Not affected by extreme values

#### Which Measure of Location is the 'best' in this situation

- The mean is generally used most often, unless extreme values (outliers) exist
- The median is often used, since it is not sensitive to extreme values
- The mode is usually the least used of the three

### Quartile

Quartiles split the ranked data into four segments, with an equal number of values per segment

First quartile position: $Q1 = \frac{ n+1 } { 4 }$

Second quartile position: $Q2 = \frac{(n+1)} {2}$ (the median)

Third quartile position: $Q3 = \frac {3(n+1)} {4}$

where n is the number of observed values (sample size)

### Measure of Variation

- Range
- Inter Quartile Range
- Variance
- Standard Deviation
- Coefficient of Variation

Measures of variation give information on the spread or variability of the data values

$Range = X_{Largest} - X_{Smallest}$

$IQR = Q_3 - Q_1 = 3^{rd}quartile - 1^{st}quartile$

***The Sample Variance*** $S^{2} =\frac { \sum\limits_{i=1}^{n}(X_i - \overline {X})^{2} }{ n }$

- $\overline {X}$ = mean

- $n$ = sample size

- $X_i$ = $i^{th}$ value of the variable x

The Sample Standard Deviation - S

$$S = \sqrt\frac { \sum\limits_{i=1}^{n}(X_i - \overline {X})^{2} }{ n }$$

Coefficient of Variation

$$ CV = (\frac{ S }{ \overline X} \cdot 100) = \frac { \sigma } { \mu } $$

#### Z Score

The difference between a given observation and the mean, divided by the standard deviation

$$Z = \frac { X - \overline X} {S}$$

#### Numerical Measures for a Population

Population summary measures are called parameters

The population mean is the sum of the values in the population divided by the population size, N, calculated by following

$$ \mu = \frac {\sum\limits_{i=1}^{N} X_i} {N} = \frac{X_1+X_2+\ldots+X_N}{N}$$

## Week 3

## Basic Probability

### Concepts

**Probability**: a numerical value that represent the likelihood of an event occurring.

There are two type of events: **Impossible Event** and **Certain Event**. Which the first one is an event that can not occur, while later is the one that will occur.

There are also three approach of probability:

1. *Priori* Classical Probability: Objective probability based on prior knowledge and experience: e.g. toss a coin, head 50% tail 50%.
2. Empirical Classical Probability: Objective probability, obtained from the relative frequency of occurrence of an event. e.g. probability of Toyota pass a crossing.
3. Subjective Probability: probability that reflect an individual's belief that an event occurs. e.g. 'I think England have 70% in beating NZ tonight.'

The **probability of occurrence** can be defined as:

Probability of Occurrence $= \large\frac{X}{T}$</br> Where: *X* = number of ways in which the event will occurs *T* = total number of possible outcomes

### Event and Sample Space

**Random experiment**: a precise describe scenario that leads to an outcome that cannot be predicted with certainty.

**Event**: an event is one or more outcomes of a random experiment.

**Simple Event**: a single outcome of a random experiment.

**Sample Space**: collection of all sample events.

**Joint Event**: an event described by two or more characteristics.

From the concepts above we can know that:</br>

``` {.mermaid}
graph LR;
    A[Random Experiment]-- Generate -->B[Event];
    A[Random Experiment]-- Generate -->C[Simple Event];
    A[Random Experiment]-- Generate -->D[Joint Event];
    D[Joint Event]-- Result -->E[Sample Space];
    C[Simple Event]-- Result -->E[Sample Space];
    B[Event]-- Result-->E[Sample Space];
```

**Complement** of event A (written in A'): include all simple event that are not included in the event A.

### Graphing Possibilities, Contingency Table and Venn Diagram

**Contingency Table** table that represents a sample space for joint events classified by two characteristics; Each cell represent the joint event satisfying given values of both characteristics.

Example on page 114 of textbook

**Venn Diagram** is the graphical representation of a sample space;joint events shown as 'unions'(symbol $\cup$) and 'intersections'(Symbol $\cap$) of circles representing simple events

Example on page 115 of textbook

## Week 4

### Time Series Analysis

#### Laspeyres Index

Laspeyres index is being calculated by the formula below:

$$P_L=\frac {\sum (P_{c,t_n})*(q_c,t_0) }{\sum(P_{c,t_0})*{(q_c,t_0)}}$$

#### Paasche Index

Paasche index is being calculated by the formula below:

$$P_P=\frac {\sum (P_{c,t_n})*(q_c,t_n) }{\sum(P_{c,t_0})*{(q_c,t_n)}}$$

### Probability Distributions

#### Random Variable

There are discrete random variable and continuous random variable

discrete variable fall into numbers, while continuous random variable fall into the range.

## Distribution

3 type of distribution:

- Normal Distribution (sometimes referred as the *Gaussian* distribution)

- Uniform Distribution

- Exponential Distribution

Only Normal Distribution will be discussed in this chapter.

### The Standardised Normal Probability Density Function

the **Continuous Probability Density Function**: It is the mathematical expression that defines the distribution of the values for a continuous random variable.

If mean = medium, the range satisfied standard distribution.

See 6.1 of textbook

$$ f(Z) = \frac{1} {\sqrt{2\pi}}e^{-(\frac{1}{2})Z^2} $$

this formula can be transformed into:

$$f(X) = \frac{1} {\sqrt{2\pi}}e^{-(\frac{1}{2}) [\frac{(X-\mu)}{\sigma})]^2}$$

### the Transformation Formula

Check textbook 6.2 for definition.

Any normal distribution (with any mean and standard deviation combination) can be transformed into the standardised normal distribution (Z).</br> Z score formula can be used to convert any normal random variable to the standardised normal random variable.

*Z* can be expressed as : $Z = \frac{X-\mu}{\sigma}$

By finding an X value associated with known probability

$$X = \mu+Z\sigma$$

While:

*Z* is Z value</br> *X* is the normal random variable</br> $\mu$ is the mean of the range</br> $\sigma$ is the standard deviation

### the Normal Distribution

**Normal distribution** is a continuous probability distribution with the following theoretical property:

1. Represented by a bell-shaped curve.
2. It's mean and medium are equal
3. Its middle 50% of data is within approximately $\large\frac{4}{3}$standard deviations. This means that the IQR is contained within an interval of $\large\frac{2}{3}$of a standard deviation below the mean to $\large\frac{2}{3}$ of a standard deviation above the mean - that is, the middle 50% of data have Z scores $-\large\frac{2}{3} < Z < \frac{2}{3}$
4. Its associated random variables has an infinity range ($-\infty < X < \infty$)

## Z Score Table

The table only tell the left area of some number.

The application are shown on textbook example 6.1 to 6.7.

Calculation:</br>

1. Calculate Z value from the formula above.
2. Then find Z value on the table, mind first digit and second digit
3. Get result.</br>

*N.B.* remind that Z score table is giving the value to the left hand side area of standard deviation distribution graph.

### 68-95-99.7 Rule

In normal distribution, 68.27%, 95.45% and 99.73% of the values lie within one, two and three standard deviations of the mean.

Mathematically:

${\displaystyle{\begin{aligned}\Pr(\mu -\;\,\sigma \leq X\leq \mu +\;\,\sigma )&\approx 0.6827\\\Pr(\mu -2\sigma \leq X\leq \mu +2\sigma )&\approx 0.9545\\\Pr(\mu -3\sigma \leq X\leq \mu +3\sigma )&\approx 0.9974\end{aligned}}}$

## Week 6

### Sampling Method

Convenience sample:

- Street Survey
- Online

Both of the samples are biased

**Unbiased** are defined as: if the average of all possible sample means of given sample size *n* ($\mu_{\overline{X}}$) equals the population mean($\mu$), then the sample mean is unbiased.

### Sampling Distribution

A **sampling distribution** is a distribution of all of the possible values of a statistic for a given size sample selected from a population.

**Sampling distribution of the mean** is the distribution of all possible sample means from samples of a given size for a given population.

**Population Mean** is the sum of the values in the population divided by the population size *N*.

### Hands on Developing a Sampling Distribution

Assume there is a population:

    Population size N=4

    Random variable, X, is age of individuals.

    Values of X: 18, 20, 22, 24 (years).

#### Summary

$\mu = \frac{\sum X_i}{N} = \frac{18+20+22+24}{4} = 21$

$\sigma = \sqrt{\frac{\sum(X_i - \mu)^2}{N}} = 2.236$

The result generate a uniform distribution
