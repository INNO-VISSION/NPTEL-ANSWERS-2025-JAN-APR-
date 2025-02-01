### Week 1: Assignment 1 - Machine Learning

### Questions and Answers

#### **1. Which of the following is/are unsupervised learning problem(s)?**
**Options:**  
 a) Sorting a set of news articles into four categories based on their titles  
 b) Forecasting the stock price of a given company based on historical data  
 c) Predicting the type of interaction (positive/negative) between a new drug and a set of human proteins  
 d) Identifying close-knit communities of people in a social network  
 e) Learning to generate artificial human faces using the faces from a facial recognition dataset  
**Answer:** a, d, e

---

#### **2. Which of the following statement(s) about Reinforcement Learning (RL) is/are true?**
**Options:**  
 a) While learning a policy, the goal is to maximize the reward for the current time step  
 b) During training, the agent is explicitly provided the most optimal action to be taken in each state.  
 c) The actions taken by an agent do not affect the environment in any way.  
 d) RL agents used for playing turn-based games like chess can be trained by playing the agent against itself (self-play).  
 e) RL can be used in an autonomous driving system.  
**Answer:** d, e

---

#### **3. Which of the following is/are regression tasks(s)?**
**Options:**  
 a) Predicting whether an email is spam or not spam  
 b) Predicting the number of new CoVID cases in a given time period  
 c) Predicting the total number of goals a given football team scores in a year  
 d) Identifying the language used in a given text document  
**Answer:** b, c

---

#### **4. Which of the following is/are classification task(s)?**
**Options:**  
 a) Predicting whether or not a customer will repay a loan based on their credit history  
 b) Forecasting the weather (temperature, humidity, rainfall, etc.) at a given place for the following 24 hours  
 c) Predicting the price of a house 10 years after it is constructed.  
 d) Predicting if a house will be standing 50 years after it is constructed.  
**Answer:** a, d

---

#### **5. Consider the following dataset. Fit a linear regression model of the form 𝑦=𝛽0+𝛽1𝑥1+𝛽2𝑥2 using the mean-squared error loss. Using this model, the predicted value of 𝑦 at the point (𝑥1,𝑥2) = (0.5, −1.0) is:**
**Options:**  
 a) 4.05  
 b) 2.05  
 c) −1.95  
 d) −3.95  
**Answer:** b

---

#### **6. Using a k-nearest neighbour (k-NN) regression model with 𝑘 = 3, predict the value of 𝑦 at (𝑥1,𝑥2) = (1.0, 0.5). Use the Euclidean distance to find the nearest neighbours.**
**Options:**  
 a) −1.766  
 b) −1.166  
 c) 1.133  
 d) 1.733  
**Answer:** b

---

#### **7. Using a k-NN classifier with k = 5, predict the class label at the point (𝑥1,𝑥2) = (1.0, 1.0). Use the Euclidean distance to find the nearest neighbours.**
**Options:**  
 a) 0  
 b) 1  
 c) 2  
 d) Cannot be predicted  
**Answer:** b

---

#### **8. Consider the following statements regarding linear regression and k-NN regression models. Select the true statements.**
**Options:**  
 a) A linear regressor requires the training data points during inference.  
 b) A k-NN regressor requires the training data points during inference.  
 c) A k-NN regressor with a higher value of k is less prone to overfitting.  
 d) A linear regressor partitions the input space into multiple regions such that the prediction over a given region is constant.  
**Answer:** b, c

---

#### **9. Which of the following statement(s) regarding bias and variance is/are correct?**
**Options:**  
 a) Bias=𝔼[(𝔼[𝑓̂ (𝑥)]−𝑓̂ (𝑥))2]; Variance=𝔼[(𝑓̂ (𝑥)−𝑓(𝑥))2]  
 b) Bias=𝔼[𝑓̂ (𝑥)]−𝑓(𝑥); Variance=𝔼[(𝔼[𝑓̂ (𝑥)]−𝑓̂ (𝑥))2]  
 c) Low bias and high variance is a sign of overfitting  
 d) Low variance and high bias is a sign of overfitting  
 e) Low variance and high bias is a sign of underfitting  
**Answer:** c, e

---

#### **10. Suppose that we train two kinds of regression models corresponding to the following equations.**
(i). 𝑦=𝛽0+𝛽1𝑥1+𝛽2𝑥2  
(ii). 𝑦=𝛽0+𝛽1𝑥1+𝛽2𝑥2+𝛽3𝑥1𝑥2+𝛽4𝑥21+𝛽5𝑥22  

Which of the following statement(s) is/are correct?

**Options:**  
 a) On a given training dataset, the mean-squared error of (i) is always less than or equal to that of (ii).  
 b) (i) is likely to have a higher variance than (ii).  
 c) (ii) is likely to have a higher variance than (i).  
 d) If (i) overfits the data, then (ii) will definitely overfit.  
 e) If (ii) underfits the data, then (i) will definitely underfit.  
**Answer:** c, e
