Recursion

Objectives:
  1) Define recursion.
  2) Write the base case and recursive case of a recursive function.
  3) Identify functions that use recursion and explain why it’s used.

Simply put, recursion is when a function calls itself.

We can break down the process of recursion into 3 steps:

  1) Base Case: when the process can stop
  2) Action: putting the function to work
  3) Recursive case: the function is called again, but with assurance that progress
    is being made toward the base case.

Consider this relatively simple example:
```js
  function countDown(num){
    if(num < 0){
      return;
    }
    console.log(num)
    return countDown(num - 1)
  }
```
The Base Case:
  We put the condition that must be met for the process to complete.
```js
  function countDown(num)
    if(num < 0){
      return;
    }
```

The Action:
  We want something to happen during each step, so we console.log(num)
```js
  function countDown(num){
  if(num < 0){
    return;
  }
  console.log(num)
  }
```

The Recursive Case:
  We call the function again, but slightly alter the argument
```js
  function countDown(num){
    if(num < 0){
      return;
    }
    console.log(num)
    return countDown(num - 1)
  }
```
