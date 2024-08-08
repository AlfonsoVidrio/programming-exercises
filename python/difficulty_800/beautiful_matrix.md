## A. Beautiful Matrix

**Time Limit per Test**: 2 seconds  
**Memory Limit per Test**: 256 megabytes

You have a \(5 \times 5\) matrix consisting of 24 zeroes and a single number one. The rows of the matrix are indexed from 1 to 5 from top to bottom, and the columns are indexed from 1 to 5 from left to right. In one move, you can apply one of the following transformations to the matrix:

1. Swap two neighboring rows, that is, rows with indices \(i\) and \(i + 1\) for some integer \(i\) (\(1 \leq i < 5\)).
2. Swap two neighboring columns, that is, columns with indices \(j\) and \(j + 1\) for some integer \(j\) (\(1 \leq j < 5\)).

A matrix is considered beautiful if the single number one is located in the middle cell (i.e., at the intersection of the third row and the third column). Your task is to count the minimum number of moves needed to make the matrix beautiful.

### Input

The input consists of five lines, each containing five integers: the \(j\)-th integer in the \(i\)-th line represents the element of the matrix located at the intersection of the \(i\)-th row and the \(j\)-th column. It is guaranteed that the matrix consists of 24 zeroes and a single number one.

### Output

Print a single integer — the minimum number of moves needed to make the matrix beautiful.

### Examples

***

**Input**

0 0 0 0 0
0 0 0 0 1
0 0 0 0 0
0 0 0 0 0
0 0 0 0 0


**Output**

3

***
**Input**

0 0 0 0 0
0 0 0 0 0
0 1 0 0 0
0 0 0 0 0
0 0 0 0 0

**Output**

1

***

### Solution
[Try it online!](https://tio.run/##hY3BbsMgDIbP8VP4VtC6Ktm0y6Q9SRVFNHVXtAQiA@vWl09NUNXsNCGB/fN99vQbz969zvNoItsrfuDeuilFpXdhGqy8ePKMHVqHbNwnqTfdAnybIVEXyHB/FmfTbAAyZ92Rfjr2ly3KlSVyaSQ2kVTZoN@hsif8MyDP9hf5qIrf@yGNTuZKulsitea1gL33fBRCrTau5cwcmMwXAFNIQ8zsIu3rFp/xZYula5ZOVxDS2C1RENQcgiqe4Bqf1kHTaoCJrYvq4ehqnmssp4F7Vf9T3QA "Python 3 – Try It Online")