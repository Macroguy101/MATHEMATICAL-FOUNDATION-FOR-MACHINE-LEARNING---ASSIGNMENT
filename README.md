# MATHEMATICAL-FOUNDATION-FOR-MACHINE-LEARNING---ASSIGNMENT
This is a Repository for all assignemnts of MFML 3RD SEM
# Linear Algebra and Computer Vision Class Projects (Module 1)

**Department of Artificial Intelligence & Data Science (AI&DS)**  
**Department of Computer Science & Engineering (Data Science)**  

- **Student Name:** Rajdeep Sarkar  
- **Registration Number:** 202500412  
- **Roll Number:** 16  
- **Branch:** B.Tech CSE (Data Science)  

---

## Part 1: Implementation of Gaussian Elimination Algorithm

### 1. Objective
To construct a generalized, numerically stable Python program implementing the Gaussian Elimination algorithm with partial pivoting and back substitution to solve systems of linear algebraic equations of order $n \times n$.

### 2. Mathematical Formulation

A general system of $n$ linear equations with $n$ unknowns is written in matrix form as:

$$A x = b$$

Where:
- $A \in \mathbb{R}^{n \times n}$ is the coefficient matrix.
- $b \in \mathbb{R}^{n \times 1}$ is the right-hand side constant vector.
- $x \in \mathbb{R}^{n \times 1}$ is the vector of unknowns.

#### A. Forward Elimination with Partial Pivoting
The augmented matrix is defined as $\tilde{A} = [A \mid b]$.
At step $k$ ($k = 1, \dots, n-1$):
1. **Pivot Selection:** Find row $p \ge k$ such that $|a_{pk}| = \max_{i=k}^n |a_{ik}|$.
2. **Row Swap:** Swap row $k$ with row $p$ in $\tilde{A}$. If $|a_{kk}| < \epsilon$, the matrix is singular and does not possess a unique solution.
3. **Row Operations:** For every row $i = k+1, \dots, n$:
   $$m_{ik} = \frac{a_{ik}}{a_{kk}}$$
   $$R_i \leftarrow R_i - m_{ik} R_k$$

#### B. Back Substitution
Once $\tilde{A}$ is transformed into an upper triangular system $[U \mid y]$, the unknowns are computed sequentially:

$$x_n = \frac{y_n}{u_{nn}}$$

$$x_i = \frac{y_i - \sum_{j=i+1}^n u_{ij} x_j}{u_{ii}}, \quad \text{for } i = n-1, n-2, \dots, 1$$

---

### 3. Algorithm and Pseudocode

