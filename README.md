# Project Description

The goal of this project is to implement different classifiers to achieve face recogntion.
You are given a set of faces and their corresponding labels. The given data set is divided in training and testing set is used to train the classifiers.

There are two tasks:
1. Identifying the subject label from a test image.
2. Neutral vs. facial expression classification

# Pipeline

In this project, the following classifiers are implemented for face recognition.

**1. Bayes' Classifier:** Assuming the underlying distribution is Gaussian, you need to implement the
Maximum Likelihood estimation with Gaussian assumption followed by Bayes’
classification.

**2. k-NN Rule:** Implement the k-Nearest Neighbors (k-NN) rule to classify the test data. Vary
k to see its effect.

**3. Kernel SVM:** Implement the Kernel SVM classifier by solving the dual optimization problem. Use the Radial Basis Function (RBF) and the polynomial kernel. Choose the optimal values of &sigma;<sup>2</sup> and r using cross-validation 

**4. Boosted SVM:** Implement the AdaBoost algorithm for the class of linear SVMs. Investigate the improvement of the boosted classifiers with respect to the iterations of
AdaBoost, and compare it with the performance of the Kernel SVMs. 

**5. PCA:** Implement Principal Component Analysis (PCA) and apply it to
the data before feeding it into the classifiers above.

**6. MDA:** Similar to PCA, implement MDA followed by the training/appli-
cation of the classifiers.
