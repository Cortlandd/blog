---
title: Haskell for the C Programmer
---

---
Haskell for the C Programmer

---


# UNDER CONSTRUCTION
> Note: If you'd like to contribute, then by all means do. Any information to shed light and make learning Haskell an easier transition for programmers of other paradigms then thats cool.

## Background on Haskell

Haskell is a pure functional language. By pure I mean it's solely based on Lambda Calculus. More on Lambda Calculus next. If it were an impure Functional Programming, it'd add ambient effects, mutation, and imperative step wise-wise encoding of instructions. Basically what you do in C. No offence.

## Benefits

...

## Difference

explaining how Haskell and FP being very algorithm oriented where languages like C focus more on the data.
(gotta confirm this information) 

## Some syntax beforehand

```haskell
-- I may show examples in haskell. Here is a simple example to show whats going on.
-- a function named f takes an argument x and returns the argument x
f x = x
```

``` c
// in C it'd look like: 
int f(x) {

  return x;
}
```

## Lambda Calculus

Functional programming languages are based on the lambda calculus and rely on expressions. Lambda Calculus has three basic components: expressions, variables, and abstrations. An Expression can be a variable name, an abstraction (a lambda itself), a function application (a variable or lambda applied to an argument) or a combination of all three. The head of the function is a λ (lambda) followed by a variable name that is the parameter
or argument of that function. The body of the function is another expression. Lambda abstractions have the following basic structure (HB, P. 54):
```c
λ x . x
|___|______
the head of the lambda (everything to the left of the .)
```
```c
λ x . x
__|________
the single argument the lambda takes. the variable is bound when the function is applied
```
```c
λ x . x
______|____
the head of the lambda returns when applied. this is a bound variable.
```

This is an identiy function in lambda calculus so all it does is accept a single argument x and returns the same argument. X is bound by the enclosing lambda because it is defined when the lambda is applied to an argument. X is bound to the head of the function and when the function is applied to an argument, all instances of x within the function body must be bound to the same value.

example:
```haskell
> λ x . x (2)
> λ 2 . 2
2
-- eliminate the head
-- substitute 2 for each x in the body
```

The identity of 2 is 2. Pretty cool right? If you'd like to learn more, I highly recommend buying Haskell Programming from First Principles. It has a great and more thorough introduction to Lambda Calculus and is best resource on the market to learn Haskell.


## Functions

A function is a relation between two sets, a set of inputs and a set of outputs. The function itself defines and represents the relationship (haskellbook, p. 48).

think of this in C:
``` c
// the input is x
int square(x) {
  // the output is x * x
  x * x;
  
  return 0;
}
// the function itself, square, defines and represents the relationship
square(2)
```


in haskell it'd be written as:
``` haskell
-- read :: as "has type"
-- square has type integer, and returns an integer

square :: Int -> Int
square x = x * x

main = print (square 2)
```

---------------

## Types

Haskell, like C is statically typed. 


## Type System

Haskell has a robust and expressive type system. 

 
# Comments
### Haskell
```haskell
-- This is a single line comment

{-
  This is a multiple
  line
  comment
-}
```

### C

```c
// This is a single line comment

/* 
  This is a multiple
  line
  comment
*/
```


# Program Structure
> The syntax for the main function. The place where all code is ran.
### Haskell
```haskell
main = putStrLn "Hello World"
```

### C

```c
int main() {

  println("Hello World");
  // more later
  return 0;
}
```

# Importing
> Importing functions and other definitions from other modules/header files.
### Haskell
```Haskell
import ModuleName
```

### C

```c
#include <header file name>
```



# Variable Definition
> Defining variables along with said variables type (int, string, long, etc).

### Haskell
```Haskell
thisInteger :: Int
thisInteger = 2
```

### C
```c
int thisInteger;
thisInteger = 2;
// or 
int thisInteger = 2;
```

# Type Declaration
### Haskell
```Haskell

```

### C

```c

```

# Data Structure

> not sure if this is accurate

### Haskell
```Haskell
data Fish = Name | Species | Teeth | Age
```

### C

```c
struct fish {
  const char *name;
  const char *species;
  int teeth;
  int age;
};
```

To Be Continued