# Machine Learning Project

This is the optional project of machine learning.
Detailed report: [Report](https://github.com/SandyHuang119/ML-project/tree/master/Report)

---------------------------
## Motivation

Our project comes from a problem of twitter: User vs. Bots, a user recognition problem aimed to distinguish users from Twitterbots. In this project, we try to build a model to classify bots to solve this problem, and give prediction of whether an account is a user or a bot.

---------------------------
## Data
[bots_data.csv](https://github.com/SandyHuang119/ML-project/blob/master/Data/bots_data.csv)

[nonbots_data.csv](https://github.com/SandyHuang119/ML-project/blob/master/Data/nonbots_data.csv)

## Conclusion
According to the training model,  
Auc score  Decision Tree > Random Forest > Gradient Boosting Decision Tree > Logistic Regression > BernoulliNB
The best model is Decision tree, but according to the result of testing data, the accuracy and precision of decision tree is not as better as random forest, which is due to decision tree will easily cause overfiting, so it can do it pretty well in training data but badly in testing data.

Logistic regression is the worst result,  because there are 16 attributes in each sample, it is hard to guarantee these samples are linear. For logistic regression, it can perform really well in linear data instead of non-linear data. So in this method, we simply deal with samples as linear data, which is not very accurate, so the testing accuracy is not very good compared with other algorithm.For decision tree, we have 16 attributes in each sample, one single decision tree can easily have high depth which causes over fit. But Random forest solve the over fit problem by randomly chose fixed samples and build decision tree for multiple times, then computing the mean. So, that is why random forest perform better than single decision tree.


