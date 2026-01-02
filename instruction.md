# Word Count Task

You are given an input text file at `/app/input.txt`.  
Your task is to create an output file at `/app/output.txt`.

## Requirements

- Read the file `/app/input.txt`.
- Count how many times each unique word appears.
- Consider words case-insensitive (e.g., `Hello` and `hello` are the same).
- Treat any sequence of alphabetic characters `a-z` or `A-Z` as a word.
- Output must be written to `/app/output.txt`.

## Output format

- Each line must contain one word and its count, separated by a single space.
- Lines must be sorted by the word in ascending alphabetical order.
- Example (format only):

```text
apple 3
banana 1
orange 2
