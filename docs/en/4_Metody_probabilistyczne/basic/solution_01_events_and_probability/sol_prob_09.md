# Task 9 — Weekly Weather Probabilities

Suppose the weather for each day can be **sunny (S), cloudy (C), or rainy (R)**, with equal probability:

$$
P(S) = P(C) = P(R) = \frac{1}{3}
$$

---

# 1. Sample Space

For **7 days (one week)**:

$$
\Omega_7 = \Omega^7
$$

Number of outcomes:

$$
|\Omega_7| = 3^7 = 2187
$$

Each outcome is an **ordered 7-tuple** representing weather each day.

Example:

$$
(S, C, R, S, S, C, R)
$$

---

# 2. Event Probabilities

---

## Event $A$: Weekend Sunny (Saturday and Sunday both sunny)

Each day is independent:

$$
P(A) = \frac{1}{3} \times \frac{1}{3} = \frac{1}{9}
$$

---

## Event $B$: Wednesday to Friday Rainy (three consecutive days rainy)

$$
P(B) = \frac{1}{3} \times \frac{1}{3} \times \frac{1}{3} = \frac{1}{27}
$$

---

## Event $C$: At Least One Sunny Day

Use the complement (no sunny days):

* Probability of **not sunny** in a day: $\frac{2}{3}$
* Probability of **no sunny day in 7 days**: $\left(\frac{2}{3}\right)^7$

$$
P(C) = 1 - \left(\frac{2}{3}\right)^7
$$

---

## Event $D$: No Rain All Week

* Probability of **not rainy** in a day: $\frac{2}{3}$
* Probability of **no rain in 7 days**: $\left(\frac{2}{3}\right)^7$

$$
P(D) = \left(\frac{2}{3}\right)^7
$$

---

## Event $E$: Exactly Two Sunny Days

Use **binomial formula**:

$$
P(E) = \binom{7}{2} \left(\frac{1}{3}\right)^2 \left(\frac{2}{3}\right)^5
$$

$$
P(E) = 21 \cdot \frac{1}{9} \cdot \frac{32}{243} = \frac{672}{2187}
$$

---

# 3. Possible Questions and Answers

---

### Question 1

**What is the probability that both Saturday and Sunday are sunny?**

Answer:

$$
P = \frac{1}{3} \times \frac{1}{3} = \frac{1}{9}
$$

---

### Question 2

**What is the probability that Wednesday, Thursday, and Friday are rainy?**

Answer:

$$
P = \frac{1}{27}
$$

---

### Question 3

**What is the probability of at least one sunny day in the week?**

Answer:

$$
P = 1 - \left(\frac{2}{3}\right)^7
$$

---

### Question 4

**What is the probability of no rain all week?**

Answer:

$$
P = \left(\frac{2}{3}\right)^7
$$

---

### Question 5

**What is the probability of exactly two sunny days?**

Answer:

$$
P = \binom{7}{2} \left(\frac{1}{3}\right)^2 \left(\frac{2}{3}\right)^5 = \frac{672}{2187}
$$

