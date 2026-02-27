# 📊 E-Commerce Transaction Statistical Analysis

> A complete statistical modeling project analyzing e-commerce transaction data using probability distributions and transformation techniques.

---

## 📌 Project Overview

This project applies **probability theory and statistical modeling** to real-world e-commerce transaction data.

The objective is to:

- Understand transaction success behavior
- Model transaction frequency over time
- Analyze revenue distribution patterns
- Test normality assumptions
- Improve data using transformation techniques

This project connects **theoretical statistics with practical business insights**.

---

## 🧠 Statistical Concepts Implemented

- Bernoulli Distribution
- Binomial Distribution
- Poisson Distribution
- Log-Normal Distribution
- Pareto (Power Law) Distribution
- Q-Q Plot (Normality Testing)
- Box-Cox Transformation
- Z-Score Standardization
- PDF & CDF Analysis

---

## 📂 Dataset Description

The dataset includes:

- `customer_id`
- `transaction_date`
- `transaction_status` (Success / Fail)
- `transaction_amount`

This allows modeling of:

- Binary outcomes
- Event frequency
- Heavy-tailed financial behavior
- High-value transaction risk

---

## 🔍 Analysis Breakdown

### 1️⃣ Bernoulli Distribution
Modeled transaction success probability using binary outcomes.

### 2️⃣ Binomial Distribution
Analyzed weekly transaction counts per customer.

### 3️⃣ Poisson Distribution
Modeled daily transaction arrivals as a random process.

### 4️⃣ Log-Normal Distribution
Examined positive skewness in transaction amounts.

### 5️⃣ Pareto (Power Law) Distribution
Identified heavy-tailed revenue patterns.

### 6️⃣ Q-Q Plot
Tested whether transaction amounts follow a normal distribution.

### 7️⃣ Box-Cox Transformation
Reduced skewness and improved modeling suitability.

### 8️⃣ Z-Score & Probability
Calculated standardized values and probability of high-value transactions.

---

## 📈 Key Insights

- Transaction outcomes behave like independent Bernoulli trials.
- Daily transactions resemble a Poisson arrival process.
- Transaction amounts are right-skewed.
- A small percentage of transactions contribute disproportionately to total revenue.
- Log-Normal and Pareto distributions model revenue better than Normal distribution.
- Box-Cox transformation improves statistical modeling performance.

---

## 🛠️ Tech Stack

- Python
- NumPy
- Pandas
- SciPy
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## 🚀 How to Run

```bash
# Clone repository
git clone https://github.com/yourusername/ecommerce-statistical-analysis.git

# Navigate into folder
cd ecommerce-statistical-analysis

# Install required libraries
pip install -r requirements.txt

# Launch notebook
jupyter notebook

📁 Project Structure
E-Commerce-Statistical-Analysis/
│
├── ecommerce_transaction.ipynb
├── ecommerce_transactions.csv
├── README.md
└── requirements.txt

🎯 Business Applications

This analysis can support:

Fraud detection modeling

Revenue forecasting

Risk evaluation

Customer behavior segmentation

High-value transaction monitoring

📚 Learning Outcomes

Through this project, the following were strengthened:

Real-world distribution fitting

Heavy-tailed financial data understanding

Practical probability modeling

Data transformation techniques

Statistical interpretation for business decisions

👤 Author

Maitrak Kunjadiya
Computer Science (AI & ML) Student
Aspiring Data Scientist