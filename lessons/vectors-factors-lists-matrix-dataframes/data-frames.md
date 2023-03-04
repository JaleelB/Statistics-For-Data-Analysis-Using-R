# Data Frames in R
A data frame in R is a two-dimensional table-like data structure. It is a collection of vectors of equal length, with each vector representing a column of data.

## Creating Data Frames
Data frames can be created using the `data.frame()` function. The function takes vectors of data as arguments, and converts them into a data frame.

```
# create a data frame
my_df <- data.frame(name = c("Alice", "Bob", "Charlie"), 
                    age = c(25, 30, 35), 
                    sex = c("F", "M", "M"))

# print the data frame
my_df
```

Output:

```
      name age sex
1    Alice  25   F
2      Bob  30   M
3 Charlie  35   M
```

## Accessing Elements of a Data Frame
Elements of a data frame can be accessed using the `$` operator or the `[]` operator.

```
# create a data frame
my_df <- data.frame(name = c("Alice", "Bob", "Charlie"), 
                    age = c(25, 30, 35), 
                    sex = c("F", "M", "M"))

# access the age column using the $ operator
my_df$age

# access the second row using the [] operator
my_df[2, ]
```

## Adding and Removing Columns
New columns can be added to a data frame using the `$` operator or the `[]` operator.

```
# create a data frame
my_df <- data.frame(name = c("Alice", "Bob", "Charlie"), 
                    age = c(25, 30, 35), 
                    sex = c("F", "M", "M"))

# add a new column
my_df$height <- c(160, 180, 175)

# print the data frame
my_df
```

Output:

```
      name age sex height
1    Alice  25   F    160
2      Bob  30   M    180
3 Charlie  35   M    175
```

Columns can be removed using the `subset()` function.

```
# create a data frame
my_df <- data.frame(name = c("Alice", "Bob", "Charlie"), 
                    age = c(25, 30, 35), 
                    sex = c("F", "M", "M"))

# remove the age column
my_df <- subset(my_df, select = c(name, sex))

# print the data frame
my_df
```

Output:

```
      name sex
1    Alice  F
2      Bob  M
3 Charlie  M
```



## Filtering and Subsetting Data Frames
Data frames can be subsetted using the `[]` operator.

```
# create a data frame
my_df <- data.frame(name = c("Alice", "Bob", "Charlie"), 
                    age = c(25, 30, 35), 
                    sex = c("F", "M", "M"))

# subset the data frame to include only individuals under the age of 30
my_df_subset <- my_df[my_df$age < 30, ]

# print the subsetted data frame
my_df_subset
```

Output:

```
    name age sex
1  Alice  25   F
2    Bob  30   M
```

Data frames can also be filtered using the `subset()` function.

```
# create a data frame
my_df <- data.frame(name = c("Alice", "Bob", "Charlie"), 
```

