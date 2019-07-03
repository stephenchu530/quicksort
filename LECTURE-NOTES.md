# Lecture Notes: Merge Sort

This sort is one of the more common sorts used in many built-in sorts. We should care because it is ubiquitous.

Insertion Sort has the following performance profile:
* Time Complexity: `O(nlg(n))`
* Space Complexity: `O(1)`

## Learning Objectives:
The student will learn the following:
* Merge sort algorithm
* Java implementation
* Unittests for the code
* Time and space complexity

## Lecture Flow:
Main Point:
 * Merge Sort is a recursive sort
 * Merge Sort works on the principal of 'divide and conquer'
 * Keep splitting the array of elements in half until left with 1 or 2 elements
 * "Merge" the 1 or 2 elements back together in sorted order
 * Keep doing this work back toward the single combined array 

## Diagram
![Visual Diagrom](MergeSort.jpg)

## Algorithm/Pseudocode
Gotten from Code Fellows 401:
```
ALGORITHM Mergesort(arr)
    DECLARE n <-- arr.length
           
    if arr.length > 1
      DECLARE mid <-- n/2
      DECLARE b <-- arr[0...mid]
      DECLARE c <-- arr[mid...n]
      // break down the left side
      Mergesort(b)
      // break down the right side
      Mergesort(c)
      // merge the left and the right side together
      Merge(b, c, arr)

ALGORITHM Merge(b, c, a)
    DECLARE i <-- 0
    DECLARE j <-- 0
    DECLARE k <-- 0

    while i < b && j < c
        if b[i] <= c[j]
            a[k] <-- b[i]
            i <-- i + 1
        else
            a[k] = c[j]
            j <-- j + 1
            
        k <-- k + 1

    if i = b.length
       add remaining items in array c to array a
    else
       add remaining items in array b to array a
       
    return a
```

## Readings and References
Watch
* [Merge Sort in 3 Minutes](https://www.youtube.com/watch?v=4VqmGXwpLqc)

Read
* [Geeks for Geeks](https://www.geeksforgeeks.org/merge-sort/)
* [Tutorial Point](https://www.tutorialspoint.com/data_structures_algorithms/merge_sort_algorithm.htm)

Bookmark
* [Wiki Merge Sort](https://en.wikipedia.org/wiki/Merge_sort)
