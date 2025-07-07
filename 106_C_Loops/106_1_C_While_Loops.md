# C While Loops

A `while` loop iterates through a block of code as long as a specified condition is `true`. For example:

```c
while (condition) {
  // code block to be executed
}
```

A more in-depth example would be having a loop iterate whilst a variable's value is less than 5:

```c
int i = 0;

while (i < 5) {
  printf("%d\n", i);
  i++;
}
```

If you do not increment the variable used in the above example, the loop will never end.