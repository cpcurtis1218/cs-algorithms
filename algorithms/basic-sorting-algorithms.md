Basic Sorting Algorithms

-Objectives-
  1) Describe the time and space complexity of bubble and insertion sorts.
  2) Implement bubble and insertion sorts.

-Bubble and Insertion Sort-
  * They're slow, inefficient, and infrequently used.
  * They prep us for more complicated sorting algorithms.

-The Bubble Sort-

  Puts values in order by iterating through the data and comparing neighboring
  numbers.  When the sort encounters a smaller value before a greater value,
  it swaps the numbers.  The sort continues to iterate until the array is sorted.

  Here is the basic algorithm:
    1) Start at the beginning of an array of items.
    2) Compare the item you’re looking at to the next item in the list.
    3) If this item is smaller than the next one, keep it in place. If it’s
        greater, swap them.
    4) Move on to the next item.
    5) Repeat Steps 1–4 until you can go through the whole list without
        making any swaps.

  **Bubble Sort is stable becuase the items stay in order as we continue to iterate

-The Insertion Sort-

  Takes each items and places it into the proper right place in the array.
  Not super efficient, still ends up traversing the array many times.
  Often used in conjunction with bucket sort.

  **Insertion Sort is stable becuase the items stay in order as we continue to iterate

-In an Interview-

  Might be asked to descibe or illustrate a bubble sort.

  [Questions](https://hoven-in.appspot.com/Home/Data-Structures/Data-Structure-Interview-Questions/interview-questions-on-bubble-sort-01.html)
