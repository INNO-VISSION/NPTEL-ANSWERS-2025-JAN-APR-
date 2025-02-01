## Week 2: Assignment 2 - Machine Learning

#### 1. In a linear regression model:

\[ y = \theta_0 + \theta_1 x_1 + \theta_2 x_2 + ... + \theta_p x_p \]

What is the purpose of adding an intercept term (\( \theta_0 \))?

- (a) To increase the model’s complexity
- (b) To account for the effect of independent variables
- (c) To adjust for the baseline level of the dependent variable when all predictors are zero
- (d) To ensure the coefficients of the model are unbiased

**Answer:** (c) To adjust for the baseline level of the dependent variable when all predictors are zero

---

#### 2.Which of the following is true about the cost function (objective function) used in linear regression?

- (a) It is non-convex
- (b) It is always minimized at \( \theta = 0 \)
- (c) It measures the sum of squared differences between predicted and actual values
- (d) It assumes the dependent variable is categorical

**Answer:** (c) It measures the sum of squared differences between predicted and actual values

---

#### 3. Which of these would most likely indicate that Lasso regression is a better choice than Ridge regression?

**Options:**
- (a) All features are equally important
- (b) Features are highly correlated
- (c) Most features have small but non-zero impact
- (d) Only a few features are truly relevant

**Answer:** (d) Only a few features are truly relevant

---

#### 4. Which of the following conditions must hold for the least squares estimator in linear regression to be unbiased?

- (a) The independent variables must be normally distributed
- (b) The relationship between predictors and the response must be non-linear
- (c) The errors must have a mean of zero
- (d) The sample size must be larger than the number of predictors

**Answer:** (c) The errors must have a mean of zero

---

#### 5. When performing linear regression, which of the following is most likely to cause overfitting?

- (a) Adding too many regularization terms
- (b) Including irrelevant predictors in the model
- (c) Increasing the sample size
- (d) Using a smaller design matrix

**Answer:** (b) Including irrelevant predictors in the model

---

#### 6.You have trained a complex regression model on a dataset. To reduce its complexity, you decide to apply Ridge regression, using a regularization parameter \( \lambda \). How does the relationship between bias and variance change as \( \lambda \) becomes very large?

- (a) Bias is low, variance is low
- (b) Bias is low, variance is high
- (c) Bias is high, variance is low
- (d) Bias is high, variance is high

**Answer:** (c) Bias is high, variance is low

---

#### 7.Given a training dataset of 10,000 instances, with each input instance having 12 dimensions and each output instance having 3 dimensions, what are the dimensions of the design matrix used in applying linear regression to this data?

- (a) 10000 × 12
- (b) 10003 × 12
- (c) 10000 × 13
- (d) 10000 × 15

**Answer:** (c) 10000 × 13 (including the intercept term)

---

#### 8. The linear regression model:

\[ y = a_0 + a_1 x_1 + a_2 x_2 + ... + a_p x_p \]

is to be fitted to a set of \( N \) training data points having \( p \) attributes each. Let \( X \) be an \( N \times (p+1) \) matrix of input values (augmented by 1’s), \( Y \) be an \( N \times 1 \) vector of target values, and \( \theta \) be a \( (p+1) \times 1 \) vector of parameter values. If the sum squared error is minimized for obtaining the optimal regression model, which of the following equations holds?

- (a) \( X^T X = X Y \)
- (b) \( X \theta = X^T Y \)
- (c) \( X^T X \theta = Y \)
- (d) \( X^T X \theta = X^T Y \)

**Answer:** (d) \( X^T X \theta = X^T Y \)

---

#### 9. Which of the following scenarios is most appropriate for using Partial Least Squares (PLS) regression instead of ordinary least squares (OLS)?

- (a) When the predictors are uncorrelated and the number of samples is much larger than the number of predictors
- (b) When there is significant multicollinearity among predictors or the number of predictors exceeds the number of samples
- (c) When the response variable is categorical and the predictors are highly non-linear
- (d) When the primary goal is to interpret the relationship between predictors and response, rather than prediction accuracy

**Answer:** (b) When there is significant multicollinearity among predictors or the number of predictors exceeds the number of samples

---

#### 10. Consider forward selection, backward selection, and best subset selection with respect to the same dataset. Which of the following is true?

- (a) Best subset selection can be computationally more expensive than forward selection
- (b) Forward selection and backward selection always lead to the same result
- (c) Best subset selection can be computationally less expensive than backward selection
- (d) Best subset selection and forward selection are computationally equally expensive
- (e) Both (b) and (d)

**Answer:** (a) Best subset selection can be computationally more expensive than forward selection

