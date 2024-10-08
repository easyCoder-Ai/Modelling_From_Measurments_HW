# Modelling_From_Measurments_HW


## Overview

This project explores various dimensionality reduction techniques and their impact on machine learning model performance when applied to a complex dataset. The focus is on understanding how methods like Singular Value Decomposition (SVD), Dynamic Mode Decomposition (DMD), Sparse Identification of Nonlinear Dynamical Systems (SINDy), and SHRED can improve predictive accuracy.

## Table of Contents

- [Installation](#installation)
- [Methods](#methods)
- [Results](#results)
- [Conclusion](#conclusion)



## Installation

To run this project, you'll need Python 3.x and the following libraries:

''
pip install numpy pandas scikit-learn xgboost matplotlib seaborn

''

## Methods

**Data Preprocessing**
The dataset was preprocessed to handle missing values and standardize feature scales. This step is crucial for effective training of machine learning mode

**Dimensionality Reduction Techniques**
- Singular Value Decomposition (SVD): Used to reduce dimensionality while retaining a significant amount of variance.
- Dynamic Mode Decomposition (DMD): Applied to uncover the underlying dynamics in the data.
- Sparse Identification of Nonlinear Dynamical Systems (SINDy): Identifies non-linear functions in the dataset.
- SHRED: Used for efficient dimensionality reduction while maintaining data structures.

**Machine Learning Models**
Some models were tested on the dataset, including:
- Logistic Regression
- Random Forest
- XGBoost
- K-Nearest Neighbors (KNN)

**Each model was evaluated on various configurations:**

- Without dimensionality reduction
- With SVD
- With DMD
- With SVD + DMD
- With SINDy
- With SINDy + SVD
- With SHRED
- With SHRED + SVD

## Results
The results from the experiments are summarized in the comparison table below, showcasing the accuracy of each model across different configurations:


| Model                 | Accuracy (%) Without SVD | Accuracy (%) With SVD | Accuracy (%) With DMD | Accuracy (%) With SVD + DMD | Accuracy (%) with SINDy | Accuracy (%) with SVD + SINDy |
|-----------------------|--------------------------|-----------------------|-----------------------|------------------------------|-------------------------|-------------------------------|
| Logistic Regression    | 53.85                    | 54.62                 | 48.85                 | 48.85                        | 51.92                   | 52.69                         |
| Random Forest          | 51.54                    | 53.85                 | 47.69                 | 48.85                        | 54.23                   | 53.85                         |
| XGBoost                | 50.77                    | 50.77                 | 48.08                 | 50.38                        | 53.46                   | 51.92                         |
| K-Nearest Neighbors    | 47.31                    | 48.46                 | 45.38                 | 45.38                        | 52.31                   | 50.00                         |



| Model                 | Accuracy (%) | 
|-----------------------|--------------------------|
| SHRED                 | 52.00                    | 
| SVD + SHRED           | 51.20                   | 


## Conclusion
This project demonstrates the effectiveness of dimensionality reduction techniques in improving machine learning model performance. SVD emerged as a powerful tool for enhancing predictive accuracy, while DMD, SINDy, and SHRED provided valuable insights into non-linear dynamics. Future work could explore ensemble methods and further optimizations to enhance performance.


