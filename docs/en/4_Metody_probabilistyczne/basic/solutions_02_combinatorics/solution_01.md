## **Task 1 — Recognizing Counting Models**

### **Question**

For each situation determine which combinatorial model is most appropriate:

1. Arranging 7 students in a line.
2. Choosing 4 members of a committee from 12 people.
3. Assigning gold, silver, and bronze medals among 15 athletes.
4. Forming a 6-digit PIN code.
5. Arranging the letters of the word **BANANA**.
6. Seating 6 people around a round table.

---

## **Solutions (with short explanations)**

### **1. Arranging 7 students in a line**

**Answer:**
$$\text{Permutation}$$

**Explanation:**
All objects are used, order matters, and no repetitions → classic permutation.

---

### **2. Choosing 4 members of a committee from 12 people**

**Answer:**
$$\text{Combination}$$

**Explanation:**
We select some people, and order does **not** matter → combinations.

---

### **3. Assigning gold, silver, and bronze medals among 15 athletes**

**Answer:**
$$\text{k-permutation (ordered selection without repetition)}$$

**Explanation:**
Only 3 athletes are chosen, and order matters (gold ≠ silver ≠ bronze), no repetition.

---

### **4. Forming a 6-digit PIN code**

**Answer:**
$$\text{Sequence with repetition}$$

**Explanation:**
Each position can be any digit, order matters, and repetition is allowed.

---

### **5. Arranging the letters of the word BANANA**

**Answer:**
$$\text{Permutation with repeated elements}$$

**Explanation:**
All letters are used, but some are identical (A appears 3 times, N appears 2 times).

---

### **6. Seating 6 people around a round table**

**Answer:**
$$\text{Circular permutation}$$

**Explanation:**
All people are arranged, but rotations are considered the same → circular setting.

---

# **Extra Questions Your Teacher Might Ask (with answers)**

---

### **Q1. Why is problem 2 not a permutation?**

**Answer:**
Because the order of selection does not matter.

$${A,B,C,D} = {D,C,B,A}$$

So we use combinations, not permutations.

---

### **Q2. What would change in problem 3 if medals were identical?**

**Answer:**
Then order would not matter → it becomes a **combination**.

**Explanation:**
If gold, silver, bronze are indistinguishable, we only care who gets a medal, not which one.

---

### **Q3. What if repetition was NOT allowed in the PIN code?**

**Answer:**
$$\text{k-permutation}$$

**Explanation:**
Now digits cannot repeat, order still matters → ordered selection without repetition.

---

### **Q4. Why is BANANA not a simple permutation?**

**Answer:**
Because letters repeat.

**Explanation:**
Swapping identical letters (like A’s) does not create new arrangements, so we must divide by factorials of repetitions.

---

### **Q5. Why do we subtract 1 in circular permutations?**

**Answer:**
Because rotations are identical.

$$ (n-1)! $$

**Explanation:**
Fix one person to remove rotational symmetry, then arrange the rest.

---

### **Q6. How do you quickly decide the model in exams?**

**Answer (decision shortcut):**

* All objects + order → permutation
* All objects + circle → circular permutation
* Some objects + no order → combination
* Some objects + order → k-permutation
* Repetition allowed → sequence
* Identical objects → permutation with repetition

---


