# Task 1 

Let the set of possible outcomes of a **single coin toss** be

$$
\Omega = {H, T}
$$

where
$H$ = heads,
$T$ = tails.

---

## One Toss

The sample space is

$$
\Omega_1 = \Omega = {H, T}
$$

and

$$
|\Omega_1| = 2
$$

---

## Two Tosses

The sample space is the **Cartesian product**

$$
\Omega_2 = \Omega \times \Omega
$$

Thus

$$
\Omega_2 =
{(H,H),(H,T),(T,H),(T,T)}
$$

and

$$
|\Omega_2| = 2^2 = 4
$$

---

## Three Tosses

The sample space becomes

$$
\Omega_3 = \Omega \times \Omega \times \Omega = \Omega^3
$$

Thus

$$
\Omega_3 =
{(H,H,H),(H,H,T),(H,T,H),(H,T,T),
(T,H,H),(T,H,T),(T,T,H),(T,T,T)}
$$

and

$$
|\Omega_3| = 2^3 = 8
$$

---

## General Case

For $n$ coin tosses

$$
\Omega_n = \Omega^n
$$

and the number of elementary outcomes is

$$
|\Omega_n| = 2^n
$$

---

## Meaning of an Elementary Outcome

An **elementary outcome** is one element of $\Omega_n$ describing the **exact sequence of results**.

Example:

$$
(H,T,H) \in \Omega_3
$$

means:

* first toss: heads
* second toss: tails
* third toss: heads

---

# Possible Questions for Task 1

## 1. Define the sample space

Example question:

> Define the sample space for $n$ tosses of a fair coin.

Answer idea:

$$
\Omega = {H,T}
$$

For $n$ tosses:

$$
\Omega_n = \Omega^n
$$

---

# 2. List all elementary outcomes

Example:

> List all elementary outcomes for two coin tosses.

$$
\Omega_2 =
{(H,H),(H,T),(T,H),(T,T)}
$$

---

# 3. Determine the size of the sample space

Example question:

> How many elementary outcomes are there after $n$ tosses?

Answer:

$$
|\Omega_n| = 2^n
$$

Example:

* $n=1 \Rightarrow 2$
* $n=2 \Rightarrow 4$
* $n=3 \Rightarrow 8$

---

# 4. Define an event

Example question:

> Define the event that exactly one head occurs in two tosses.

Event:

$$
A = {(H,T),(T,H)}
$$

---

# 5. Probability of an event

Example:

> What is the probability of exactly one head in two tosses?

Since

$$
|\Omega_2| = 4
$$

and

$$
|A| = 2
$$

then

$$
P(A) = \frac{2}{4} = \frac{1}{2}
$$

---

# 6. Probability of at least one head

Example question:

> What is the probability of getting at least one head in three tosses?

Event:

$$
A = \Omega_3 \setminus {(T,T,T)}
$$

So

$$
P(A) = 1 - \frac{1}{8} = \frac{7}{8}
$$

---

# 7. Probability of exactly $k$ heads

Example question:

> What is the probability of exactly $k$ heads in $n$ tosses?

This follows the **binomial distribution**:

$$
P(X = k) =
\binom{n}{k} \left(\frac{1}{2}\right)^n
$$

---

# 8. Describe outcomes using random variables

Example question:

> Let $X$ be the number of heads in three tosses. What are possible values?

$$
X \in {0,1,2,3}
$$

---

# 9. Complement events

Example question:

> What is the complement of the event “at least one head”?

Complement:

$$
A^c = {(T,T,T)}
$$

---

💡 **Most likely exam questions** from such a task are:

1. Write the **sample space $\Omega_n$**
2. Compute **$|\Omega_n|$**
3. Define an **event as a subset of $\Omega_n$**
4. Compute a **probability**
5. Count sequences with **exactly $k$ heads**




