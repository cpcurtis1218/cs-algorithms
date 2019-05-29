Sorting Intro

-Objectives-
  1) Define the two sorting methods, and when to use each.
  2) Identify if a sort is stable or unstable, and the impact it can have.
  3) Explain how Big O complexity applies to sorting.

-What is sorting?
  Taking an unordered collection and making it ordered

-Types of sorts-

  Comparison sort: compares two items and decides which one to put first

  Distribution sort: compares one property of the item and decides where it belongs

-Stability-
  Stable: when we use 2 factor sorting, we maintain the order of the first sort

  Unstable: when we lose one sort method when applying another

-Space Complexity and Sorting-
  In Place: O(1) or (Olog(N)) - The sort takes up a predictable amount of memory
    and does not depend on the size of input

  Out of Place: O(N) or O(N^2) - The algorithm uses an extra array, or more, to
    sort the values

-Worst, Average, and Best Case-
  Worst Case: Big O

  Average Case: Big Theta - The typical runtime

  Best Case: Big Omega - sorting an already sorted data set

-Takeaway-
  In additioan to complexity, there are 3 things we want to keep in mind when
  we think about sorting algorithms:

  Stability: Whether or not the items stay in order
  Sorting method: Comparison, Distribution, or a combination
  The size and structure of the data: Is it already sorted, unsorted, very large, etc.)
