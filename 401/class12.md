# Introduction to Pandas

Pandas is a data analysis and manipulation tool built on top of Python

## Object Creation

Create a series by passing a list of values, and Pandas will create a default integer index. Shown below:

    import pandas as pd
    s = pd.Series([1, 3, 5, np.nan, 6, 8])

    s
    0    1.0
    1    3.0
    2    5.0
    3    NaN
    4    6.0
    5    8.0

Create a data frame with datetime index and labeled columns to help organize it. From there, you can organize the columns further by giving more specific variables.

Going from this:

    dates = pd.date_range("20130101", periods=6)

    dates
    Out[6]: 
    DatetimeIndex(['2013-01-01', '2013-01-02', '2013-01-03', '2013-01-04',
    '2013-01-05', '2013-01-06'],
    dtype='datetime64[ns]', freq='D')

    df = pd.DataFrame(np.random.randn(6, 4), index=dates, columns=list("ABCD"))

    df
    Out[8]:
          A         B         C         D
          2013-01-01  0.469112 -0.282863 -1.509059 -1.135632
          2013-01-02  1.212112 -0.173215  0.119209 -1.044236
          2013-01-03 -0.861849 -2.104569 -0.494929  1.071804
          2013-01-04  0.721555 -0.706771 -1.039575  0.271860
          2013-01-05 -0.424972  0.567020  0.276232 -1.087401
          2013-01-06 -0.673690  0.113648 -1.478427  0.524988

To this:

    df2 = pd.DataFrame(
    {
        "A": 1.0,
        "B": pd.Timestamp("20130102"),
        "C": pd.Series(1, index=list(range(4)), dtype="float32"),
        "D": np.array([3] * 4, dtype="int32"),
        "E": pd.Categorical(["test", "train", "test", "train"]),
        "F": "foo",
    }
    )
    df2
    Out[10]: 
        A     B         C   D      E    F
    0  1.0 2013-01-02  1.0  3   test  foo
    1  1.0 2013-01-02  1.0  3  train  foo
    2  1.0 2013-01-02  1.0  3   test  foo
    3  1.0 2013-01-02  1.0  3  train  foo

## Viewing Data

By referencing the head() or the tail() and passing in the however many rows of either the top or bottom respectively, these rows will be displayed.

Dataframe to numpy can be used to give numpy access to the values within the dataframe, but keep in mind that numpy can only parse values of the same kind of data.

name_of_list.describe shows a quick statistic summary of the data. The values can also be sorted by axis or value of that axis with .sort_index() and .sort_values() respectively.

## Selection

Selecting a single column will yield a series. do so with name_of_dataframe[selected_column]. The slicing method can also be used here to select multiple columns.

Selection by label can be achieved by using labels to get a cross section of the index you would like to pull from.

Selection by position can why rows you want to pull the values of.

## Missing Data

If a cell is missing in the dataframe, pandas primarily uses the np.nan to represent the missing spot.

## Grouping

Grouping consists of three steps:

1. Splitting the data into groups based on some criteria

2. Applying a function to each group independently

3. Combining the results into a data structure
