# Linear Regressions

## How to Run Linear Regression in Python

**sklearn.linear_model module**- contains "methods intended for regression in which the target value is expected to be a linear combination of the input variables”

## Working through data sets

First step import libraries

Second import data sets

```Python
from sklearn.datasets import datasets
boston = datasets()
```
To explore the data set keys

Use boston.keys()

To check shape of dictionary

boston.data.shape

`(506,13)

This means I have 506 instances(rows) and 13 attributes or parameters(columns)

To print feature names Use

print boston.feature_names

To get a description of the data Use

print boston.DESCR

### How to convert to pandas

To convert to pandas table use the following

```Python
bos = pd.DataFrame(boston.data)
bos.head()
```

Then to convert the columns names with will automatically be numbers from panda to the feature names you provide. replace them with this code.

```Python
bos.columns = boston.feature_names
bos.head()
```

### Scikit Learn

####  least square methods


Y = boston housing price called target

X = all the other variables


Type LinearRegression. and Tab-  This will give a list of functions available

#### important functions

lm.fit() -> fits a linear model

lm.predict() -> Predict Y using the linear model with estimated coefficients

lm.score() -> Returns the coefficient of determination (R^2). A measure of how well observed outcomes are replicated by the model, as the proportion of total variation of outcomes explained by the model.

<cite>How to run Linear regression in Python scikit-Learn, Manu Jeevan,https://bigdata-madesimple.com/how-to-run-linear-regression-in-python-scikit-learn</cite>
