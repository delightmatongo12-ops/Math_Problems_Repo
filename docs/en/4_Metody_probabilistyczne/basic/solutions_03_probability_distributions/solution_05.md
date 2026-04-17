# 🔷 Given data and framework

We are given results of **1000 throws of a fair die**.

The sample space is:

$$
\Omega = {1,2,3,4,5,6}
$$

The observed counts:

$$
n({1})=168,\quad
n({2})=154,\quad
n({3})=181,
$$

$$
n({4})=167,\quad
n({5})=160,\quad
n({6})=170.
$$

---

## 🔷 Definition of observed frequency

For any event $A \subseteq \Omega$:

$$
f(A) = \frac{n(A)}{1000}
$$

where:

* $n(A)$ = number of occurrences of outcomes in $A$,
* $f(A)$ = **observed frequency**.

---

# 🔷 Part A — From elementary outcomes to events

We compute:

1. $n(A)$ by summing counts,
2. then $f(A)$.

---

## **1. $A = {2,4,6}$**

### Step 1: Count occurrences

$$
n(A) = n({2}) + n({4}) + n({6})
$$

$$
n(A) = 154 + 167 + 170 = 491
$$

### Step 2: Frequency

$$
f(A) = \frac{491}{1000} = 0.491
$$

---

## **2. $B = {1,2,3}$**

$$
n(B) = 168 + 154 + 181 = 503
$$

$$
f(B) = \frac{503}{1000} = 0.503
$$

---

## **3. $C = {5,6}$**

$$
n(C) = 160 + 170 = 330
$$

$$
f(C) = \frac{330}{1000} = 0.33
$$

---

## **4. $D = {1,3,5}$**

$$
n(D) = 168 + 181 + 160 = 509
$$

$$
f(D) = \frac{509}{1000} = 0.509
$$

---

## **5. $E = {1,2,3,4}$**

$$
n(E) = 168 + 154 + 181 + 167 = 670
$$

$$
f(E) = \frac{670}{1000} = 0.67
$$

---

# 🔷 Part B — How frequencies combine

We now verify structural properties.

---

## **1. Additivity for disjoint singleton events**

We check:

$$
f({2,4,6}) = f({2}) + f({4}) + f({6})
$$

Left-hand side:

$$
f({2,4,6}) = \frac{491}{1000}
$$

Right-hand side:

$$
f({2}) + f({4}) + f({6}) = \frac{154}{1000} + \frac{167}{1000} + \frac{170}{1000}
$$

$$
= \frac{491}{1000}
$$

✔ Equality holds.

### Explanation

The sets ${2}, {4}, {6}$ are:

* **disjoint** (no overlap),
* so their counts simply add.

---

## **2. Grouping events**

We verify:

$$
f({1,2,3,4}) = f({1,2}) + f({3,4})
$$

Left-hand side:

$$
f({1,2,3,4}) = \frac{670}{1000}
$$

Right-hand side:

$$
f({1,2}) = \frac{168+154}{1000} = \frac{322}{1000}
$$

$$
f({3,4}) = \frac{181+167}{1000} = \frac{348}{1000}
$$

$$
f({1,2}) + f({3,4}) = \frac{322+348}{1000} = \frac{670}{1000}
$$

✔ Equality holds.

### Explanation

We split a set into **disjoint parts** → additivity still works.

---

## **3. Complementary events**

We check:

$$
f({1,3,5}) + f({2,4,6}) = 1
$$

$$
0.509 + 0.491 = 1
$$

✔ True.

### Explanation

These two sets:

* are disjoint,
* together cover all of $\Omega$.

---

## **4. Complement rule**

We verify:

$$
f({5,6}) = 1 - f({1,2,3,4})
$$

$$
0.33 = 1 - 0.67
$$

✔ True.

### Explanation

${5,6}$ is the **complement** of ${1,2,3,4}$.

---

# 🔷 Part C — When addition works and when it fails

---

## **1. Disjoint union**

We check:

$$
f({1,2} \cup {5,6}) = f({1,2}) + f({5,6})
$$

Left:

$$
f({1,2,5,6}) = \frac{168+154+160+170}{1000} = \frac{652}{1000}
$$

Right:

$$
f({1,2}) + f({5,6}) = \frac{322}{1000} + \frac{330}{1000} = \frac{652}{1000}
$$

