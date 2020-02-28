---
title: como usar o weightedSample no javascript es6
date: "2020-01-04"
description: ''
tags: array,random,advanced
---

Returns a random element from an array, using the provided `weights` as the probabilities for each element.

Use `Array.prototype.reduce()` to create an array of partial sums for each value in `weights`.
Use `Math.random()` to generate a random number and `Array.prototype.findIndex()` to find the correct index based on the array previously produced.
Finally, return the element of `arr` with the produced index.


```js
const weightedSample = (arr, weights) => {
  let roll = Math.random();
  return arr[
    weights
      .reduce((acc, w, i) => (i === 0 ? [w] : [...acc, acc[acc.length - 1] + w]), [])
      .findIndex((v, i, s) => roll >= (i === 0 ? 0 : s[i - 1]) && roll < v)
  ];
};
```

```js
weightedSample([3, 7, 9, 11], [0.1, 0.2, 0.6, 0.1]); // 9
```

[Acesse a Referência original](http://github.com/30-seconds/)
