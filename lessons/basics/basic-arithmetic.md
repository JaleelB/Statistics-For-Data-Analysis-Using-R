# Basic Arithmetics in R

R is a powerful and versatile programming language that is widely used for data analysis and statistical computing. In this guide, we will cover the basics of arithmetic operations in R, including addition, subtraction, multiplication, division, and exponentiation. Whether you're just starting out with R or you're a seasoned user, this guide will provide you with a comprehensive understanding of how arithmetic works in R.

## Addition
Addition in R is performed using the + operator. For example, to add two numbers together, you would write the following code:

```
x <- 2
y <- 3
z <- x + y
```

In this example, x is assigned the value 2, y is assigned the value 3, and z is assigned the value 5, which is the result of adding x and y together.

You can also perform addition with multiple numbers. For example, to add three numbers together, you would write the following code:

```
a <- 2
b <- 3
c <- 4
d <- a + b + c
```

In this example, a, b, and c are assigned the values 2, 3, and 4, respectively. The value of d is the result of adding all three values together, which is equal to 9.

You can also perform addition with vectors. For example, to add two vectors together, you would write the following code:

```
x <- c(1, 2, 3)
y <- c(4, 5, 6)
z <- x + y
```

In this example, x and y are assigned the values 1, 2, 3 and 4, 5, 6, respectively. The value of z is the result of adding each corresponding element of x and y together, which is equal to 5, 7, 9.


## Subtraction
Subtraction in R is performed using the - operator. For example, to subtract one number from another, you would write the following code:

```
x <- 2
y <- 3
z <- y - x
```

In this example, x is assigned the value 2, y is assigned the value 3, and z is assigned the value 1, which is the result of subtracting x from y.

You can also perform subtraction with vectors. For example, to subtract one vector from another, you would write the following code:

```
x <- c(1, 2, 3)
y <- c(4, 5, 6)
z <- y - x
```

In this example, x and y are assigned the values 1, 2, 3 and 4, 5, 6, respectively. The value of z is the result of subtracting each corresponding element of x from y, which is equal to 3, 3, 3.

## Multiplication
Multiplication in R is performed using the * operator. For example, to multiply two numbers together, you would write the following code:

```
x <- 2
y <- 3
z <- x * y
```

In this example, x is assigned the value 2, y is assigned the value 3, and z is assigned the value 6, which is the result of multiplying x and y together.

You can also perform multiplication with multiple numbers. For example, to multiply three numbers together, you would write the following code:

```
a <- 2
b <- 3
c <- 4
d <- a * b * c
```

In this example, a, b, and c are assigned the values 2, 3, and 4, respectively. The value of d is the result of multiplying all three values together, which is equal to 24.

You can also perform multiplication with vectors. For example, to multiply two vectors element-wise, you would write the following code:

```
x <- c(1, 2, 3)
y <- c(4, 5, 6)
z <- x * y
```

In this example, x and y are assigned the values 1, 2, 3 and 4, 5, 6, respectively. The value of z is the result of multiplying each corresponding element of x and y together, which is equal to 4, 10, 18.

## Division
Division in R is performed using the / operator. For example, to divide one number by another, you would write the following code:

```
x <- 6
y <- 3
z <- x / y
```

In this example, x is assigned the value 6, y is assigned the value 3, and z is assigned the value 2, which is the result of dividing x by y.

You can also perform division with vectors. For example, to divide one vector by another element-wise, you would write the following code:

```
x <- c(6, 12, 18)
y <- c(2, 3, 3)
z <- x / y
```

In this example, x and y are assigned the values 6, 12, 18 and 2, 3, 3, respectively. The value of z is the result of dividing each corresponding element of x by the corresponding element of y, which is equal to 3, 4, 6.

It's important to note that when dividing by zero in R, the result will be Inf (infinity) for positive numbers and -Inf for negative numbers.