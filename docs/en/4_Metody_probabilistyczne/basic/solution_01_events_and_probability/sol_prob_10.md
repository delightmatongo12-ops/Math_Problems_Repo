# Task 10 — Buffon’s Needle Probability

Buffon’s Needle is a **geometric probability experiment**:

* A needle of length $L$ is dropped onto a floor with **parallel lines spaced $d$ units apart**.
* The needle may **intersect a line** or **not intersect**.

---

# 1. Condition for Intersection

Let:

* $X$ = distance from the **center of the needle** to the nearest line
* $\theta$ = angle between the **needle and the parallel lines**

The needle **intersects a line** if:

$$
X \le \frac{L}{2} \sin \theta
$$

---

# 2. Sample Space

The sample space is **continuous**:

$$
\Omega = \left[0,\frac{d}{2}\right] \times \left[0,\frac{\pi}{2}\right]
$$

An elementary outcome is:

$$
(X, \theta)
$$

---

# 3. Probability of Intersection

If the needle length $L \le d$, the probability of intersection is given by the **famous Buffon formula**:

$$
P(\text{intersection}) = \frac{2L}{\pi d}
$$

---

# 4. Probability of No Intersection

Complement:

$$
P(\text{no intersection}) = 1 - \frac{2L}{\pi d}
$$

---

# 5. Meaning of an Outcome

Example:

$$
\left(\frac{d}{4}, \frac{\pi}{6}\right)
$$

* Needle center is $\frac{d}{4}$ units from the nearest line
* Needle makes an angle of $\frac{\pi}{6}$ with the lines
* Determine if it **intersects** using $X \le \frac{L}{2}\sin\theta$

---

# Possible Questions and Answers

---

### Question 1

**When does the needle intersect a line?**

Answer:

$$
X \le \frac{L}{2}\sin\theta
$$

---

### Question 2

**What is the probability of intersection if $L \le d$?**

Answer:

$$
P = \frac{2L}{\pi d}
$$

---

### Question 3

**What is the probability that the needle does not intersect a line?**

Answer:

$$
P = 1 - \frac{2L}{\pi d}
$$

---

### Question 4

**Why is the sample space continuous?**

Answer:

Because both $X$ and $\theta$ can take **infinitely many real values**:

$$
\Omega = \left[0,\frac{d}{2}\right] \times \left[0,\frac{\pi}{2}\right]
$$

---

### Question 5

**Example:** Needle center at $X = d/4$ and angle $\theta = \pi/6$. Does it intersect if $L = d/2$?

Answer:

Check condition:

$$
\frac{d}{4} \le \frac{L}{2} \sin\theta = \frac{d/2}{2} \sin(\pi/6) = \frac{d}{4} \cdot \frac{1}{2} = \frac{d}{8}
$$

Since $\frac{d}{4} > \frac{d}{8}$, the needle **does not intersect**.

