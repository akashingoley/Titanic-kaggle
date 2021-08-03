# Titanic-kaggle

The sinking of the Titanic is one of the most infamous shipwrecks in history.

On April 15, 1912, during her maiden voyage, the widely considered “unsinkable” RMS Titanic sank after colliding with an iceberg. Unfortunately, there weren’t enough lifeboats for everyone onboard, resulting in the death of 1502 out of 2224 passengers and crew.

While there was some element of luck involved in surviving, it seems some groups of people were more likely to survive than others.

In this challenge, we have to build a predictive model that answers the question: “what sorts of people were more likely to survive?” using passenger data (ie name, age, gender, socio-economic class, etc).

## Data Description
The data has been split into two groups:

1] Training set (train.csv)

2] Test set (test.csv)

The training set should be used to build your machine learning models. For the training set, we provide the outcome (also known as the “ground truth”) for each passenger. Model will be based on “features” like passengers’ gender and class. You can also use feature engineering to create new features.

The test set should be used to see how well your model performs on unseen data. For the test set, no ground truth is provided for each passenger. We have to predict these outcomes. For each passenger in the test set, use the model you trained to predict whether or not they survived the sinking of the Titanic.

## Variable Notes
Pclass: A proxy for socio-economic status (SES)

1st = Upper

2nd = Middle

3rd = Lower


Age: Age is fractional if less than 1. 
If the age is estimated, is it in the form of xx.5


Sibsp: The dataset defines family relations in this way...

Sibling = brother, sister, stepbrother, stepsister

Spouse = husband, wife (mistresses and fiancés were ignored)


Parch: The dataset defines family relations in this way...

Parent = mother, father

Child = daughter, son, stepdaughter, stepson

Some children travelled only with a nanny, therefore parch=0 for them.

### Models used

1] kagle.ipynb : Decision Tree from scratch with max depth = 5 
Submitted to kaggle with score 0.77511

2] DT_sklearn.ipynb : Decision Tree using sklearn DecisionTreeClassifier and cross_val_score on RandomForestClassifier
max depth = 5 cv = 5
Submitted to kaggle with score 0.77751

