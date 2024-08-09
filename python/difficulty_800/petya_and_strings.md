## A. Petya and Strings

**Time limit per test**: 2 seconds  
**Memory limit per test**: 256 megabytes

Little Petya loves presents. His mum bought him two strings of the same size for his birthday. The strings consist of uppercase and lowercase Latin letters. Now Petya wants to compare those two strings lexicographically. The letters' case does not matter, that is an uppercase letter is considered equivalent to the corresponding lowercase letter. Help Petya perform the comparison.

### Input

Each of the first two lines contains a bought string. The strings' lengths range from 1 to 100 inclusive. It is guaranteed that the strings are of the same length and also consist of uppercase and lowercase Latin letters.

### Output

If the first string is less than the second one, print `-1`. If the second string is less than the first one, print `1`. If the strings are equal, print `0`. Note that the letters' case is not taken into consideration when the strings are compared.

### Examples

***

**Input**

aaaa
aaaA

**Output**

0

***

**Input**

abs
Abz

**Output**

-1

***

**Input**

abcdefg
AbCdEfF

**Output**

1

***

### Note

If you want more formal information about the lexicographical order (also known as the "dictionary order" or "alphabetical order"), you can visit the following site:

[Lexicographical Order](http://en.wikipedia.org/wiki/Lexicographical_order)

### Solution

[Try it online!](https://tio.run/##lc89CgIxEAXgOnOKKRNQcbETV/Aksj8TDaxJmMwievm4hYURU9jO@3iPiQ@5Br/L2TpOck7Czl@wRefjLNpspnAn1gYSDcGP9RxGsjiEW@yY3ipp/CxdYdlh9qCcxXK3LdFCFJPM7HELiqZvf6zy5hc/VPm6AYjLTfR/P5icuz7BqX/CCw "Python 3 – Try It Online")