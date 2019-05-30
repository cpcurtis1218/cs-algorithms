Distribution Sorting Algorithms

-Objectives-

  1) Explain how bucket and radix sorts work.
  2) Identify the scenarios where bucket and radix sorts should be used.
  3) Describe the time complexity of bucket sort.
  4) Implement bucket sort.

-Refresher-

  Whats the difference between distribution sort and comparison sorting methods?
    - Distribution uses one property of each element to decide where it fits
      - ONLY LOOKS AT THE ELEMENT ITSELF, MAY HAVE MULTIPLE ELEMENTS WITH THE SAME PROPERTY
    - Comparison compares one element to another
      - COMPARES ELEMENTS TO EACH OTHER

-Bucket and Radix Sort-

  Bucket Sort: is a lot like the essay-grading scenario. It sorts elements
    into buckets based on their value and then uses another method
    to sort the elements within those bins. It can be used for integers
    or strings.

  Radix Sort: operates in basically the same way as bucket sort but is
    only used for integers.

  For Both:
    The most important thing to decide: How many 'buckets' should there be?
    -A general rule of thumb: use the square root of the total # of elements

-Bucket Sort-

  Space Complexity: O(N) becuase it creates an entirely new array for sorted values.

  Most useful when values are relatively dense (not a major differentiation between values)

  The General Idea of the Bucket Sort:
    1) Start with your initial array
    2) Set up an array of initially empty “buckets.”
    3) Go over the original array and scatter each object in its bucket.
    4) Sort each bucket.
    5) Gather: Go through the buckets sequentially and gather everything back into the original single array.

-Radix Sort-

  Radix sort operates by looking at the individual digits in a set of numbers.
  Radix starts at either the beginning of a number (the most significant digit approach) or the end of a number (the least significant digit approach) and works through each digit until it’s reached the end and the values are sorted.
