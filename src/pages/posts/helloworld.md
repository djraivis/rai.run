---
description: Write a function called `helloWorld` that returns a string of 'Hello World!'.
slug: helloworld
public: true
layout: ../../layouts/BlogPost.astro
title: Hello World
createdAt: 1705009954772
updatedAt: 1705019412330
tags:
  - JavaScript
heroImage: /posts/helloworld_thumbnail.png
---


### Function Signature

```js
/**
 * Returns a string containing 'Hello World!'.
 * @returns {string} - The string 'Hello World!'.
 */
function helloWorld(): string;
```

### Examples

```js
helloWorld() // 'Hello World!'
```

### Constraints

I will put any constraints here. They will vary depending on the challenge.

- The function must return a string

### Hints

- I will put a couple hints here. You can choose to use them or not.

## Solutions

<details>
  <summary>Click For Solution</summary>

```js
function printHelloWorld() {
  return 'Hello World!';
}
```

### Explanation

I will put the explanation to the solution here. The length and depth of the explanation will vary depending on the challenge.

</details>

### Test Cases

The Jest tests will go here. They are already included in the course files. You just need to run `npm test`. Sometimes I will also put manual tests here.

```js
test("Returning 'Hello, World!' as a string", () => {
  const result = helloWorld();
  expect(result).toBe('Hello World!');
});
```

