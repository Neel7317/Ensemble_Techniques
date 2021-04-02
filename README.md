# Ensemble_Techniques
# (1) Bagging 
  # *random Forest*:
 Random Forest is a popular machine learning algorithm that belongs to the supervised learning technique. It can be used for both Classification and Regression problems in ML. It is based on the concept of ensemble learning, which is a process of combining multiple classifiers to solve a complex problem and to improve the performance of the model.

As the name suggests, "Random Forest is a classifier that contains a number of decision trees on various subsets of the given dataset and takes the average to improve the predictive accuracy of that dataset." Instead of relying on one decision tree, the random forest takes the prediction from each tree and based on the majority votes of predictions, and it predicts the final output
  How dose rendom forest is work:

Step-1: Select random K data points from the training set.

Step-2: Build the decision trees associated with the selected data points (Subsets).

Step-3: Choose the number N for decision trees that you want to build.

Step-4: Repeat Step 1 & 2.

Step-5: For new data points, find the predictions of each decision tree, and assign the new data points to the category that wins the majority votes.
# (2) Boosting:
 # *Adaboost Classifier* 
 The general idea behind boosting methods is to train predictors sequentially, each trying to correct its predecessor. The two most commonly used boosting algorithms are AdaBoost and Gradient Boosting. In the proceeding article, we’ll cover AdaBoost. At a high level, AdaBoost is similar to Random Forest in that they both tally up the predictions made by each decision trees within the forest to decide on the final classification. There are however, some subtle differences. For instance, in AdaBoost, the decision trees have a depth of 1 (i.e. 2 leaves). In addition, the predictions made by each decision tree have varying impact on the final prediction made by the model.
  Algorithm
In the proceeding example, we’ll be using a dataset that categories people as attractive or not based on certain features.
How does the AdaBoost algorithm work?

It works in the following steps:

1.Initially, Adaboost selects a training subset randomly.

2.It iteratively trains the AdaBoost machine learning model by selecting the training set based on the accurate prediction of the last training.

3.It assigns the higher weight to wrong classified observations so that in the next iteration these observations will get the high probability for classification.

4.Also, It assigns the weight to the trained classifier in each iteration according to the accuracy of the classifier. The more accurate classifier will get high weight.

5.This process iterate until the complete training data fits without any error or until reached to the specified maximum number of estimators.

6.To classify, perform a "vote" across all of the learning algorithms you built.
