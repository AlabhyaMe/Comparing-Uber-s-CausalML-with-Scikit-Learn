🧠 Causal Inference with T-Learners: Scikit-Learn vs. CausalML
This project demonstrates how to implement and compare T-Learners using both a manual approach with Scikit-Learn and an automated approach using CausalML, Uber’s open-source Python package for estimating individualized treatment effects.

The goal is to:

Build intuition around meta-learners like the T-Learner

Understand what happens under the hood of the CausalML API

Validate that both implementations produce consistent results

Showcase how CausalML simplifies causal modeling while preserving rigor

📂 Contents
notebook.ipynb: Full code walkthrough comparing the two methods

README.md: Project overview and instructions

Simulated dataset using random assignment and known treatment effects

⚙️ What’s Covered
Data Preparation

Synthetic dataset simulating randomized treatment (insurance) and expenditure outcome

T-Learner with Scikit-Learn

Manual implementation of T-Learner using LinearRegression

Separate models for treatment and control groups

Prediction and calculation of individual treatment effects (ITEs)

T-Learner with CausalML

Streamlined implementation using BaseTLearner from causalml.inference.meta

Automated handling of treatment/control modeling and ITE prediction

Conversion to NumPy (as CausalML does not support Polars directly)

Validation & Comparison

Row-wise comparison of ITEs from both methods

Statistical checks (mean, std, min, max)

Visual comparison using histograms

Summary

Key findings about accuracy, efficiency, and clarity of the CausalML package

🛠 Requirements
Python 3.8+

scikit-learn

causalml

polars

numpy

matplotlib or seaborn for visualization

🚀 Running the Project
Clone this repository

Open the Jupyter notebook

Run each cell to walk through the manual and automated T-Learner implementations

Review the final comparison metrics and visualizations

🧾 Conclusion
Both Scikit-Learn and CausalML implementations produce nearly identical individual treatment effects, validating the consistency of the methods. However, CausalML offers a cleaner, faster, and more maintainable approach, especially for large-scale or production-grade causal inference tasks.
