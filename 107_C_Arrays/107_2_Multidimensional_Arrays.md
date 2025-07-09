# Multidimensional Arrays

A multidimensional array is an array of arrays and can have any number of dimensions.

## 2D Arrays

A 2D array is also known as a matrix. An example of a 2D array is:

```c
int matrix[2][3] = { {1, 4, 2}, {3, 6, 8} };
```

Rows are represented by `[2]` and columns `[3]`, where values are placed in row-order.

You access and modify elements in a 2D array the same way you would as with any other array, but you need to specify its position across all dimensions. For example, if you wanted to change 3 to 9, you would do:

```c
int matrix[2][3] = { {1, 4, 2}, {3, 6, 8} };
matrix[1][0] = 9;
```

To loop through a 2D array, you need to add an extra loop depth as shown below:

```c
int matrix[2][3] = { {1, 4, 2}, {3, 6, 8} };

int i, j;
for (i = 0; i < 2; i++) {
  for (j = 0; j < 3; j++) {
    printf("%d\n", matrix[i][j]);
  }
}
```