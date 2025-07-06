# C Numbers

Use `int` when you need to store a whole number without decimals, like 35 or 1000, and `float` or `double` when you need a floating point number (with decimals), like 9.99 or 3.14515.

## `int`

```c
int myNum = 1000;
printf("%d", myNum);
```

## `float`

```c
float myNum = 5.75;
printf("%f", myNum);
```

## `double`

```c
double myNum = 19.99;
printf("%lf", myNum);
```

## The difference between `float` and `double`

The precision of a floating point value indicates how many digits the value can have after the decimal point. The precision of `float` is six or seven decimal digits, while `double` variables have a precision of about 15 digits. Therefore, it is often safer to use `double` for most calculations - but note that it takes up twice as much memory as `float` (8 bytes vs. 4 bytes).

## Scientific numbers

In C, you can write very large or very small floating-point numbers using scientific notation.

This is done using the letter e (or E), which stands for "times 10 to the power of".

This is useful for writing numbers in a shorter way. Especially when working with scientific values or large-scale data.

```c
float f1 = 35e3;   // 35 * 10^3 = 35000
double d1 = 12E4;  // 12 * 10^4 = 120000

printf("%f\n", f1);
printf("%lf", d1);
```