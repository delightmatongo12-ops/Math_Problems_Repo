---

# **Task 11 — Modeling Outcomes**

## **Question**

### **1. Distinguishable vs Indistinguishable Objects**

A box contains 4 red, 4 blue, 3 green balls (11 total).

1. Number of linear arrangements if balls of same color are indistinguishable
2. Number of arrangements if all balls are labeled
3. Explain why answers differ

---

### **Solutions**

#### **1.**

$$\frac{11!}{4!4!3!} = 11550$$

**Explanation:**
Repeated colors → divide by factorials.

---

#### **2.**

$$11! = 39916800$$

**Explanation:**
All balls are different → full permutation.

---

#### **3.**

**Answer:**
Indistinguishable objects reduce the number of distinct arrangements.

**Explanation:**
Swapping identical balls does not create a new outcome.

---

---

### **2. Recording Order vs Ignoring Order**

Draw 3 balls without replacement.

---

#### **Solutions**

##### **1. (Order ignored)**

$$\binom{11}{3} = 165$$

**Explanation:**
Only the set matters → combination.

---

##### **2. (Order recorded)**

$$11 \cdot 10 \cdot 9 = 990$$

**Explanation:**
Sequence → permutation.

---

##### **3.**

**Answer:**
Recording order increases outcomes.

**Explanation:**
Each set corresponds to multiple sequences.

---

---

### **3. PIN Code vs Number**

---

#### **Solutions**

##### **1. PIN codes**

$$10^4 = 10000$$

---

##### **2. 4-digit numbers**

$$9 \cdot 10^3 = 9000$$

---

##### **3.**

**Answer:**
PIN allows leading zero, numbers do not.

---

##### **4.**

**Answer:**
$$1234 \neq 4321$$

**Explanation:**
Order defines different outcomes.

---

---

## **Teacher Questions**

* Why does order increase outcomes? → More distinguishable cases
* Why allow leading zero in PIN? → It’s a code, not a number
* Why divide in indistinguishable case? → Remove duplicates

---

