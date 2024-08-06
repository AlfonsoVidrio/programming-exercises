# A. Way Too Long Words

**Time limit per test:** 1 second  
**Memory limit per test:** 256 megabytes

Sometimes some words like "localization" or "internationalization" are so long that writing them many times in one text is quite tiresome.

Let's consider a word too long if its length is strictly more than 10 characters. All too long words should be replaced with a special abbreviation.

This abbreviation is made like this: we write down the first and the last letter of a word and between them we write the number of letters between the first and the last letters. That number is in decimal system and doesn't contain any leading zeroes.

Thus, "localization" will be spelt as "l10n", and "internationalization" will be spelt as "i18n".

You are suggested to automatize the process of changing the words with abbreviations. All too long words should be replaced by the abbreviation and the words that are not too long should not undergo any changes.

## Input

The first line contains an integer `n` (1 ≤ `n` ≤ 100). Each of the following `n` lines contains one word. All the words consist of lowercase Latin letters and have lengths from 1 to 100 characters.

## Output

Print `n` lines. The i-th line should contain the result of replacing the i-th word from the input data.

## Examples

**Input**
4
word
localization
internationalization
pneumonoultramicroscopicsilicovolcanoconiosis


**Output**

word
l10n
i18n
p43s

```python
n = int(input())

for _ in range(n):
	word = input()
	if len(word) > 10:
		print(f'{word[0]}{len(word)-2}{word[-1]}')
	else:
		print(word)
```

[Try it online!](https://tio.run/##RYxBCsIwFETXzSmya7ootOpK0ItIkRBT/ZD@H5JU0dKzxySC3Q1v3ox9hwfhPkbkJw4YBKCdg2gaxkZy/JoYdxLvWmBzZNWL3K2IRWIVjNxoFBk3/Mz7LjmVdflorJeML92wLn@n3a0/2vbDWqcDbbzeNsWJ8cByYIaUNPCRAQhZqrXDkjdoUc8TIc0mODmBcuQVWVAeDCh6klESSRECefBf "Python 3 – Try It Online")