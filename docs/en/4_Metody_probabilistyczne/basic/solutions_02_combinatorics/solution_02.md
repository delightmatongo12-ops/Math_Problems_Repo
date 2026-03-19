## **Task 2 — Permutations**

### **Question**

1. In how many ways can 8 different books be arranged on a shelf?
2. In how many ways can 8 people sit in a row if two particular people must sit next to each other?
3. In how many ways can they sit if those two people must **not** sit next to each other?
4. In how many ways can 10 questions in a test be ordered if the first question is fixed?

---

## **Solutions**

### **1.**

$$8! = 40320$$
**Explanation:** All objects arranged, order matters.

---

### **2.**

Treat the two people as one block:
$$7! \cdot 2! = 5040 \cdot 2 = 10080$$
**Explanation:** Arrange 7 units, then swap inside the pair.

---

### **3.**

$$8! - 7!\cdot 2! = 40320 - 10080 = 30240$$
**Explanation:** Total minus cases where they sit together.

---

### **4.**

$$9! = 362880$$
**Explanation:** First position fixed, arrange remaining 9.

---

## **Teacher Questions**

* Why use subtraction in (3)? → Complement counting is easier.
* Why multiply by $2!$? → Internal order of the pair matters.

---

