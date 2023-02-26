# Measurement of central tendency - Median and Mode using R.
In statistics, the measurement of central tendency is used to describe the central or typical value of a set of data. In addition to the mean, the median and mode are also commonly used measures of central tendency. In this answer, we will focus on how to calculate the median and mode using R.

## Median
The median is the middle value in a dataset when the data is arranged in order from smallest to largest. It is denoted by the symbol "Me" or "Meⁿ" where "n" denotes the size of the dataset. If the dataset has an even number of values, then the median is the average of the two middle values. The formula to calculate the median is:
```
Me = { (n + 1) / 2 }th value

```

where "n" is the total number of data points.

In R, we can calculate the median using the median() function. The function takes a vector of values as input and returns the median of those values.

Here's an example:
```
# Create a vector of values
values <- c(2, 4, 6, 8, 10)

# Calculate the median
median(values)

```

Output:
```
[1] 6
```

The `median()` function calculates the median of the values in the values vector, which is 6.

If the dataset has an even number of values, the median can be calculated as follows:
```
# Create a vector of values with an even number of elements
values <- c(2, 4, 6, 8)

# Calculate the median
median(values)
```

Output:
```
[1] 5
```

In this example, the `median()` function calculates the median of the values in the values vector, which is the average of the two middle values, `(4 + 6) / 2 = 5`.


##  Mode
The mode is the value that appears most frequently in a dataset. It is denoted by the symbol "Mo". In some cases, a dataset may have multiple modes if there are multiple values that appear with the same frequency.

In R, we can calculate the mode using the `Mode()` function. The function is not built-in to R, so we need to define it ourselves.

Here's an example of how to define the `Mode()` function:
```
# Define the Mode function
Mode <- function(x) {
  ux <- unique(x)
  ux[which.max(tabulate(match(x, ux)))]
}
```

In this function, we first use the `unique()` function to find the unique values in the input vector x. We then use the `match()` function to match the values in x to the unique values in ux, and the `tabulate()` function to count the frequency of each unique value. Finally, we use the `which.max()` function to find the index of the value with the maximum frequency, and return that value.

Here's an example of how to use the `Mode()` function:
```
# Create a vector of values
values <- c(2, 4, 6, 8, 6, 10)

# Calculate the mode
Mode(values)
```

Output:
`[1] 6`

The `Mode()` function calculates the mode of the values in the `values` vector, which is 6.

In some cases, a dataset may not have a mode, or may have multiple modes with the same frequency. In such cases, the `Mode()` function will return one of the modes or NA if there is no mode.

Overall, the median and mode are useful measures of central tendency that can provide additional insights into the characteristics of a dataset, especially when used in conjunction with the mean. Calculating these measures using R is straightforward and can be done using built-in functions or user-defined functions.
