# C String Functions

You can import useful functions to use on strings by adding the `string.h` header file:

```c
#include <string.h>
```

## String Length

To get the length of a string, you can use the `strlen` function:

```c
char alphabet[] = "ABCDEFGHIJKLMNOPQRSTUVWXYZ";
printf("%zu", strlen(alphabet));
```

Note that `strlen` acts differently to `sizeof` as the former does not account for the null terminator `\0` when counting.

Additionally, `sizeof` will always return the memory size (in bytes) instead of the string's actual length:

```c
char alphabet[50] = "ABCDEFGHIJKLMNOPQRSTUVWXYZ";
printf("%zu\n", strlen(alphabet));   // 26
printf("%zu\n", sizeof(alphabet));   // 50
```

## Concatenate Strings

To combine two strings, you can use the `strcat` function:

```c
char str1[20] = "Hello ";
char str2[] = "World!";

// Concatenate str2 to str1 (result is stored in str1)
strcat(str1, str2);

// Print str1
printf("%s", str1);
```

Note that the _memory_ size of the first string should be large enough to store the result of the two strings combined.

## Copy Strings

To copy the value of one string to another, you can use the `strcpy` function:

```c
char str1[20] = "Hello World!";
char str2[20];

// Copy str1 to str2
strcpy(str2, str1);

// Print str2
printf("%s", str2);
```

Note that the memory size of the second string should be large enough to store the copied string.

## Compare Strings

To compare two strings, you can use the `strcmp` function which will return 0 if the two strings are equal, otherwise a value that is not 0.

```c
char str1[] = "Hello";
char str2[] = "Hello";
char str3[] = "Hi";

// Compare str1 and str2, and print the result
printf("%d\n", strcmp(str1, str2));  // Returns 0 (the strings are equal)

// Compare str1 and str3, and print the result
printf("%d\n", strcmp(str1, str3));  // Returns -4 (the strings are not equal)
```

For a full breakdown of the String functions, go to https://www.w3schools.com/c/c_ref_string.php.