# **Problem 2 — Die × Die**

We consider an experiment consisting of **two independent rolls of a six-sided die**.

---

## **Step 1: Define the sample space**

Each die can take values:

$$
{1,2,3,4,5,6}
$$

So the sample space is:

$$
\Omega = {(i,j) \mid i \in {1,\dots,6},; j \in {1,\dots,6}}
$$

* $i$ = result of the **first die**
* $j$ = result of the **second die**

There are:

$$
|\Omega| = 6 \cdot 6 = 36
$$

possible outcomes.

---

## **Graphical Representation**

```text
      1 2 3 4 5 6
1     . . . . . .
2     . . . . . .
3     . . . . . .
4     . . . . . .
5     . . . . . .
6     . . . . . .
```

Each cell corresponds to one ordered pair $(i,j)$.

---

# **Part A — Marking Events**

---

## **1. The sum is equal to 8**

---

### Step 1: Translate into a condition

We want:

$$
i + j = 8
$$

---

### Step 2: Find all solutions

We list all integer pairs:

$$
(2,6),; (3,5),; (4,4),; (5,3),; (6,2)
$$

---

### Step 3: Mark the table

```text
      1 2 3 4 5 6
1     . . . . . .
2     . . . . . X
3     . . . . X .
4     . . . X . .
5     . . X . . .
6     . X . . . .
```

---

### Step 4: Event

$$
A = {(i,j) \in \Omega : i + j = 8}
$$

---

## **2. The first die is greater than the second**

---

### Step 1: Condition

$$
i > j
$$

---

### Step 2: Structure insight

This corresponds to:

* all entries **below the diagonal** (excluding diagonal)

---

### Step 3: Table

```text
      1 2 3 4 5 6
1     . . . . . .
2     X . . . . .
3     X X . . . .
4     X X X . . .
5     X X X X . .
6     X X X X X .
```

---

### Step 4: Event

$$
B = {(i,j) : i > j}
$$

---

## **3. Both dice show even numbers**

---

### Step 1: Even numbers

$$
{2,4,6}
$$

---

### Step 2: Cartesian product

We take:

$$
{2,4,6} \times {2,4,6}
$$

---

### Step 3: Table

```text
      1 2 3 4 5 6
1     . . . . . .
2     . X . X . X
3     . . . . . .
4     . X . X . X
5     . . . . . .
6     . X . X . X
```

---

### Step 4: Event

$$
C = {(i,j) : i \in {2,4,6},; j \in {2,4,6}}
$$

---

## **4. At least one die shows 6**

---

### Step 1: Logical interpretation

“At least one” means:

$$
i = 6 ;\text{OR}; j = 6
$$

---

### Step 2: Build as union

$$
D = {i=6} \cup {j=6}
$$

---

### Step 3: Table

```text
      1 2 3 4 5 6
1     . . . . . X
2     . . . . . X
3     . . . . . X
4     . . . . . X
5     . . . . . X
6     X X X X X X
```

---

### Step 4: Event

$$
D = {(i,j) : i=6 \text{ or } j=6}
$$

---

## **5. Exactly one die shows 1**

---

### Step 1: Careful interpretation

“Exactly one” means:

* one equals 1
* the other is **not** 1

---

### Step 2: Construct the set

$$
(1,j),; j \neq 1
\quad \text{and} \quad
(i,1),; i \neq 1
$$

---

### Step 3: Table

```text
      1 2 3 4 5 6
1     . X X X X X
2     X . . . . .
3     X . . . . .
4     X . . . . .
5     X . . . . .
6     X . . . . .
```

---

### Step 4: Event

$$
E = {(1,j): j \neq 1} \cup {(i,1): i \neq 1}
$$

---

# **Part B — Interpretation**

---

## **Case 1**

```text
      1 2 3 4 5 6
1     . . . . . .
2     . . . . . .
3     . . X X X X
4     . . X X X X
5     . . X X X X
6     . . X X X X
```

---

### Step 1: Observe the structure

* Rows: $i = 3,4,5,6$
* Columns: $j = 3,4,5,6$

So:

$$
i \geq 3 \quad \text{and} \quad j \geq 3
$$

---

### Step 2: Interpretation

> Both dice show numbers **at least 3**

---

### Final description

$$
A = {(i,j) : i \geq 3 \text{ and } j \geq 3}
$$

---

## **Case 2**

```text
      1 2 3 4 5 6
1     X . . . . .
2     . X . . . .
3     . . X . . .
4     . . . X . .
5     . . . . X .
6     . . . . . X
```

---

### Step 1: Recognize pattern

Marked cells:

$$
(1,1), (2,2), (3,3), (4,4), (5,5), (6,6)
$$

---

### Step 2: Condition

$$
i = j
$$

---

### Final interpretation

> Both dice show the **same number**

---

### Event

$$
B = {(i,j) : i = j}
$$

---

# **Conceptual Summary**

This problem deepens three key ideas:

---

### 1. Events as geometric regions

* Diagonal → $i = j$
* Triangle → $i > j$
* Rectangle → independent conditions like $i \geq 3$, $j \geq 3$

---

### 2. Logical structure → set operations

* “and” → intersection
* “or” → union
* “exactly one” → careful exclusion

---

### 3. Product structure of the sample space

$$
\Omega = {1,\dots,6} \times {1,\dots,6}
$$

This allows us to describe events like:

$$
A \times B
$$

which is a **rectangular region** in the table.

---

If you want, next we can go to **Problem 3**, where things become more abstract (events are no longer single outcomes but *constraints over time*).
