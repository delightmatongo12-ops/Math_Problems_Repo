# Task 3 — Drawing Cards from a Deck

A standard deck contains **52 cards** consisting of:

* 4 suits: hearts, diamonds, clubs, spades
* 13 ranks in each suit

Thus the total number of cards is

$$
52 = 4 \times 13
$$

---

# 1. Sample Space for One Card

The sample space contains **all 52 cards**.

$$
\Omega_1 = {\text{all 52 cards}}
$$

Number of outcomes:

$$
|\Omega_1| = 52
$$

Example elementary outcomes:

* Ace of Hearts
* 7 of Clubs
* King of Spades

Each outcome represents **one specific card drawn**.

---

# 2. Sample Space for Two Cards (With Replacement)

After the first card is drawn, it is **returned to the deck**, so the second draw again has **52 possibilities**.

The sample space is

$$
\Omega_2 = \Omega_1 \times \Omega_1
$$

Number of outcomes:

$$
|\Omega_2| = 52^2
$$

$$
|\Omega_2| = 2704
$$

Example outcome:

$$
(\text{Ace of Hearts},\ \text{King of Spades})
$$

Meaning:

* first draw = Ace of Hearts
* second draw = King of Spades

---

# 3. Sample Space for Two Cards (Without Replacement)

If the first card is **not returned**, the second draw has only **51 possibilities**.

Number of outcomes:

$$
|\Omega_2| = 52 \times 51
$$

$$
|\Omega_2| = 2652
$$

Example outcome:

$$
(\text{Queen of Hearts},\ \text{7 of Clubs})
$$

Meaning:

* first draw = Queen of Hearts
* second draw = 7 of Clubs

---

# 4. Meaning of an Elementary Outcome

An **elementary outcome** describes the **exact ordered sequence of drawn cards**.

Example:

$$
(\text{10 of Diamonds},\ \text{Ace of Spades})
$$

This means:

* first card = 10 of Diamonds
* second card = Ace of Spades

---

# Possible Questions and Answers

---

## Question 1

**How many possible outcomes exist when drawing one card?**

Answer:

$$
|\Omega_1| = 52
$$

---

## Question 2

**How many ordered outcomes exist when drawing two cards with replacement?**

Answer:

$$
52^2 = 2704
$$

---

## Question 3

**How many ordered outcomes exist when drawing two cards without replacement?**

Answer:

$$
52 \times 51 = 2652
$$

---

## Question 4

**Why is the sample space smaller without replacement?**

Answer:

Because the first drawn card **cannot appear again**, reducing the possibilities for the second draw from **52 to 51**.

---

## Question 5

**What does the outcome**

$$
(\text{King of Clubs},\ \text{5 of Hearts})
$$

**represent?**

Answer:

* first card drawn = King of Clubs
* second card drawn = 5 of Hearts



