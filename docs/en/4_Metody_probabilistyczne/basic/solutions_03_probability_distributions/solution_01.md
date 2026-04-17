# **Problem 1 — Coin × Coin**

We analyze an experiment consisting of **two coin tosses**.

## **Step 1: Define the sample space**

Each toss can result in:

* $H$ (Head)
* $T$ (Tail)

So the **sample space** is:

$$
\Omega = {(H,H), (H,T), (T,H), (T,T)}
$$

We represent it in the given table:

```
      H   T
H     .   .
T     .   .
```

Each cell corresponds to:

* Row = first toss
* Column = second toss

So:

| Outcome | Meaning               |
| ------- | --------------------- |
| $(H,H)$ | first = H, second = H |
| $(H,T)$ | first = H, second = T |
| $(T,H)$ | first = T, second = H |
| $(T,T)$ | first = T, second = T |

---

# **Part A — Marking Events**

We now translate each **verbal statement → set of outcomes → graphical marking**.

---

## **1. Exactly one head**

### Step 1: Interpret the condition

“Exactly one head” means:

* One toss is $H$, the other is $T$

So the valid outcomes are:

$$
(H,T), \quad (T,H)
$$

---

### Step 2: Mark in the table

```
      H   T
H     .   X
T     X   .
```

---

### Step 3: Final description

This event is:

$$
A = {(H,T), (T,H)}
$$

---

## **2. Both tosses are the same**

### Step 1: Interpret

“Same” means:

* both heads OR both tails

So:

$$
(H,H), \quad (T,T)
$$

---

### Step 2: Table

```
      H   T
H     X   .
T     .   X
```

---

### Step 3: Event

$$
B = {(H,H), (T,T)}
$$

---

## **3. At least one head**

### Step 1: Interpret carefully

“At least one head” means:

* one OR two heads

So include:

* $(H,H)$
* $(H,T)$
* $(T,H)$

Exclude only:

* $(T,T)$

---

### Step 2: Table

```
      H   T
H     X   X
T     X   .
```

---

### Step 3: Event

$$
C = \Omega \setminus {(T,T)}
$$

---

## **4. The first toss is tails**

### Step 1: Fix the first coordinate

We select all outcomes where the first element is $T$:

$$
(T,H), \quad (T,T)
$$

---

### Step 2: Table

```
      H   T
H     .   .
T     X   X
```

---

### Step 3: Event

$$
D = {(T,H), (T,T)}
$$

---

## **5. The second toss is heads**

### Step 1: Fix second coordinate

We take all outcomes where second = $H$:

$$
(H,H), \quad (T,H)
$$

---

### Step 2: Table

```
      H   T
H     X   .
T     X   .
```

---

### Step 3: Event

$$
E = {(H,H), (T,H)}
$$

---

# **Part B — Interpretation of Given Diagrams**

Now we reverse the process:
**table → set → verbal description**

---

## **Case 1**

```
      H   T
H     X   X
T     .   .
```

---

### Step 1: Identify marked outcomes

Marked cells:

* $(H,H)$
* $(H,T)$

So:

$$
A = {(H,H), (H,T)}
$$

---

### Step 2: Find the pattern

In both outcomes:

* the **first toss is always $H$**

---

### ✅ Final interpretation

> **“The first toss is heads.”**

---

## **Case 2**

```
      H   T
H     .   X
T     X   .
```

---

### Step 1: Outcomes

Marked:

* $(H,T)$
* $(T,H)$

---

### Step 2: Recognize structure

This is exactly:

* one head and one tail

---

### ✅ Final interpretation

> **“Exactly one head occurs.”**

---

# **Conceptual Summary (Very Important)**

This problem builds the key bridge:

### 1. Outcomes → pairs

Each result is an **ordered pair** $(\text{first}, \text{second})$.

---

### 2. Events → subsets

Every event is a subset:

$$
A \subseteq \Omega
$$

---

### 3. Language → sets

Statements like:

* “at least one head”
* “first toss is tails”

must be translated into **precise sets of outcomes**.

---

### 4. Tables → structure

The grid is not decoration—it shows:

* how events are structured
* how conditions restrict rows/columns

---

If you want, I can continue with **Problem 2** in the same level of detail (it gets more interesting with dice and structure).
