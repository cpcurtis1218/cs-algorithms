Big O Notation

The efficiency of algorithms.

Objectives:
  1) Explain how Big O notation is used to describe algorithms.
  2) Define constant, linear, quadratic, logarithmic, and factorial Big O runtimes.
  3) Analyze algorithms to determine their Big O runtime.

The Worst Case Scenario: The way we compare algorithms
  - The worst way the code could perform, take the longest, use the most memory

Big O Notation- The relationship between functions based on their growth rates
  Time complexity - slightly more complicated than space complexity
    - Not actually measuring the amount of time in ms or sec.  Instead, considering
      the number of basic steps the algorithm needs to execute, relative to the
      size of the data set.

  Space complexity -

                            Classes of Complexity:

-Highly Efficient-
  Constant complexity: Constant space and time complexity
    (think throwing away a bag of apples, it doesnt matter how many apples are in the bag)
    Big O: O(1)
  Logarithmic complexity: This type of algorithm cuts the problem in half each time
    (think finding a name in phonebook, flip to a random page and then go forward or backward)
    (a binary search is one example of logarithmic complexity)
    Big O: O(log(N))

-Pretty Good-
  Linear complexity: As input size increases, processing time increases linearly
    (one more input = one more basic step for the algorithm)
    Big O: O(N)

-Inefficient-
  Quadratic complexity: As input size increases, processing time increases by magnitudes
    (think nested iterations)
    Big O: O(N^2)
  Factorial complexity: As input size increases, the processes increases by magnitudes
    Big O: O(N!)

We can drop coefficients when figuring out Big O complexity.  Dont worry about O(2N), this is still O(N).

In an interview, might be asked about the following, related to Big O:

- Does the function have to go through an entire list? If so, there's an N in that Big O class somewhere.
- Are there nested loops? That might give you O(N^2) (or worse).
- Does the function break the list into smaller chunks? You could have O(log(N)).
- Is the amount of work the same, regardless of the size of the dataset? That means it's O(1).
