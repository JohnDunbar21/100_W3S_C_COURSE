# C Constants

A variable can be declared as a _constant_, wich means *unchangeable* and *read-only*. Constants can be created by adding `const` to a variable's definition. For example:

```c
const int myNum = 15;  // myNum will always be 15
myNum = 10;  // error: assignment of read-only variable 'myNum'
```

You should always declare the variable as constant when you have values that are unlikely to change.

Note that if you are declaring a constant, you _must_ assign it with a value.

It is generally good practice to declare constants in uppercase to improve the readability of the code.