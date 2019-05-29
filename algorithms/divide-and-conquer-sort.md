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

-The Quick Sort-

  Divides the array into 3 parts:

    The Pivot: a single element
    The Left Partition: should contain a number lower than the Pivot
    The Right Partition: should contain a number greater than the Pivot

    After this, the pivot is sorted.  Now, recursive call quicksort on either side
      of the pivot until the entire array is sorted.

  It's convention to pick either the first or last value in an array as the
    initial pivot element.

  We continue partitioning and choosing new pivots as we work through the array
  until we are down to single elements.

-Quick Sort vs Merge Sort-

      Quick Sort	                              Merge Sort
Better in a virtual memory                Useful in database scenarios.
environment.                              Useful when additional data may
Built-in sort function in C               arrive during or after sorting.
programming languages, Java, and          Used by Safari and Firefox in their
Python.                                   implementation of JavaScript’s sort function.
Works better for caching environments.

-In an interview-
  May be asked to compare and contrast merge and quick sorts.
  May be asked to describe a scenario where you'd pick one over the other.
