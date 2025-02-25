### Week 4: Assignment 4 - Machine Learning  



##### 1. The Perceptron Learning Algorithm can always converge to a solution if the dataset is linearly separable.  

- a) True  
- b) False  
- c) Depends on learning rate  
- d) Depends on initial weights  

**Answer:** a) True  

---

##### 2. Consider the 1-dimensional dataset:  

State true or false: The dataset becomes linearly separable after using basis expansion with the following basis function  
𝜙(𝑥) = [ 1 𝑥² ]  

- a) True  
- b) False  

**Answer:** a) True  

---

##### 3. For a binary classification problem with the hinge loss function  
**𝑚𝑎𝑥(0,1−𝑦(𝑤·𝑥))**, which of the following statements is correct?  

- a) The loss is zero only when the prediction is exactly equal to the true label  
- b) The loss is zero when the prediction is correct and the margin is at least 1  
- c) The loss is always positive  
- d) The loss increases linearly with the distance from the decision boundary regardless of classification  

**Answer:** b) The loss is zero when the prediction is correct and the margin is at least 1  

---

##### 4. For a dataset with n points in d dimensions, what is the maximum number of support vectors possible in a hard-margin SVM?  

- a) 2  
- b) d  
- c) n/2  
- d) n  

**Answer:** d) n  

---

##### 5. In the context of soft-margin SVM, what happens to the number of support vectors as the parameter C increases?  

- a) Generally increases  
- b) Generally decreases  
- c) Remains constant  
- d) Changes unpredictably  

**Answer:** a) Generally increases  

---

##### 6. Consider the following dataset:  

Which of these is not a support vector when using a Support Vector Classifier with a polynomial kernel with degree = 3, C = 1, and gamma = 0.1?  

- a) 2  
- b) 1  
- c) 9  
- d) 10  

**Answer:** c) 9  

---

##### 7. Train a Linear Perceptron classifier on the modified Iris dataset. Use only the first two features for your model and report the best classification accuracy for L1 and L2 penalty terms.  

- a) 0.91, 0.64  
- b) 0.88, 0.71  
- c) 0.71, 0.65  
- d) 0.78, 0.64  

**Answer:** a) 0.91, 0.64  

---

##### 8. Train an SVM classifier on the modified Iris dataset. Use only the first three features. Experiment with different kernels and hyperparameters. Specifically, train models with the following set of hyperparameters:  
**RBF-kernel, gamma = 0.5, one-vs-rest classifier, no-feature-normalization.**  
Try **C = 0.01, 1, 10** and report the best classification accuracy.  

- a) 0.98  
- b) 0.88  
- c) 0.99  
- d) 0.92  

**Answer:** c) 0.99  
