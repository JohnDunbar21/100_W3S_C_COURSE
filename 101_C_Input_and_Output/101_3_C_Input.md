# C Input

To get user input, you can use the `scanf` function:

```c
// Create an integer variable that will store the number we get from the user
int myNum;

// Ask the user to type a number
printf("Type a number: \n");

// Get and save the number the user types
scanf("%d", &myNum);

// Output the number the user typed
printf("Your number is: %d", myNum);
```

The `scanf` function takes _two_ arguments:

1. The format specifier of the variable (such as `%d` or `%c`).
2. The reference operator which stores the memory address of the variable.

The `scanf` function also allows multiple inputs, for example:

```c
// Create an int and a char variable
int myNum;
char myChar;

// Ask the user to type a number AND a character
printf("Type a number AND a character and press enter: \n");

// Get and save the number AND character the user types
scanf("%d %c", &myNum, &myChar);

// Print the number
printf("Your number is: %d\n", myNum);

// Print the character
printf("Your character is: %c\n", myChar);
```

You can also get a string entered by a user by defining a `char` array:

```c
// Create a string
char firstName[30];

// Ask the user to input some text
printf("Enter your first name: \n");

// Get and save the text
scanf("%s", firstName);

// Output the text
printf("Hello %s", firstName);
```

When working with strings in `scanf`, you must specify the size of the string, but you don't have to use the reference operator `&`.

However, the `scanf` function has some limitations: it considers any whitespacew as a terminating character which means it can only ever display a single word (even if you type multiple words).

In the event you need to obtain multi-word string inputs from a user, you can use the `fgets` function.