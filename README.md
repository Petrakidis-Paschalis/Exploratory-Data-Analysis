# 🌌 SDSS Galaxy Redshift Prediction

An end-to-end Exploratory Data Analysis (EDA) and Machine Learning pipeline exploring the relationship between a galaxy's photometric flux and its cosmic distance (Redshift).

Built using the **Multimodal Universe SDSS Galaxy Catalog**, this project processes photometric and spectral modalities to train regression models from scratch.

## 🚀 Project Highlights
* **Multimodal Feature Engineering:** Extracted and combined photometric bands (u, g, r, i, z) with spectral kinematic data (Velocity Dispersion).
* **Custom Gradient Descent:** Implemented a gradient descent optimization algorithm entirely from scratch to train the models.
* **Non-Linear Modeling:** Successfully diagnosed an L-shaped data distribution, transitioned from Linear to Polynomial Regression, and handled exploding gradients via targeted feature scaling.
* **Probabilistic Evaluation:** Conducted residual analysis comparing parametric Gaussian fits against non-parametric Kernel Density Estimation (KDE) to prove the nature of astronomical errors.

## 📊 Models Built
1. **Simple Linear Regression** (Predicting Redshift via r-band Flux)
2. **Multivariate Linear Regression** (Incorporating 5 bands + Velocity Dispersion)
3. **Degree-2 Polynomial Regression** (Capturing the non-linear physics of the dataset)

## 🛠️ How to Run
1. Clone this repository.
2. Have a look at the **hw1** notebook!
* The dataset **sdss_data.csv** is included, but ensure you have the datasets library installed:

```
pip install datasets
```