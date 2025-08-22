# Optimizing Convolutional Neural Networks: A Comparative Study of Scheduling Algorithms and Regularization Techniques

## Overview
This project investigates the optimization of Convolutional Neural Networks (CNNs) through a comparative study of scheduling algorithms and regularization methods. The goal is to enhance accuracy, improve training efficiency, and mitigate overfitting by applying diverse optimization strategies.


## Problem Definition
Training CNNs often suffers from overfitting and unstable convergence due to learning rate and regularization challenges. This project explores how different schedulers and regularization techniques influence model performance.  

Optimization problem:  
\[
\min L(\lambda) \quad \text{subject to regularization constraints}
\]  
where \( L(\lambda) \) is the CNN loss function and constraints include dropout and weight decay.  

## Methodology
1. **Datasets**: CIFAR-10, MNIST  
2. **Scheduling Algorithms**: Step decay, one-cycle policy, cosine annealing  
3. **Regularization Techniques**: Dropout, weight decay, batch normalization  
4. **Evaluation Metrics**: Training/validation accuracy, validation loss, overfitting reduction  

## Results
- **Model 1**: Step decay scheduler, dropout, batch normalization → 59.7% validation accuracy  
- **Model 2**: One-cycle scheduler, tuned dropout and weight decay → 66% validation accuracy  
- **Model 3**: Cosine annealing scheduler, deeper architecture, data augmentation → **84% validation accuracy**, lowest overfitting  

Key finding: Advanced scheduling combined with stronger regularization significantly improves CNN generalization and performance.  

## Tools and Libraries
- TensorFlow / Keras  
- NumPy, pandas  
- Matplotlib, seaborn  

## Code
Project notebook: [Google Colab Link](https://colab.research.google.com/drive/1CuuAmssE992Du9oSdwQYNozIB417Hk_v?authuser=1#scrollTo=3IG2TPC3tJvr)  

## References
1. Goodfellow, I., Bengio, Y., & Courville, A. (2016). *Deep Learning*. MIT Press.  
2. He, K., Zhang, X., Ren, S., & Sun, J. (2016). Deep Residual Learning for Image Recognition. *CVPR*.  
3. Srivastava, N., Hinton, G. E., Krizhevsky, A., Sutskever, I., & Salakhutdinov, R. (2014). Dropout: A Simple Way to Prevent Neural Networks from Overfitting. *JMLR*.  
