# Panda

## Pandas in 10

panda is a python library for data science

### Creating a Series

pass list of values and panda will create index

`s = pd.Series([1, 3, 5, np.nan, 6, 8])`

### Creating a DataFrame

pass a Numpy array with a datetime index and columns labeled

`dates = pd.date_range("20130101", periods=6)`

`df = pd.DataFrame(np.random.randn(6, 4), index=dates, columns=list("ABCD"))`

Looks like this

```py
# index=dates
                  A         B         C         D   # columns=list("ABCD")
2013-01-01  0.469112 -0.282863 -1.509059 -1.135632
2013-01-02  1.212112 -0.173215  0.119209 -1.044236
2013-01-03 -0.861849 -2.104569 -0.494929  1.071804
2013-01-04  0.721555 -0.706771 -1.039575  0.271860
2013-01-05 -0.424972  0.567020  0.276232 -1.087401
2013-01-06 -0.673690  0.113648 -1.478427  0.524988
```

<cite>10 minutes to pandas,https://pandas.pydata.org/pandas-docs/stable/user_guide/10min.html</cite>

## Commom panda methods

### Checking the data

- data.shape - gives you rows, columns
- data.describe() - creates basic statistics

### Seeing the data

- data.head(#) - prints # rows of the data
- data.loc[#] - Print the #th row
- data.loc[#, 'column_1'] - Prints the value of #th row in column_1
- data.loc[range(#,#)] - Subset from row 4 to 6 (excluded)

### Basic plotting

`data['column_numerical'].plot()`

or histogram

`data['column_numerical'].hist()`

<cite>10 minutes to pandas,https://pandas.pydata.org/pandas-docs/stable/user_guide/10min.html</cite>
