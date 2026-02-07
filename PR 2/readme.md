# 📊 Expectation Decider – Probability & Bayes’ Theorem on Student Data

> A statistics-focused Python notebook that applies **probability concepts, random variables, contingency tables, conditional probability, Venn diagrams, and Bayes’ Theorem** to a real student dataset to study exam outcomes.

![Python](https://img.shields.io/badge/Python-3.x-blue)
![Stats](https://img.shields.io/badge/Statistics-Probability%20%26%20Bayes-orange)
![Status](https://img.shields.io/badge/Project-Completed-success)

---

## 🔎 Project Summary

This project analyzes a **student performance dataset (200 rows, 5 columns)** and demonstrates core **probability & statistics concepts** using Python:

- Empirical vs Theoretical Probability  
- Random Variables & Probability Distribution  
- Expected Value and Variance  
- Venn Diagram (Study Hours vs Attendance)  
- Contingency Table  
- Joint, Marginal & Conditional Probability  
- **Bayes’ Theorem (application on attendance vs pass outcome)**

Notebook: `expectation_decider.ipynb`  
Dataset: `students_data.csv`

---

## 🧾 Dataset

**Columns used:**
- `study_hours` – weekly study hours  
- `attendance` – attendance percentage  
- `group_discussion` – Yes/No  
- `previous_test_score` – numeric  
- `final_exam_pass` – Pass/Fail (target)

**Shape:** 200 × 5

---

## 🧠 Concepts Implemented (from the Notebook)

### 1️⃣ Empirical vs Theoretical Probability
- Empirical: `P(Pass)` computed from dataset  
- Theoretical: simple sample space `{pass, fail}` with `P(pass)=1/2`

### 2️⃣ Random Variable, Distribution, Mean & Variance
- Random variable **X = number of students passing out of 3**
- Distribution table created for `X = {0,1,2,3}`
- **Expected Value (E[X]) = 1.5**  
- **Variance = 0.625**

### 3️⃣ Venn Diagram (Study > 10 hrs & Attendance > 80%)
- Visualizes overlap between:
  - Study > 10 hours/week  
  - Attendance > 80%  
- Counts printed and Venn diagram plotted using `matplotlib_venn`


## 4️⃣ Contingency Table

**Cross-tab between:**
- `group_discussion` (Yes / No)
- `final_exam_pass` (Pass / Fail)

**Key Observations:**
- Students who joined **group discussions** had a much higher pass count.  
- Students who **did not join** group discussions had **zero passes** in the table.

---

## 5️⃣ Joint, Marginal & Conditional Probability

- **Joint Probability:**  
  `P(GroupDiscussion = Yes ∩ Pass)`

- **Marginal Probability:**  
  `P(Pass)`

- **Conditional Probability:**  
  `P(Pass | GroupDiscussion = Yes) ≈ 0.807`

**Interpretation (from notebook):**
- *Group discussion* and *passing the exam* are **dependent events**.  
- The events are **not independent**; a **strong relationship** is observed between participation in group discussion and exam success.

---

## 6️⃣ Bayes’ Theorem (Application)

**Computed from the dataset:**
- `P(Pass) = 0.545`  
- `P(High Attendance) = 0.475`  
- `P(High Attendance | Pass) ≈ 0.8624`  
- `P(High Attendance | Fail) ≈ 0.011`

**Bayes’ Result:**
> **`P(Pass | High Attendance) ≈ 0.9895`**

**Interpretation:**
Students with **high attendance (> 80%)** have an **extremely high probability of passing** the final exam, as demonstrated using **Bayes’ Theorem**.

