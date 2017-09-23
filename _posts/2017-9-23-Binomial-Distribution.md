---
layout: post
title: The Binomial distribution
date: 2017-09-23
---

## 1. Binomial Experiments

Binomial distribution is the discrete probability distribution. If we want to know what is binomial distribution, we must know what is *binomial experiments*.

As the *"bi"* in *"binomial"* suggests, each 'mini-experiment' (or **trial**) in a binomial experiment can result in one of only two possible outcomes.

An everyday example of a binomial experiment is tossing a coin, where the result will be either *heads* or *tails*. If we assume that the coin is not biased towards either outcome (that is, it is **fair**), then the **probability** of getting either heads or tails will be the same every time it is tossed. If such a coin is flipped again and again, the outcomes will follow what's know as a *binomial distribution*.## 2. *Toss a coin!*
In this section, let's try to imagine a few experiments where we flip a fair coin.

---

#### Experiment A. We toss a fair coin once. There are two possible outcomes:

> $$H,T$$
> where $H$ = heads and $T$ = tails.

As discussed above, the probability for each is $p=\frac{1}{2}$.

| Event | Number of outcomes | Probability for each  | Probability of event| 
| :--------: | :--------: | :--------: | :--------: |
| Zero Head     |  $1$    |    $1/2$ | $1/2$|
| One Head   |  $1$  |    $1/2$ | $1/2$|

---

#### Experiment B. We toss a fair coin twice. There are four possible outcomes:

> $$(H,H), (H,T), (T,H), (T,T)$$

As we see in experiment *A*, the probability of H or T each time we flip this coin is still $p=\frac{1}{2}$.

So for each of the four above outcomes, we have the same probability:

$$ P = p^2 = \left(\frac{1}{2}\right)^2 = \left(\frac{1}{2}\right)\left(\frac{1}{2}\right) = \frac{1}{4} $$

| Event | Number of outcomes | Probability for each  | Probability of event| 
| -------- | -------- | -------- | -------- |
| Zero Head     |  $1$    |    $1/4$ | $1/4$|
| One Head   |  $2$  |    $1/4$ | $1/2$|
| Two Head |  $1$  |    $1/4$ | $1/4$|

--- 

#### Experiment C. We toss a fair coin three times. There are eight possible outcomes:

> $$ (H,H,H), (H,H,T), (H,T,T), (H,T,H), (T,H,H), (T,H,T), (T,T,T), (T,T,H)$$

For every H or T, the probability of it is 
$$p = \frac{1}{2}$$
So each outcomes (above eight outcomes), have the same probability:
$$ P= p^3=\frac{1}{8}$$

Notice that the order of the output did not matter, so we can sort out outcomes:

| Event | Number of outcomes | Probability for each  | Probability of event| 
| -------- | -------- | -------- | -------- |
| Zero Head     |  $1$    |    $1/8$ | $1/8$|
| One Head   |  $3$  |    $1/8$ | $3/8$|
| Two Head |  $3$  |    $1/8$ | $3/8$|
| Three Head |  $1$    |    $1/8$ | $1/8$|

---

##### We could go on imaging experiments like this forever. Instead, let's stop here and see if we can figure out a *formula* that captures what we've seen in this section.

## 3. Formula: Probability mass function

We define the random variable $X$ as the number of Heads that happen, and follow the binomial distribution. 

The number of experiments is parameter $n$. $n$ is contained in the natural numbers. $n ∈ ℕ$.

And $p$ is the probability of each outcome $H, p ∈ [0,1]$
$$X \sim B(n, p)$$

$$P(X=x)={n \choose x}p^x(1-p)^{n-x}$$

$${n \choose x} =\frac{n!}{x!(n-x)!}$$

You can use this formula to calculate our three experiment's outcomes again, and you will get the same result.

For example, in experiment C, 
$$n =3,  p=0.5 $$
$$P(Zero head)=P(X=0)=\frac{3!}{0!(3-0)!}0.5^0(1-0.5)^{3-0}=\frac{1}{8}$$

$$P(One head)=P(X=1)=\frac{3!}{1!(3-1)!}0.5^1(1-0.5)^{3-1}=\frac{3}{8}$$

$$P(Two head)=P(X=2)=\frac{3!}{2!(3-2)!}0.5^2(1-0.5)^{3-2}=\frac{3}{8}$$

$$P(Three head)=P(X=3)=\frac{3!}{3!(3-3)!}0.5^3(1-0.5)^{3-3}=\frac{1}{8}$$

The results are totally the same as above.


## 4.Mean and variance




## 5. Limitations:

Binomial distribution as a tool, can easily get the probability for experiments that have large number of trails. But we must notice that Binomial distribution cannot apply to all experiments. 

For tossing a coin, binomial distribution must follow the conditions below:

1. Do $n$ experiments.
2. Every experiment only has two outcomes. (Outcome H and T)
3. The probability of every time we get H is same. (Probability $P$)
4. Each experiment is independent.




Thanks for reading and hopefully this is useful to you.