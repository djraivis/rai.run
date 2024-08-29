---
description: Get familiar with first most basic js functions.
slug: firstjs
public: true
layout: ../../layouts/BlogPost.astro
title: First JS
createdAt: 1705009954772
updatedAt: 1724942223210
tags:
  - JavaScript
heroImage: /posts/firstjs_thumbnail.jpg
---

## Challanges

<details>

<summary>Find Max Number</summary>
  
## Find Max Number

Write a function called `findMaxNumber` that takes in an array of numbers and returns the largest number in the array.

#### Solution 1
```js
function findMaxNumber(arr) {
  return Math.max(...arr);
}
```

#### Solution 2
```js
function findMaxNumber(arr) {
  let max = arr[0];

  for (let i = 1; i < arr.length; i++) {
    if (arr[i] > max) {
      max = arr[i];
    }
  }
  return max;
}

findMaxNumber([1, 2, 3, 4, 5, 6, 7, 8, 9, 10]); // 10
findMaxNumber([10, 9, 8, 7, 6, 5, 4, 3, 2, 1]); // 10
findMaxNumber([1, 2, 3, 4, 5, 10, 9, 8, 7, 6]); // 10
```
#### Solution 3
```js
  function findMaxNumber(arr) {
    if (arr.length === 0) {
        return undefined; // return undefined for an empty array
    }

    let max = arr[0]; // Assume the first element is the maximum

    for (let i = 1; i < arr.length; i++) {
        if (arr[i] > max) {
            max = arr[i]; // Update max if current element is greater
        }
    }

    return max; // Return the maximum number
}

// Example usage:
const numbers = [10, 5, 20, 8, 15];
console.log(findMaxNumber(numbers)); // Output: 20
``` 
</details>
  
<details>
  <summary>Calculator - Switch / else if</summary>

#### Uisng a switch:
 
```js
function calculator(num1, num2, operator) {
  let result;

  switch (operator) {
    case '+':
      result = num1 + num2;
      break;
    case '-':
      result = num1 - num2;
      break;
    case '*':
      result = num1 * num2;
      break;
    case '/':
      result = num1 / num2;
      break;
    default:
      throw new Error('Invalid operator');
  }

  return result;
}

calculator(1, 2, '+') // 3
calculator(10, 5, '-') // 5
calculator(2, 2, '*') // 4
calculator(10, 5, '/') // 2
```

#### Using an if statement:
```js
function calculator(num1, num2, operator) {
  let result;

  if (operator === '+') {
    result = num1 + num2;
  } else if (operator === '-') {
    result = num1 - num2;
  } else if (operator === '*') {
    result = num1 * num2;
  } else if (operator === '/') {
    result = num1 / num2;
  } else {
    throw new Error('Invalid operator');
  }

  return result;
}
```
</details>


<details>
  <summary>Get Sum - a + b</summary>

```js
function getSum(a, b) {
  return a + b;
}
```
</details>
  
<details>
<summary>Hello JavaScript</summary>

```js
function printHelloWorld() {
  return 'Hello World!';
}
```
</details>