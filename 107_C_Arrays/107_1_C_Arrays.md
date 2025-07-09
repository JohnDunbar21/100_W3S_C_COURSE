# C Arrays

To create an array, define the data type and specify the name of the array followed by square brackets `[]`. An initialised array may look like:

```c
int myNumbers[] = {25, 50, 75, 100};
```

To access data in an array, refer to its index - which starts at 0 in ascending order. Accessing the first element in the `myNumbers` array would be done by using `myNumbers[0]`.

You can also use the index to reassign a value in the array by using the assignment operator `=`.

A common way to create arrays is to specify the array's size and add elements later. This may look like:

```c
// Declare an array of four integers:
int myNumbers[4];

// Add elements
myNumbers[0] = 25;
myNumbers[1] = 50;
myNumbers[2] = 75;
myNumbers[3] = 100;
```

In using this method, you should know the number of array elements in advance in order to ensure enough memory is allocated.

To get the size of an array, you can use the `sizeof` operator:

```c
int myNumbers[] = {10, 25, 50, 75, 100};
printf("%zu", sizeof(myNumbers)); // Prints 20
```

The above code prints 20 instead of 5 because it returns the size of a type in bytes. Since an `int` is 4 bytes, the value goes from 5 to 20.

To get the _length_ of an array, you would do the following:

```c
int myNumbers[] = {10, 25, 50, 75, 100};
int length = sizeof(myNumbers) / sizeof(myNumbers[0]);

printf("%d", length);  // Prints 5
```

You can use the length to make dynamic for-loops as shown below:

```c
int myNumbers[] = {25, 50, 75, 100};
int length = sizeof(myNumbers) / sizeof(myNumbers[0]);
int i;

for (i = 0; i < length; i++) {
  printf("%d\n", myNumbers[i]);
}
```