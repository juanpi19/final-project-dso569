# Deep Learning for Causal Inference

This README summarizes the key points and contributions of the paper "Deep Learning for Causal Inference" by Vikas Ramachandra.

## 1. Generalized Neighbor Matching using Autoencoders

The paper proposes using autoencoders, a type of deep neural network, for dimensionality reduction while preserving the local neighborhood structure of the data. This is useful for generalized neighbor matching to estimate individual treatment effects (ITEs).

The key points are:

* In high dimensions, traditional neighbor matching methods like k-nearest neighbors struggle
* Autoencoders can learn a low-dimensional representation that captures the manifold structure
* This low-dimensional encoding preserves local neighborhoods for accurate neighbor identification
* Experiments show autoencoders outperform methods like manifold learning for ITE estimation

## 2. Deep Neural Networks (DNNs) for Propensity Score Matching

Propensity score matching is a popular technique, but traditionally uses logistic regression for propensity score estimation. The paper proposes using deep neural network classifiers instead, presenting a model called PropensityNet.

The key points are:

* DNNs can potentially capture complex non-linear relationships better than logistic regression
* PropensityNet is trained to estimate propensity scores as a binary classification problem
* Experiments show PropensityNet outperforms logistic regression for propensity score estimation
* This leads to better matching of treated and untreated units for ITE calculation

## Overall Contribution

The paper argues that deep learning models like autoencoders and DNNs can improve upon traditional methods for neighbor matching and propensity score estimation, two crucial steps in causal inference for estimating individual and average treatment effects.

The main contributions are introducing these deep learning approaches, evaluating them on simulated datasets, and demonstrating their potential advantages over existing techniques through experimental results.
