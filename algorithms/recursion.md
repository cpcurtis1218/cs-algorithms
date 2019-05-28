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

There are 4 steps to writing recusive functions:

  1) Define your function and parameters.
  2) Define your base case and return the computed result.
  3) Perform the action step.
  4) Return the function with new arguments to make progress toward the base case.

Recursive Helper Functions:

  A non-recursive parent function can help take out some of the confusion

Why Recursion?

  We can compare recursion to loops, which use iteration.

  A simple for loop is a good example:
  ```js
    function countDown(num){
      for (x = num; x > 0; x--) {
        console.log(x);
      }
    }
  ```
  In most cases, iteration is more efficient. So why use recursion?

  -- Recursion is often easier to read, and uses fewer lines of code.
      Ultimately it comes down to what the developer understands better.

When to use Recursion:
  It's great when a problem needs to be broken into smaller chunks or
    especially when we need to look for all possible combinations of something.
  Recursion is great for:
    -Calculating all possible combinations of elements.
    -Checking all possible routes between two destinations.
    -Problems that can be broken down into smaller subproblems.

Recursion in interviews:
[Coding interview recursion](https://hackernoon.com/coding-interview-recursion-f0d60c9dbb60)
[Recursion](https://www.byte-by-byte.com/recursion/)

Practice:
[Codepen](https://codepen.io/cpcurtis1218/pen/PvBvXJ?editors=0010#0)
