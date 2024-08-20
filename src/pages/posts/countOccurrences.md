---
description: >-
  Takes in a string and a character; returns the number of occurrences of that
  character in the string.
slug: countOccurrences
public: true
layout: ../../layouts/BlogPost.astro
title: Count Occurrences
createdAt: 1705018772359
updatedAt: 1712231618171
tags:
  - JavaScript
heroImage: /posts/countOccurrences_thumbnail.jpg
---

## Function Signature

```js

 // Returns the number of occurrences of a character in a string.
 * @param {string} str - The string to search.
 * @param {string} char - The character to search for.
 * @returns {number} - The number of occurrences of the character in the string.

function countOccurrences(str: string, char: string): number;

Examples
countOccurrences('hello', 'l'); // 2
countOccurrences('hello', 'z'); // 0
```

### Test Cases

```js
test('Count Occurrences of a Character', () => {
  expect(countOccurrences('hello', 'l')).toBe(2);
  expect(countOccurrences('programming', 'm')).toBe(2);
  expect(countOccurrences('banana', 'a')).toBe(3);
});
```

#### Solution

```js
function countOccurrences(str, char) {
  // Declare a variable to store the number of occurrences
  let count = 0;

  // Loop through the string
  for (let i = 0; i < str.length; i++) {
    // If the current character is the same as the character we're looking for, increment the count
    if (str[i] === char) {
      count++;
    }
  }
  return count;
}

```

#### Solution 2
```js
function countOccurrences(str, char) {
    let count = 0;
    for (let i = 0; i < str.length; i++) {
        if (str[i] === char) {
            count++;
        }
    }
    return count;
}

// Example usage:
const myString = "hello world";
const myCharacter = "o";
console.log(countOccurrences(myString, myCharacter)); // Output: 2
```

#### Solution 3
```js
const countOccurrences = (str, char) => str.split(char).length - 1;
```

