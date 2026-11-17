
# WHOLESALE CUSTOMER SPENDING ANALYSIS

---

## A. Proposed Study

This project will use the Wholesale Customers dataset to study how business customers spend on different product categories. The data records the annual spending of customers of a wholesale distributor. By applying linear algebra, the group will organize the spending data, look for patterns among customers, and examine how spending on selected product categories is related to grocery spending.

The main goal is to show how numerical data can help a business understand its customers. The results may help a wholesaler recognize customers with similar buying habits and make better decisions when planning product stocks and customer offers.

---

## B. Objectives

1. Organize the customers' annual spending into a numerical matrix using Python and NumPy.
2. Use linear algebra operations to examine relationships and patterns among product categories.
3. Group customers with similar spending behavior based on the selected numerical features.
4. Build a basic regression model to estimate grocery spending from the other product-category spending values.

---

## C. Dataset Information

| Information | Details |
|:---|:---|
| Dataset Name | Wholesale Customers Dataset |
| Dataset Source | UCI Machine Learning Repository |
| Dataset Link | [View Dataset](https://archive.ics.uci.edu/dataset/292/wholesale+customers) |
| Number of Observations | 440 customers |
| Number of Selected Features | 6 numerical variables |
| Target Variable | Grocery |
| File Format | CSV |
| Dataset Description | Annual spending information of wholesale distributor customers across six product categories, with customer channel and region information. |

### Dataset Description

The dataset contains information about 440 wholesale customers. It includes their annual spending on fresh products, milk products, grocery items, frozen products, detergents and paper products, and delicatessen items. It also records each customer's business channel and region. For this project, the group will focus on the six numerical spending variables.

---

## D. Description of Variables

| Variable Name | Description | Data Type | Role |
|:---|:---|:---|:---|
| Fresh | Annual spending on fresh products | Numerical | Independent |
| Milk | Annual spending on milk products | Numerical | Independent |
| Grocery | Annual spending on grocery products | Numerical | Dependent |
| Frozen | Annual spending on frozen products | Numerical | Independent |
| Detergents_Paper | Annual spending on detergents and paper products | Numerical | Independent |
| Delicassen | Annual spending on delicatessen products | Numerical | Independent |

### Justification of the Selected Variables

The six variables represent the main product groups purchased by each wholesale customer. Looking at these spending amounts together can show which product categories customers tend to buy more often or in larger amounts. Grocery spending is selected as the target variable, while spending on the other five categories will be used as the input variables for the basic prediction model. The channel and region fields are not included in the numerical feature matrix because they are categorical information.

---

## E. Sample Dataset

The table below shows five sample observations from the Wholesale Customers dataset. The values are annual spending amounts in monetary units (m.u.).

| Observation | Fresh | Milk | Grocery | Frozen | Detergents_Paper | Delicacies |
|:---:|---:|---:|---:|---:|---:|---:|
| 1 | 12,669 | 9,656 | 7,561 | 214 | 2,674 | 1,338 |
| 2 | 7,057 | 9,810 | 9,568 | 1,762 | 3,293 | 1,776 |
| 3 | 6,353 | 8,808 | 7,684 | 2,405 | 3,516 | 7,844 |
| 4 | 13,265 | 1,196 | 4,221 | 6,404 | 507 | 1,788 |
| 5 | 22,615 | 5,410 | 7,198 | 3,915 | 1,777 | 5,185 |

> **Note:** These are the first five customer records shown in the dataset. Values are presented as recorded.

---

## F. Proposed Application of Linear Algebra Concepts

| Linear Algebra Concept | Proposed Application |
|:---|:---|
| **Matrices** | Arrange the five input variables (Fresh, Milk, Frozen, Detergents_Paper, and Delicassen) into a feature matrix X. Grocery spending will be stored separately as the target vector y. |
| **Vector Spaces** | Examine the columns of the feature matrix and determine whether some spending variables provide similar or repeated information by checking their linear independence and the rank of X. |
| **Linear Transformations** | Standardize the spending values so that categories with larger amounts do not dominate the analysis simply because of their scale. |
| **Determinants** | Use determinants on suitable square matrices, such as a selected covariance or Gram matrix, to help check whether the matrix is invertible. This will be done only when the matrix is square. |
| **Eigenvalues and Eigenvectors** | Calculate the eigenvalues and eigenvectors of the covariance matrix to identify the main directions in which customer spending varies. |
| **Diagonalization** | Use the eigenvectors and eigenvalues as part of Principal Component Analysis (PCA) to reduce the number of dimensions while keeping as much of the variation in the spending data as possible. |
| **Regression Model** | Apply Ordinary Least Squares regression to estimate a customer's grocery spending using the other five product-category spending variables. |

### Example of the Proposed Matrix Representation

Using the first three observations and the five independent variables, the feature matrix can be represented as:

**Feature Matrix (X)**

```text
X = [ 12669   9656    214   2674   1338 ]
    [  7057   9810   1762   3293   1776 ]
    [  6353   8808   2405   3516   7844 ]
```

This sample matrix has three rows and five columns. Each row represents one customer, while each column represents one spending category used as an input.

The full feature matrix will contain 440 rows and five columns. Grocery spending will be arranged separately as the target vector with 440 values. The group will use Python and NumPy to perform the matrix operations, then use the results to explore customer spending patterns.

---

## References

1. Cardoso, M. (2013). *Wholesale Customers* [Dataset]. UCI Machine Learning Repository. https://doi.org/10.24432/C5030X

2. UCI Machine Learning Repository. (n.d.). *Wholesale customers.* https://archive.ics.uci.edu/dataset/292/wholesale+customers

---

**Project Title:** Wholesale Customer Spending Analysis

**Programming Language:** Python

**Main Library:** NumPy

**Dataset:** Wholesale Customers Dataset
