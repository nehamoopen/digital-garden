# Basics

## Arithmetic

- **Addition**: `2 + 2`
- **Subtraction**: `3 - 3`
- **Multiplication**: `4 * 4`
- **Division**: `(5 + 5) / 5`
- **Exponentiation**: `2^6`
- **Modulo**: `28 %% 7`

## Assignment Operators

The operators `<-` and `=` assign into the environment in which they are evaluated.
The operator `<-` can be used anywhere, whereas the operator `=` is only allowed at the top level (e.g., in the complete expression typed at the command prompt) or as one of the subexpressions in a braced list of expressions.

source: https://stat.ethz.ch/R-manual/R-devel/library/base/html/assignOps.html

## Data Types

- numeric
- character
- logical

The `class()` function can be used to check the data type of a variable.

## Vectors

- The `c()` function (combine) is used to create vectors. 
- The `names()` function can be used to name elements of a vector. Another way to do it would be to name the elements directly like: `vector <- c(Name1 = 1, Name2 = 2)`.
- The `sum()` function calculates the sum of all elements of a vector. 
- Braces or square brackets `[]` can be used to select elements of a vector. Elements can be selected by position `my_vector[2]` or by name `my_vector['Name3']`
- To select multiple elements, incorporate the `c()` function again: `x <- vector[c(1, 5)]`
- A range of elements can be selected with the colon operator, `my_vector[2:5]` but note that this does not work with named elements.
- You can subset a vector with another vector, like `x <- vector2[vector1]` - this works by comparing the two vectors.
