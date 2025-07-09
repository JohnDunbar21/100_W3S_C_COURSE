# C Strings

To create a string in C, you need to use the `char` type and create an array of characters. For example:

```c
char greetings[] = "Hello World!";
```

Note that you have to use _double quotes_ `""` instead of the standard `char` single quotes `''`.

Since strings are `char` arrays, you can access a character in the string by referring to its index in the string.

To modify a character in a string, you must use single quotes as shown below:

```c
char greetings[] = "Hello World!";
greetings[0] = 'J';
printf("%s", greetings);
// Outputs Jello World! instead of Hello World!
```

In fact, anything that can be done on an array can be done on a string!