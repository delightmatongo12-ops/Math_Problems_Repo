# Task 8 — Probabilities with Cards

A standard deck has **52 cards**:

* 4 suits: hearts, diamonds, clubs, spades
* 13 ranks in each suit

---

# 1. One Card Draw

## Sample Space

$$
\Omega_1 = {\text{all 52 cards}}
$$

Number of outcomes:

$$
|\Omega_1| = 52
$$

---

## Events

### Event $A_1$: Drawing a Heart

Number of hearts:

$$
|A_1| = 13
$$

Probability:

$$
P(A_1) = \frac{13}{52} = \frac{1}{4}
$$

---

### Event $B_1$: Drawing a King

Number of kings:

$$
|B_1| = 4
$$

Probability:

$$
P(B_1) = \frac{4}{52} = \frac{1}{13}
$$

---

### Event $C_1$: Not a Face Card

Face cards = 12 (J, Q, K in each suit)

Number of non-face cards:

$$
|C_1| = 52 - 12 = 40
$$

Probability:

$$
P(C_1) = \frac{40}{52} = \frac{10}{13}
$$

---

# 2. Two Cards Drawn With Replacement

Each draw has 52 possibilities, and the **first card is returned**.

### Event $A_2$: Both Cards are Hearts

$$
P(A_2) = \frac{1}{4} \times \frac{1}{4} = \frac{1}{16}
$$

---

# 3. Two Cards Drawn Without Replacement

The second draw has 51 remaining cards.

### Event $A_3$: Both Cards are Hearts

$$
P(A_3) = \frac{13}{52} \cdot \frac{12}{51}
$$

$$
P(A_3) = \frac{156}{2652} = \frac{1}{17}
$$

---

# Possible Questions and Answers

---

## Question 1

**What is the probability of drawing a heart from a deck?**

Answer:

$$
P = \frac{13}{52} = \frac{1}{4}
$$

---

## Question 2

**What is the probability of drawing a king?**

Answer:

$$
P = \frac{4}{52} = \frac{1}{13}
$$

---

## Question 3

**What is the probability of drawing two hearts with replacement?**

Answer:

$$
P = \frac{1}{4} \times \frac{1}{4} = \frac{1}{16}
$$

---

## Question 4

**What is the probability of drawing two hearts without replacement?**

Answer:

$$
P = \frac{13}{52} \cdot \frac{12}{51} = \frac{1}{17}
$$

---

## Question 5

**Why is the probability different with and without replacement?**

Answer:

* **With replacement**: the deck is **restored**, so probabilities remain the same for both draws.
* **Without replacement**: the first card **reduces the total and the number of hearts**, so the probability changes.

