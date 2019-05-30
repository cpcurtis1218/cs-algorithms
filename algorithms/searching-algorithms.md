Searching Algorithms

-Objectives-

  1) Understand Big O complexity of brute force and binary search approaches.
  2) Describe how Binary Search works.
  3) Write a binary search algorithm to find a value in an array.

-Brute Force-

  The idea that an algorithm will try check every possibility or element.

-Binary Search-

  Time complexity: O(log(N))

  General Idea:
    Take the sorted array.
    First, check the middle element.
    If not this one, check to the left half or right half, depending
      on the search value.

  An Added Bonus:
    We know where the an element should go (if not found) by taking one less
    than the absolute value of the return value.
