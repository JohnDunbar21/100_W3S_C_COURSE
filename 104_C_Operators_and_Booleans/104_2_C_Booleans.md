# C Booleans

Booleans represent one of two values: `true` or `false`. The `bool` type is not a built-in data type like `int` or `char` and so must be imported into the program:

```c
#include <stdbool.h>
```

A boolean variable is declared with the `bool` keyword and can take the values `true` or `false`. Boolean values are always returned as integers:

- 1 == `true`.
- 0 == `false`.

Therefore, you must use the `%d` format specifier when printing a boolean value.