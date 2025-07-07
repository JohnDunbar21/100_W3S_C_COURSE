# C Type Conversion

Sometimes you have to convert the value of one data type to another type: this is known as _type conversion_. There are two types of conversion in C:

1. Implicit Conversion - automatically.
2. Explicit Conversion - manually.

## Implicit Conversion

Implicit conversion is done automatically by the compiler when you assign a value of one typeto another. For example, if you assign an `int` value to a `float` type:

```c
// Automatic conversion: int to float
float myFloat = 9;

printf("%f", myFloat); // 9.000000
```

The above code will convert the `int` value 9 to a `float` value of 9.000000. This also works in reverse:

```c
// Automatic conversion: float to int
int myInt = 9.99;

printf("%d", myInt); // 9
```

As another example, if you divide two `int` values, the resulting value will by rounded down to the nearest integer (5 / 2 = 2).

## Explicit Conversion

Explicit conversion is done manually by placing the type in parentheses `()` in front of the value - this is also known as _casting_. For example:

```c
// Manual conversion: int to float
float sum = (float) 5 / 2;

printf("%f", sum); // 2.500000
```