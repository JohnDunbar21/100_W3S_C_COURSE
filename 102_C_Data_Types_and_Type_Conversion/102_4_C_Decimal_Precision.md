# C Decimal Precision

If you want to remove extra zeros (set the decimal precision), you can use a dot followed by a number that specifies how many digits that should be shown after the decimal point. For example:

```c
float myFloatNum = 3.5;

printf("%f\n", myFloatNum);   // Default will show 6 digits after the decimal point
printf("%.1f\n", myFloatNum); // Only show 1 digit
printf("%.2f\n", myFloatNum); // Only show 2 digits
printf("%.4f", myFloatNum);   // Only show 4 digits
```