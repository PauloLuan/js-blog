---
title: como usar o factorial no javascript es6
date: "2020-01-04"
description: ''
tags: math,recursion,beginner
---

Calculates the factorial of a number.

Use recursion.
If `n` is less than or equal to `1`, return `1`.
Otherwise, return the product of `n` and the factorial of `n - 1`.
Throws an exception if `n` is a negative number.

```js
const factorial = n =>
  n < 0
    ? (() => {
      throw new TypeError('Negative numbers are not allowed!');
    })()
    : n <= 1
      ? 1
      : n * factorial(n - 1);
```

```js
factorial(6); // 720
```


[Acesse a Referência original](http://github.com/30-seconds/)
