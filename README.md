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

**3. Kernel SVM:** Implement the Kernel SVM classifier by solving the dual optimization problem. Use the Radial Basis Function (RBF) and the polynomial kernel. Choose the optimal values of &sigma;<sup>2</sup> and r using cross-validation.

**4. Boosted SVM:** Implement the AdaBoost algorithm for the class of linear SVMs. Investigate the improvement of the boosted classifiers with respect to the iterations of
AdaBoost, and compare it with the performance of the Kernel SVMs. 

**5. PCA:** Implement Principal Component Analysis (PCA) and apply it to
the data before feeding it into the classifiers above.

**6. MDA:** Similar to PCA, implement MDA followed by the training/appli-
cation of the classifiers.

# Dataset
Dataset consists of 600 images of 200 subjects. Each subject has one neutral face image and one image with expression and the last image is of neutral face but varied illumination.

# Results and Analysis
## Face Recognition

**1. PCA Analysis:**

![1](https://user-images.githubusercontent.com/90370308/217112368-6b8d18d5-b613-46de-b71e-ff3a67ba989e.png)![PCA image](https://user-images.githubusercontent.com/90370308/217111283-4f7fbd50-98e7-4e8e-9448-d34221691c23.png)

The above figure shows the graph of cumulative data variance vs number of eigen values. As shown in the graph, we can say that about 90% of the data variance are containing in top 100 eigen values (out of 504 eigen values). After 100 eigen values, the rate of change of variance with respect to number of eigen value is very small. Hence, to go from 90% to 95%, we need to add 100 more eigen value which is computationally expensive. Hence, in PCA compression, top 100 eigen vector are taken. So, the data is transformed from 504 dimension to 100 dimension.

**2. MDA Analysis:**

![2](https://user-images.githubusercontent.com/90370308/217113155-4b1a99c9-b94f-4c95-ad91-a4cd22e68cb7.png)![MDA image](https://user-images.githubusercontent.com/90370308/217113192-455497dd-9f88-4c46-b3de-be5a9d33988b.png)

The above figure shows the graph of cumulative data variance vs number of eigen values. As shown in
the graph, we can say that about 95% of the data variance are containing in top 100 eigen values (out of
504 eigen values). After 100 eigen values, the rate of change of variance with respect to number of
eigen value is very small. Hence, to go from 95% to 98%, we need to add 100 more eigen value which
is computationally expensive. Hence, in MDA compression, top 100 eigen vector are taken. So, the
data is transformed from 504 dimension to 100 dimension.








