# Stellar Luminosity Regression

This project explores how stellar luminosity can be modeled using regression techniques implemented from first principles. The goal is to understand the behavior and limitations of linear models and how polynomial and interaction terms can improve predictive performance.

The project is part of a machine learning bootcamp focused on understanding core concepts without relying on high-level machine learning libraries.

---

## Getting Started

These instructions will help you understand the structure of the project and how the notebooks are organized.

The implementation is fully self-contained and does not require external datasets or machine learning frameworks.

---

## Prerequisites

To run the notebooks locally, you need:

- Python 3
- NumPy
- Matplotlib

No machine learning libraries such as scikit-learn or TensorFlow are used.

---

## Project Structure


---

## Part I — Linear Regression with One Feature

In the first notebook, stellar luminosity is modeled as a linear function of stellar mass.

This part includes:
- Visualization of luminosity versus mass
- Manual implementation of the prediction function
- Mean Squared Error (MSE) as the loss function
- Cost surface visualization over the parameters
- Gradient descent implemented with loops and vectorized operations
- Convergence analysis with different learning rates

The results show that while a linear model captures the general trend, it cannot fully represent the nonlinear growth of stellar luminosity, especially for higher masses.

---

## Part II — Polynomial Regression and Interaction Terms

The second notebook extends the model by introducing polynomial and interaction features based on stellar mass and temperature.

Three feature sets are compared:
- **M1:** Mass and temperature
- **M2:** Mass, temperature, and squared mass
- **M3:** Mass, temperature, squared mass, and mass–temperature interaction

This notebook includes:
- Construction of a design matrix using NumPy
- Fully vectorized loss and gradient computation
- Gradient descent training and convergence visualization
- Feature selection comparison
- Analysis of the interaction term
- Prediction for a new hypothetical star

Adding nonlinear and interaction terms significantly improves the quality of the fit compared to the linear model.

---

## Running the Notebooks

Each notebook is designed to be run from top to bottom using the **Run All** option. All figures are generated inline.

---

## AWS SageMaker Execution Evidence

Both notebooks were uploaded and executed in **AWS SageMaker Studio** using the Code Editor environment.

### Execution summary

- A SageMaker Code Editor space was created with a standard CPU instance.
- The project files were uploaded manually to the cloud environment.
- All cells in both notebooks were executed successfully.
- Plots and outputs were rendered without errors.

### Evidence

**Project files inside SageMaker:**

![SageMaker Files](images/sagemaker_files.png)

**Execution of Part I notebook:**

![Part I Execution](images/sagemaker_part1.png)

**Execution of Part II notebook:**

![Part II Execution](images/sagemaker_part2.png)

### Local vs Cloud Execution

The notebooks produced consistent results when executed locally and in AWS SageMaker. No code modifications were required, confirming that the implementation is portable and cloud-ready.

---

## Built With

- Python
- NumPy
- Matplotlib
- AWS SageMaker Studio

---

## Author

**Samuel Antonio Gil Romero**

---

## Acknowledgments

- Course material and datasets provided as part of the Machine Learning Bootcamp
- AWS SageMaker for cloud execution support

