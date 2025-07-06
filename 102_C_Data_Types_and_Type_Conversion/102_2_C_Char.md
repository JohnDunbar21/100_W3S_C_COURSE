# C Char

The `char` data type is used to store a _single_ character, and must be surrounded by _single quotes_ like 'A' or 'b', and we use the `%c` format specifier to print them:

```c
char myGrade = 'A';
printf("%c", myGrade);
```

If you are familiar with ASCII, you can use ASCII values to display certain chatacters - note that these values are not surrounded by single quotes as they are numbers:

```c
char a = 65, b = 66, c = 67;
printf("%c", a);
printf("%c", b);
printf("%c", c);
```

If you try to store more than a single character, it will only print the last character (and may produce errors).