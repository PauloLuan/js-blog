---
title: como usar o flatten no javascript es6
date: "2020-01-04"
description: ''
tags: array,intermediate
---

Flattens an array up to the specified depth.

Use recursion, decrementing `depth` by 1 for each level of depth.
Use `Array.prototype.reduce()` and `Array.prototype.concat()` to merge elements or arrays.
Base case, for `depth` equal to `1` stops recursion.
Omit the second argument, `depth` to flatten only to a depth of `1` (single flatten).

```js
const flatten = (arr, depth = 1) =>
  arr.reduce((a, v) => a.concat(depth > 1 && Array.isArray(v) ? flatten(v, depth - 1) : v), []);
```

```js
flatten([1, [2], 3, 4]); // [1, 2, 3, 4]
flatten([1, [2, [3, [4, 5], 6], 7], 8], 2); // [1, 2, 3, [4, 5], 6, 7, 8]
```


[Acesse a Referência original](http://github.com/30-seconds/)
