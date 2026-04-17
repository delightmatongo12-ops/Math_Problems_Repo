# 🔷 1. From concrete experiments to abstraction

In the previous problems, we worked on three levels:

### (1) Elementary outcomes and events

We introduced:

* a **sample space**:
  $$
  \Omega
  $$
* and **events** as subsets:
  $$
  A \subseteq \Omega
  $$

This step already transforms a real experiment into a **mathematical object**.

---

### (2) Observed frequencies

From repeated experiments, we defined:

$$
f(A) = \frac{n(A)}{N}
$$

These frequencies revealed important patterns:

* non-negativity:
  $$
  f(A) \ge 0
  $$

* normalization:
  $$
  f(\Omega) = 1
  $$

* additivity for disjoint events:
  $$
  A \cap B = \varnothing ;\Rightarrow; f(A \cup B) = f(A) + f(B)
  $$

* complementarity:
  $$
  f(A^c) = 1 - f(A)
  $$

---

### (3) Need for abstraction

However, frequencies depend on:

* a **specific experiment**,
* a **finite number of trials**.

We now want a concept that:

* does not depend on a particular dataset,
* describes the **expected behavior**.

This leads to **probability as an abstract function**.

---

# 🔷 2. The axiomatic definition of probability

We introduce a function:

$$
P : \mathcal{P}(\Omega) \to [0,1]
$$

which assigns a number to every event.

This function must satisfy the **Kolmogorov axioms**.

---

# 🔷 3. The Kolmogorov axioms

## 🔶 Axiom 1 — Non-negativity

For every event $A \subseteq \Omega$:

$$
P(A) \ge 0
$$

### Interpretation

Probability cannot be negative.

### Connection to earlier work

From frequencies:

$$
f(A) = \frac{n(A)}{N} \ge 0
$$

So this axiom directly reflects empirical observation.

---

## 🔶 Axiom 2 — Normalization

$$
P(\Omega) = 1
$$

### Interpretation

Something must happen in every trial.

### Connection to frequencies

We observed:

$$
f(\Omega) = 1
$$

because every experiment produces exactly one outcome.

---

## 🔶 Axiom 3 — Countable additivity

If $(A_i)$ is a sequence of **pairwise disjoint events**, then:

$$
P\left(\bigcup_{i=1}^{\infty} A_i\right)
========================================

\sum_{i=1}^{\infty} P(A_i)
$$

---

### Interpretation

If events do not overlap, their probabilities **add up**, even for infinitely many events.

---

# 🔷 4. What we already discovered earlier

From Problem 5, we already had:

### ✔ Finite additivity

For disjoint $A$ and $B$:

$$
P(A \cup B) = P(A) + P(B)
$$

This came directly from:

$$
n(A \cup B) = n(A) + n(B)
$$

when $A \cap B = \varnothing$.

---

### ✔ Complement rule

From earlier:

$$
P(A^c) = 1 - P(A)
$$

This follows from:

$$
\Omega = A \cup A^c, \quad A \cap A^c = \varnothing
$$

---

### ✔ Partition of the sample space

If:

$$
\Omega = A_1 \cup \cdots \cup A_k
$$

(disjoint), then:

$$
\sum_{i=1}^k P(A_i) = 1
$$

---

# 🔷 5. What is new: countable additivity

The key new element is:

$$
P\left(\bigcup_{i=1}^{\infty} A_i\right)
========================================

\sum_{i=1}^{\infty} P(A_i)
$$

---

## 🔶 Why this does NOT come from earlier problems

In earlier tasks:

* $\Omega$ was **finite**,
* all unions were **finite**,
* all sums were finite.

So we only observed:

$$
P(A_1 \cup \cdots \cup A_k)
===========================

\sum_{i=1}^k P(A_i)
$$

---

## 🔶 Why countable additivity is deeper

It applies to:

* **infinitely many events**,
* possibly in **infinite sample spaces**.

This cannot be:

* directly observed in experiments,
* derived from finite data.

It is a **purely mathematical extension**.

---

## 🔶 Conceptual meaning

Countable additivity ensures:

* consistency when passing to limits,
* compatibility with infinite processes,
* foundation for advanced theory (integration, random variables, etc.).

---

# 🔷 6. Why axioms are necessary

The axioms:

* do not depend on a specific experiment,
* guarantee internal consistency,
* allow probability to be studied as a **mathematical structure**.

They replace:
$$
\text{empirical regularity}
\quad \longrightarrow \quad
\text{formal rule}
$$

---

# 🔷 7. Summary of the connection

We can now clearly describe the transition:

---

## 🔶 Level 1: Outcomes and events

$$
\Omega, \quad A \subseteq \Omega
$$

Pure structure — no numbers yet.

---

## 🔶 Level 2: Frequencies

$$
f(A) = \frac{n(A)}{N}
$$

* based on data,
* approximate,
* reveal patterns.

---

## 🔶 Level 3: Probability

$$
P(A)
$$

* abstract,
* exact,
* defined by axioms.

---

# 🔷 8. Final conceptual conclusion

The Kolmogorov axioms are not arbitrary.

They are:

* **motivated by observed frequencies**,
* **generalized beyond finite experiments**,
* **extended to infinite settings**.

---

## 🔶 Core insight

* Non-negativity comes from counting.
* Normalization comes from total outcomes.
* Finite additivity comes from disjoint counting.
* Countable additivity goes **beyond observation** — it is a structural requirement for a coherent theory.

---

# ✅ Final statement

Probability theory is the result of the transition:

$$
\text{experiment}
;\longrightarrow;
\text{frequency}
;\longrightarrow;
\text{axiomatic structure}
$$

where the Kolmogorov axioms provide the **formal framework** that captures and extends the regularities observed in real-world experiments.
