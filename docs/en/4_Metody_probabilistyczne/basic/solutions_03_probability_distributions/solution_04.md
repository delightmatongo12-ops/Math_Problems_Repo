# **Problem 4 — Building Complex Statements from Simple Ones**

We again consider:

$$
\Omega = {(i,j) \mid i,j \in {1,2,3,4,5,6}}
$$

---

## **Key Idea**

We define three basic events:

* $A$: “sum equals 7”
* $B$: “first die greater than second”
* $C$: “at least one die shows 6”

Then we construct new events using:

* **union**: $A \cup C$ (“or”)
* **intersection**: $A \cap C$ (“and”)
* **complement**: $A^c$ (“not”)

---

# **Part A — Basic Events**

---

## **Event $A$: sum equals 7**

We solve:

$$
i + j = 7
$$

Solutions:

$$
(1,6),(2,5),(3,4),(4,3),(5,2),(6,1)
$$

---

### Table

```text
      1 2 3 4 5 6
1     . . . . . X
2     . . . . X .
3     . . . X . .
4     . . X . . .
5     . X . . . .
6     X . . . . .
```

---

## **Event $B$: first die greater than second**

Condition:

$$
i > j
$$

---

### Table

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

## **Event $C$: at least one die shows 6**

Condition:

$$
i = 6 ;\text{or}; j = 6
$$

---

### Table

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

# **Part B — Compound Events**

We now combine $A$, $B$, $C$ using logic.

---

## **1. $A \cup C$ (sum is 7 OR at least one die is 6)**

We take all cells from **either** $A$ or $C$.

---

### Result

```text
      1 2 3 4 5 6
1     . . . . . X
2     . . . . X X
3     . . . X . X
4     . . X . . X
5     . X . . . X
6     X X X X X X
```

---

## **2. $A \cap C$ (sum is 7 AND at least one die is 6)**

We need outcomes satisfying both.

From $A$, only:

$$
(1,6), (6,1)
$$

---

### Result

```text
      1 2 3 4 5 6
1     . . . . . X
2     . . . . . .
3     . . . . . .
4     . . . . . .
5     . . . . . .
6     X . . . . .
```

---

## **3. $B \cap C$ (first > second AND at least one 6)**

From $C$: row 6 or column 6
From $B$: below diagonal

Only valid overlap:

$$
(6,1),(6,2),(6,3),(6,4),(6,5)
$$

---

### Result

```text
      1 2 3 4 5 6
1     . . . . . .
2     . . . . . .
3     . . . . . .
4     . . . . . .
5     . . . . . .
6     X X X X X .
```

---

## **4. $A \cap B^c$ (sum is 7, but first is NOT greater)**

$B^c$ means:

$$
i \le j
$$

From $A$, keep only those with $i \le j$:

$$
(1,6),(2,5),(3,4)
$$

---

### Result

```text
      1 2 3 4 5 6
1     . . . . . X
2     . . . . X .
3     . . . X . .
4     . . . . . .
5     . . . . . .
6     . . . . . .
```

---

## **5. $A \cap C^c$ (sum is 7 AND no die shows 6)**

Remove outcomes with 6 from $A$:

$$
(2,5),(3,4),(4,3),(5,2)
$$

---

### Result

```text
      1 2 3 4 5 6
1     . . . . . .
2     . . . . X .
3     . . . X . .
4     . . X . . .
5     . X . . . .
6     . . . . . .
```

---

## **6. $C \cap A^c$ (at least one 6, but sum NOT 7)**

Take all of $C$, remove $(1,6),(6,1)$.

---

### Result

```text
      1 2 3 4 5 6
1     . . . . . .
2     . . . . . X
3     . . . . . X
4     . . . . . X
5     . . . . . X
6     . X X X X X
```

---

## **7. $A^c \cap B$ (sum NOT 7 AND first > second)**

Start from $B$, remove $(4,3),(5,2),(6,1)$.

---

### Result

```text
      1 2 3 4 5 6
1     . . . . . .
2     X . . . . .
3     X X . . . .
4     X X . . . .
5     X X X X . .
6     X X X X X .
```

(with the three removed points blanked)

---

## **8. $B^c \cap C$ (first NOT greater AND at least one 6)**

$B^c$: $i \le j$
Intersect with $C$:

$$
(1,6),(2,6),(3,6),(4,6),(5,6),(6,6)
$$

---

### Result

```text
      1 2 3 4 5 6
1     . . . . . X
2     . . . . . X
3     . . . . . X
4     . . . . . X
5     . . . . . X
6     . . . . . X
```

---

## **9. $(A \cup C)^c$**

This means:

> neither sum is 7 NOR any die is 6

So:

* remove all of $A$
* remove all of $C$

---

### Result

```text
      1 2 3 4 5 6
1     X X X X X .
2     X X X X . .
3     X X X . X .
4     X X . X X .
5     X . X X X .
6     . . . . . .
```

---

## **10. $(A \cap C)^c$**

We remove only:

$$
(1,6),(6,1)
$$

Everything else remains.

---

### Result

```text
      1 2 3 4 5 6
1     X X X X X .
2     X X X X X X
3     X X X X X X
4     X X X X X X
5     X X X X X X
6     . X X X X X
```

---

# **Final Conceptual Takeaways**

---

## **1. Events behave like logical statements**

| Logic | Set operation |
| ----- | ------------- |
| AND   | $\cap$        |
| OR    | $\cup$        |
| NOT   | complement    |

---

## **2. Tables visualize set operations**

* Intersection → overlap of markings
* Union → combined markings
* Complement → everything else

---

## **3. Structure matters more than listing**

You are now thinking in terms of:

$$
A, B, C \subseteq \Omega
$$

and building new objects like:

$$
(A \cap C^c) \cup B
$$

---

## **4. This is the foundation of probability**

In the next problem, these exact operations will turn into:

$$
P(A \cup B), \quad P(A \cap B), \quad P(A^c)
$$

---

If you want, I’ll continue with **Problem 5**, where everything becomes numerical and connects directly to **probability theory**.
