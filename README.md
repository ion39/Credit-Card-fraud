# Credit-Card-fraud

The challenge is to recognize fraudulent credit card transactions so that the customers of credit card companies are not charged for items that they did not purchase.

Main challenges involved in credit card fraud detection are:

1.Enormous Data is processed every day and the model build must be fast enough to respond to the scam in time.
2.Imbalanced Data i.e most of the transactions (99.8%) are not fraudulent which makes it really hard for detecting the fraudulent ones
3.Data availability as the data is mostly private.
4.Misclassified Data can be another major issue, as not every fraudulent transaction is caught and reported.
5.Adaptive techniques used against the model by the scammers.

How to tackle these challenges?

1.The model used must be simple and fast enough to detect the anomaly and classify it as a fraudulent transaction as quickly as possible.
2.Imbalance can be dealt with by properly using some methods which we will talk about in the next paragraph
3.For protecting the privacy of the user the dimensionality of the data can be reduced.
4.A more trustworthy source must be taken which double-check the data, at least for training the model.
We can make the model simple and interpretable so that when the scammer adapts to it with just some tweaks we can have a new model up and running to deploy.

The datasets contains transactions made by credit cards in September 2013 by european cardholders. This dataset presents transactions that occurred in two days, where we have 492 frauds out of 284,807 transactions. The dataset is highly unbalanced, the positive class (frauds) account for 0.172% of all transactions.

It contains only numerical input variables which are the result of a PCA transformation.

Due to confidentiality issues, there are not provided the original features and more background information about the data.

Features V1, V2, ... V28 are the principal components obtained with PCA;
The only features which have not been transformed with PCA are Time and Amount. Feature Time contains the seconds elapsed between each transaction and the first transaction in the dataset. The feature Amount is the transaction Amount, this feature can be used for example-dependant cost-senstive learning.
Feature Class is the response variable and it takes value 1 in case of fraud and 0 otherwise.
