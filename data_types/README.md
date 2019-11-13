# Data Types

A data type is a particular kind of data item, as defined by the values it can take, the programming language used, or the operations that can be performed on it.

## Primitive Built-in Tyoes

These are the most commonly used data types in any ALB program.

#### Numeric Data Types

- `:int`: stands for _integer_ (signed and in base 10 by default). Can hold any integer numeric value or set of arithmetic operations with an integer as result. Values corresponding to this data type typically have a width of 4 bytes, and can hold decimal numbers in a range between -2147483648 and 2147483647. Examples: `321`, `2`, `613731`. This data type has a subset for integers in different bases, e.g. hexadecimal (base 16), octal (base 8) or binary (base 2).

- `:float`: stands for _floating-point number_. Can hold any floating-point numeric value or set of arithmetic operations with a floating-point number as result. Values corresponding to this data type typically have a width of 4 bytes, and can hold a range of numbers between +/- 3.4e +/- 38 (~7 digits).

#### Integer subset

Inside the integers data type (`:int`), we can find four different bases. These are: decimal, hexadecimal, octal and binary.

This is the usage of the elements of this subset. We will put the creation of a variable as an example:

`var :int:prefix myInt [value_in_base] ;`

As we are specifying the base of the integer, there is no need to include a prefix, such as `0x` (for hexadecimal numbers), `0` (for octal numbers), or `0b` (for binary numbers). Although the value will be recognized in any of the two cases, this is a bad and inefficient practice. However, the prefix specifying the integer's base is required, except for the decimal base, which is defined as the default base for integers, as will be explained now.

Example of good practice:

`var :int:hex myHex 54f1a9d ;`

Example of bad practice:

`var :int:hex myHex 0x54f1a9d ;`

This last option's compilation time would be greater than the first one. However, the result would be the same.

###### Elements of the integer subset

- Decimal numbers (prefix `:dec`). This is the default base, so the prefix is not needed to use this base in a value. For example, this is how we would create and display a variable with an integer in decimal base:

```
var :int myDecimal 15 ;
outv $myDecimal ; // to learn more about the outv function, please refer to stdlib/stdout/ (https://github.com/albpl/docs/tree/master/stdlib/stdout)
```

Note that this code snippet must be written between the `BEGIN` and `END` delimiters, as shown in _Basic structure of an ALB program_ (https://github.com/albpl/docs/blob/master/README.md)
