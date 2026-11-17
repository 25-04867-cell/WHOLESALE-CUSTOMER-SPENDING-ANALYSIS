
<div align="center">

# WHOLESALE CUSTOMER SPENDING ANALYSIS

### Applying Linear Algebra to Wholesale Customer Purchasing Patterns

![Python](https://img.shields.io/badge/Python-Programming-blue?logo=python)
![NumPy](https://img.shields.io/badge/NumPy-Linear%20Algebra-013243?logo=numpy)
![Dataset](https://img.shields.io/badge/Dataset-UCI%20Repository-orange)

</div>

---

## 1. PROPOSED STUDY

This project analyzes the annual spending patterns of wholesale customers across different product categories using linear algebra. It focuses on identifying similarities in customer purchasing behavior and examining relationships between product categories, particularly grocery spending. The results aim to help businesses understand customer demand, recognize purchasing trends, improve inventory management, and make better stocking decisions.

---

## 2. OBJECTIVES

The study aims to:

1. Organize customers' annual spending data into numerical matrices using Python and NumPy.
2. Apply linear algebra operations to identify patterns and relationships among product categories.
3. Identify customers with similar purchasing behaviors based on their spending patterns.
4. Develop a basic regression model to estimate grocery spending using other product-category expenditures.

---

## 3. DATASET INFORMATION

| Dataset Details | Description |
|:---|:---|
| Dataset Name | Wholesale Customers Dataset |
| Source | UCI Machine Learning Repository |
| Total Observations | 440 customers |
| Numerical Variables | 6 product categories |
| Target Variable | Grocery |
| File Format | CSV |
| Data Type | Numerical and categorical |

**Dataset Source:** [UCI Wholesale Customers Dataset](https://archive.ics.uci.edu/dataset/292/wholesale+customers)

### Dataset Overview

The dataset contains annual spending information from 440 wholesale customers. It includes six product categories, along with additional information about customer channels and regions.

---

## 4. DESCRIPTION OF VARIABLES

The following variables represent the annual spending of wholesale customers.

| Variable | Description |
|:---|:---|
| Fresh | Spending on fresh products |
| Milk | Spending on milk products |
| Grocery | Spending on grocery products |
| Frozen | Spending on frozen products |
| Detergents_Paper | Spending on detergents and paper |
| Delicassen | Spending on delicatessen products |

### Variable Classification

| Category | Variables |
|:---|:---|
| Independent Variables (X) | Fresh, Milk, Frozen, Detergents_Paper, Delicassen |
| Dependent Variable (Y) | Grocery |

**Explanation:** Grocery is selected as the target variable, while the remaining five product categories serve as independent variables for the proposed regression analysis.

---

## 5. SAMPLE DATASET

The following table presents five sample observations from the dataset.

| Customer | Fresh | Milk | Grocery | Frozen | Detergents | Delicassen |
|:---:|---:|---:|---:|---:|---:|---:|
| 1 | 12,669 | 9,656 | 7,561 | 214 | 2,674 | 1,338 |
| 2 | 7,057 | 9,810 | 9,568 | 1,762 | 3,293 | 1,776 |
| 3 | 6,353 | 8,808 | 7,684 | 2,405 | 3,516 | 7,844 |
| 4 | 13,265 | 1,196 | 4,221 | 6,404 | 507 | 1,788 |
| 5 | 22,615 | 5,410 | 7,198 | 3,915 | 1,777 | 5,185 |

*Note: These values represent the first five observations. Spending amounts are expressed in monetary units.*

---

## 6. APPLICATION OF LINEAR ALGEBRA CONCEPTS

The project will apply the following mathematical concepts to analyze customer spending patterns.

| Linear Algebra Concept | Application in the Study |
|:---|:---|
| Matrices | Organize customer spending data into numerical matrices. |
| Vector Spaces | Examine the linear independence and rank of spending variables. |
| Linear Transformations | Standardize data to make product-category values comparable. |
| Determinants | Examine the invertibility of suitable square matrices. |
| Eigenvalues and Eigenvectors | Identify important patterns and variations in customer spending. |
| Diagonalization | Support dimensionality reduction through Principal Component Analysis (PCA). |
| Regression | Estimate grocery spending using the other product categories. |

---

## 7. MATRIX REPRESENTATION

The spending information will be represented using a matrix containing five independent variables.

### Sample Feature Matrix (X)

```text
       Fresh  Milk  Frozen  Detergents  Delicassen

X = [ 12669   9656    214      2674       1338
       7057   9810   1762      3293       1776
       6353   8808   2405      3516       7844 ]
```

Each row represents a customer, while each column represents a product category.

### Target Vector (Y)

```text
Y = [ 7561
      9568
      7684 ]
```

The target vector contains the corresponding grocery spending values.

### Matrix Dimensions

| Matrix | Dimensions | Description |
|:---|:---:|:---|
| X | 440 × 5 | Independent variables |
| Y | 440 × 1 | Grocery spending |
| Full Dataset | 440 × 6 | Six spending categories |

---

## 8. EXPECTED OUTPUT

Through the application of linear algebra, the study expects to:

- Identify similarities in customer purchasing behavior.
- Determine relationships among product categories.
- Recognize important spending patterns.
- Estimate grocery spending through regression.
- Provide insights that can support inventory planning and business decisions.

---

## 9. TOOLS AND TECHNOLOGIES

| Tool | Purpose |
|:---|:---|
| Python | Main programming language |
| NumPy | Matrix operations and calculations |
| Pandas | Dataset organization and manipulation |
| Matplotlib | Data visualization |
| Scikit-learn | Regression and data analysis |

---

## 10. REFERENCES

1. Cardoso, M. (2013). *Wholesale Customers Dataset*. UCI Machine Learning Repository.

2. UCI Machine Learning Repository. [Wholesale Customers Dataset](https://archive.ics.uci.edu/dataset/292/wholesale+customers).

---

<div align="center">

**WHOLESALE CUSTOMER SPENDING ANALYSIS**

*Using Linear Algebra for Data-Driven Business Decisions*

</div>
