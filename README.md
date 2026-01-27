#  Stellar Luminosity Regression

Modeling stellar luminosity from first principles using regression techniques — no black boxes, just math, code, and intuition.

---

##  Project Overview

This project explores how **stellar luminosity** can be modeled using **regression techniques implemented from scratch**. The main objective is to deeply understand:

* How linear regression behaves and where it fails
* Why nonlinear relationships require richer feature representations
* How polynomial and interaction terms improve predictive performance

The project is part of a **Machine Learning Bootcamp**, with a strong emphasis on **core concepts**, **numerical intuition**, and **manual implementation**, avoiding high-level ML libraries entirely.

---

## 🧠 Key Learning Goals

* Implement regression models from first principles
* Understand loss functions and optimization landscapes
* Visualize cost surfaces and convergence behavior
* Compare feature engineering strategies
* Validate portability between local and cloud environments

---

##  Getting Started

The project is fully **self-contained** and does **not rely on external datasets** or machine learning frameworks.

All notebooks are designed to be executed **top-to-bottom** using **Run All**, producing figures and results inline.

---

##  Prerequisites

To run the notebooks locally, you only need:

* **Python 3**
* **NumPy**
* **Matplotlib**

 No use of `scikit-learn`, `TensorFlow`, or similar libraries.

---

##  Project Structure

The project is divided into two main notebooks, each building conceptually on the previous one.

---

##  Part I — Linear Regression with One Feature

In the first notebook, **stellar luminosity** is modeled as a linear function of **stellar mass**.

### Topics covered:

* Visualization of luminosity vs. mass
* Manual implementation of the prediction function
* Mean Squared Error (MSE) as the loss function
* Cost surface visualization over model parameters
* Gradient descent:

  * Loop-based implementation
  * Fully vectorized implementation
* Convergence analysis under different learning rates

### Key insight:

While the linear model captures the **general trend**, it fails to model the **nonlinear growth** of stellar luminosity, especially for higher stellar masses.

---

##  Part II — Polynomial Regression & Interaction Terms

The second notebook extends the model by incorporating **nonlinear features** and **feature interactions** using stellar mass and temperature.

### Feature sets evaluated:

* **M1:** Mass, Temperature
* **M2:** Mass, Temperature, Mass²
* **M3:** Mass, Temperature, Mass², Mass × Temperature

### Topics covered:

* Construction of the design matrix using NumPy
* Fully vectorized loss and gradient computation
* Gradient descent training and convergence plots
* Feature set comparison
* Analysis of interaction terms
* Prediction for a new hypothetical star

### Key insight:

Introducing polynomial and interaction terms **dramatically improves model fit**, highlighting the importance of feature engineering when modeling nonlinear physical phenomena.

---

##  Running the Notebooks

Each notebook can be executed using:

> **Run All**

All figures and outputs are rendered inline, with no external dependencies required.

---

## ☁️ AWS SageMaker Execution Evidence

Both notebooks were uploaded and executed in **AWS SageMaker Studio** using the **Code Editor** environment.

### Execution summary:

* A SageMaker Code Editor space was created using a standard CPU instance
* Project files were uploaded manually
* All cells executed successfully in both notebooks
* All plots rendered correctly with no errors

### Evidence

**Project files inside SageMaker:**

![SageMaker Files](https://github.com/user-attachments/assets/223571ac-2c34-45d0-b566-13f48f7e0a70)

**Execution of Part I notebook:**

![Part I Execution](https://github.com/user-attachments/assets/1b53b855-9d1e-4648-a575-0c2bc9bfc9b7)

**Execution of Part II notebook:**

![Part II Execution](https://github.com/user-attachments/assets/488e8539-7f29-43e0-a213-9b0440ee7e9f)

---

##  Local vs Cloud Execution

The notebooks produced **consistent results** when executed both locally and on **AWS SageMaker**.

 No code modifications were required

This confirms that the implementation is **portable**, **reproducible**, and **cloud-ready**.

---

##  Built With

* **Python**
* **NumPy**
* **Matplotlib**
* **AWS SageMaker Studio**

---

##  Author

**Samuel Antonio Gil Romero**

---

##  Acknowledgments

* Machine Learning Bootcamp course material
* AWS SageMaker Studio for cloud execution support

---

 If you found this project useful, feel free to explore, fork, or build upon it!
