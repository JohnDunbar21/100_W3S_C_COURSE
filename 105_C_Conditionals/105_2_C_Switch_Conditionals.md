# C Switch Conditionals

The `switch` statement selects one of many code blocks to be executed:

```c
switch (expression) {
  case x:
    // code block
    break;
  case y:
    // code block
    break;
  default:
    // code block
}
```

When C reaches a `break` keyword, it breaks out of the switch block. This will stop the execution of more code and case testing inside the block.

The `default` keyword specifies some code to run if there is no case match. The `default` keyword must be used as the last statement in the switch, and it does not need a `break`.