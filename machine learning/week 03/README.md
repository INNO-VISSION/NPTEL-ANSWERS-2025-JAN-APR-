### Week 3: Assignment 3 - Machine Learning

#### 1. Which of the following statement(s) about decision boundaries and discriminant functions of classifiers is/are true?

a) In a binary classification problem, all points x on the decision boundary satisfy δ1(𝑥) = δ2(𝑥).  
b) In a three-class classification problem, all points on the decision boundary satisfy δ1(𝑥) = δ2(𝑥) = δ3(𝑥).  
c) In a three-class classification problem, all points on the decision boundary satisfy at least one of δ1(𝑥) = δ2(𝑥), δ2(𝑥) = δ3(𝑥), or δ3(𝑥) = δ1(𝑥).  
d) If x does not lie on the decision boundary, then all points lying in a sufficiently small neighborhood around x belong to the same class.  

**Answer:** a, c, d  

---

#### 2. You train an LDA classifier on a dataset with 2 classes. The decision boundary is significantly different from the one obtained by logistic regression. What could be the reason?
 
a) The underlying data distribution is Gaussian.  
b) The two classes have equal covariance matrices.  
c) The underlying data distribution is not Gaussian.  
d) The two classes have unequal covariance matrices.  

**Answer:** c, d  

---

#### 3. The following table gives the binary ground truth labels 𝑦𝑖 for four input points 𝑥𝑖 (not given). We have a logistic regression model with some parameter values that computes the probability 𝑝1(𝑥𝑖) that the label is 1. Compute the likelihood of observing the data given these model parameters.

a) 0.072  
b) 0.144  
c) 0.288  
d) 0.002  

**Answer:** c) 0.288  

---

#### 4. Which of the following statement(s) about logistic regression is/are true?
 
a) It learns a model for the probability distribution of the data points in each class.  
b) The output of a linear model is transformed to the range (0,1) by a sigmoid function.  
c) The parameters are learned by minimizing the mean-squared loss.  
d) The parameters are learned by maximizing the log-likelihood.  

**Answer:** b, d  

---

#### 5. Consider a modified form of logistic regression given below where 𝑘 is a positive constant and β0 and β1 are parameters. Which of the following expressions correctly represents the probability function?

a) 
𝑒
−
𝛽
1
𝑥
𝑘
𝑒
𝛽
0
𝑒
−
𝛽
1
𝑥
+
𝑒
𝛽
0
e 
−β 
1
 x
 +e 
β 
0
e 
−β 
1
 x
 ke 
β 
0

  
b) 
𝑒
𝛽
1
𝑥
𝑘
𝑒
𝛽
0
𝑒
𝛽
1
𝑥
+
𝑒
𝑘
𝛽
1
𝑥
e 
β 
1
 x
 +e 
kβ 
1
 x
e 
β 
1
 x
 ke 
β 
0

c) 
𝑒
−
𝛽
1
𝑥
𝑒
−
𝛽
0
𝑒
−
𝛽
1
𝑥
+
𝑒
𝑘
𝛽
1
𝑥
e 
−β 
1
 x
 +e 
kβ 
1
 x 
e 
−β 
1
 x
 e 
−β 
0
 
d) 
𝑒
−
𝛽
1
𝑥
𝑘
𝑒
𝛽
0
𝑒
−
𝛽
1
𝑥
+
𝑒
−
𝛽
1
𝑥
e 
−β 
1
 x
 +e 
−β 
1
 x 
e 
−β 
1
 x
 ke 
β 
0 

**Answer:** a  

---

#### Question 6. Consider a Bayesian classifier for a 5-class classification problem. The following tables give the class-conditioned density 𝑓𝑘(𝑥) for class 𝑘 ∈ {1,2,...5} at some point x in the input space. Let π𝑘 denote the prior probability of class 𝑘. Which of the following statement(s) about the predicted label at x is/are true?
 
a) The predicted label at x will always be class 4.  
b) If 2π𝑖 ≤ π𝑖+1 ∀ i ∈ {1,...4}, the predicted class must be class 4.  
c) If π𝑖 ≥ 3/2π𝑖+1 ∀ i ∈ {1,...4}, the predicted class must be class 1.  
d) The predicted label at x can never be class 5.  

**Answer:** b, c  

---

#### 7. Which of the following statement(s) about a two-class LDA classification model is/are true?



a) On the decision boundary, the prior probabilities corresponding to both classes must be equal.  
b) On the decision boundary, the posterior probabilities corresponding to both classes must be equal.  
c) On the decision boundary, class-conditioned probability densities corresponding to both classes must be equal.  
d) On the decision boundary, the class-conditioned probability densities corresponding to both classes may or may not be equal.  

**Answer:** b, d  

---

#### 8. Consider the following two datasets and two LDA classifier models trained respectively on these datasets.

Dataset A: 200 samples of class 0; 50 samples of class 1  
Dataset B: 200 samples of class 0 (same as Dataset A); 100 samples of class 1 created by repeating twice the class 1 samples from Dataset A  

Let the classifier decision boundary learned be of the form w^T x + b = 0, where w is the slope and b is the intercept. Which of the given statements is true?
 
a) The learned decision boundary will be the same for both models.  
b) The two models will have the same slope but different intercepts.  
c) The two models will have different slopes but the same intercept.  
d) The two models may have different slopes and different intercepts.  

**Answer:** b  

---

#### 9. Which of the following statement(s) about LDA is/are true?

a) It minimizes the inter-class variance relative to the intra-class variance.  
b) It maximizes the inter-class variance relative to the intra-class variance.  
c) Maximizing the Fisher information results in the same direction of the separating hyperplane as the one obtained by equating the posterior probabilities of classes.  
d) Maximizing the Fisher information results in a different direction of the separating hyperplane from the one obtained by equating the posterior probabilities of classes.  

**Answer:** b, c  

---

#### 10. Which of the following statement(s) regarding logistic regression and LDA is/are true for a binary classification problem?
 
a) For any classification dataset, both algorithms learn the same decision boundary.  
b) Adding a few outliers to the dataset is likely to cause a larger change in the decision boundary of LDA compared to that of logistic regression.  
c) Adding a few outliers to the dataset is likely to cause a similar change in the decision boundaries of both classifiers.  
d) If the intra-class distributions deviate significantly from the Gaussian distribution, logistic regression is likely to perform better than LDA.  

**Answer:** b, d
