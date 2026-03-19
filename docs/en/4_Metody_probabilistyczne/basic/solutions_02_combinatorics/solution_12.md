---

# **Task 12 — Mixed Counting Problem**

## **Question**

### **1. Student ID Codes**

Letters from ${A,B,C,D,E}$ + digits

---

#### **Solutions**

##### **1. Repetition allowed**

$$5^2 \cdot 10^3 = 25 \cdot 1000 = 25000$$

---

##### **2. Letters no repetition**

$$P(5,2) \cdot 10^3 = 20 \cdot 1000 = 20000$$

---

##### **3. No repetition at all**

$$P(5,2) \cdot P(10,3) = 20 \cdot 720 = 14400$$

---

---

### **2. Medal Assignment**

---

#### **Solutions**

##### **1.**

$$P(12,3) = 1320$$

---

##### **2.**

Choose 1 more winner:
$$\binom{10}{1} \cdot 3! = 10 \cdot 6 = 60$$

---

---

### **3. Committee Selection**

---

#### **Solutions**

##### **1.**

$$\binom{10}{4} = 210$$

---

##### **2.**

$$\binom{4}{2}\binom{6}{2} = 6 \cdot 15 = 90$$

---

##### **3.**

$$\binom{10}{4} - \binom{6}{4} = 210 - 15 = 195$$

---

---

### **4. Circular Seating**

---

#### **Solutions**

##### **1.**

$$(7-1)! = 720$$

---

##### **2.**

$$(6-1)! \cdot 2 = 5! \cdot 2 = 240$$

---

---

### **5. Passwords**

Total characters: $36$

---

#### **Solutions**

##### **1. Repetition allowed**

$$36^5$$

---

##### **2. No repetition**

$$P(36,5) = 36 \cdot 35 \cdot 34 \cdot 33 \cdot 32$$

---

##### **3.**

* With repetition → sequence
* Without repetition → k-permutation

---

---

## **Teacher Questions**

* Why multiply parts? → Product rule
* Why subtract cases? → Complement counting
* Why treat letters and digits separately? → Independent choices

---

