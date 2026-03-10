# Calculative Foundation — Linear Algebra with Python

## Overview
This project demonstrates the application of **Linear Algebra concepts** using Python.  
The dataset represents **students' scores across multiple subjects**, and various mathematical operations are performed to understand the structure of the data.

The goal of this project is to build a **strong mathematical foundation for data science and machine learning** by applying vector and matrix operations in a practical way.

---

## Objectives

The main objectives of this project are:

- Understand **vectors and matrices**
- Perform **vector operations** (norm, dot product, cross product, projection)
- Apply **matrix operations** (transpose, determinant, inverse)
- Explore **linear transformations**
- Compute **eigenvalues and eigenvectors**
- Apply **Singular Value Decomposition (SVD)**
- Perform **dimensionality reduction using PCA and LDA**

These concepts are widely used in **machine learning, statistics, and data analysis**.

---

## Dataset

The dataset consists of **students' scores in multiple subjects**.

| Student | Sub1 | Sub2 | Sub3 | Sub4 | Sub5 |
|--------|------|------|------|------|------|
| S1 | 88 | 92 | 85 | 78 | 95 |
| S2 | 72 | 68 | 74 | 85 | 70 |
| S3 | 95 | 91 | 89 | 82 | 98 |
| S4 | 60 | 55 | 62 | 70 | 58 |
| S5 | 78 | 80 | 75 | 88 | 83 |
| S6 | 50 | 48 | 53 | 65 | 45 |

The data is represented as a **matrix where rows represent students and columns represent subjects**.

---

# Project Structure

```
Calculative-Foundation/
│
├── calculative_foundation.ipynb
├── README.md
```

---

# Technologies Used

- Python
- NumPy
- Scikit-learn
- Jupyter Notebook

---

# Part A — Vector Operations

Vector operations performed:

- **L1 Norm**
- **L2 Norm**
- **Dot Product**
- **Angle Between Vectors**
- **Cross Product**
- **Vector Projection**

Example:

```python
np.dot(s1, s2)
```

These operations help measure **similarity and relationships between vectors**.

---

# Part B — Matrix Operations

Matrix operations performed:

- Matrix addition
- Matrix multiplication
- Matrix transpose
- Determinant
- Matrix inverse

Example:

```python
np.matmul(scores, scores.T)
```

Matrix operations are fundamental for **linear algebra computations used in machine learning algorithms**.

---

# Part C — Linear Transformation

Linear transformations map vectors from one space to another using a **transformation matrix**.

Example:

```python
transformed_data = np.dot(data_2d, T)
```

These transformations are used for **scaling, rotation, and projection of data**.

---

# Part D — Eigenvalues and Matrix Decomposition

The following were computed:

- **Covariance Matrix**
- **Eigenvalues**
- **Eigenvectors**
- **Singular Value Decomposition (SVD)**

Example:

```python
eigenvalues, eigenvectors = np.linalg.eig(cov_matrix)
```

Eigenvalues represent **variance captured along principal directions**.

---

# Part E — Dimensionality Reduction

Two dimensionality reduction techniques were implemented:

## PCA (Principal Component Analysis)

Reduces data dimensionality while preserving maximum variance.

```python
pca = PCA(n_components=2)
X_pca = pca.fit_transform(scores)
```

## LDA (Linear Discriminant Analysis)

Finds the best projection that separates classes.

```python
lda = LinearDiscriminantAnalysis(n_components=1)
X_lda = lda.fit_transform(scores, labels)
```

---

# Key Learnings

From this project:

- Linear algebra is the **core foundation of machine learning**
- Vectors and matrices are used to represent real-world data
- Eigenvalues and SVD help understand **data structure**
- PCA and LDA are powerful tools for **dimensionality reduction**

---

# Conclusion

This project demonstrates how **linear algebra concepts can be applied using Python to analyze datasets**.  
Understanding these foundations is essential for building advanced **machine learning and AI systems**.

---

# Author

**Maitrak Kunjadiya**

Aspiring **AI / ML Engineer**