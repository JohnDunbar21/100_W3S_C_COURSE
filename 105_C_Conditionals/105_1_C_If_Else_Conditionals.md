# C If Else Conditionals

C has the following conditional statements:

- Use `if` to specify a block of code to be executed, if a specified condition is `true`.
- Use `else` to specify a block of code to be executed, if the same condition is `false`.
- Use `else if` to specify a new condition to test, if the first condition is `false`.

Syntax:

```c
if (condition1) {
  // block of code to be executed if condition1 is true
} else if (condition2) {
  // block of code to be executed if the condition1 is false and condition2 is true
} else {
  // block of code to be executed if the condition1 is false and condition2 is false
}
```

There is also a short-hand if else, which is known as the ternary operator because it consists of three operands. It can be used to replace multiple lines of code with a single line. It is often used to replace simple if else statements:

`variable = (condition) ? expressionTrue : expressionFalse;`