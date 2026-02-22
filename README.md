# Texture Feature Classification on Fashion-MNIST

A comparative study of classical machine learning models using texture-based feature extraction on the Fashion-MNIST dataset.

---

## Overview

This project implements an image classification pipeline that replaces raw pixel inputs with structured texture features using Histogram of Oriented Gradients (HOG). The extracted features are evaluated using Gaussian Naïve Bayes and Random Forest classifiers.

The objective is to analyze the trade-off between computational efficiency and predictive performance.

---

## Dataset

**Fashion-MNIST**

- 70,000 grayscale images (28×28)
- 10 clothing categories
- 60,000 training samples
- 10,000 testing samples
- Pixel values normalized to [0, 1]

---

## Methodology

### Feature Extraction — HOG

- 9 orientation bins  
- 8×8 pixel cell size  
- 2×2 cell block size  

HOG captures local gradient patterns and produces a compact, discriminative feature representation.

---

### Classification Models

#### Gaussian Naïve Bayes
- Probabilistic generative model  
- Assumes conditional independence  
- Extremely fast training  

#### Random Forest (100 Trees)
- Ensemble of decision trees  
- Uses bagging and random feature selection  
- Captures nonlinear feature interactions  

---

## Results

| Model | Test Accuracy | Training Time (s) |
|--------|--------------|-------------------|
| Gaussian Naïve Bayes | 70.90% | 0.07 |
| Random Forest (100 Trees) | 82.49% | 153.15 |

---

## Key Observations

- Random Forest achieved higher accuracy.
- Naïve Bayes trained significantly faster.
- Improved predictive performance comes at higher computational cost.

---


## Technologies

- Python  
- NumPy  
- scikit-learn  
- scikit-image  
- Matplotlib  

---

## Conclusion

Texture-based feature extraction combined with classical machine learning provides strong performance on Fashion-MNIST. Random Forest offers higher accuracy, while Gaussian Naïve Bayes delivers superior computational efficiency, highlighting the trade-off between model complexity and training cost.


## Authors
Rahul Suresh , Arjun Balaji 

CSE Department , SSNCE
