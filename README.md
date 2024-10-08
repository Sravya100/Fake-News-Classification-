# Fake-News-Classification

Problem Statement:
The problem at hand is to detect fake news that is being generated in textual format on digital media platforms. We employ a two-phase approach to implement machine learning models where news articles are classified as fake or real and then we examine which category of news, for example political, entertainment, business, or technology contains the highest amount of fake news, thus helping us determine which domain needs the maximum regulation.


In the first phase, we train several linear models and ensemble models like K-NN (K-Nearest Neighbours) Classifier, Decision Trees Classifier, Random Forest Classifier, Naïve Bayes Classifier, XGB Classifier, which is a gradient boosting classifier and some other classifiers using the train data. Then, we use them to make predictions on our test data. We observe that using ensemble methods has been more efficient than using linear classifiers as they improve themselves constantly. We use the train-test split technique and F1-score metric to measure the performance of the models and select a model that most accurately predicts real and fake news.


In the second phase, we extract all the news that has been classified as fake in phase one and classify them into major categories of interest like politics, technology, entertainment, or business. We use several models like linear regression model, a multinomial naïve bayes classifier, decision tree classifier, random forest classifier, and ADA Boost. We train these models with a new dataset that has category labels and then we give the fake news extracted in phase one as input to these to predict the news category.
