# Measurement of central tendency - MEAN in R
> In statistics, the measurement of central tendency is used to describe the central or typical value of a set of data. The most commonly used measures of central tendency are mean, median, and mode. In this answer, we will focus on the mean and how to calculate it in R. The mean is the sum of all the values in a dataset divided by the total number of values. It is denoted by the symbol "µ" for the population mean and "x̄" for the sample mean. 

The formula to calculate the mean is:
```µ = (x₁ + x₂ + ... + xn) / n```

where x₁, x₂, ..., xn are the individual data points, and n is the total number of data points.

In R, we can calculate the mean using the `mean()` function. The function takes a vector of values as input and returns the mean of those values.

Here's an example:
```
# Create a vector of values
values <- c(2, 4, 6, 8, 10)

# Calculate the mean
mean(values)

```

Output:
`[1] 6`

The `mean()` function calculates the mean of the values in the values vector, which is 6.

We can also calculate the mean of a subset of values in a dataset. For example, suppose we have a dataset of students' test scores, and we want to calculate the mean of only the scores from the first exam. We can do this using indexing in R:

```
# Create a vector of test scores
test_scores <- c(80, 90, 70, 85, 95)

# Calculate the mean of the first three scores
mean(test_scores[1:3])

```

Output:
`[1] 80`

In this example, we used indexing (test_scores[1:3]) to select only the first three test scores and calculated their mean using the `mean()` function.

In addition to calculating the mean of a vector of values, we can also calculate the mean of multiple vectors using the `rowMeans()` function or the mean of values grouped by a categorical variable using the `aggregate()` function.

Overall, the mean is a useful measure of central tendency that provides insight into the typical value of a dataset. By using the `mean()` function in R, we can easily calculate the mean of a vector of values, a subset of values, or values grouped by a categorical variable.