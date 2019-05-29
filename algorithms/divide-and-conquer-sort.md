Divide-and-Conquer Sorting Algorithms

Merge Sort and Quick Sort

-Objecties-
  1) Describe how merge sort and quick sort work
  2) Explain space and time complexities for merge and quick sorts
  3) Identify when to use merge and quick sorts

-The Merge Sort-
  Takes an array and splits it in half over and over until its small and sorted.
  Then, merges the small pieces back together on their way back up.

  Two Premises of Merge Sort:
    1) The easiest list to sort is a single list item.
    2) Creating one large array by merging two smaller, sorted arrays is not difficult.

  Merge sort is techincally broken up into two parts, the merge sort algorithm and
   the merge algorithm.

   Phase 1: Split the array in half until you cant anymore.  This is the merge sort algorithm.
   Phase 2: Merge the pieces back together. This is the merge algorithm (aka 'merge helper function')

-The Merge Sort Algorithm-
  Time Complexity: O(log(N))
  Base Case: The array is 1 element or shorter
  Recursive Case: The array is longer than 1 element

-The Merge Algorithm-
  Time Complexity: O(N)
  The basic process of the merge algorithm.  It starts with sorted single-element arrays
  that are the result of the Merge Sort Algoritm above.
    1) Start at the beginning of two arrays of items.
    2) Compare the first item from each array to each other.
    3) Whichever value is less, copy it to a results list.
    4) Move on to the next item in the array that just gave its first element to the results list.
    5) Repeat Steps 1–4 until you have all of the elements from both arrays in the results list.

-Time Complexity for Merge Sort-
  O(N) * O(log(N)) = O(N log(N))
