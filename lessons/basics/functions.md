# Functions in R
Functions are a fundamental part of any programming language, and R is no exception. Functions are self-contained blocks of code that perform specific tasks, and they can be called and executed repeatedly with different inputs. In this guide, we'll take a look at what functions are and how they're used in R.

## Defining Functions
Functions in R are defined using the function keyword. The basic syntax for defining a function in R is as follows:

```
function_name <- function(arg1, arg2, ...) {
  # Code to be executed goes here
}
```

Here, function_name is the name of the function, and arg1, arg2, etc. are the function arguments. The code inside the function is executed when the function is called, and the result is returned to the caller.

For example, let's define a function that calculates the sum of two numbers:

```
addition <- function(x, y) {
  result <- x + y
  return(result)
}
```

In this example, the function is named addition, and it takes two arguments, x and y. The code inside the function calculates the sum of x and y and returns the result.

## Calling Functions
Functions are called by simply writing their name followed by the required arguments in parentheses. For example, let's call the addition function:

``` addition(2, 3) ```

This code will call the addition function and pass 2 and 3 as arguments. The function will return 5, which is the sum of 2 and 3.


## Return Values
The `return` statement is used to return the result of a function. In the example above, the addition function returns the sum of x and y as a result. It's important to note that a function can have multiple return statements, but it will only execute the first one it encounters.


## Arguments
Functions can take any number of arguments, and the number of arguments required by a function is defined when the function is created. When a function is called, the values of the arguments are passed to the function, and the function operates on those values.

In the example above, the addition function takes two arguments, x and y. When the function is called, the values of x and y are set to the values of the arguments passed to the function.


## Default Arguments
Functions can have default arguments, which are values that are used if no value is passed for that argument when the function is called. Default arguments are specified in the function definition by assigning a value to the argument.

For example, let's modify the addition function to include a default argument for y:

```
addition <- function(x, y = 1) {
  result <- x + y
  return(result)
}
```

In this example, y has a default value of 1. This means that if the addition function is called without a value for y, it will use the default value of 1.
