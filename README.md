# Merge Sort

## Description/Challenge Summary
This project uses Java Spring and other dependencies to create a "lecture" on `Merge Sort` suitable for Code Fellow's 301 level course.

## Installation

```
 $ git clone git@github.com:stephenchu530/mergesort.git
```
or
```
 $ git clone https://github.com/stephenchu530/mergesort.git
```

## Requirements:

Ensure the following are installed:
* `OpenJDK 8`
* `Gradle`

## Usage

*Command Line:*
```
 $ ./gradlew run --args '<integers in any order>'
```

*Example Input:*
```
 $ ./gradlw run --args '2 8 5 7'
```

*Example Output:*
```
 [2 5 7 8]
```

## Approach & Efficiency
`public static int[] mergeSort(int[] numbers)` - O(nlg(n))

## Solution / Lecture Notes
* [Solution Code](src/main/java/mergesort/App.java)
* [Lecture Notes](LECTURE-NOTES.md)

## Contributors
* Stephen Chu, [stephenchu530](https://github.com/stephenchu530)

## License
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/stephenchu530/mergesort/blob/master/LICENSE)