✔ Works.

### Reason

The sets are **disjoint**.

---

## **2. Non-disjoint case**

Let:

$$
M = {1,2,3}, \quad N = {3,4,5}
$$

---

### Compute frequencies

$$
f(M) = \frac{168+154+181}{1000} = \frac{503}{1000}
$$

$$
f(N) = \frac{181+167+160}{1000} = \frac{508}{1000}
$$

---

### Union

$$
M \cup N = {1,2,3,4,5}
$$

$$
f(M \cup N) = \frac{168+154+181+167+160}{1000} = \frac{830}{1000}
$$

---

### Compare

$$
f(M) + f(N) = \frac{503+508}{1000} = \frac{1011}{1000}
$$

❌ Not equal.

---

## **3. Why inequality occurs**

Because:

$$
M \cap N = {3}
$$

Outcome $3$ is counted:

* once in $f(M)$,
* once in $f(N)$.

So it is **counted twice**.

---

## **4. Correct formula**

This leads to:

$$
f(M \cup N) = f(M) + f(N) - f(M \cap N)
$$

Here:

$$
f(M \cap N) = f({3}) = \frac{181}{1000}
$$

Check:

$$
\frac{503}{1000} + \frac{508}{1000} - \frac{181}{1000}
= \frac{830}{1000}
$$

✔ Correct.

---

# 🔷 Part D — Covering the whole sample space

---

## **1. Sum of singleton frequencies**

$$
\sum_{i=1}^{6} f({i}) = \frac{168+154+181+167+160+170}{1000}
$$

$$
= \frac{1000}{1000} = 1
$$

---

## **2. Why must this equal 1?**

Because:

* every experiment produces exactly one outcome,
* all outcomes together cover all possibilities.

---

## **3. Partition into disjoint sets**

Consider:

$$
{1,2}, \quad {3,4}, \quad {5,6}
$$

Frequencies:

$$
\frac{322}{1000} + \frac{348}{1000} + \frac{330}{1000} = \frac{1000}{1000} = 1
$$

---

## **4. General principle**

If:

$$
\Omega = A_1 \cup A_2 \cup \cdots \cup A_k
$$

with all $A_i$ disjoint, then:

$$
f(\Omega) = \sum_{i=1}^k f(A_i) = 1
$$

---

# 🔷 Part E — From frequency to probability

We now abstract.

We want a function:

$$
P: \mathcal{P}(\Omega) \to [0,1]
$$

such that:

---

## **1. Range**

$$
0 \leq P(A) \leq 1
$$

Because frequencies are proportions.

---

## **2. Impossible event**

$$
P(\varnothing) = 0
$$

No outcomes → no occurrences.

---

## **3. Whole space**

$$
P(\Omega) = 1
$$

Something always happens.

---

## **4. Additivity (disjoint events)**

If $A \cap B = \varnothing$, then:

$$
P(A \cup B) = P(A) + P(B)
$$

---

## **5. Complement rule**

$$
P(A^c) = 1 - P(A)
$$

---

These properties come directly from observed frequencies.

---

# 🔷 Part F — Final conceptual connection

We now connect three levels:

---

## **1. Elementary outcomes and events**

* $\Omega$ = all possible outcomes,
* events = subsets of $\Omega$.

---

## **2. Observed frequencies**

From experiments:

$$
f(A) = \frac{n(A)}{N}
$$

They:

* approximate regularities,
* reveal structure (additivity, complements).

---

## **3. Probability (abstraction)**

We replace empirical data with a function:

$$
P(A)
$$

that:

* behaves like frequency,
* but is defined mathematically,
* independent of a specific experiment.

---

## 🔷 Key philosophical point

* Frequency = **what we observe**
* Probability = **what we model**

Probability is a **mathematical idealization** of long-run behavior.

---

# ✅ Final conclusion

From raw data:
$$
n(A)
$$

we move to:
$$
f(A)
$$

and finally to:
$$
P(A)
$$

This is the transition:

$$
\text{experiment} ;\longrightarrow; \text{regularity} ;\longrightarrow; \text{formal theory}
$$

---

If you want, I can now:

* turn this into a clean “submission-ready” write-up, or
* connect it directly to Kolmogorov axioms (Problem 6).
